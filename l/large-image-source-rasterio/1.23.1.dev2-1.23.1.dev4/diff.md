# Comparing `tmp/large-image-source-rasterio-1.23.1.dev2.tar.gz` & `tmp/large-image-source-rasterio-1.23.1.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-rasterio-1.23.1.dev2.tar", last modified: Mon Jun 26 12:53:42 2023, max compression
+gzip compressed data, was "large-image-source-rasterio-1.23.1.dev4.tar", last modified: Mon Jun 26 18:48:12 2023, max compression
```

## Comparing `large-image-source-rasterio-1.23.1.dev2.tar` & `large-image-source-rasterio-1.23.1.dev4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-26 12:53:42.568805 large-image-source-rasterio-1.23.1.dev2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-06-26 12:53:42.000000 large-image-source-rasterio-1.23.1.dev2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-06-26 12:53:42.568805 large-image-source-rasterio-1.23.1.dev2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-06-26 12:53:42.000000 large-image-source-rasterio-1.23.1.dev2/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-26 12:53:42.564805 large-image-source-rasterio-1.23.1.dev2/large_image_source_rasterio/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43037 2023-06-26 12:51:56.000000 large-image-source-rasterio-1.23.1.dev2/large_image_source_rasterio/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-06-26 12:51:56.000000 large-image-source-rasterio-1.23.1.dev2/large_image_source_rasterio/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-26 12:53:42.568805 large-image-source-rasterio-1.23.1.dev2/large_image_source_rasterio.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-06-26 12:53:42.000000 large-image-source-rasterio-1.23.1.dev2/large_image_source_rasterio.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-06-26 12:53:42.000000 large-image-source-rasterio-1.23.1.dev2/large_image_source_rasterio.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-26 12:53:42.000000 large-image-source-rasterio-1.23.1.dev2/large_image_source_rasterio.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-06-26 12:53:42.000000 large-image-source-rasterio-1.23.1.dev2/large_image_source_rasterio.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-06-26 12:53:42.000000 large-image-source-rasterio-1.23.1.dev2/large_image_source_rasterio.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-06-26 12:53:42.000000 large-image-source-rasterio-1.23.1.dev2/large_image_source_rasterio.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-26 12:53:42.568805 large-image-source-rasterio-1.23.1.dev2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2564 2023-06-26 12:51:56.000000 large-image-source-rasterio-1.23.1.dev2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-26 18:48:12.038563 large-image-source-rasterio-1.23.1.dev4/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-06-26 18:48:11.000000 large-image-source-rasterio-1.23.1.dev4/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-06-26 18:48:12.038563 large-image-source-rasterio-1.23.1.dev4/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-06-26 18:48:11.000000 large-image-source-rasterio-1.23.1.dev4/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-26 18:48:12.038563 large-image-source-rasterio-1.23.1.dev4/large_image_source_rasterio/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43037 2023-06-26 18:46:37.000000 large-image-source-rasterio-1.23.1.dev4/large_image_source_rasterio/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-06-26 18:46:37.000000 large-image-source-rasterio-1.23.1.dev4/large_image_source_rasterio/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-26 18:48:12.038563 large-image-source-rasterio-1.23.1.dev4/large_image_source_rasterio.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      845 2023-06-26 18:48:11.000000 large-image-source-rasterio-1.23.1.dev4/large_image_source_rasterio.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-06-26 18:48:12.000000 large-image-source-rasterio-1.23.1.dev4/large_image_source_rasterio.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-26 18:48:11.000000 large-image-source-rasterio-1.23.1.dev4/large_image_source_rasterio.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-06-26 18:48:11.000000 large-image-source-rasterio-1.23.1.dev4/large_image_source_rasterio.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-06-26 18:48:11.000000 large-image-source-rasterio-1.23.1.dev4/large_image_source_rasterio.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-06-26 18:48:11.000000 large-image-source-rasterio-1.23.1.dev4/large_image_source_rasterio.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-26 18:48:12.042563 large-image-source-rasterio-1.23.1.dev4/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2564 2023-06-26 18:46:37.000000 large-image-source-rasterio-1.23.1.dev4/setup.py
```

### Comparing `large-image-source-rasterio-1.23.1.dev2/LICENSE` & `large-image-source-rasterio-1.23.1.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.23.1.dev2/PKG-INFO` & `large-image-source-rasterio-1.23.1.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.23.1.dev2
+Version: 1.23.1.dev4
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-rasterio-1.23.1.dev2/README.rst` & `large-image-source-rasterio-1.23.1.dev4/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.23.1.dev2/large_image_source_rasterio/__init__.py` & `large-image-source-rasterio-1.23.1.dev4/large_image_source_rasterio/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.23.1.dev2/large_image_source_rasterio/girder_source.py` & `large-image-source-rasterio-1.23.1.dev4/large_image_source_rasterio/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.23.1.dev2/large_image_source_rasterio.egg-info/PKG-INFO` & `large-image-source-rasterio-1.23.1.dev4/large_image_source_rasterio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.23.1.dev2
+Version: 1.23.1.dev4
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-rasterio-1.23.1.dev2/setup.py` & `large-image-source-rasterio-1.23.1.dev4/setup.py`

 * *Files identical despite different names*

