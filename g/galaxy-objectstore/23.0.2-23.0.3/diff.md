# Comparing `tmp/galaxy-objectstore-23.0.2.tar.gz` & `tmp/galaxy-objectstore-23.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/objectstore/dist/.tmp-wl06vpzt/galaxy-objectstore-23.0.2.tar", last modified: Tue Jun 13 17:08:00 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/objectstore/dist/.tmp-qp8drzd9/galaxy-objectstore-23.0.3.tar", last modified: Mon Jun 26 09:51:50 2023, max compression
```

## Comparing `galaxy-objectstore-23.0.2.tar` & `galaxy-objectstore-23.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:00.000000 galaxy-objectstore-23.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-13 17:04:37.000000 galaxy-objectstore-23.0.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-13 17:04:36.000000 galaxy-objectstore-23.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-13 17:04:37.000000 galaxy-objectstore-23.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-13 17:08:00.000000 galaxy-objectstore-23.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-13 17:04:37.000000 galaxy-objectstore-23.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 17:04:37.000000 galaxy-objectstore-23.0.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:00.000000 galaxy-objectstore-23.0.2/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-13 17:04:37.000000 galaxy-objectstore-23.0.2/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:00.000000 galaxy-objectstore-23.0.2/galaxy/objectstore/
--rw-r--r--   0 runner    (1001) docker     (123)    48143 2023-06-13 17:04:37.000000 galaxy-objectstore-23.0.2/galaxy/objectstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26038 2023-06-13 17:04:37.000000 galaxy-objectstore-23.0.2/galaxy/objectstore/azure_blob.py
--rw-r--r--   0 runner    (1001) docker     (123)    32912 2023-06-13 17:04:37.000000 galaxy-objectstore-23.0.2/galaxy/objectstore/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    31799 2023-06-13 17:04:37.000000 galaxy-objectstore-23.0.2/galaxy/objectstore/irods.py
--rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-06-13 17:04:37.000000 galaxy-objectstore-23.0.2/galaxy/objectstore/pithos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-13 17:04:37.000000 galaxy-objectstore-23.0.2/galaxy/objectstore/pulsar.py
--rw-r--r--   0 runner    (1001) docker     (123)    33532 2023-06-13 17:04:37.000000 galaxy-objectstore-23.0.2/galaxy/objectstore/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-13 17:04:37.000000 galaxy-objectstore-23.0.2/galaxy/objectstore/s3_multipart_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:00.000000 galaxy-objectstore-23.0.2/galaxy/objectstore/unittest_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-13 17:04:37.000000 galaxy-objectstore-23.0.2/galaxy/objectstore/unittest_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-objectstore-23.0.2/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:00.000000 galaxy-objectstore-23.0.2/galaxy_objectstore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-13 17:08:00.000000 galaxy-objectstore-23.0.2/galaxy_objectstore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-13 17:08:00.000000 galaxy-objectstore-23.0.2/galaxy_objectstore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:08:00.000000 galaxy-objectstore-23.0.2/galaxy_objectstore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 17:08:00.000000 galaxy-objectstore-23.0.2/galaxy_objectstore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:08:00.000000 galaxy-objectstore-23.0.2/galaxy_objectstore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 17:04:37.000000 galaxy-objectstore-23.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-13 17:08:00.000000 galaxy-objectstore-23.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:04:37.000000 galaxy-objectstore-23.0.2/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:50.000000 galaxy-objectstore-23.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-26 09:48:33.000000 galaxy-objectstore-23.0.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-26 09:48:32.000000 galaxy-objectstore-23.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 09:48:33.000000 galaxy-objectstore-23.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-26 09:51:50.000000 galaxy-objectstore-23.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-26 09:48:33.000000 galaxy-objectstore-23.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 09:48:33.000000 galaxy-objectstore-23.0.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:50.000000 galaxy-objectstore-23.0.3/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-26 09:48:33.000000 galaxy-objectstore-23.0.3/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:50.000000 galaxy-objectstore-23.0.3/galaxy/objectstore/
+-rw-r--r--   0 runner    (1001) docker     (123)    48143 2023-06-26 09:48:33.000000 galaxy-objectstore-23.0.3/galaxy/objectstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26038 2023-06-26 09:48:33.000000 galaxy-objectstore-23.0.3/galaxy/objectstore/azure_blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32912 2023-06-26 09:48:33.000000 galaxy-objectstore-23.0.3/galaxy/objectstore/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31799 2023-06-26 09:48:33.000000 galaxy-objectstore-23.0.3/galaxy/objectstore/irods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-06-26 09:48:33.000000 galaxy-objectstore-23.0.3/galaxy/objectstore/pithos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-26 09:48:33.000000 galaxy-objectstore-23.0.3/galaxy/objectstore/pulsar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33532 2023-06-26 09:48:33.000000 galaxy-objectstore-23.0.3/galaxy/objectstore/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-26 09:48:33.000000 galaxy-objectstore-23.0.3/galaxy/objectstore/s3_multipart_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:50.000000 galaxy-objectstore-23.0.3/galaxy/objectstore/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-26 09:48:33.000000 galaxy-objectstore-23.0.3/galaxy/objectstore/unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:48:33.000000 galaxy-objectstore-23.0.3/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:50.000000 galaxy-objectstore-23.0.3/galaxy_objectstore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-26 09:51:50.000000 galaxy-objectstore-23.0.3/galaxy_objectstore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-26 09:51:50.000000 galaxy-objectstore-23.0.3/galaxy_objectstore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:51:50.000000 galaxy-objectstore-23.0.3/galaxy_objectstore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 09:51:50.000000 galaxy-objectstore-23.0.3/galaxy_objectstore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 09:51:50.000000 galaxy-objectstore-23.0.3/galaxy_objectstore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 09:48:33.000000 galaxy-objectstore-23.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-26 09:51:50.000000 galaxy-objectstore-23.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 09:48:33.000000 galaxy-objectstore-23.0.3/test-requirements.txt
```

### Comparing `galaxy-objectstore-23.0.2/HISTORY.rst` & `galaxy-objectstore-23.0.3/HISTORY.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,19 @@
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

