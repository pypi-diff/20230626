# Comparing `tmp/pyperf2-0.3-py3-none-any.whl.zip` & `tmp/pyperf2-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11145 bytes, number of entries: 6
--rw-r--r--  2.0 unx    24262 b- defN 23-Jun-23 09:06 pyperf2/__init__.py
--rwxr-xr-x  2.0 unx    11357 b- defN 23-Jun-23 09:07 pyperf2-0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     3314 b- defN 23-Jun-23 09:07 pyperf2-0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 09:07 pyperf2-0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-23 09:07 pyperf2-0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      453 b- defN 23-Jun-23 09:07 pyperf2-0.3.dist-info/RECORD
-6 files, 39486 bytes uncompressed, 10331 bytes compressed:  73.8%
+Zip file size: 11357 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    25016 b- defN 23-Jun-25 23:32 pyperf2/__init__.py
+-rwxr-xr-x  2.0 unx    11357 b- defN 23-Jun-25 23:38 pyperf2-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3340 b- defN 23-Jun-25 23:38 pyperf2-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-25 23:38 pyperf2-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-25 23:38 pyperf2-0.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      463 b- defN 23-Jun-25 23:38 pyperf2-0.3.1.dist-info/RECORD
+6 files, 40276 bytes uncompressed, 10523 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pyperf2/__init__.py
 Comment: 
 
-Filename: pyperf2-0.3.dist-info/LICENSE
+Filename: pyperf2-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: pyperf2-0.3.dist-info/METADATA
+Filename: pyperf2-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: pyperf2-0.3.dist-info/WHEEL
+Filename: pyperf2-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyperf2-0.3.dist-info/top_level.txt
+Filename: pyperf2-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyperf2-0.3.dist-info/RECORD
+Filename: pyperf2-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyperf2/__init__.py

