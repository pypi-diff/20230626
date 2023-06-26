# Comparing `tmp/rosetta-ce-1.1.0.tar.gz` & `tmp/rosetta-ce-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosetta-ce-1.1.0.tar", last modified: Wed Apr 26 16:28:38 2023, max compression
+gzip compressed data, was "rosetta-ce-1.2.0.tar", last modified: Mon Jun 26 16:20:18 2023, max compression
```

## Comparing `rosetta-ce-1.1.0.tar` & `rosetta-ce-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-04-26 16:28:38.373327 rosetta-ce-1.1.0/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.1.0/LICENSE
--rw-r--r--   0 amahmoud   (502) staff       (20)    11282 2023-04-26 16:28:38.372767 rosetta-ce-1.1.0/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)    10750 2023-04-26 16:15:22.000000 rosetta-ce-1.1.0/README.md
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-04-26 16:28:38.367803 rosetta-ce-1.1.0/rosetta/
--rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.1.0/rosetta/__init__.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-04-26 16:28:38.369421 rosetta-ce-1.1.0/rosetta/constants/
--rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.1.0/rosetta/constants/__init__.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.1.0/rosetta/constants/sensors.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.1.0/rosetta/constants/sources.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.1.0/rosetta/constants/systems.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.1.0/rosetta/rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)    30202 2023-04-25 15:10:04.000000 rosetta-ce-1.1.0/rosetta/rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     8012 2023-04-26 13:49:21.000000 rosetta-ce-1.1.0/rosetta/rsender.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-04-26 16:28:38.370857 rosetta-ce-1.1.0/rosetta_ce.egg-info/
--rw-r--r--   0 amahmoud   (502) staff       (20)    11282 2023-04-26 16:28:38.000000 rosetta-ce-1.1.0/rosetta_ce.egg-info/PKG-INFO
--rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-04-26 16:28:38.000000 rosetta-ce-1.1.0/rosetta_ce.egg-info/SOURCES.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-04-26 16:28:38.000000 rosetta-ce-1.1.0/rosetta_ce.egg-info/dependency_links.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-04-26 16:28:38.000000 rosetta-ce-1.1.0/rosetta_ce.egg-info/requires.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-04-26 16:28:38.000000 rosetta-ce-1.1.0/rosetta_ce.egg-info/top_level.txt
--rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-04-26 16:28:38.373371 rosetta-ce-1.1.0/setup.cfg
--rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-04-26 16:28:00.000000 rosetta-ce-1.1.0/setup.py
-drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-04-26 16:28:38.372340 rosetta-ce-1.1.0/tests/
--rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.1.0/tests/test_rconverter.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.1.0/tests/test_rfaker.py
--rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.1.0/tests/test_rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-26 16:20:18.387352 rosetta-ce-1.2.0/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1070 2023-04-08 17:22:13.000000 rosetta-ce-1.2.0/LICENSE
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11282 2023-06-26 16:20:18.387063 rosetta-ce-1.2.0/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)    10750 2023-04-26 16:15:22.000000 rosetta-ce-1.2.0/README.md
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-26 16:20:18.380371 rosetta-ce-1.2.0/rosetta/
+-rw-r--r--   0 amahmoud   (502) staff       (20)       92 2023-04-09 08:11:12.000000 rosetta-ce-1.2.0/rosetta/__init__.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-26 16:20:18.382609 rosetta-ce-1.2.0/rosetta/constants/
+-rw-r--r--   0 amahmoud   (502) staff       (20)        0 2023-04-12 16:36:37.000000 rosetta-ce-1.2.0/rosetta/constants/__init__.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1936 2023-04-09 13:32:25.000000 rosetta-ce-1.2.0/rosetta/constants/sensors.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1658 2023-04-25 15:36:11.000000 rosetta-ce-1.2.0/rosetta/constants/sources.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     6697 2023-04-25 15:36:11.000000 rosetta-ce-1.2.0/rosetta/constants/systems.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     3008 2023-04-26 09:01:43.000000 rosetta-ce-1.2.0/rosetta/rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)    32080 2023-06-26 16:13:20.000000 rosetta-ce-1.2.0/rosetta/rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     8012 2023-04-26 13:49:21.000000 rosetta-ce-1.2.0/rosetta/rsender.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-26 16:20:18.385047 rosetta-ce-1.2.0/rosetta_ce.egg-info/
+-rw-r--r--   0 amahmoud   (502) staff       (20)    11282 2023-06-26 16:20:18.000000 rosetta-ce-1.2.0/rosetta_ce.egg-info/PKG-INFO
+-rw-r--r--   0 amahmoud   (502) staff       (20)      459 2023-06-26 16:20:18.000000 rosetta-ce-1.2.0/rosetta_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        1 2023-06-26 16:20:18.000000 rosetta-ce-1.2.0/rosetta_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       23 2023-06-26 16:20:18.000000 rosetta-ce-1.2.0/rosetta_ce.egg-info/requires.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)        8 2023-06-26 16:20:18.000000 rosetta-ce-1.2.0/rosetta_ce.egg-info/top_level.txt
+-rw-r--r--   0 amahmoud   (502) staff       (20)       38 2023-06-26 16:20:18.387403 rosetta-ce-1.2.0/setup.cfg
+-rw-r--r--   0 amahmoud   (502) staff       (20)      851 2023-06-26 16:17:04.000000 rosetta-ce-1.2.0/setup.py
+drwxr-xr-x   0 amahmoud   (502) staff       (20)        0 2023-06-26 16:20:18.386542 rosetta-ce-1.2.0/tests/
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1040 2023-04-26 09:01:43.000000 rosetta-ce-1.2.0/tests/test_rconverter.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     5226 2023-04-25 15:36:11.000000 rosetta-ce-1.2.0/tests/test_rfaker.py
+-rw-r--r--   0 amahmoud   (502) staff       (20)     1763 2023-04-26 09:02:44.000000 rosetta-ce-1.2.0/tests/test_rsender.py
```

### Comparing `rosetta-ce-1.1.0/LICENSE` & `rosetta-ce-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.1.0/PKG-INFO` & `rosetta-ce-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.1.0
+Version: 1.2.0
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.1.0/README.md` & `rosetta-ce-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.1.0/rosetta/constants/sensors.py` & `rosetta-ce-1.2.0/rosetta/constants/sensors.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.1.0/rosetta/constants/sources.py` & `rosetta-ce-1.2.0/rosetta/constants/sources.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.1.0/rosetta/constants/systems.py` & `rosetta-ce-1.2.0/rosetta/constants/systems.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.1.0/rosetta/rconverter.py` & `rosetta-ce-1.2.0/rosetta/rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.1.0/rosetta/rfaker.py` & `rosetta-ce-1.2.0/rosetta/rfaker.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import ipaddress
 import json
 import csv
 import hashlib
 from enum import Enum
 from functools import reduce
 from faker import Faker
