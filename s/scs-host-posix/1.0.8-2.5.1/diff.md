# Comparing `tmp/scs-host-posix-1.0.8.tar.gz` & `tmp/scs-host-posix-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs-host-posix-1.0.8.tar", last modified: Wed Sep 15 08:44:22 2021, max compression
+gzip compressed data, was "scs-host-posix-2.5.1.tar", last modified: Mon Jun 26 10:32:49 2023, max compression
```

## Comparing `scs-host-posix-1.0.8.tar` & `scs-host-posix-2.5.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 jade      (1000) jade      (1000)        0 2021-09-15 08:44:22.819261 scs-host-posix-1.0.8/
--rw-rw-r--   0 jade      (1000) jade      (1000)     1076 2020-12-23 11:43:26.000000 scs-host-posix-1.0.8/LICENSE
--rw-rw-r--   0 jade      (1000) jade      (1000)       32 2021-09-15 08:44:09.000000 scs-host-posix-1.0.8/MANIFEST.in
--rw-rw-r--   0 jade      (1000) jade      (1000)     1231 2021-09-15 08:44:22.819261 scs-host-posix-1.0.8/PKG-INFO
--rw-rw-r--   0 jade      (1000) jade      (1000)      504 2020-12-23 11:43:26.000000 scs-host-posix-1.0.8/README.md
--rw-rw-r--   0 jade      (1000) jade      (1000)        0 2020-12-23 11:43:26.000000 scs-host-posix-1.0.8/README.rst
--rw-rw-r--   0 jade      (1000) jade      (1000)       16 2021-06-08 09:08:15.000000 scs-host-posix-1.0.8/requirements.txt
--rw-rw-r--   0 jade      (1000) jade      (1000)       38 2021-09-15 08:44:22.819261 scs-host-posix-1.0.8/setup.cfg
--rwxrwxr-x   0 jade      (1000) jade      (1000)     2049 2021-09-15 08:44:09.000000 scs-host-posix-1.0.8/setup.py
-drwxrwxr-x   0 jade      (1000) jade      (1000)        0 2021-09-15 08:44:22.815261 scs-host-posix-1.0.8/src/
-drwxrwxr-x   0 jade      (1000) jade      (1000)        0 2021-09-15 08:44:22.815261 scs-host-posix-1.0.8/src/scs_host/
--rw-rw-r--   0 jade      (1000) jade      (1000)      183 2021-09-15 07:48:01.000000 scs-host-posix-1.0.8/src/scs_host/__init__.py
-drwxrwxr-x   0 jade      (1000) jade      (1000)        0 2021-09-15 08:44:22.819261 scs-host-posix-1.0.8/src/scs_host/client/
--rw-rw-r--   0 jade      (1000) jade      (1000)        0 2020-12-23 11:43:26.000000 scs-host-posix-1.0.8/src/scs_host/client/__init__.py
--rw-rw-r--   0 jade      (1000) jade      (1000)     1865 2020-12-23 11:43:26.000000 scs-host-posix-1.0.8/src/scs_host/client/http_streaming_client.py
--rw-rw-r--   0 jade      (1000) jade      (1000)     4757 2020-12-23 11:43:26.000000 scs-host-posix-1.0.8/src/scs_host/client/mqtt_client.py
--rw-rw-r--   0 jade      (1000) jade      (1000)     3209 2020-12-23 11:43:26.000000 scs-host-posix-1.0.8/src/scs_host/client/sftp_client.py
-drwxrwxr-x   0 jade      (1000) jade      (1000)        0 2021-09-15 08:44:22.819261 scs-host-posix-1.0.8/src/scs_host/comms/
--rw-rw-r--   0 jade      (1000) jade      (1000)        0 2020-12-23 11:43:26.000000 scs-host-posix-1.0.8/src/scs_host/comms/__init__.py
--rw-rw-r--   0 jade      (1000) jade      (1000)     4972 2021-09-15 07:48:01.000000 scs-host-posix-1.0.8/src/scs_host/comms/domain_socket.py
--rw-rw-r--   0 jade      (1000) jade      (1000)     3433 2021-09-15 07:48:01.000000 scs-host-posix-1.0.8/src/scs_host/comms/network_socket.py
--rw-rw-r--   0 jade      (1000) jade      (1000)     3260 2021-09-15 07:48:01.000000 scs-host-posix-1.0.8/src/scs_host/comms/stdio.py
-drwxrwxr-x   0 jade      (1000) jade      (1000)        0 2021-09-15 08:44:22.819261 scs-host-posix-1.0.8/src/scs_host/sys/
--rw-rw-r--   0 jade      (1000) jade      (1000)        0 2020-12-23 11:43:26.000000 scs-host-posix-1.0.8/src/scs_host/sys/__init__.py
--rw-rw-r--   0 jade      (1000) jade      (1000)     2452 2021-09-15 07:48:01.000000 scs-host-posix-1.0.8/src/scs_host/sys/host.py
-drwxrwxr-x   0 jade      (1000) jade      (1000)        0 2021-09-15 08:44:22.819261 scs-host-posix-1.0.8/src/scs_host_posix.egg-info/
--rw-rw-r--   0 jade      (1000) jade      (1000)     1231 2021-09-15 08:44:22.000000 scs-host-posix-1.0.8/src/scs_host_posix.egg-info/PKG-INFO
--rw-rw-r--   0 jade      (1000) jade      (1000)      633 2021-09-15 08:44:22.000000 scs-host-posix-1.0.8/src/scs_host_posix.egg-info/SOURCES.txt
--rw-rw-r--   0 jade      (1000) jade      (1000)        1 2021-09-15 08:44:22.000000 scs-host-posix-1.0.8/src/scs_host_posix.egg-info/dependency_links.txt
--rw-rw-r--   0 jade      (1000) jade      (1000)       16 2021-09-15 08:44:22.000000 scs-host-posix-1.0.8/src/scs_host_posix.egg-info/requires.txt
--rw-rw-r--   0 jade      (1000) jade      (1000)        9 2021-09-15 08:44:22.000000 scs-host-posix-1.0.8/src/scs_host_posix.egg-info/top_level.txt
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:32:49.200132 scs-host-posix-2.5.1/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:07.000000 scs-host-posix-2.5.1/LICENSE
+-rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:07.000000 scs-host-posix-2.5.1/MANIFEST.in
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1212 2023-06-26 10:32:49.200132 scs-host-posix-2.5.1/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)      504 2022-08-17 09:53:07.000000 scs-host-posix-2.5.1/README.md
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:07.000000 scs-host-posix-2.5.1/README.rst
+-rw-rw-r--   0 jade      (1002) jade      (1002)       16 2023-06-26 10:32:32.000000 scs-host-posix-2.5.1/requirements.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-06-26 10:32:49.200132 scs-host-posix-2.5.1/setup.cfg
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2049 2022-08-17 09:53:07.000000 scs-host-posix-2.5.1/setup.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:32:49.196132 scs-host-posix-2.5.1/src/
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:32:49.196132 scs-host-posix-2.5.1/src/scs_host/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      183 2023-06-26 10:32:32.000000 scs-host-posix-2.5.1/src/scs_host/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:32:49.200132 scs-host-posix-2.5.1/src/scs_host/client/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:07.000000 scs-host-posix-2.5.1/src/scs_host/client/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1865 2022-08-17 09:53:07.000000 scs-host-posix-2.5.1/src/scs_host/client/http_streaming_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4757 2022-08-17 09:53:07.000000 scs-host-posix-2.5.1/src/scs_host/client/mqtt_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3209 2022-08-17 09:53:07.000000 scs-host-posix-2.5.1/src/scs_host/client/sftp_client.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:32:49.200132 scs-host-posix-2.5.1/src/scs_host/comms/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:07.000000 scs-host-posix-2.5.1/src/scs_host/comms/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4972 2022-08-17 09:53:07.000000 scs-host-posix-2.5.1/src/scs_host/comms/domain_socket.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3433 2022-08-17 09:53:07.000000 scs-host-posix-2.5.1/src/scs_host/comms/network_socket.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3821 2023-06-26 09:33:48.000000 scs-host-posix-2.5.1/src/scs_host/comms/stdio.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:32:49.200132 scs-host-posix-2.5.1/src/scs_host/sys/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:07.000000 scs-host-posix-2.5.1/src/scs_host/sys/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2463 2022-08-17 09:53:07.000000 scs-host-posix-2.5.1/src/scs_host/sys/host.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:32:49.200132 scs-host-posix-2.5.1/src/scs_host_posix.egg-info/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1212 2023-06-26 10:32:49.000000 scs-host-posix-2.5.1/src/scs_host_posix.egg-info/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)      633 2023-06-26 10:32:49.000000 scs-host-posix-2.5.1/src/scs_host_posix.egg-info/SOURCES.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-06-26 10:32:49.000000 scs-host-posix-2.5.1/src/scs_host_posix.egg-info/dependency_links.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)       16 2023-06-26 10:32:49.000000 scs-host-posix-2.5.1/src/scs_host_posix.egg-info/requires.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)        9 2023-06-26 10:32:49.000000 scs-host-posix-2.5.1/src/scs_host_posix.egg-info/top_level.txt
```

### Comparing `scs-host-posix-1.0.8/LICENSE` & `scs-host-posix-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scs-host-posix-1.0.8/PKG-INFO` & `scs-host-posix-2.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: scs-host-posix
-Version: 1.0.8
+Version: 2.5.1
 Summary: Host abstractions for data consumers running POSIX-compliant operating systems, including Windows 10.
 Home-page: https://github.com/south-coast-science/scs_host_posix
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
-License: UNKNOWN
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX
@@ -30,9 +29,7 @@
 
 
 **Branches:**
 
 The stable branch of this repository is master. For deployment purposes, use:
 
     git clone --branch=master https://github.com/south-coast-science/scs_host_posix.git
