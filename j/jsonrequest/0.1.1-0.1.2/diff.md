# Comparing `tmp/jsonrequest-0.1.1.tar.gz` & `tmp/jsonrequest-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrequest-0.1.1.tar", last modified: Mon Jun 26 06:12:21 2023, max compression
+gzip compressed data, was "jsonrequest-0.1.2.tar", last modified: Mon Jun 26 06:35:41 2023, max compression
```

## Comparing `jsonrequest-0.1.1.tar` & `jsonrequest-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 06:12:21.596464 jsonrequest-0.1.1/
--rw-r--r--   0 JustinRWong   (502) staff       (20)    11357 2023-06-26 05:51:37.000000 jsonrequest-0.1.1/LICENSE
--rw-r--r--   0 JustinRWong   (502) staff       (20)      939 2023-06-26 06:12:21.596336 jsonrequest-0.1.1/PKG-INFO
--rw-r--r--   0 JustinRWong   (502) staff       (20)      630 2023-06-26 06:10:47.000000 jsonrequest-0.1.1/README.md
-drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 06:12:21.596176 jsonrequest-0.1.1/jsonrequest.egg-info/
--rw-r--r--   0 JustinRWong   (502) staff       (20)      939 2023-06-26 06:12:21.000000 jsonrequest-0.1.1/jsonrequest.egg-info/PKG-INFO
--rw-r--r--   0 JustinRWong   (502) staff       (20)      200 2023-06-26 06:12:21.000000 jsonrequest-0.1.1/jsonrequest.egg-info/SOURCES.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)        1 2023-06-26 06:12:21.000000 jsonrequest-0.1.1/jsonrequest.egg-info/dependency_links.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)       18 2023-06-26 06:12:21.000000 jsonrequest-0.1.1/jsonrequest.egg-info/requires.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)        1 2023-06-26 06:12:21.000000 jsonrequest-0.1.1/jsonrequest.egg-info/top_level.txt
--rw-r--r--   0 JustinRWong   (502) staff       (20)       38 2023-06-26 06:12:21.596509 jsonrequest-0.1.1/setup.cfg
--rw-r--r--   0 JustinRWong   (502) staff       (20)      527 2023-06-26 06:10:05.000000 jsonrequest-0.1.1/setup.py
+drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 06:35:41.462377 jsonrequest-0.1.2/
+-rw-r--r--   0 JustinRWong   (502) staff       (20)    11357 2023-06-26 05:51:37.000000 jsonrequest-0.1.2/LICENSE
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      925 2023-06-26 06:35:41.462238 jsonrequest-0.1.2/PKG-INFO
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      671 2023-06-26 06:13:40.000000 jsonrequest-0.1.2/README.md
+drwxr-xr-x   0 JustinRWong   (502) staff       (20)        0 2023-06-26 06:35:41.462061 jsonrequest-0.1.2/jsonrequest.egg-info/
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      925 2023-06-26 06:35:41.000000 jsonrequest-0.1.2/jsonrequest.egg-info/PKG-INFO
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      200 2023-06-26 06:35:41.000000 jsonrequest-0.1.2/jsonrequest.egg-info/SOURCES.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)        1 2023-06-26 06:35:41.000000 jsonrequest-0.1.2/jsonrequest.egg-info/dependency_links.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)       18 2023-06-26 06:35:41.000000 jsonrequest-0.1.2/jsonrequest.egg-info/requires.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)        1 2023-06-26 06:35:41.000000 jsonrequest-0.1.2/jsonrequest.egg-info/top_level.txt
+-rw-r--r--   0 JustinRWong   (502) staff       (20)       38 2023-06-26 06:35:41.462418 jsonrequest-0.1.2/setup.cfg
+-rw-r--r--   0 JustinRWong   (502) staff       (20)      527 2023-06-26 06:35:32.000000 jsonrequest-0.1.2/setup.py
```

### Comparing `jsonrequest-0.1.1/LICENSE` & `jsonrequest-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonrequest-0.1.1/PKG-INFO` & `jsonrequest-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: jsonrequest
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lightweight wrapper to make http(s) requests. POST, PATCH, and DELETE requests only support json content.
-Home-page: UNKNOWN
 Author: Justin Wong
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# JSONRequest
+# [JSONRequest](https://pypi.org/project/jsonrequest/)
 Lightweight wrapper for requests library that only supports Content-Type: application/json.
 
 This only supports `GET`, `POST`, `PATCH`, and `DELETE` http(s) request methods.
 
 ## Note:
 This data passed also only applies to `application/json` content.
 
 
 Across multiple times over the past many years in my python projects, I found this codeblock repeated whenever I tried to make various http(s) requests using the requests library and thought it'd be much simpler to pass the method as a parameter instead of changing the function. I created this package as a result. Hope this helps and Happy coding :)
 
 - by Justin
-
```

### Comparing `jsonrequest-0.1.1/README.md` & `jsonrequest-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# JSONRequest
+# [JSONRequest](https://pypi.org/project/jsonrequest/)
 Lightweight wrapper for requests library that only supports Content-Type: application/json.
 
 This only supports `GET`, `POST`, `PATCH`, and `DELETE` http(s) request methods.
 
 ## Note:
 This data passed also only applies to `application/json` content.
```

### Comparing `jsonrequest-0.1.1/jsonrequest.egg-info/PKG-INFO` & `jsonrequest-0.1.2/jsonrequest.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: jsonrequest
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lightweight wrapper to make http(s) requests. POST, PATCH, and DELETE requests only support json content.
-Home-page: UNKNOWN
 Author: Justin Wong
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# JSONRequest
+# [JSONRequest](https://pypi.org/project/jsonrequest/)
 Lightweight wrapper for requests library that only supports Content-Type: application/json.
 
 This only supports `GET`, `POST`, `PATCH`, and `DELETE` http(s) request methods.
 
 ## Note:
 This data passed also only applies to `application/json` content.
 
 
 Across multiple times over the past many years in my python projects, I found this codeblock repeated whenever I tried to make various http(s) requests using the requests library and thought it'd be much simpler to pass the method as a parameter instead of changing the function. I created this package as a result. Hope this helps and Happy coding :)
 
 - by Justin
-
```

### Comparing `jsonrequest-0.1.1/setup.py` & `jsonrequest-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='jsonrequest',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=[
         'requests',
         'pydantic',
     ],
     author='Justin Wong',
     description='Lightweight wrapper to make http(s) requests. POST, PATCH, and DELETE requests only support json content.',
```