+from datetime import datetime, timedelta
 from typing import Optional, List
 from rosetta.constants.sources import BAD_IP_SOURCES, GOOD_IP_SOURCES, BAD_URL_SOURCES, GOOD_URL_SOURCES, \
     BAD_SHA256_SOURCES, GOOD_SHA256_SOURCES, CVE_SOURCES, TERMS_SOURCES
 from rosetta.constants.systems import UNIX_CMD, WINDOWS_CMD, WIN_PROCESSES, WIN_EVENTS, INCIDENTS_TYPES
 from rosetta.constants.sensors import ACTIONS, PROTOCOLS, TECHNIQUES, ERROR_CODE
 
 
@@ -253,39 +254,42 @@
         """
         Returns:
             Faker instance.
         """
         return Observables()
 
     @classmethod
-    def syslog(cls, count: int, observables: Optional[Observables] = None) -> List[str]:
+    def syslog(cls, count: int, timestamp: Optional[datetime] = None, observables: Optional[Observables] = None) -> List[str]:
         """
         Generate fake syslog messages.
 
         Args:
             count: The number of syslog messages to generate.
-            observables: An observables object. If not provided, random objservable will be generated and used.
-
+            timestamp: Optional. The starting timestamp for the syslog messages. If not provided, a random time during
+            the past hour from now will be used.
+            observables: Optional. An observables object. If not provided, random objservable will be generated and used.
         Returns:
             A list of syslog messages.
 
         Examples:
             >>> Events.syslog(5)
             ['Jan 01 05:32:48 myhostname sudo[1023]: username : COMMAND ; cat /etc/shadow',
-             'Feb 03 10:17:59 myhostname sudo[2019]: username : COMMAND ; find / -name \'*.log\' -exec rm -f {} \\;',
-             'Mar 12 22:46:16 myhostname sudo[3132]: username : COMMAND ; dd if=/dev/zero of=/dev/sda',
-             'Apr 07 02:08:08 myhostname sudo[4111]: username : COMMAND ; chmod -R 777 /',
-             'May 30 16:59:41 myhostname sudo[5195]: username : COMMAND ; chown -R nobody:nogroup /']
+             'Jan 01 05:17:59 myhostname sudo[2019]: username : COMMAND ; find / -name \'*.log\' -exec rm -f {} \\;',
+             'Jan 01 05:46:16 myhostname sudo[3132]: username : COMMAND ; dd if=/dev/zero of=/dev/sda',
+             'Jan 01 05:08:08 myhostname sudo[4111]: username : COMMAND ; chmod -R 777 /',
+             'Jan 01 05:59:41 myhostname sudo[5195]: username : COMMAND ; chown -R nobody:nogroup /']
 
         """
         syslog_messages = []
         faker = cls._create_faker()