```diff
@@ -8,24 +8,28 @@
 import os
 import pyjq
 import copy
 from decimal import Decimal
 from pprint import pprint, pformat
 import logging
 import datetime
+from pyroute2 import netns
+
 
 
 def output_reader(proc, outq, parent):
     for line in iter(proc.stdout.readline, b""):
         outq.put(line.decode("utf-8"))
 
         # print("{0} {1}".format(parent.name,line.decode('utf-8')))
 
         parent.line_ready_callback()
 
+class NameSpaceNotFoundError(Exception):
+    pass
 
 class IPerfInstance(object):
     def __init__(self):
         self.type = None
         self.report_interval = "1"
         self.protocol = "tcp"
         self.iperf_binary_path = "/usr/bin/iperf"
@@ -40,25 +44,26 @@
         self.port = "5001"
         self.status = "configured"
         self.packet_len = "1470"
         self.dscp = None
         self._result_regex = None
         self._info_regex = None
         self._results = {}
-        self.test_duration = "86400"
+        self.test_duration = 0
         self.client_source_port = None
         self.use_linux_namespace = None
         self._on_data_callbacks = []
         self._on_packetloss_callbacks = []
         self.currently_has_loss = {}
         self._output_reader_thread = None
         self._cleanup_timer_thread = None
         self._raw_log_filepath = None
         self._raw_log_filehandler = None
         self._creation_time = datetime.datetime.now().replace(microsecond=0).isoformat()
+        self.ttl=255
 
         if "pps" in self.bandwidth:
             self.expected_interval_packets = int(
                 Decimal(self.report_interval) * Decimal(self.bandwidth[:-3])
             )
         else:
             self.expected_interval_packets = None
@@ -91,15 +96,17 @@
         packets_received = None
         packet_loss_event_message = False
         report_message = False
         timestamp = datetime.datetime.now().isoformat()
         if self._raw_log_filehandler:
             self._raw_log_filehandler.write(line)
             self._raw_log_filehandler.flush()
-
+        if not self._info_regex:
+            raise RuntimeError("missing regex for parsing output",pformat(self.generate_cli_from_options()))
+        
         result = self._info_regex.match(line)  # check if it's an info header
         if result:
             info_data = result.groupdict()
             stream_id = info_data["stream_id"]
             if (
                 stream_id not in self._results
             ):  # new stream id detected -> create new result structure
@@ -406,37 +413,44 @@
 
     def output_reader(self):
         for line in iter(self._proc.stdout.readline, b""):
             self._outq.put(line.decode("utf-8"))
 
     def set_options(self, **kwargs):
         for option_name, option_value in kwargs.items():
+            if option_name in ["status"]:
+                continue
             self.__setattr__(option_name, str(option_value))
         if "pps" in self.bandwidth:
             self.expected_interval_packets = int(
                 Decimal(self.report_interval) * Decimal(self.bandwidth[:-3])
             )
         else:
             self.expected_interval_packets = None
+        if self.test_duration == None:
+            self.test_duration = 0
 
     def get_options(self):
         retval = {}
         for k, v in self.__dict__.items():
             if not k.startswith("_"):
                 retval[k] = v
         return retval
 
     def generate_cli_from_options(self):
         _cli = []
         if self.use_linux_namespace:
+            if self.use_linux_namespace not in list(netns.listnetns()):
+                raise NameSpaceNotFoundError(f"Namespace {self.use_linux_namespace} cannot be found.")
             _cli.extend("ip netns exec {0}".format(self.use_linux_namespace).split(" "))
         _cli.append(self.iperf_binary_path)
         _cli.append("-e")
-        _cli.append("-t")
-        _cli.append(self.test_duration)
+        if self.test_duration:
+            _cli.append("-t")
+            _cli.append(self.test_duration)
         if self.type == "server":
             _cli.append("-s")
             if self.bind_ip:
                 _cli.append("-B")
                 _cli.append(self.bind_ip)
             if self.protocol == "udp":
                 # multicast server result
@@ -457,14 +471,18 @@
             if self.protocol == "udp":
                 _cli.append("-l")
                 _cli.append(self.packet_len)
                 # [  3] local 192.168.51.154 port 54877 connected with 225.0.0.5 port 5001
                 self._result_regex = re.compile(
                     r"^\[\s*(?P<stream_id>\d+)\]\s+(?P<interval_begin>\d+\.\d+)-(?P<interval_end>\d+\.\d+)\s+(?P<interval_unit>\S+)\s+(?P<transferred>\S+)\s+(?P<transferred_unit>\S+)\s+(?P<bandwidth>\S+)\s+(?P<bandwidth_unit>\S+)\s+(?P<packets_written>\S+)/(?P<packets_error>\S+)\s+(?P<packet_rate>\d+)\s+(?P<packet_rate_unit>\S+)"
                 )
+            if self.ttl:
+                _cli.append("-T")
+                _cli.append(str(self.ttl))
+
         else:
             raise ValueError("type must be set to either server or client")
         if self.protocol == "udp":
             _cli.append("-u")
             self._info_regex = re.compile(
                 r"^\[\s*(?P<stream_id>\d+)\]\s+local\s+(?P<local_ip>\S+)\s+port\s+(?P<local_port>\S+)\s+connected\s+with\s+(?P<remote_ip>\S+)\s+port\s+(?P<remote_port>\S+)"
             )
@@ -531,28 +549,31 @@
     def start(self, create_thread_function=threading.Thread):
         self._results = {}
         if self._cleanup_timer_thread:
             self._cleanup_timer_thread.join()
             del self._cleanup_timer_thread
             self._cleanup_timer_thread = None
         # print(' '.join(self.generate_cli_from_options()))
+        # pprint(self.generate_cli_from_options())
         self._proc = subprocess.Popen(
             self.generate_cli_from_options(),
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
         )
+
         if not self._output_reader_thread:
             self._output_reader_thread = create_thread_function(
                 target=output_reader, args=(self._proc, self._outq, self)
             )
 
         self._output_reader_thread.start()
         self._running = True
         self.status = "running"
         time.sleep(0.2)
+
         self._cleanup_timer_thread = threading.Timer(
             int(self.test_duration) + 10, self.stop
         )
         self._cleanup_timer_thread.start()
 
         if self._proc.poll() is not None:
             self.stop()
```

## Comparing `pyperf2-0.3.dist-info/LICENSE` & `pyperf2-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyperf2-0.3.dist-info/METADATA` & `pyperf2-0.3.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyperf2
-Version: 0.3
+Version: 0.3.1
 Summary: Abstraction layer for iperf2 linux binary
 Home-page: https://github.com/jinjamator/pyperf2
 Author: Wilhelm Putz
 Author-email: wp@aci.guru
 License: ASL V2
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,14 +13,15 @@
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: pyjq
+Requires-Dist: pyroute2
 
 Introduction
 ==================
 
 Pyperf2 is an abstraction layer to simplify programatic use of the iperf2 binary for linux. It was written to have a simple interface for network test setups. It is mostly used for unicast/multicast network convergence tests so the defaults are tcp 1000pps per instance to have packetloss == 1ms/second. Nevertheless all options are configurable.
 
 Why iperf2 and not iperf3
```

