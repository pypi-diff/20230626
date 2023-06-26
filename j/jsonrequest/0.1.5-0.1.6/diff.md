# Comparing `tmp/jsonrequest-0.1.5.tar.gz` & `tmp/jsonrequest-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrequest-0.1.5.tar", last modified: Mon Jun 26 08:02:14 2023, max compression
+gzip compressed data, was "jsonrequest-0.1.6.tar", last modified: Mon Jun 26 08:07:16 2023, max compression
```

## Comparing `jsonrequest-0.1.5.tar` & `jsonrequest-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 08:02:14.167487 jsonrequest-0.1.5/
--rw-r--r--   0 JustinRWong   (502) staff       (20)     1734 2023-06-26 08:02:14.167326 jsonrequest-0.1.5/PKG-INFO
--rw-r--r--   0 JustinRWong   (502) staff       (20)     1103 2023-06-26 07:12:08.000000 jsonrequest-0.1.5/README.md
-drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 08:02:14.166394 jsonrequest-0.1.5/jsonrequest/
--rw-r--r--   0 JustinRWong   (502) staff       (20)      395 2023-06-26 08:01:51.000000 jsonrequest-0.1.5/jsonrequest/RequestModel.py
--rw-r--r--   0 JustinRWong   (502) staff       (20)       74 2023-06-26 07:59:32.000000 jsonrequest-0.1.5/jsonrequest/__init__.py
--rw-r--r--   0 JustinRWong   (502) staff       (20)      604 2023-06-26 07:59:30.000000 jsonrequest-0.1.5/jsonrequest/jsonrequest.py
-drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 08:02:14.167049 jsonrequest-0.1.5/jsonrequest.egg-info/
--rw-r--r--   0 JustinRWong   (502) staff       (20)     1734 2023-06-26 08:02:14.000000 jsonrequest-0.1.5/jsonrequest.egg-info/PKG-INFO
--rw-r--r--   0 JustinRWong   (502) staff       (20)      286 2023-06-26 08:02:14.000000 jsonrequest-0.1.5/jsonrequest.egg-info/SOURCES.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)        1 2023-06-26 08:02:14.000000 jsonrequest-0.1.5/jsonrequest.egg-info/dependency_links.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)       18 2023-06-26 08:02:14.000000 jsonrequest-0.1.5/jsonrequest.egg-info/requires.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)       12 2023-06-26 08:02:14.000000 jsonrequest-0.1.5/jsonrequest.egg-info/top_level.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)      597 2023-06-26 08:00:35.000000 jsonrequest-0.1.5/pyproject.toml
--rw-r--r--   0 JustinRWong   (502) staff       (20)       38 2023-06-26 08:02:14.167536 jsonrequest-0.1.5/setup.cfg
--rw-r--r--   0 JustinRWong   (502) staff       (20)      621 2023-06-26 07:59:59.000000 jsonrequest-0.1.5/setup.py
+drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 08:07:16.851633 jsonrequest-0.1.6/
+-rw-r--r--   0 JustinRWong   (502) staff       (20)     1734 2023-06-26 08:07:16.851498 jsonrequest-0.1.6/PKG-INFO
+-rw-r--r--   0 JustinRWong   (502) staff       (20)     1103 2023-06-26 07:12:08.000000 jsonrequest-0.1.6/README.md
+drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 08:07:16.850671 jsonrequest-0.1.6/jsonrequest/
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      395 2023-06-26 08:01:51.000000 jsonrequest-0.1.6/jsonrequest/RequestModel.py
+-rw-r--r--   0 JustinRWong   (502) staff       (20)       99 2023-06-26 08:05:47.000000 jsonrequest-0.1.6/jsonrequest/__init__.py
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      616 2023-06-26 08:06:52.000000 jsonrequest-0.1.6/jsonrequest/make_request.py
+drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 08:07:16.851325 jsonrequest-0.1.6/jsonrequest.egg-info/
+-rw-r--r--   0 JustinRWong   (502) staff       (20)     1734 2023-06-26 08:07:16.000000 jsonrequest-0.1.6/jsonrequest.egg-info/PKG-INFO
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      287 2023-06-26 08:07:16.000000 jsonrequest-0.1.6/jsonrequest.egg-info/SOURCES.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)        1 2023-06-26 08:07:16.000000 jsonrequest-0.1.6/jsonrequest.egg-info/dependency_links.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)       18 2023-06-26 08:07:16.000000 jsonrequest-0.1.6/jsonrequest.egg-info/requires.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)       12 2023-06-26 08:07:16.000000 jsonrequest-0.1.6/jsonrequest.egg-info/top_level.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      597 2023-06-26 08:07:14.000000 jsonrequest-0.1.6/pyproject.toml
+-rw-r--r--   0 JustinRWong   (502) staff       (20)       38 2023-06-26 08:07:16.851672 jsonrequest-0.1.6/setup.cfg
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      621 2023-06-26 08:06:56.000000 jsonrequest-0.1.6/setup.py
```

### Comparing `jsonrequest-0.1.5/PKG-INFO` & `jsonrequest-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrequest
-Version: 0.1.5
+Version: 0.1.6
 Summary: Lightweight wrapper to make http(s) requests. POST, PATCH, and DELETE requests only support json content.
 Author: Justin Wong
 Author-email: Justin Wong <justinryanwong@berkeley.edu>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/JustinRWong/JSONRequest
 Project-URL: Bug Tracker, https://github.com/JustinRWong/JSONRequest/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jsonrequest-0.1.5/README.md` & `jsonrequest-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `jsonrequest-0.1.5/jsonrequest/jsonrequest.py` & `jsonrequest-0.1.6/jsonrequest/make_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import requests
-from RequestModel import RequestModel
+from jsonrequest.RequestModel import RequestModel
 
 def make_request(request: RequestModel) -> requests.Response:
     '''
     Lightweight wrapper for requests library that only supports Content-Type: application/json.
     '''
     url = f"{request.url}/{request.endpoint}"
     if request.method == 'GET':
```

### Comparing `jsonrequest-0.1.5/jsonrequest.egg-info/PKG-INFO` & `jsonrequest-0.1.6/jsonrequest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrequest
-Version: 0.1.5
+Version: 0.1.6
 Summary: Lightweight wrapper to make http(s) requests. POST, PATCH, and DELETE requests only support json content.
 Author: Justin Wong
 Author-email: Justin Wong <justinryanwong@berkeley.edu>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/JustinRWong/JSONRequest
 Project-URL: Bug Tracker, https://github.com/JustinRWong/JSONRequest/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jsonrequest-0.1.5/pyproject.toml` & `jsonrequest-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jsonrequest"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Justin Wong", email="justinryanwong@berkeley.edu" },
 ]
 description = "Lightweight wrapper to make http(s) requests. POST, PATCH, and DELETE requests only support json content."
 readme = "README.md"
 requires-python = ">=3.2"
 classifiers = [
```

### Comparing `jsonrequest-0.1.5/setup.py` & `jsonrequest-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='jsonrequest',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     install_requires=[
         'requests',
         'pydantic',
     ],
     author='Justin Wong',
     description='Lightweight wrapper to make http(s) requests. POST, PATCH, and DELETE requests only support json content.',
```