-
+        if timestamp is None:
+            timestamp = datetime.now() - timedelta(hours=1)
+            timestamp += timedelta(seconds=faker.random_int(min=0, max=3599))
         for i in range(count):
-            timestamp = faker.date_time_this_year()
+            timestamp += timedelta(seconds=1)
             pid = faker.random_int(min=1000, max=65535)
             action = "COMMAND"
             host = random.choice(observables.src_host) if observables and observables.src_host \
                 else faker.hostname()
             user = random.choice(observables.user) if observables and observables.user \
                 else faker.user_name()
             process = random.choice(observables.process) if observables and observables.process \
@@ -293,20 +297,21 @@
             command = random.choice(observables.cmd) if observables and observables.cmd \
                 else random.choice(UNIX_CMD)
             syslog_messages.append(f"{timestamp.strftime('%b %d %H:%M:%S')} {host} {process}[{pid}]: {user}"
                                    f" : {action} ; {command}")
         return syslog_messages
 
     @classmethod
-    def cef(cls, count: int, observables: Optional[Observables] = None) -> List[str]:
+    def cef(cls, count: int, timestamp: Optional[datetime] = None, observables: Optional[Observables] = None) -> List[str]:
         """
         Generates fake CEF (Common Event Format) messages.
 
         Args:
             count: The number of CEF messages to generate.
+            timestamp: Optional. The starting timestamp for the syslog messages. If not provided, a random time during
             observables: An observables object. If not provided, random objservable will be generated and used.
         Returns:
             A list of fake CEF messages in string format.
 
         Raises:
             None.
 
@@ -321,15 +326,19 @@
              'CEF:0|Acme|Firewall|1.0.0|a3faedaa-5109-4849-b9ec-1ad6c5f8a5ec|Firewall ALLOW TCP traffic
              from example.com:25068 to 81.171.9.216:6157|2|src=example.com spt=25068 dst=81.171.9.216
              dpt=6157 proto=TCP act=ALLOW']
         """
         cef_messages = []
         faker = cls._create_faker()
         version = faker.numerify("1.0.#")
+        if timestamp is None:
+            timestamp = datetime.now() - timedelta(hours=1)
+            timestamp += timedelta(seconds=faker.random_int(min=0, max=3599))
         for i in range(count):
+            timestamp += timedelta(seconds=1)
             uuid = faker.uuid4()
             vendor = faker.company()
             src_port = faker.random_int(min=1024, max=65535)
             host = random.choice(observables.src_host) if observables and observables.src_host \
                 else faker.hostname()
             dst_ip = random.choice(observables.dst_ip) if observables and observables.dst_ip \
                 else Observables.generator(observable_type=ObservableType.IP, known=ObservableKnown.BAD, count=1)
@@ -340,26 +349,27 @@
             protocol = random.choice(observables.protocol) if observables and observables.protocol \
                 else random.choice(PROTOCOLS)
             action = random.choice(observables.action) if observables and observables.action \
                 else random.choice(ACTIONS)
             event_id = random.choice(observables.event_id) if observables and observables.event_id \
                 else faker.random_int(min=1, max=10)
             event_description = f"Firewall {action} {protocol} traffic from {host}:{src_port} to {dst_ip}:{dst_port}"
