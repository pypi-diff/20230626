# Comparing `tmp/large-image-source-vips-1.23.0.tar.gz` & `tmp/large-image-source-vips-1.23.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-vips-1.23.0.tar", last modified: Thu Jun 22 21:41:42 2023, max compression
+gzip compressed data, was "large-image-source-vips-1.23.1.dev2.tar", last modified: Mon Jun 26 12:54:00 2023, max compression
```

## Comparing `large-image-source-vips-1.23.0.tar` & `large-image-source-vips-1.23.1.dev2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-22 21:41:42.815100 large-image-source-vips-1.23.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-06-22 21:41:42.000000 large-image-source-vips-1.23.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      914 2023-06-22 21:41:42.815100 large-image-source-vips-1.23.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-06-22 21:41:42.000000 large-image-source-vips-1.23.0/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-22 21:41:42.815100 large-image-source-vips-1.23.0/large_image_source_vips/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24064 2023-06-22 21:39:48.000000 large-image-source-vips-1.23.0/large_image_source_vips/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      374 2023-06-22 21:39:48.000000 large-image-source-vips-1.23.0/large_image_source_vips/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-22 21:41:42.815100 large-image-source-vips-1.23.0/large_image_source_vips.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      914 2023-06-22 21:41:42.000000 large-image-source-vips-1.23.0/large_image_source_vips.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      388 2023-06-22 21:41:42.000000 large-image-source-vips-1.23.0/large_image_source_vips.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-22 21:41:42.000000 large-image-source-vips-1.23.0/large_image_source_vips.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2023-06-22 21:41:42.000000 large-image-source-vips-1.23.0/large_image_source_vips.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      120 2023-06-22 21:41:42.000000 large-image-source-vips-1.23.0/large_image_source_vips.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-06-22 21:41:42.000000 large-image-source-vips-1.23.0/large_image_source_vips.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-22 21:41:42.815100 large-image-source-vips-1.23.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2590 2023-06-22 21:39:48.000000 large-image-source-vips-1.23.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-26 12:54:00.089053 large-image-source-vips-1.23.1.dev2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-06-26 12:53:59.000000 large-image-source-vips-1.23.1.dev2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      919 2023-06-26 12:54:00.089053 large-image-source-vips-1.23.1.dev2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-06-26 12:53:59.000000 large-image-source-vips-1.23.1.dev2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-26 12:54:00.085052 large-image-source-vips-1.23.1.dev2/large_image_source_vips/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24064 2023-06-26 12:51:56.000000 large-image-source-vips-1.23.1.dev2/large_image_source_vips/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      374 2023-06-26 12:51:56.000000 large-image-source-vips-1.23.1.dev2/large_image_source_vips/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-26 12:54:00.089053 large-image-source-vips-1.23.1.dev2/large_image_source_vips.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      919 2023-06-26 12:53:59.000000 large-image-source-vips-1.23.1.dev2/large_image_source_vips.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      388 2023-06-26 12:54:00.000000 large-image-source-vips-1.23.1.dev2/large_image_source_vips.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-26 12:53:59.000000 large-image-source-vips-1.23.1.dev2/large_image_source_vips.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2023-06-26 12:53:59.000000 large-image-source-vips-1.23.1.dev2/large_image_source_vips.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      125 2023-06-26 12:53:59.000000 large-image-source-vips-1.23.1.dev2/large_image_source_vips.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-06-26 12:53:59.000000 large-image-source-vips-1.23.1.dev2/large_image_source_vips.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-26 12:54:00.089053 large-image-source-vips-1.23.1.dev2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2590 2023-06-26 12:51:56.000000 large-image-source-vips-1.23.1.dev2/setup.py
```

### Comparing `large-image-source-vips-1.23.0/LICENSE` & `large-image-source-vips-1.23.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.23.0/PKG-INFO` & `large-image-source-vips-1.23.1.dev2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-vips
-Version: 1.23.0
+Version: 1.23.1.dev2
 Summary: A libvips tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-vips-1.23.0/README.rst` & `large-image-source-vips-1.23.1.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.23.0/large_image_source_vips/__init__.py` & `large-image-source-vips-1.23.1.dev2/large_image_source_vips/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.23.0/large_image_source_vips.egg-info/PKG-INFO` & `large-image-source-vips-1.23.1.dev2/large_image_source_vips.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-vips
-Version: 1.23.0
+Version: 1.23.1.dev2
 Summary: A libvips tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-vips-1.23.0/setup.py` & `large-image-source-vips-1.23.1.dev2/setup.py`

 * *Files identical despite different names*

