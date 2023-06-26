# Comparing `tmp/jsonrequest-0.1.3.tar.gz` & `tmp/jsonrequest-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrequest-0.1.3.tar", last modified: Mon Jun 26 06:42:32 2023, max compression
+gzip compressed data, was "jsonrequest-0.1.4.tar", last modified: Mon Jun 26 07:01:06 2023, max compression
```

## Comparing `jsonrequest-0.1.3.tar` & `jsonrequest-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 06:42:32.441647 jsonrequest-0.1.3/
--rw-r--r--   0 JustinRWong   (502) staff       (20)    11357 2023-06-26 05:51:37.000000 jsonrequest-0.1.3/LICENSE
--rw-r--r--   0 JustinRWong   (502) staff       (20)     1231 2023-06-26 06:42:32.441518 jsonrequest-0.1.3/PKG-INFO
--rw-r--r--   0 JustinRWong   (502) staff       (20)      979 2023-06-26 06:40:48.000000 jsonrequest-0.1.3/README.md
-drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 06:42:32.441345 jsonrequest-0.1.3/jsonrequest.egg-info/
--rw-r--r--   0 JustinRWong   (502) staff       (20)     1231 2023-06-26 06:42:32.000000 jsonrequest-0.1.3/jsonrequest.egg-info/PKG-INFO
--rw-r--r--   0 JustinRWong   (502) staff       (20)      200 2023-06-26 06:42:32.000000 jsonrequest-0.1.3/jsonrequest.egg-info/SOURCES.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)        1 2023-06-26 06:42:32.000000 jsonrequest-0.1.3/jsonrequest.egg-info/dependency_links.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)       18 2023-06-26 06:42:32.000000 jsonrequest-0.1.3/jsonrequest.egg-info/requires.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)        1 2023-06-26 06:42:32.000000 jsonrequest-0.1.3/jsonrequest.egg-info/top_level.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)       38 2023-06-26 06:42:32.441691 jsonrequest-0.1.3/setup.cfg
--rw-r--r--   0 JustinRWong   (502) staff       (20)      621 2023-06-26 06:42:29.000000 jsonrequest-0.1.3/setup.py
+drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 07:01:06.944153 jsonrequest-0.1.4/
+-rw-r--r--   0 JustinRWong   (502) staff       (20)    11357 2023-06-26 05:51:37.000000 jsonrequest-0.1.4/LICENSE
+-rw-r--r--   0 JustinRWong   (502) staff       (20)     1610 2023-06-26 07:01:06.944025 jsonrequest-0.1.4/PKG-INFO
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      979 2023-06-26 06:40:48.000000 jsonrequest-0.1.4/README.md
+drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 07:01:06.943872 jsonrequest-0.1.4/jsonrequest.egg-info/
+-rw-r--r--   0 JustinRWong   (502) staff       (20)     1610 2023-06-26 07:01:06.000000 jsonrequest-0.1.4/jsonrequest.egg-info/PKG-INFO
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      215 2023-06-26 07:01:06.000000 jsonrequest-0.1.4/jsonrequest.egg-info/SOURCES.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)        1 2023-06-26 07:01:06.000000 jsonrequest-0.1.4/jsonrequest.egg-info/dependency_links.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)       18 2023-06-26 07:01:06.000000 jsonrequest-0.1.4/jsonrequest.egg-info/requires.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)        1 2023-06-26 07:01:06.000000 jsonrequest-0.1.4/jsonrequest.egg-info/top_level.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      597 2023-06-26 06:55:16.000000 jsonrequest-0.1.4/pyproject.toml
+-rw-r--r--   0 JustinRWong   (502) staff       (20)       38 2023-06-26 07:01:06.944193 jsonrequest-0.1.4/setup.cfg
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      621 2023-06-26 06:55:26.000000 jsonrequest-0.1.4/setup.py
```

### Comparing `jsonrequest-0.1.3/LICENSE` & `jsonrequest-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonrequest-0.1.3/PKG-INFO` & `jsonrequest-0.1.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: jsonrequest
-Version: 0.1.3
-Summary: Lightweight wrapper to make http(s) requests. POST, PATCH, and DELETE requests only support json content.
-Author: Justin Wong
-License: Apache 2.0
-Description-Content-Type: text/markdown
-
 # [JSONRequest](https://pypi.org/project/jsonrequest/)
 Lightweight wrapper for requests library that only supports Content-Type: application/json.
 
 This only supports `GET`, `POST`, `PATCH`, and `DELETE` http(s) request methods.
 
 ## How to Use
 
@@ -29,8 +21,8 @@
 
 ## Note:
 This data passed also only applies to `application/json` content.
 
 
 Across multiple times over the past many years in my python projects, I found this codeblock repeated whenever I tried to make various http(s) requests using the requests library and thought it'd be much simpler to pass the method as a parameter instead of changing the function. I created this package as a result. Hope this helps and Happy coding :)
 
-- by Justin
+- by Justin
```

### Comparing `jsonrequest-0.1.3/jsonrequest.egg-info/PKG-INFO` & `jsonrequest-0.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 Metadata-Version: 2.1
 Name: jsonrequest
-Version: 0.1.3
+Version: 0.1.4
 Summary: Lightweight wrapper to make http(s) requests. POST, PATCH, and DELETE requests only support json content.
 Author: Justin Wong
+Author-email: Justin Wong <justinryanwong@berkeley.edu>
 License: Apache 2.0
+Project-URL: Homepage, https://github.com/JustinRWong/JSONRequest
+Project-URL: Bug Tracker, https://github.com/JustinRWong/JSONRequest/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.2
 Description-Content-Type: text/markdown
 
 # [JSONRequest](https://pypi.org/project/jsonrequest/)
 Lightweight wrapper for requests library that only supports Content-Type: application/json.
 
 This only supports `GET`, `POST`, `PATCH`, and `DELETE` http(s) request methods.
```

### Comparing `jsonrequest-0.1.3/setup.py` & `jsonrequest-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='jsonrequest',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
         'requests',
         'pydantic',
     ],
     author='Justin Wong',
     description='Lightweight wrapper to make http(s) requests. POST, PATCH, and DELETE requests only support json content.',
```

