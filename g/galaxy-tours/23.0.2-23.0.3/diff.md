# Comparing `tmp/galaxy-tours-23.0.2.tar.gz` & `tmp/galaxy-tours-23.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/tours/dist/.tmp-gmqvt1l_/galaxy-tours-23.0.2.tar", last modified: Tue Jun 13 17:10:15 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/tours/dist/.tmp-1i5wtccj/galaxy-tours-23.0.3.tar", last modified: Mon Jun 26 09:53:53 2023, max compression
```

## Comparing `galaxy-tours-23.0.2.tar` & `galaxy-tours-23.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:10:15.000000 galaxy-tours-23.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-13 17:04:37.000000 galaxy-tours-23.0.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-13 17:04:36.000000 galaxy-tours-23.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-13 17:04:37.000000 galaxy-tours-23.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-13 17:10:15.000000 galaxy-tours-23.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-13 17:04:37.000000 galaxy-tours-23.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 17:04:37.000000 galaxy-tours-23.0.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:10:15.000000 galaxy-tours-23.0.2/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 17:04:37.000000 galaxy-tours-23.0.2/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-tours-23.0.2/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:10:15.000000 galaxy-tours-23.0.2/galaxy/tours/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-13 17:04:37.000000 galaxy-tours-23.0.2/galaxy/tours/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-13 17:04:37.000000 galaxy-tours-23.0.2/galaxy/tours/_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-13 17:04:37.000000 galaxy-tours-23.0.2/galaxy/tours/_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-13 17:04:37.000000 galaxy-tours-23.0.2/galaxy/tours/_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-13 17:04:37.000000 galaxy-tours-23.0.2/galaxy/tours/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:10:15.000000 galaxy-tours-23.0.2/galaxy_tours.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-13 17:10:15.000000 galaxy-tours-23.0.2/galaxy_tours.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-13 17:10:15.000000 galaxy-tours-23.0.2/galaxy_tours.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:10:15.000000 galaxy-tours-23.0.2/galaxy_tours.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 17:10:15.000000 galaxy-tours-23.0.2/galaxy_tours.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-13 17:10:15.000000 galaxy-tours-23.0.2/galaxy_tours.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:10:15.000000 galaxy-tours-23.0.2/galaxy_tours.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 17:04:37.000000 galaxy-tours-23.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-13 17:10:15.000000 galaxy-tours-23.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:04:37.000000 galaxy-tours-23.0.2/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:53:53.000000 galaxy-tours-23.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-26 09:48:33.000000 galaxy-tours-23.0.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-26 09:48:32.000000 galaxy-tours-23.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 09:48:33.000000 galaxy-tours-23.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-26 09:53:53.000000 galaxy-tours-23.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-26 09:48:33.000000 galaxy-tours-23.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 09:48:33.000000 galaxy-tours-23.0.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:53:53.000000 galaxy-tours-23.0.3/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 09:48:33.000000 galaxy-tours-23.0.3/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:48:33.000000 galaxy-tours-23.0.3/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:53:53.000000 galaxy-tours-23.0.3/galaxy/tours/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-26 09:48:33.000000 galaxy-tours-23.0.3/galaxy/tours/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-06-26 09:48:33.000000 galaxy-tours-23.0.3/galaxy/tours/_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-26 09:48:33.000000 galaxy-tours-23.0.3/galaxy/tours/_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-26 09:48:33.000000 galaxy-tours-23.0.3/galaxy/tours/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-26 09:48:33.000000 galaxy-tours-23.0.3/galaxy/tours/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:53:53.000000 galaxy-tours-23.0.3/galaxy_tours.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-26 09:53:53.000000 galaxy-tours-23.0.3/galaxy_tours.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-26 09:53:53.000000 galaxy-tours-23.0.3/galaxy_tours.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:53:53.000000 galaxy-tours-23.0.3/galaxy_tours.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 09:53:53.000000 galaxy-tours-23.0.3/galaxy_tours.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 09:53:53.000000 galaxy-tours-23.0.3/galaxy_tours.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 09:53:53.000000 galaxy-tours-23.0.3/galaxy_tours.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 09:48:33.000000 galaxy-tours-23.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-26 09:53:53.000000 galaxy-tours-23.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 09:48:33.000000 galaxy-tours-23.0.3/test-requirements.txt
```

### Comparing `galaxy-tours-23.0.2/LICENSE.txt` & `galaxy-tours-23.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `galaxy-tours-23.0.2/PKG-INFO` & `galaxy-tours-23.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-tours
-Version: 23.0.2
+Version: 23.0.3
 Summary: Galaxy tours backend framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -44,14 +44,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.3 (2023-06-26)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.2 (2023-06-13)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.1 (2023-06-08)
```

### Comparing `galaxy-tours-23.0.2/galaxy/tours/_impl.py` & `galaxy-tours-23.0.3/galaxy/tours/_impl.py`

 * *Files identical despite different names*

### Comparing `galaxy-tours-23.0.2/galaxy/tours/_schema.py` & `galaxy-tours-23.0.3/galaxy/tours/_schema.py`

 * *Files identical despite different names*

### Comparing `galaxy-tours-23.0.2/galaxy/tours/validate.py` & `galaxy-tours-23.0.3/galaxy/tours/validate.py`

 * *Files identical despite different names*

### Comparing `galaxy-tours-23.0.2/galaxy_tours.egg-info/PKG-INFO` & `galaxy-tours-23.0.3/galaxy_tours.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-tours
-Version: 23.0.2
+Version: 23.0.3
 Summary: Galaxy tours backend framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -44,14 +44,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.3 (2023-06-26)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.2 (2023-06-13)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.1 (2023-06-08)
```

### Comparing `galaxy-tours-23.0.2/setup.cfg` & `galaxy-tours-23.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-tours
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.2
+version = 23.0.3
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-navigation
 	pydantic
 	PyYAML
```

