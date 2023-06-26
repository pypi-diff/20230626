# Comparing `tmp/memoiz-0.0.8.tar.gz` & `tmp/memoiz-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memoiz-0.0.8.tar", last modified: Thu Dec  8 20:05:16 2022, max compression
+gzip compressed data, was "memoiz-0.0.9.tar", last modified: Mon Jun 12 15:06:03 2023, max compression
```

## Comparing `memoiz-0.0.8.tar` & `memoiz-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 adpatter  (1000) adpatter  (1000)        0 2022-12-08 20:05:16.947682 memoiz-0.0.8/
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)     1067 2022-12-05 17:05:11.000000 memoiz-0.0.8/LICENSE
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)     1367 2022-12-08 20:05:16.947682 memoiz-0.0.8/PKG-INFO
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)      639 2022-12-05 17:05:17.000000 memoiz-0.0.8/README.md
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)      800 2022-12-08 20:03:13.000000 memoiz-0.0.8/pyproject.toml
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)       38 2022-12-08 20:05:16.947682 memoiz-0.0.8/setup.cfg
-drwxrwxr-x   0 adpatter  (1000) adpatter  (1000)        0 2022-12-08 20:05:16.943682 memoiz-0.0.8/src/
-drwxrwxr-x   0 adpatter  (1000) adpatter  (1000)        0 2022-12-08 20:05:16.947682 memoiz-0.0.8/src/memoiz/
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)        0 2022-12-03 02:13:23.000000 memoiz-0.0.8/src/memoiz/__init__.py
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)     2040 2022-12-08 20:02:35.000000 memoiz-0.0.8/src/memoiz/cache.py
-drwxrwxr-x   0 adpatter  (1000) adpatter  (1000)        0 2022-12-08 20:05:16.947682 memoiz-0.0.8/src/memoiz.egg-info/
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)     1367 2022-12-08 20:05:16.000000 memoiz-0.0.8/src/memoiz.egg-info/PKG-INFO
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)      211 2022-12-08 20:05:16.000000 memoiz-0.0.8/src/memoiz.egg-info/SOURCES.txt
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)        1 2022-12-08 20:05:16.000000 memoiz-0.0.8/src/memoiz.egg-info/dependency_links.txt
--rw-rw-r--   0 adpatter  (1000) adpatter  (1000)        7 2022-12-08 20:05:16.000000 memoiz-0.0.8/src/memoiz.egg-info/top_level.txt
+drwxrwxr-x   0 adpatter  (1000) adpatter  (1000)        0 2023-06-12 15:06:03.434477 memoiz-0.0.9/
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)     1067 2022-12-05 17:05:11.000000 memoiz-0.0.9/LICENSE
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)     1367 2023-06-12 15:06:03.434477 memoiz-0.0.9/PKG-INFO
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)      639 2022-12-05 17:05:17.000000 memoiz-0.0.9/README.md
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)      800 2023-06-12 15:04:13.000000 memoiz-0.0.9/pyproject.toml
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)       38 2023-06-12 15:06:03.434477 memoiz-0.0.9/setup.cfg
+drwxrwxr-x   0 adpatter  (1000) adpatter  (1000)        0 2023-06-12 15:06:03.422477 memoiz-0.0.9/src/
+drwxrwxr-x   0 adpatter  (1000) adpatter  (1000)        0 2023-06-12 15:06:03.430477 memoiz-0.0.9/src/memoiz/
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)        0 2022-12-03 02:13:23.000000 memoiz-0.0.9/src/memoiz/__init__.py
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)     3172 2023-06-12 14:35:17.000000 memoiz-0.0.9/src/memoiz/cache.py
+drwxrwxr-x   0 adpatter  (1000) adpatter  (1000)        0 2023-06-12 15:06:03.434477 memoiz-0.0.9/src/memoiz.egg-info/
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)     1367 2023-06-12 15:06:03.000000 memoiz-0.0.9/src/memoiz.egg-info/PKG-INFO
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)      211 2023-06-12 15:06:03.000000 memoiz-0.0.9/src/memoiz.egg-info/SOURCES.txt
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)        1 2023-06-12 15:06:03.000000 memoiz-0.0.9/src/memoiz.egg-info/dependency_links.txt
+-rw-rw-r--   0 adpatter  (1000) adpatter  (1000)        7 2023-06-12 15:06:03.000000 memoiz-0.0.9/src/memoiz.egg-info/top_level.txt
```

### Comparing `memoiz-0.0.8/LICENSE` & `memoiz-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `memoiz-0.0.8/PKG-INFO` & `memoiz-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memoiz
-Version: 0.0.8
+Version: 0.0.9
 Summary: Memoiz is a memoization decorator that makes resonable assumptions about how and if to cache the return value of a function or method based on the arguments passed to it. The decorator can be used on both free and bound functions.
 Author-email: Adam Patterson <adam@faranalytics.net>
 Project-URL: Homepage, https://github.com/faranalytics/python_memoiz.git
 Project-URL: Bug Tracker, https://github.com/faranalytics/python_memoiz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `memoiz-0.0.8/README.md` & `memoiz-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `memoiz-0.0.8/pyproject.toml` & `memoiz-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "memoiz"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Adam Patterson", email="adam@faranalytics.net" },
 ]
 description = "Memoiz is a memoization decorator that makes resonable assumptions about how and if to cache the return value of a function or method based on the arguments passed to it. The decorator can be used on both free and bound functions."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `memoiz-0.0.8/src/memoiz.egg-info/PKG-INFO` & `memoiz-0.0.9/src/memoiz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memoiz
-Version: 0.0.8
+Version: 0.0.9
 Summary: Memoiz is a memoization decorator that makes resonable assumptions about how and if to cache the return value of a function or method based on the arguments passed to it. The decorator can be used on both free and bound functions.
 Author-email: Adam Patterson <adam@faranalytics.net>
 Project-URL: Homepage, https://github.com/faranalytics/python_memoiz.git
 Project-URL: Bug Tracker, https://github.com/faranalytics/python_memoiz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

