# Comparing `tmp/arkdriver-1.0.8.tar.gz` & `tmp/arkdriver-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkdriver-1.0.8.tar", last modified: Wed May 10 06:36:52 2023, max compression
+gzip compressed data, was "arkdriver-1.0.9.tar", last modified: Wed May 10 06:39:46 2023, max compression
```

## Comparing `arkdriver-1.0.8.tar` & `arkdriver-1.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 06:36:52.555234 arkdriver-1.0.8/
--rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:50.000000 arkdriver-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     1935 2023-05-10 06:36:52.555234 arkdriver-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1305 2023-03-25 16:35:50.000000 arkdriver-1.0.8/README.md
--rw-rw-rw-   0        0        0      690 2023-05-10 06:36:29.000000 arkdriver-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0     1201 2023-05-10 06:36:52.557234 arkdriver-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-10 06:36:52.521376 arkdriver-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 06:36:52.528376 arkdriver-1.0.8/src/arkdriver/
--rw-rw-rw-   0        0        0      102 2023-04-27 01:08:24.000000 arkdriver-1.0.8/src/arkdriver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:36:52.549234 arkdriver-1.0.8/src/arkdriver/driver/
--rw-rw-rw-   0        0        0      182 2023-04-21 03:31:49.000000 arkdriver-1.0.8/src/arkdriver/driver/__init__.py
--rw-rw-rw-   0        0        0    10696 2023-04-14 00:06:06.000000 arkdriver-1.0.8/src/arkdriver/driver/application.py
--rw-rw-rw-   0        0        0     2830 2023-03-31 21:05:16.000000 arkdriver-1.0.8/src/arkdriver/driver/driver.py
--rw-rw-rw-   0        0        0     4177 2023-05-10 05:06:47.000000 arkdriver-1.0.8/src/arkdriver/driver/run.py
--rw-rw-rw-   0        0        0     4657 2023-04-30 23:44:23.000000 arkdriver-1.0.8/src/arkdriver/main.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:36:52.551234 arkdriver-1.0.8/src/arkdriver/presentation/
--rw-rw-rw-   0        0        0        0 2023-03-31 07:17:37.000000 arkdriver-1.0.8/src/arkdriver/presentation/__init__.py
--rw-rw-rw-   0        0        0    12071 2023-04-02 00:47:11.000000 arkdriver-1.0.8/src/arkdriver/presentation/presentation.py
--rw-rw-rw-   0        0        0        0 2023-03-25 16:35:50.000000 arkdriver-1.0.8/src/arkdriver/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-10 06:36:52.553234 arkdriver-1.0.8/src/arkdriver/session/
--rw-rw-rw-   0        0        0        0 2023-04-30 23:29:41.000000 arkdriver-1.0.8/src/arkdriver/session/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-04-30 23:48:48.000000 arkdriver-1.0.8/src/arkdriver/session/session.py
-drwxrwxrwx   0        0        0        0 2023-05-10 06:36:52.546234 arkdriver-1.0.8/src/arkdriver.egg-info/
--rw-rw-rw-   0        0        0     1935 2023-05-10 06:36:52.000000 arkdriver-1.0.8/src/arkdriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-10 06:36:52.000000 arkdriver-1.0.8/src/arkdriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 06:36:52.000000 arkdriver-1.0.8/src/arkdriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      170 2023-05-10 06:36:52.000000 arkdriver-1.0.8/src/arkdriver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-10 06:36:52.000000 arkdriver-1.0.8/src/arkdriver.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-10 06:36:52.555234 arkdriver-1.0.8/tests/
--rw-rw-rw-   0        0        0      342 2023-03-25 16:35:50.000000 arkdriver-1.0.8/tests/test_lib.py
--rw-rw-rw-   0        0        0      580 2023-03-25 16:35:50.000000 arkdriver-1.0.8/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:39:46.727216 arkdriver-1.0.9/
+-rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:50.000000 arkdriver-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1935 2023-05-10 06:39:46.727216 arkdriver-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1305 2023-03-25 16:35:50.000000 arkdriver-1.0.9/README.md
+-rw-rw-rw-   0        0        0      690 2023-05-10 06:36:29.000000 arkdriver-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1201 2023-05-10 06:39:46.733216 arkdriver-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 06:39:46.695216 arkdriver-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 06:39:46.703216 arkdriver-1.0.9/src/arkdriver/
+-rw-rw-rw-   0        0        0      102 2023-04-27 01:08:24.000000 arkdriver-1.0.9/src/arkdriver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:39:46.721216 arkdriver-1.0.9/src/arkdriver/driver/
+-rw-rw-rw-   0        0        0      182 2023-04-21 03:31:49.000000 arkdriver-1.0.9/src/arkdriver/driver/__init__.py
+-rw-rw-rw-   0        0        0    10696 2023-04-14 00:06:06.000000 arkdriver-1.0.9/src/arkdriver/driver/application.py
+-rw-rw-rw-   0        0        0     2830 2023-03-31 21:05:16.000000 arkdriver-1.0.9/src/arkdriver/driver/driver.py
+-rw-rw-rw-   0        0        0     4177 2023-05-10 05:06:47.000000 arkdriver-1.0.9/src/arkdriver/driver/run.py
+-rw-rw-rw-   0        0        0     4657 2023-04-30 23:44:23.000000 arkdriver-1.0.9/src/arkdriver/main.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:39:46.723219 arkdriver-1.0.9/src/arkdriver/presentation/
+-rw-rw-rw-   0        0        0        0 2023-03-31 07:17:37.000000 arkdriver-1.0.9/src/arkdriver/presentation/__init__.py
+-rw-rw-rw-   0        0        0    12071 2023-04-02 00:47:11.000000 arkdriver-1.0.9/src/arkdriver/presentation/presentation.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:35:50.000000 arkdriver-1.0.9/src/arkdriver/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-10 06:39:46.724216 arkdriver-1.0.9/src/arkdriver/session/
+-rw-rw-rw-   0        0        0        0 2023-04-30 23:29:41.000000 arkdriver-1.0.9/src/arkdriver/session/__init__.py
+-rw-rw-rw-   0        0        0     1927 2023-05-10 06:39:24.000000 arkdriver-1.0.9/src/arkdriver/session/session.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:39:46.718216 arkdriver-1.0.9/src/arkdriver.egg-info/
+-rw-rw-rw-   0        0        0     1935 2023-05-10 06:39:46.000000 arkdriver-1.0.9/src/arkdriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-10 06:39:46.000000 arkdriver-1.0.9/src/arkdriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 06:39:46.000000 arkdriver-1.0.9/src/arkdriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      170 2023-05-10 06:39:46.000000 arkdriver-1.0.9/src/arkdriver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-10 06:39:46.000000 arkdriver-1.0.9/src/arkdriver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 06:39:46.726216 arkdriver-1.0.9/tests/
+-rw-rw-rw-   0        0        0      342 2023-03-25 16:35:50.000000 arkdriver-1.0.9/tests/test_lib.py
+-rw-rw-rw-   0        0        0      580 2023-03-25 16:35:50.000000 arkdriver-1.0.9/tests/test_main.py
```

### Comparing `arkdriver-1.0.8/LICENSE` & `arkdriver-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.8/PKG-INFO` & `arkdriver-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkdriver
-Version: 1.0.8
+Version: 1.0.9
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/mjlomeli/arkdriver
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/arkdriver/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arkdriver-1.0.8/README.md` & `arkdriver-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.8/pyproject.toml` & `arkdriver-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.8/setup.cfg` & `arkdriver-1.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 726b 6472 6976 6572 0d0a 7665   = arkdriver..ve
-00000020: 7273 696f 6e20 3d20 312e 302e 380d 0a74  rsion = 1.0.8..t
+00000020: 7273 696f 6e20 3d20 312e 302e 390d 0a74  rsion = 1.0.9..t
 00000030: 6573 745f 7665 7273 696f 6e20 3d20 312e  est_version = 1.
 00000040: 302e 370d 0a70 726f 6475 6374 696f 6e5f  0.7..production_
