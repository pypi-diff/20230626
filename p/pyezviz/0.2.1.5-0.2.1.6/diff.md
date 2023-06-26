# Comparing `tmp/pyezviz-0.2.1.5.tar.gz` & `tmp/pyezviz-0.2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyezviz-0.2.1.5.tar", last modified: Sun Jun 25 18:27:08 2023, max compression
+gzip compressed data, was "pyezviz-0.2.1.6.tar", last modified: Mon Jun 26 05:50:06 2023, max compression
```

## Comparing `pyezviz-0.2.1.5.tar` & `pyezviz-0.2.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:27:08.119688 pyezviz-0.2.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-25 18:27:08.115688 pyezviz-0.2.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:27:08.115688 pyezviz-0.2.1.5/pyezviz/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/api_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/cas.py
--rw-r--r--   0 runner    (1001) docker     (123)    59873 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/test_cam_rtsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/pyezviz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 18:27:08.115688 pyezviz-0.2.1.5/pyezviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-25 18:27:08.000000 pyezviz-0.2.1.5/pyezviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-25 18:27:08.000000 pyezviz-0.2.1.5/pyezviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 18:27:08.000000 pyezviz-0.2.1.5/pyezviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-25 18:27:08.000000 pyezviz-0.2.1.5/pyezviz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 18:27:08.000000 pyezviz-0.2.1.5/pyezviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 18:27:08.000000 pyezviz-0.2.1.5/pyezviz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 18:27:08.119688 pyezviz-0.2.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-25 18:26:55.000000 pyezviz-0.2.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:50:06.358931 pyezviz-0.2.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-26 05:50:06.358931 pyezviz-0.2.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:50:06.358931 pyezviz-0.2.1.6/pyezviz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/api_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/cas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60024 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/test_cam_rtsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/pyezviz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:50:06.358931 pyezviz-0.2.1.6/pyezviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-26 05:50:06.000000 pyezviz-0.2.1.6/pyezviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-26 05:50:06.000000 pyezviz-0.2.1.6/pyezviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 05:50:06.000000 pyezviz-0.2.1.6/pyezviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 05:50:06.000000 pyezviz-0.2.1.6/pyezviz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 05:50:06.000000 pyezviz-0.2.1.6/pyezviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 05:50:06.000000 pyezviz-0.2.1.6/pyezviz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 05:50:06.358931 pyezviz-0.2.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-26 05:49:55.000000 pyezviz-0.2.1.6/setup.py
```

### Comparing `pyezviz-0.2.1.5/LICENSE.md` & `pyezviz-0.2.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.5/README.md` & `pyezviz-0.2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.5/pyezviz/__init__.py` & `pyezviz-0.2.1.6/pyezviz/__init__.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.5/pyezviz/__main__.py` & `pyezviz-0.2.1.6/pyezviz/__main__.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.5/pyezviz/api_endpoints.py` & `pyezviz-0.2.1.6/pyezviz/api_endpoints.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.5/pyezviz/camera.py` & `pyezviz-0.2.1.6/pyezviz/camera.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.5/pyezviz/cas.py` & `pyezviz-0.2.1.6/pyezviz/cas.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.5/pyezviz/client.py` & `pyezviz-0.2.1.6/pyezviz/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,22 +415,25 @@
             raise PyEzvizError(
                 f"Could not get unified message list: Got {json_output})"
             )
 
         return json_output
 
     def switch_status(
-        self, serial: str, status_type: int, enable: int, max_retries: int = 0
+        self,
+        serial: str,
+        status_type: int,
+        enable: int,
+        channel_no: int = 0,
+        max_retries: int = 0,
     ) -> bool:
         """Camera features are represented as switches. Switch them on or off."""
         if max_retries > MAX_RETRIES:
             raise PyEzvizError("Can't gather proper data. Max retries exceeded.")
 
-        channel_no = 0
-
         try:
             req = self._session.put(
                 url=f"https://{self._token['api_url']}{API_ENDPOINT_DEVICES}{serial}/{channel_no}/{enable}/{status_type}{API_ENDPOINT_SWITCH_STATUS}",
                 timeout=self._timeout,
             )
 
             req.raise_for_status()
@@ -453,14 +456,17 @@
                 + "\nResponse was: "
                 + str(req.text)
             ) from err
 
         if json_output["meta"]["code"] != 200:
             raise PyEzvizError(f"Could not set the switch: Got {json_output})")
 
+        if self._cameras.get(serial):
+            self._cameras[serial]["switches"][status_type] = bool(enable)
+
         return True
 
     def switch_status_other(
         self,
         serial: str,
         status_type: int,
         enable: int,
```

### Comparing `pyezviz-0.2.1.5/pyezviz/constants.py` & `pyezviz-0.2.1.6/pyezviz/constants.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.5/pyezviz/exceptions.py` & `pyezviz-0.2.1.6/pyezviz/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.5/pyezviz/mqtt.py` & `pyezviz-0.2.1.6/pyezviz/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.5/pyezviz/test_cam_rtsp.py` & `pyezviz-0.2.1.6/pyezviz/test_cam_rtsp.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.5/pyezviz/utils.py` & `pyezviz-0.2.1.6/pyezviz/utils.py`

 * *Files identical despite different names*

### Comparing `pyezviz-0.2.1.5/setup.py` & `pyezviz-0.2.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyezviz',
-    version="0.2.1.5",
+    version="0.2.1.6",
     license='Apache Software License 2.0',
     author='Pierre Ourdouille',
     author_email='baqs@users.github.com',
     description='Pilot your Ezviz cameras',
     long_description="Pilot your Ezviz cameras with this module. Please view readme on github",
     url='http://github.com/baqs/pyEzviz/',
     packages=setuptools.find_packages(),
```

