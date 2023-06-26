# Comparing `tmp/Jedutils-0.1.0.tar.gz` & `tmp/Jedutils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jedutils-0.1.0.tar", last modified: Sun Jun 25 06:51:24 2023, max compression
+gzip compressed data, was "Jedutils-0.1.1.tar", last modified: Mon Jun 26 04:16:36 2023, max compression
```

## Comparing `Jedutils-0.1.0.tar` & `Jedutils-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:51:24.451923 Jedutils-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:51:24.451923 Jedutils-0.1.0/Jedutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-25 06:51:24.000000 Jedutils-0.1.0/Jedutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-25 06:51:24.000000 Jedutils-0.1.0/Jedutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 06:51:24.000000 Jedutils-0.1.0/Jedutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 06:51:24.000000 Jedutils-0.1.0/Jedutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-25 06:51:22.000000 Jedutils-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-25 06:51:22.000000 Jedutils-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-25 06:51:24.451923 Jedutils-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-25 06:51:22.000000 Jedutils-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:51:24.451923 Jedutils-0.1.0/jedutils/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-25 06:51:22.000000 Jedutils-0.1.0/jedutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:51:24.451923 Jedutils-0.1.0/jedutils/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-25 06:51:22.000000 Jedutils-0.1.0/jedutils/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-25 06:51:22.000000 Jedutils-0.1.0/jedutils/asyncio/_run_async.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 06:51:24.451923 Jedutils-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-25 06:51:22.000000 Jedutils-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:16:36.526326 Jedutils-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:16:36.522326 Jedutils-0.1.1/Jedutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-26 04:16:36.000000 Jedutils-0.1.1/Jedutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-26 04:16:36.000000 Jedutils-0.1.1/Jedutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 04:16:36.000000 Jedutils-0.1.1/Jedutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 04:16:36.000000 Jedutils-0.1.1/Jedutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 04:16:35.000000 Jedutils-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 04:16:35.000000 Jedutils-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-26 04:16:36.526326 Jedutils-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-26 04:16:35.000000 Jedutils-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:16:36.522326 Jedutils-0.1.1/jedutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-26 04:16:35.000000 Jedutils-0.1.1/jedutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 04:16:36.526326 Jedutils-0.1.1/jedutils/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 04:16:35.000000 Jedutils-0.1.1/jedutils/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-26 04:16:35.000000 Jedutils-0.1.1/jedutils/asyncio/_async_redis_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-26 04:16:35.000000 Jedutils-0.1.1/jedutils/asyncio/_run_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 04:16:36.526326 Jedutils-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-26 04:16:35.000000 Jedutils-0.1.1/setup.py
```

### Comparing `Jedutils-0.1.0/Jedutils.egg-info/PKG-INFO` & `Jedutils-0.1.1/Jedutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jedutils
-Version: 0.1.0
+Version: 0.1.1
 Summary: Jedutils is a Python utilities package that provides a collection of useful helper functions.
 Home-page: https://github.com/AYMENJD/jedutils
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AYMENJD/jedutils
 Project-URL: Tracker, https://github.com/AYMENJD/jedutils/issues
```

### Comparing `Jedutils-0.1.0/LICENSE` & `Jedutils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Jedutils-0.1.0/PKG-INFO` & `Jedutils-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jedutils
-Version: 0.1.0
+Version: 0.1.1
 Summary: Jedutils is a Python utilities package that provides a collection of useful helper functions.
 Home-page: https://github.com/AYMENJD/jedutils
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AYMENJD/jedutils
 Project-URL: Tracker, https://github.com/AYMENJD/jedutils/issues
```

### Comparing `Jedutils-0.1.0/README.md` & `Jedutils-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `Jedutils-0.1.0/setup.py` & `Jedutils-0.1.1/setup.py`

 * *Files identical despite different names*