-            cef_messages.append(f"CEF:0|{vendor}|Firewall|{version}|{uuid}|{event_description}|"
-                                f"{event_id}|src={host} spt={src_port} dst={dst_ip} url={url} "
+            cef_messages.append(f"CEF:0|{vendor}|Firewall|{version}|{uuid}|{timestamp}|"
+                                f"{event_description}|{event_id}|src={host} spt={src_port} dst={dst_ip} url={url}"
                                 f"dpt={dst_port} proto={protocol} act={action}")
         return cef_messages
 
     @classmethod
-    def leef(cls, count, observables: Optional[Observables] = None) -> List[str]:
+    def leef(cls, count, timestamp: Optional[datetime] = None, observables: Optional[Observables] = None) -> List[str]:
         """
         Generates fake LEEF (Log Event Extended Format) messages.
 
         Parameters:
             count (int): The number of LEEF messages to generate.
+            timestamp: Optional. The starting timestamp for the syslog messages. If not provided, a random time during
             observables: An observables object. If not provided, random objservable will be generated and used.
 
         Returns:
             A list of generated LEEF messages.
 
         Example:
             To generate 10 fake LEEF messages:
@@ -374,16 +384,19 @@
              'LEEF:1.0|Leef|Payment Portal|1.0|192.168.0.1|mycomputer|08:00:27:da:2e:2e|08:00:27:da:2e:2f|src=10.0.0.2
               dst=mycomputer spt=57251 dpt=443 request=https://example.com/admin.php?sessionid=12345 method=POST
                proto=HTTP/1.1 status=404 request_size=1216 response_size=9729 user_agent=Mozilla/5.0
                (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3']
         """
         leef_messages = []
         faker = cls._create_faker()
-
+        if timestamp is None:
+            timestamp = datetime.now() - timedelta(hours=1)
+            timestamp += timedelta(seconds=faker.random_int(min=0, max=3599))
         for i in range(count):
+            timestamp += timedelta(seconds=1)
             src_port = faker.random_int(min=1024, max=65535)
             request_size = faker.random_int(min=100, max=10000)
             response_size = faker.random_int(min=100, max=10000)
             user_agent = faker.user_agent()
             host = random.choice(observables.src_host) if observables and observables.src_host \
                 else faker.hostname()
             src_ip = random.choice(observables.src_ip) if observables and observables.src_ip \
@@ -393,48 +406,52 @@
             file_hash = random.choice(observables.file_hash) if observables and observables.file_hash \
                 else Observables.generator(observable_type=ObservableType.SHA256, known=ObservableKnown.BAD, count=1)
             method = random.choice(observables.technique).get('mechanism') if observables and observables.technique \
                 else random.choice(TECHNIQUES).get('mechanism')
             error_code = random.choice(observables.error_code) if observables and observables.error_code \
                 else random.choice(ERROR_CODE)
 
-            leef_log = f"LEEF:1.0|Leef|Payment Portal|1.0|{faker.ipv4()}|{host}|{faker.mac_address()}|" \
-                       f"{faker.mac_address()}|"
+            leef_log = f"LEEF:1.0|Leef|Payment Portal|1.0|deviceEventDate={timestamp}|{faker.ipv4()}|{host}|" \
+                       f"{faker.mac_address()}|{faker.mac_address()}|"
             leef_log += f"src={src_ip} dst={host} spt={src_port} dpt=443 request={url} "
             leef_log += f"method={method} proto=HTTP/1.1 status={str(error_code)} hash={file_hash}"
             leef_log += f"request_size={request_size} " \
                         f"response_size={response_size} "
             leef_log += f"user_agent={user_agent}"
             leef_messages.append(leef_log)
         return leef_messages
 
     @classmethod
-    def winevent(cls, count, observables: Optional[Observables] = None) -> List[str]:
+    def winevent(cls, count, timestamp: Optional[datetime] = None, observables: Optional[Observables] = None) -> List[str]:
         """
         Generates fake Windows Event Log messages.
 
         Args:
             count (int): The number of fake messages to generate.
+            timestamp: Optional. The starting timestamp for the syslog messages. If not provided, a random time during
             observables: An observables object. If not provided, random objservable will be generated and used.
 
         Returns:
             list: A list of fake Windows Event Log messages.
 
         Examples:
             >>> Events.winevent(1)
             ['<Event xmlns="http://schemas.microsoft.com/win/2004/08/events/event">...</Event>', ...]
         """
         winevent_messages = []
         faker = cls._create_faker()
-
+        if timestamp is None:
+            timestamp = datetime.now() - timedelta(hours=1)
+            timestamp += timedelta(seconds=faker.random_int(min=0, max=3599))
         for i in range(count):
+            timestamp += timedelta(seconds=1)
             guid = faker.uuid4()
             src_port = faker.random_int(min=1024, max=65535)
             transmitted_services = faker.sentence(nb_words=5)
-            system_time = faker.date_time_this_year().isoformat()
+            system_time = timestamp
             process_id = faker.random_int()
             new_process_id = faker.random_int()
             thread_id = faker.random_int()
             target_pid = faker.random_int()
             domain_name = faker.domain_name()
             subject_login_id = faker.random_int()
             user_id = "S-1-" + str(faker.random_int())
@@ -464,36 +481,41 @@
                                                  destination_login_id=destination_login_id,
                                                  source_network_address=source_network_address, source_port=src_port,
                                                  transmitted_services=transmitted_services, file_name=file_name)
             winevent_messages.append(win_event)
         return winevent_messages
 
     @classmethod
