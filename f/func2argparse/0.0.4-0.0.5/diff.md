# Comparing `tmp/func2argparse-0.0.4.tar.gz` & `tmp/func2argparse-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func2argparse-0.0.4.tar", last modified: Wed Jun 21 08:57:01 2023, max compression
+gzip compressed data, was "func2argparse-0.0.5.tar", last modified: Mon Jun 26 08:43:47 2023, max compression
```

## Comparing `func2argparse-0.0.4.tar` & `func2argparse-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:57:01.921024 func2argparse-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 08:56:41.000000 func2argparse-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-21 08:57:01.921024 func2argparse-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-21 08:56:41.000000 func2argparse-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:57:01.925025 func2argparse-0.0.4/func2argparse/
--rw-r--r--   0 runner    (1001) docker     (123)    12715 2023-06-21 08:56:41.000000 func2argparse-0.0.4/func2argparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-21 08:57:01.925025 func2argparse-0.0.4/func2argparse/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-21 08:56:41.000000 func2argparse-0.0.4/func2argparse/logging.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:57:01.921024 func2argparse-0.0.4/func2argparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-21 08:57:01.000000 func2argparse-0.0.4/func2argparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-21 08:57:01.000000 func2argparse-0.0.4/func2argparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:57:01.000000 func2argparse-0.0.4/func2argparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 08:57:01.000000 func2argparse-0.0.4/func2argparse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 08:57:01.000000 func2argparse-0.0.4/func2argparse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-21 08:56:41.000000 func2argparse-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 08:57:01.925025 func2argparse-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-21 08:56:41.000000 func2argparse-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 08:57:01.921024 func2argparse-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-21 08:56:41.000000 func2argparse-0.0.4/tests/test_func_to_argparse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:43:47.936403 func2argparse-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 08:43:31.000000 func2argparse-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-26 08:43:47.936403 func2argparse-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-26 08:43:31.000000 func2argparse-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:43:47.936403 func2argparse-0.0.5/func2argparse/
+-rw-r--r--   0 runner    (1001) docker     (123)    19534 2023-06-26 08:43:31.000000 func2argparse-0.0.5/func2argparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-26 08:43:47.936403 func2argparse-0.0.5/func2argparse/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-26 08:43:31.000000 func2argparse-0.0.5/func2argparse/logging.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:43:47.936403 func2argparse-0.0.5/func2argparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-26 08:43:47.000000 func2argparse-0.0.5/func2argparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-26 08:43:47.000000 func2argparse-0.0.5/func2argparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 08:43:47.000000 func2argparse-0.0.5/func2argparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 08:43:47.000000 func2argparse-0.0.5/func2argparse.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 08:43:47.000000 func2argparse-0.0.5/func2argparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-26 08:43:31.000000 func2argparse-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 08:43:47.936403 func2argparse-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-26 08:43:31.000000 func2argparse-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:43:47.936403 func2argparse-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-26 08:43:31.000000 func2argparse-0.0.5/tests/test_func_to_argparse.py
```

### Comparing `func2argparse-0.0.4/PKG-INFO` & `func2argparse-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func2argparse
-Version: 0.0.4
+Version: 0.0.5
 Summary: Convert python functions to argparse objects
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/func2argparse
 Project-URL: Bug Tracker, https://github.com/Acellera/func2argparse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.9
```

### Comparing `func2argparse-0.0.4/README.md` & `func2argparse-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `func2argparse-0.0.4/func2argparse.egg-info/PKG-INFO` & `func2argparse-0.0.5/func2argparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func2argparse
-Version: 0.0.4
+Version: 0.0.5
 Summary: Convert python functions to argparse objects
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/func2argparse
 Project-URL: Bug Tracker, https://github.com/Acellera/func2argparse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.9
```

### Comparing `func2argparse-0.0.4/pyproject.toml` & `func2argparse-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `func2argparse-0.0.4/tests/test_func_to_argparse.py` & `func2argparse-0.0.5/tests/test_func_to_argparse.py`

 * *Files identical despite different names*