### Comparing `galaxy-objectstore-23.0.2/LICENSE` & `galaxy-objectstore-23.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-23.0.2/PKG-INFO` & `galaxy-objectstore-23.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-objectstore
-Version: 23.0.2
+Version: 23.0.3
 Summary: Galaxy objectstore framework and plugins
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,20 @@
 
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

### Comparing `galaxy-objectstore-23.0.2/galaxy/objectstore/__init__.py` & `galaxy-objectstore-23.0.3/galaxy/objectstore/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-23.0.2/galaxy/objectstore/azure_blob.py` & `galaxy-objectstore-23.0.3/galaxy/objectstore/azure_blob.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-23.0.2/galaxy/objectstore/cloud.py` & `galaxy-objectstore-23.0.3/galaxy/objectstore/cloud.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-23.0.2/galaxy/objectstore/irods.py` & `galaxy-objectstore-23.0.3/galaxy/objectstore/irods.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-23.0.2/galaxy/objectstore/pithos.py` & `galaxy-objectstore-23.0.3/galaxy/objectstore/pithos.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-23.0.2/galaxy/objectstore/pulsar.py` & `galaxy-objectstore-23.0.3/galaxy/objectstore/pulsar.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-23.0.2/galaxy/objectstore/s3.py` & `galaxy-objectstore-23.0.3/galaxy/objectstore/s3.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-23.0.2/galaxy/objectstore/s3_multipart_upload.py` & `galaxy-objectstore-23.0.3/galaxy/objectstore/s3_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-23.0.2/galaxy/objectstore/unittest_utils/__init__.py` & `galaxy-objectstore-23.0.3/galaxy/objectstore/unittest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-23.0.2/galaxy_objectstore.egg-info/PKG-INFO` & `galaxy-objectstore-23.0.3/galaxy_objectstore.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-objectstore
-Version: 23.0.2
+Version: 23.0.3
 Summary: Galaxy objectstore framework and plugins
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,20 @@
 
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

### Comparing `galaxy-objectstore-23.0.2/galaxy_objectstore.egg-info/SOURCES.txt` & `galaxy-objectstore-23.0.3/galaxy_objectstore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-objectstore-23.0.2/setup.cfg` & `galaxy-objectstore-23.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-objectstore
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.2
+version = 23.0.3
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 	PyYAML
 packages = find:
```