-    def json(cls, count, observables: Optional[Observables] = None) -> List[dict]:
+    def json(cls, count, timestamp: Optional[datetime] = None, observables: Optional[Observables] = None) -> List[dict]:
         """
         Generate fake JSON messages representing discovered vulnerabilities.
 
         Args:
             count (int): The number of JSON messages to generate.
+            timestamp: Optional. The starting timestamp for the syslog messages. If not provided, a random time during
             observables: An observables object. If not provided, random objservable will be generated and used.
         Returns:
             List[Dict[str, Union[str, int]]]: A list of dictionaries representing the generated JSON messages.
 
         Example:
             >>> fake_messages = json(5)
             >>> len(fake_messages)
             5
             >>> isinstance(fake_messages[0], dict)
             True
 
         """
+        if timestamp is None:
+            timestamp = datetime.now() - timedelta(hours=1)
+            timestamp += timedelta(seconds=faker.random_int(min=0, max=3599))
         json_messages = []
         faker = cls._create_faker()
         for i in range(count):
-            system_time = faker.date_time_this_year().isoformat()
+            timestamp += timedelta(seconds=1)
+            system_time = timestamp
             cve_id = random.choice(observables.cve) if observables and observables.cve \
                 else Observables.generator(observable_type=ObservableType.CVE, count=1)
             host = random.choice(observables.src_host) if observables and observables.src_host \
                 else faker.hostname()
             severity = random.choice(observables.severity) if observables and observables.severity \
                 else faker.random_int(min=1, max=5)
             file_hash = random.choice(observables.file_hash) if observables and observables.file_hash \
```

### Comparing `rosetta-ce-1.1.0/rosetta/rsender.py` & `rosetta-ce-1.2.0/rosetta/rsender.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.1.0/rosetta_ce.egg-info/PKG-INFO` & `rosetta-ce-1.2.0/rosetta_ce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosetta-ce
-Version: 1.1.0
+Version: 1.2.0
 Summary: Rosetta is a Python package that can be used to fake security logs and alerts for testing different detection and response use cases.
 Home-page: https://github.com/ayman-m/rosetta
 Author: Ayman Mahmoud
 Author-email: content@ayman.online
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rosetta-ce-1.1.0/setup.py` & `rosetta-ce-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rosetta-ce",
-    version="1.1.0",
+    version="1.2.0",
     author="Ayman Mahmoud",
     author_email="content@ayman.online",
     description="Rosetta is a Python package that can be used to fake security logs and alerts for testing different "
                 "detection and response use cases.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ayman-m/rosetta",
```

### Comparing `rosetta-ce-1.1.0/tests/test_rconverter.py` & `rosetta-ce-1.2.0/tests/test_rconverter.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.1.0/tests/test_rfaker.py` & `rosetta-ce-1.2.0/tests/test_rfaker.py`

 * *Files identical despite different names*

### Comparing `rosetta-ce-1.1.0/tests/test_rsender.py` & `rosetta-ce-1.2.0/tests/test_rsender.py`

 * *Files identical despite different names*

