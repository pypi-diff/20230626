# Comparing `tmp/pyporscheconnectapi-0.1.4.tar.gz` & `tmp/pyporscheconnectapi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyporscheconnectapi-0.1.4.tar", last modified: Mon Jun 26 13:26:54 2023, max compression
+gzip compressed data, was "pyporscheconnectapi-0.1.5.tar", last modified: Mon Jun 26 15:15:50 2023, max compression
```

## Comparing `pyporscheconnectapi-0.1.4.tar` & `pyporscheconnectapi-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:54.652121 pyporscheconnectapi-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 13:26:44.000000 pyporscheconnectapi-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-26 13:26:54.652121 pyporscheconnectapi-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-26 13:26:44.000000 pyporscheconnectapi-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:54.652121 pyporscheconnectapi-0.1.4/pyporscheconnectapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:44.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10930 2023-06-26 13:26:44.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    19908 2023-06-26 13:26:44.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-06-26 13:26:44.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-26 13:26:44.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:54.652121 pyporscheconnectapi-0.1.4/pyporscheconnectapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-26 13:26:54.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-26 13:26:54.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:26:54.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 13:26:54.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 13:26:54.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 13:26:54.000000 pyporscheconnectapi-0.1.4/pyporscheconnectapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-26 13:26:54.652121 pyporscheconnectapi-0.1.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      951 2023-06-26 13:26:44.000000 pyporscheconnectapi-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:50.810182 pyporscheconnectapi-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 15:15:39.000000 pyporscheconnectapi-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-26 15:15:50.810182 pyporscheconnectapi-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-26 15:15:39.000000 pyporscheconnectapi-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:50.810182 pyporscheconnectapi-0.1.5/pyporscheconnectapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:39.000000 pyporscheconnectapi-0.1.5/pyporscheconnectapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10930 2023-06-26 15:15:39.000000 pyporscheconnectapi-0.1.5/pyporscheconnectapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19940 2023-06-26 15:15:39.000000 pyporscheconnectapi-0.1.5/pyporscheconnectapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-06-26 15:15:39.000000 pyporscheconnectapi-0.1.5/pyporscheconnectapi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-26 15:15:39.000000 pyporscheconnectapi-0.1.5/pyporscheconnectapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:50.810182 pyporscheconnectapi-0.1.5/pyporscheconnectapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-26 15:15:50.000000 pyporscheconnectapi-0.1.5/pyporscheconnectapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-26 15:15:50.000000 pyporscheconnectapi-0.1.5/pyporscheconnectapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:15:50.000000 pyporscheconnectapi-0.1.5/pyporscheconnectapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 15:15:50.000000 pyporscheconnectapi-0.1.5/pyporscheconnectapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 15:15:50.000000 pyporscheconnectapi-0.1.5/pyporscheconnectapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 15:15:50.000000 pyporscheconnectapi-0.1.5/pyporscheconnectapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-26 15:15:50.810182 pyporscheconnectapi-0.1.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      951 2023-06-26 15:15:39.000000 pyporscheconnectapi-0.1.5/setup.py
```

### Comparing `pyporscheconnectapi-0.1.4/LICENSE` & `pyporscheconnectapi-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.1.4/PKG-INFO` & `pyporscheconnectapi-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyporscheconnectapi
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python library and CLI for communicating with Porsche Connect API.
 Home-page: https://github.com/cjne/pyporscheconnectapi
 Author: Johan Isaksson
 Author-email: johan@generatorhallen.se
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pyporscheconnectapi-0.1.4/README.md` & `pyporscheconnectapi-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.1.4/pyporscheconnectapi/cli.py` & `pyporscheconnectapi-0.1.5/pyporscheconnectapi/cli.py`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.1.4/pyporscheconnectapi/client.py` & `pyporscheconnectapi-0.1.5/pyporscheconnectapi/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,21 +94,21 @@
         model=None,
         waitForConfirmation=True,
     ):
         if model is None:
             data = await self.getCapabilities(vin)
             model = data["carModel"]
         progressResult = await self._connection.post(
-            f"https://api.porsche.com/e-mobility/{self.locale_str}/{model}/{vin}/toggle-direct-charging/{action}",
+            f"https://api.porsche.com/e-mobility/{self.locale_str}/{model}/{vin}/toggle-direct-charging/{action}?hasDX1=false",
             json={},
         )
         if not waitForConfirmation:
             return progressResult
         result = await self._spinner(
-            f"https://api.porsche.com/e-mobility/{self.locale_str}/{model}/{vin}/toggle-direct-charging/status/{progressResult['requestId']}"
+            f"https://api.porsche.com/e-mobility/{self.locale_str}/{model}/{vin}/toggle-direct-charging/status/{progressResult['requestId']}?toggledOn={action}"
         )
         return result
 
     async def _setHonkAndFlash(self, vin, waitForConfirmation=True):
         progressResult = await self._connection.post(
             f"https://api.porsche.com/service-vehicle/honk-and-flash/{vin}/honk-and-flash",
             json={},
```

### Comparing `pyporscheconnectapi-0.1.4/pyporscheconnectapi/connection.py` & `pyporscheconnectapi-0.1.5/pyporscheconnectapi/connection.py`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.1.4/pyporscheconnectapi/exceptions.py` & `pyporscheconnectapi-0.1.5/pyporscheconnectapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyporscheconnectapi-0.1.4/pyporscheconnectapi.egg-info/PKG-INFO` & `pyporscheconnectapi-0.1.5/pyporscheconnectapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyporscheconnectapi
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python library and CLI for communicating with Porsche Connect API.
 Home-page: https://github.com/cjne/pyporscheconnectapi
 Author: Johan Isaksson
 Author-email: johan@generatorhallen.se
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `pyporscheconnectapi-0.1.4/setup.py` & `pyporscheconnectapi-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 
 setup(
     name="pyporscheconnectapi",
-    version="0.1.4",
+    version="0.1.5",
     author="Johan Isaksson",
     author_email="johan@generatorhallen.se",
     description="Python library and CLI for communicating with Porsche Connect API.",
     long_description=open("README.md", 'r').read(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     url="https://github.com/cjne/pyporscheconnectapi",
```