-
-
```

### Comparing `scs-host-posix-1.0.8/setup.py` & `scs-host-posix-2.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-1.0.8/src/scs_host/client/http_streaming_client.py` & `scs-host-posix-2.5.1/src/scs_host/client/http_streaming_client.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-1.0.8/src/scs_host/client/mqtt_client.py` & `scs-host-posix-2.5.1/src/scs_host/client/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-1.0.8/src/scs_host/client/sftp_client.py` & `scs-host-posix-2.5.1/src/scs_host/client/sftp_client.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-1.0.8/src/scs_host/comms/domain_socket.py` & `scs-host-posix-2.5.1/src/scs_host/comms/domain_socket.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-1.0.8/src/scs_host/comms/network_socket.py` & `scs-host-posix-2.5.1/src/scs_host/comms/network_socket.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-1.0.8/src/scs_host/comms/stdio.py` & `scs-host-posix-2.5.1/src/scs_host/comms/stdio.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 """
 
 import os
 import readline
 import sys
 import termios
 
+from getpass import getpass
+
+from scs_core.sys.filesystem import Filesystem
 from scs_core.sys.logging import Logging
 from scs_core.sys.process_comms import ProcessComms
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class StdIO(ProcessComms):
@@ -30,23 +33,38 @@
 
     __READLINE_COMPLETION_DEFAULT = 'tab: complete'
     __READLINE_COMPLETION_DARWIN = 'bind ^I rl_complete'
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @staticmethod
-    def prompt(prompt_str):
+    def prompt(request, default=None):
         try:
             termios.tcflush(sys.stdin, termios.TCIOFLUSH)           # flush stdin
         except termios.error:
             pass
 
+        try:
+            prompt_str = request + ' (%s): ' % default if default else request + ': '
+        except TypeError:
+            prompt_str = request + ': '            # no % format in request string
+
         line = input(prompt_str).strip()
 
-        return line.strip()
+        return line if line else default
+
+
+    @staticmethod
+    def password(request):
+        try:
+            termios.tcflush(sys.stdin, termios.TCIOFLUSH)           # flush stdin
+        except termios.error:
+            pass
+
+        return getpass(request).strip()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def set(cls, vocabulary=(), history_filename=None):
         # completion...
@@ -77,18 +95,19 @@
 
 
     @classmethod
     def load_history(cls, filename):
         if os.path.exists(filename):
             try:
                 readline.read_history_file(filename)
-            except PermissionError as ex:                         # macOS does this sometimes for no good reason
+            except PermissionError as ex:                     # macOS darwin does this sometimes for no good reason
                 logger = Logging.getLogger()
                 logger.error("PermissionError: %s: %s" % (filename, ex))
-                # Filesystem.rm(filename)
+                Filesystem.rm(filename)
+                pass
 
 
     @classmethod
     def save_history(cls, filename):
         readline.set_history_length(cls.__HISTORY_LENGTH)
         readline.write_history_file(filename)
```

### Comparing `scs-host-posix-1.0.8/src/scs_host/sys/host.py` & `scs-host-posix-2.5.1/src/scs_host/sys/host.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     __SCS_DIR =             "SCS"                               # hard-coded rel path
     __LATEST_UPDATE =       "latest_update.txt"                 # hard-coded rel path
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # host acting as DHCP server...
 
-    __SERVER_IPV4_ADDRESS =      None                           # had-coded abs path
+    __SERVER_IPV4_ADDRESS = "192.168.2.1"                       # had-coded abs path - was None
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # network identity...
 
     @classmethod
     def name(cls):
```

### Comparing `scs-host-posix-1.0.8/src/scs_host_posix.egg-info/PKG-INFO` & `scs-host-posix-2.5.1/src/scs_host_posix.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: scs-host-posix
-Version: 1.0.8
+Version: 2.5.1
 Summary: Host abstractions for data consumers running POSIX-compliant operating systems, including Windows 10.
 Home-page: https://github.com/south-coast-science/scs_host_posix
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
-License: UNKNOWN
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: POSIX
@@ -30,9 +29,7 @@
 
 
 **Branches:**
 
 The stable branch of this repository is master. For deployment purposes, use:
 
     git clone --branch=master https://github.com/south-coast-science/scs_host_posix.git
-
-
```

### Comparing `scs-host-posix-1.0.8/src/scs_host_posix.egg-info/SOURCES.txt` & `scs-host-posix-2.5.1/src/scs_host_posix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

