# Comparing `tmp/pyIndego-3.0.1.tar.gz` & `tmp/pyIndego-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyIndego-3.0.1.tar", last modified: Thu Apr 27 05:39:16 2023, max compression
+gzip compressed data, was "pyIndego-3.1.0.tar", last modified: Mon Jun 26 14:07:15 2023, max compression
```

## Comparing `pyIndego-3.0.1.tar` & `pyIndego-3.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 05:39:16.851784 pyIndego-3.0.1/
--rw-rw-rw-   0        0        0     1091 2023-04-26 19:17:02.000000 pyIndego-3.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0    21543 2023-04-27 05:39:16.850801 pyIndego-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    21093 2023-04-27 05:28:43.000000 pyIndego-3.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 05:39:16.783809 pyIndego-3.0.1/pyIndego/
--rw-rw-rw-   0        0        0      397 2023-04-26 19:17:02.000000 pyIndego-3.0.1/pyIndego/__init__.py
--rw-rw-rw-   0        0        0     6612 2023-04-27 05:28:43.000000 pyIndego-3.0.1/pyIndego/const.py
--rw-rw-rw-   0        0        0     2301 2023-04-26 19:17:02.000000 pyIndego-3.0.1/pyIndego/helpers.py
--rw-rw-rw-   0        0        0    20193 2023-04-27 05:28:43.000000 pyIndego-3.0.1/pyIndego/indego_async_client.py
--rw-rw-rw-   0        0        0    15805 2023-04-27 05:28:43.000000 pyIndego-3.0.1/pyIndego/indego_base_client.py
--rw-rw-rw-   0        0        0    15500 2023-04-27 05:28:43.000000 pyIndego-3.0.1/pyIndego/indego_client.py
--rw-rw-rw-   0        0        0     9103 2023-04-26 19:17:02.000000 pyIndego-3.0.1/pyIndego/states.py
-drwxrwxrwx   0        0        0        0 2023-04-27 05:39:16.830516 pyIndego-3.0.1/pyIndego.egg-info/
--rw-rw-rw-   0        0        0    21543 2023-04-27 05:39:16.000000 pyIndego-3.0.1/pyIndego.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2023-04-27 05:39:16.000000 pyIndego-3.0.1/pyIndego.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 05:39:16.000000 pyIndego-3.0.1/pyIndego.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-04-27 05:39:16.000000 pyIndego-3.0.1/pyIndego.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-27 05:39:16.000000 pyIndego-3.0.1/pyIndego.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 05:39:16.851784 pyIndego-3.0.1/setup.cfg
--rw-rw-rw-   0        0        0      821 2023-04-27 05:33:58.000000 pyIndego-3.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 05:39:16.846774 pyIndego-3.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-04-26 19:17:02.000000 pyIndego-3.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0    39869 2023-04-26 19:17:02.000000 pyIndego-3.0.1/tests/test_indego.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:07:15.459982 pyIndego-3.1.0/
+-rw-rw-rw-   0        0        0     1091 2023-04-26 19:17:02.000000 pyIndego-3.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0    21543 2023-06-26 14:07:15.459982 pyIndego-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    21093 2023-04-27 05:28:43.000000 pyIndego-3.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 14:07:15.419804 pyIndego-3.1.0/pyIndego/
+-rw-rw-rw-   0        0        0      397 2023-04-26 19:17:02.000000 pyIndego-3.1.0/pyIndego/__init__.py
+-rw-rw-rw-   0        0        0     6803 2023-06-26 13:58:41.000000 pyIndego-3.1.0/pyIndego/const.py
+-rw-rw-rw-   0        0        0     2301 2023-04-26 19:17:02.000000 pyIndego-3.1.0/pyIndego/helpers.py
+-rw-rw-rw-   0        0        0    20193 2023-04-27 05:28:43.000000 pyIndego-3.1.0/pyIndego/indego_async_client.py
+-rw-rw-rw-   0        0        0    15805 2023-04-27 05:28:43.000000 pyIndego-3.1.0/pyIndego/indego_base_client.py
+-rw-rw-rw-   0        0        0    15500 2023-04-27 05:28:43.000000 pyIndego-3.1.0/pyIndego/indego_client.py
+-rw-rw-rw-   0        0        0     9103 2023-04-26 19:17:02.000000 pyIndego-3.1.0/pyIndego/states.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:07:15.448425 pyIndego-3.1.0/pyIndego.egg-info/
+-rw-rw-rw-   0        0        0    21543 2023-06-26 14:07:15.000000 pyIndego-3.1.0/pyIndego.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-06-26 14:07:15.000000 pyIndego-3.1.0/pyIndego.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 14:07:15.000000 pyIndego-3.1.0/pyIndego.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-06-26 14:07:15.000000 pyIndego-3.1.0/pyIndego.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-26 14:07:15.000000 pyIndego-3.1.0/pyIndego.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 14:07:15.459982 pyIndego-3.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      821 2023-06-26 14:01:32.000000 pyIndego-3.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:07:15.458312 pyIndego-3.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-26 19:17:02.000000 pyIndego-3.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0    39869 2023-04-26 19:17:02.000000 pyIndego-3.1.0/tests/test_indego.py
```

### Comparing `pyIndego-3.0.1/LICENSE.txt` & `pyIndego-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyIndego-3.0.1/PKG-INFO` & `pyIndego-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyIndego
-Version: 3.0.1
+Version: 3.1.0
 Summary: API for Bosch Indego mower
 Home-page: https://github.com/jm-73/pyIndego
 Author: jm-73, sander1988
 Author-email: jens@myretyr.se
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyIndego-3.0.1/README.md` & `pyIndego-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyIndego-3.0.1/pyIndego/const.py` & `pyIndego-3.1.0/pyIndego/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Constants for pyIndego."""
 from enum import Enum
-
+import random
+import string
 
 class Methods(Enum):
     """Enum with HTTP methods."""
 
     GET = "GET"
     POST = "POST"
     PUT = "PUT"
@@ -19,15 +20,16 @@
 CONTENT_TYPE = "Content-Type"
 COMMANDS = ("mow", "pause", "returnToDock")
 
 DEFAULT_HEADER = {
     CONTENT_TYPE: CONTENT_TYPE_JSON,
     # We need to change the user-agent!
     # The Microsoft Azure proxy seems to block all requests (HTTP 403) for the default 'python-requests' user-agent.
-    "User-Agent": "pyIndego"
+    # We also need to use a random agent for each client: https://github.com/jm-73/pyIndego/issues/119
+    "User-Agent": ''.join(random.choices(string.ascii_uppercase + string.digits, k=12))
 }
 DEFAULT_LOOKUP_VALUE = "Not in database."
 
 DEFAULT_CALENDAR = {
     "sel_cal": 1,
     "cals": [
         {
```

### Comparing `pyIndego-3.0.1/pyIndego/helpers.py` & `pyIndego-3.1.0/pyIndego/helpers.py`

 * *Files identical despite different names*

### Comparing `pyIndego-3.0.1/pyIndego/indego_async_client.py` & `pyIndego-3.1.0/pyIndego/indego_async_client.py`

 * *Files identical despite different names*

### Comparing `pyIndego-3.0.1/pyIndego/indego_base_client.py` & `pyIndego-3.1.0/pyIndego/indego_base_client.py`

 * *Files identical despite different names*

### Comparing `pyIndego-3.0.1/pyIndego/indego_client.py` & `pyIndego-3.1.0/pyIndego/indego_client.py`

 * *Files identical despite different names*

### Comparing `pyIndego-3.0.1/pyIndego/states.py` & `pyIndego-3.1.0/pyIndego/states.py`

 * *Files identical despite different names*

### Comparing `pyIndego-3.0.1/pyIndego.egg-info/PKG-INFO` & `pyIndego-3.1.0/pyIndego.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyIndego
-Version: 3.0.1
+Version: 3.1.0
 Summary: API for Bosch Indego mower
 Home-page: https://github.com/jm-73/pyIndego
 Author: jm-73, sander1988
 Author-email: jens@myretyr.se
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyIndego-3.0.1/setup.py` & `pyIndego-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pyIndego",
-    version="3.0.1",
+    version="3.1.0",
     author="jm-73, sander1988",
     author_email="jens@myretyr.se",
     description="API for Bosch Indego mower",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jm-73/pyIndego",
     packages=find_packages("."),
```

### Comparing `pyIndego-3.0.1/tests/test_indego.py` & `pyIndego-3.1.0/tests/test_indego.py`

 * *Files identical despite different names*