-00000050: 7665 7273 696f 6e20 3d20 312e 302e 380d  version = 1.0.8.
+00000050: 7665 7273 696f 6e20 3d20 312e 302e 390d  version = 1.0.9.
 00000060: 0a61 7574 686f 7220 3d20 4d61 7572 6963  .author = Mauric
 00000070: 696f 0d0a 6175 7468 6f72 5f65 6d61 696c  io..author_email
 00000080: 203d 2064 6576 2e6d 6175 7269 6369 6f2e   = dev.mauricio.
 00000090: 6c6f 6d65 6c69 4067 6d61 696c 2e63 6f6d  lomeli@gmail.com
 000000a0: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 000000b0: 5468 6973 2061 7070 6c69 6361 7469 6f6e  This application
 000000c0: 2061 6363 6573 7365 7320 7468 6520 4172   accesses the Ar
```

### Comparing `arkdriver-1.0.8/src/arkdriver/driver/application.py` & `arkdriver-1.0.9/src/arkdriver/driver/application.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.8/src/arkdriver/driver/driver.py` & `arkdriver-1.0.9/src/arkdriver/driver/driver.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.8/src/arkdriver/driver/run.py` & `arkdriver-1.0.9/src/arkdriver/driver/run.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.8/src/arkdriver/main.py` & `arkdriver-1.0.9/src/arkdriver/main.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.8/src/arkdriver/presentation/presentation.py` & `arkdriver-1.0.9/src/arkdriver/presentation/presentation.py`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.8/src/arkdriver/session/session.py` & `arkdriver-1.0.9/src/arkdriver/session/session.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import requests
 import os
 import webbrowser
 import secrets
 from time import sleep
 import tempfile
-import webbrowser
-import jinja2
 from io import BytesIO
 
 
 def authenticate(domain: str, security_token: str, timeout=60) -> dict:
     """Returns the driver token and gamertag"""
     data = {'security_token': security_token}
     seconds_wait = 5
```

### Comparing `arkdriver-1.0.8/src/arkdriver.egg-info/PKG-INFO` & `arkdriver-1.0.9/src/arkdriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkdriver
-Version: 1.0.8
+Version: 1.0.9
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/mjlomeli/arkdriver
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/mjlomeli/arkdriver/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arkdriver-1.0.8/src/arkdriver.egg-info/SOURCES.txt` & `arkdriver-1.0.9/src/arkdriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arkdriver-1.0.8/tests/test_main.py` & `arkdriver-1.0.9/tests/test_main.py`

 * *Files identical despite different names*

