# Comparing `tmp/wafermap-clustering-0.2.2.tar.gz` & `tmp/wafermap-clustering-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafermap-clustering-0.2.2.tar", last modified: Mon Jun 26 08:49:58 2023, max compression
+gzip compressed data, was "wafermap-clustering-0.2.3.tar", last modified: Mon Jun 26 08:56:30 2023, max compression
```

## Comparing `wafermap-clustering-0.2.2.tar` & `wafermap-clustering-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 08:49:58.488990 wafermap-clustering-0.2.2/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0      561 2023-06-26 08:49:58.487007 wafermap-clustering-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-26 08:49:58.489997 wafermap-clustering-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      910 2023-06-26 08:49:27.000000 wafermap-clustering-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 08:49:58.422266 wafermap-clustering-0.2.2/tests/
--rw-rw-rw-   0        0        0     7900 2023-06-26 07:49:34.000000 wafermap-clustering-0.2.2/tests/test_clustering.py
-drwxrwxrwx   0        0        0        0 2023-06-26 08:49:58.427265 wafermap-clustering-0.2.2/wafermap_clustering/
-drwxrwxrwx   0        0        0        0 2023-06-26 08:49:58.461073 wafermap-clustering-0.2.2/wafermap_clustering/configs/
--rw-rw-rw-   0        0        0     4769 2023-06-26 07:52:53.000000 wafermap-clustering-0.2.2/wafermap_clustering/configs/config.py
--rw-rw-rw-   0        0        0     1275 2023-06-26 07:55:59.000000 wafermap-clustering-0.2.2/wafermap_clustering/configs/logging_config.py
-drwxrwxrwx   0        0        0        0 2023-06-26 08:49:58.464723 wafermap-clustering-0.2.2/wafermap_clustering/libs/
--rw-rw-rw-   0        0        0     4304 2023-04-06 09:28:27.000000 wafermap-clustering-0.2.2/wafermap_clustering/libs/klarf_lib.py
-drwxrwxrwx   0        0        0        0 2023-06-26 08:49:58.482992 wafermap-clustering-0.2.2/wafermap_clustering/models/
--rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.2.2/wafermap_clustering/models/clustered_defect.py
--rw-rw-rw-   0        0        0      521 2023-04-06 11:28:53.000000 wafermap-clustering-0.2.2/wafermap_clustering/models/clustering_performance.py
--rw-rw-rw-   0        0        0      763 2023-04-06 10:14:19.000000 wafermap-clustering-0.2.2/wafermap_clustering/models/clustering_result.py
--rw-rw-rw-   0        0        0      405 2023-03-31 19:52:57.000000 wafermap-clustering-0.2.2/wafermap_clustering/models/config.py
--rw-rw-rw-   0        0        0     5113 2023-06-26 07:56:19.000000 wafermap-clustering-0.2.2/wafermap_clustering/wafermap_clustering.py
-drwxrwxrwx   0        0        0        0 2023-06-26 08:49:58.451071 wafermap-clustering-0.2.2/wafermap_clustering.egg-info/
--rw-rw-rw-   0        0        0      561 2023-06-26 08:49:58.000000 wafermap-clustering-0.2.2/wafermap_clustering.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-06-26 08:49:58.000000 wafermap-clustering-0.2.2/wafermap_clustering.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 08:49:58.000000 wafermap-clustering-0.2.2/wafermap_clustering.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-26 08:49:58.000000 wafermap-clustering-0.2.2/wafermap_clustering.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-26 08:49:58.000000 wafermap-clustering-0.2.2/wafermap_clustering.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 08:56:30.990756 wafermap-clustering-0.2.3/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      568 2023-06-26 08:56:30.988738 wafermap-clustering-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 08:56:30.991256 wafermap-clustering-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      917 2023-06-26 08:51:49.000000 wafermap-clustering-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:56:30.920610 wafermap-clustering-0.2.3/tests/
+-rw-rw-rw-   0        0        0     7900 2023-06-26 07:49:34.000000 wafermap-clustering-0.2.3/tests/test_clustering.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:56:30.923785 wafermap-clustering-0.2.3/wafermap_clustering/
+drwxrwxrwx   0        0        0        0 2023-06-26 08:56:30.960576 wafermap-clustering-0.2.3/wafermap_clustering/configs/
+-rw-rw-rw-   0        0        0     4769 2023-06-26 07:52:53.000000 wafermap-clustering-0.2.3/wafermap_clustering/configs/config.py
+-rw-rw-rw-   0        0        0     1275 2023-06-26 07:55:59.000000 wafermap-clustering-0.2.3/wafermap_clustering/configs/logging_config.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:56:30.966315 wafermap-clustering-0.2.3/wafermap_clustering/libs/
+-rw-rw-rw-   0        0        0     4304 2023-04-06 09:28:27.000000 wafermap-clustering-0.2.3/wafermap_clustering/libs/klarf_lib.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:56:30.984455 wafermap-clustering-0.2.3/wafermap_clustering/models/
+-rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.2.3/wafermap_clustering/models/clustered_defect.py
+-rw-rw-rw-   0        0        0      521 2023-04-06 11:28:53.000000 wafermap-clustering-0.2.3/wafermap_clustering/models/clustering_performance.py
+-rw-rw-rw-   0        0        0      763 2023-04-06 10:14:19.000000 wafermap-clustering-0.2.3/wafermap_clustering/models/clustering_result.py
+-rw-rw-rw-   0        0        0      405 2023-03-31 19:52:57.000000 wafermap-clustering-0.2.3/wafermap_clustering/models/config.py
+-rw-rw-rw-   0        0        0     5113 2023-06-26 07:56:19.000000 wafermap-clustering-0.2.3/wafermap_clustering/wafermap_clustering.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:56:30.951747 wafermap-clustering-0.2.3/wafermap_clustering.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-06-26 08:56:30.000000 wafermap-clustering-0.2.3/wafermap_clustering.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-06-26 08:56:30.000000 wafermap-clustering-0.2.3/wafermap_clustering.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 08:56:30.000000 wafermap-clustering-0.2.3/wafermap_clustering.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-26 08:56:30.000000 wafermap-clustering-0.2.3/wafermap_clustering.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-26 08:56:30.000000 wafermap-clustering-0.2.3/wafermap_clustering.egg-info/top_level.txt
```

### Comparing `wafermap-clustering-0.2.2/LICENSE.txt` & `wafermap-clustering-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.2/PKG-INFO` & `wafermap-clustering-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.2.2
+Version: 0.2.3
 Summary: A project to apply clustering on wafermaps
-Home-page: https://github.com/Impro02/klarf_reader
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.2.tar.gz
+Home-page: https://github.com/Impro02/wafermap-clustering
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.3.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.2.2/tests/test_clustering.py` & `wafermap-clustering-0.2.3/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.2/wafermap_clustering/configs/config.py` & `wafermap-clustering-0.2.3/wafermap_clustering/configs/config.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.2/wafermap_clustering/configs/logging_config.py` & `wafermap-clustering-0.2.3/wafermap_clustering/configs/logging_config.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.2/wafermap_clustering/libs/klarf_lib.py` & `wafermap-clustering-0.2.3/wafermap_clustering/libs/klarf_lib.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.2/wafermap_clustering/models/clustering_performance.py` & `wafermap-clustering-0.2.3/wafermap_clustering/models/clustering_performance.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.2/wafermap_clustering/models/clustering_result.py` & `wafermap-clustering-0.2.3/wafermap_clustering/models/clustering_result.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.2/wafermap_clustering/wafermap_clustering.py` & `wafermap-clustering-0.2.3/wafermap_clustering/wafermap_clustering.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.2/wafermap_clustering.egg-info/PKG-INFO` & `wafermap-clustering-0.2.3/wafermap_clustering.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.2.2
+Version: 0.2.3
 Summary: A project to apply clustering on wafermaps
-Home-page: https://github.com/Impro02/klarf_reader
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.2.tar.gz
+Home-page: https://github.com/Impro02/wafermap-clustering
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.3.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.2.2/wafermap_clustering.egg-info/SOURCES.txt` & `wafermap-clustering-0.2.3/wafermap_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

