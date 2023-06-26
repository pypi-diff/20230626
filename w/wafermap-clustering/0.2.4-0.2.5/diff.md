# Comparing `tmp/wafermap-clustering-0.2.4.tar.gz` & `tmp/wafermap-clustering-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafermap-clustering-0.2.4.tar", last modified: Mon Jun 26 09:23:19 2023, max compression
+gzip compressed data, was "wafermap-clustering-0.2.5.tar", last modified: Mon Jun 26 13:29:42 2023, max compression
```

## Comparing `wafermap-clustering-0.2.4.tar` & `wafermap-clustering-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 09:23:19.249531 wafermap-clustering-0.2.4/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.2.4/LICENSE.txt
--rw-rw-rw-   0        0        0      568 2023-06-26 09:23:19.245945 wafermap-clustering-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-26 09:23:19.250531 wafermap-clustering-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      917 2023-06-26 09:21:35.000000 wafermap-clustering-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:23:19.182350 wafermap-clustering-0.2.4/tests/
--rw-rw-rw-   0        0        0     7725 2023-06-26 09:12:45.000000 wafermap-clustering-0.2.4/tests/test_clustering.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:23:19.186890 wafermap-clustering-0.2.4/wafermap_clustering/
-drwxrwxrwx   0        0        0        0 2023-06-26 09:23:19.219071 wafermap-clustering-0.2.4/wafermap_clustering/configs/
--rw-rw-rw-   0        0        0     3472 2023-06-26 09:19:26.000000 wafermap-clustering-0.2.4/wafermap_clustering/configs/config.py
--rw-rw-rw-   0        0        0      913 2023-06-26 09:21:07.000000 wafermap-clustering-0.2.4/wafermap_clustering/configs/logging_config.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:23:19.224777 wafermap-clustering-0.2.4/wafermap_clustering/libs/
--rw-rw-rw-   0        0        0     4304 2023-04-06 09:28:27.000000 wafermap-clustering-0.2.4/wafermap_clustering/libs/klarf_lib.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:23:19.241175 wafermap-clustering-0.2.4/wafermap_clustering/models/
--rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.2.4/wafermap_clustering/models/clustered_defect.py
--rw-rw-rw-   0        0        0      521 2023-04-06 11:28:53.000000 wafermap-clustering-0.2.4/wafermap_clustering/models/clustering_performance.py
--rw-rw-rw-   0        0        0      763 2023-04-06 10:14:19.000000 wafermap-clustering-0.2.4/wafermap_clustering/models/clustering_result.py
--rw-rw-rw-   0        0        0     5142 2023-06-26 09:20:09.000000 wafermap-clustering-0.2.4/wafermap_clustering/wafermap_clustering.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:23:19.210901 wafermap-clustering-0.2.4/wafermap_clustering.egg-info/
--rw-rw-rw-   0        0        0      568 2023-06-26 09:23:19.000000 wafermap-clustering-0.2.4/wafermap_clustering.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2023-06-26 09:23:19.000000 wafermap-clustering-0.2.4/wafermap_clustering.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 09:23:19.000000 wafermap-clustering-0.2.4/wafermap_clustering.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-26 09:23:19.000000 wafermap-clustering-0.2.4/wafermap_clustering.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-26 09:23:19.000000 wafermap-clustering-0.2.4/wafermap_clustering.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 13:29:42.371841 wafermap-clustering-0.2.5/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      568 2023-06-26 13:29:42.368845 wafermap-clustering-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 13:29:42.372712 wafermap-clustering-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      917 2023-06-26 13:28:21.000000 wafermap-clustering-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:29:42.283073 wafermap-clustering-0.2.5/tests/
+-rw-rw-rw-   0        0        0     7745 2023-06-26 13:24:39.000000 wafermap-clustering-0.2.5/tests/test_clustering.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:29:42.288255 wafermap-clustering-0.2.5/wafermap_clustering/
+drwxrwxrwx   0        0        0        0 2023-06-26 13:29:42.335161 wafermap-clustering-0.2.5/wafermap_clustering/configs/
+-rw-rw-rw-   0        0        0     3472 2023-06-26 09:19:26.000000 wafermap-clustering-0.2.5/wafermap_clustering/configs/config.py
+-rw-rw-rw-   0        0        0      913 2023-06-26 09:21:07.000000 wafermap-clustering-0.2.5/wafermap_clustering/configs/logging_config.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:29:42.342509 wafermap-clustering-0.2.5/wafermap_clustering/libs/
+-rw-rw-rw-   0        0        0     4304 2023-04-06 09:28:27.000000 wafermap-clustering-0.2.5/wafermap_clustering/libs/klarf_lib.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:29:42.362126 wafermap-clustering-0.2.5/wafermap_clustering/models/
+-rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.2.5/wafermap_clustering/models/clustered_defect.py
+-rw-rw-rw-   0        0        0      521 2023-04-06 11:28:53.000000 wafermap-clustering-0.2.5/wafermap_clustering/models/clustering_performance.py
+-rw-rw-rw-   0        0        0      763 2023-04-06 10:14:19.000000 wafermap-clustering-0.2.5/wafermap_clustering/models/clustering_result.py
+-rw-rw-rw-   0        0        0     5464 2023-06-26 13:27:41.000000 wafermap-clustering-0.2.5/wafermap_clustering/wafermap_clustering.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:29:42.321889 wafermap-clustering-0.2.5/wafermap_clustering.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-06-26 13:29:42.000000 wafermap-clustering-0.2.5/wafermap_clustering.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      582 2023-06-26 13:29:42.000000 wafermap-clustering-0.2.5/wafermap_clustering.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 13:29:42.000000 wafermap-clustering-0.2.5/wafermap_clustering.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-26 13:29:42.000000 wafermap-clustering-0.2.5/wafermap_clustering.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-26 13:29:42.000000 wafermap-clustering-0.2.5/wafermap_clustering.egg-info/top_level.txt
```

### Comparing `wafermap-clustering-0.2.4/LICENSE.txt` & `wafermap-clustering-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.4/PKG-INFO` & `wafermap-clustering-0.2.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.2.4
+Version: 0.2.5
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.4.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.5.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.2.4/setup.py` & `wafermap-clustering-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.2.4"
+version = "0.2.5"
 
 setup(
     name="wafermap-clustering",
     version=version,
     packages=[
         "wafermap_clustering",
         "wafermap_clustering.configs",
```

### Comparing `wafermap-clustering-0.2.4/tests/test_clustering.py` & `wafermap-clustering-0.2.5/tests/test_clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             }
         ]
 
         # WHEN
         clustering = Clustering(config=self.config, autocreate_logger=True)
         results = clustering.apply(
             self.path_klarf_single_wafer_large_klarf,
-            output_path=ASSETS_OUPUT_PATH,
+            output_directory=ASSETS_OUPUT_PATH,
             klarf_format=KlarfFormat.FULL.value,
         )
 
         summary = [
             {
                 "result_timestamp": res.result_timestamp,
                 "lot_id": res.lot_id,
@@ -129,15 +129,15 @@
 
         expected_clusters = [615]
 
         # WHEN
         clustering = Clustering(config=self.config, autocreate_logger=True)
         results = clustering.apply(
             klarf_path=self.path_klarf_single_wafer,
-            output_path=output_path,
+            output_directory=output_path,
             klarf_format=KlarfFormat.FULL.value,
             clustering_mode=ClusteringMode.HDBSCAN.value,
         )
 
         # THEN
         self.assertEqual([res.clusters for res in results], expected_clusters)
 
@@ -209,15 +209,15 @@
         output_path = ASSETS_OUPUT_PATH / "J237DTA_3236_clustered.000"
         saved_klarf_path = ASSETS_PATH / "saved" / "J237DTA_3236_baby_clustered.000"
 
         # WHEN
         clustering = Clustering(config=self.config, autocreate_logger=True)
         clustering.apply(
             klarf_path=self.path_klarf_multi_wafers,
-            output_path=output_path,
+            output_directory=output_path,
             klarf_format=KlarfFormat.BABY.value,
         )
 
         # THEN
         self.assertEqual(
             compare_files(saved_klarf_path, output_path),
             True,
@@ -228,15 +228,15 @@
         output_path = ASSETS_OUPUT_PATH / "J237DTA_3236_clustered.000"
         saved_klarf_path = ASSETS_PATH / "saved" / "J237DTA_3236_full_clustered.000"
 
         # WHEN
         clustering = Clustering(config=self.config, autocreate_logger=True)
         clustering.apply(
             klarf_path=self.path_klarf_multi_wafers,
-            output_path=output_path,
+            output_directory=output_path,
             klarf_format=KlarfFormat.FULL.value,
         )
 
         # THEN
         self.assertEqual(
             compare_files(saved_klarf_path, output_path),
             True,
```

### Comparing `wafermap-clustering-0.2.4/wafermap_clustering/configs/config.py` & `wafermap-clustering-0.2.5/wafermap_clustering/configs/config.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.4/wafermap_clustering/configs/logging_config.py` & `wafermap-clustering-0.2.5/wafermap_clustering/configs/logging_config.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.4/wafermap_clustering/libs/klarf_lib.py` & `wafermap-clustering-0.2.5/wafermap_clustering/libs/klarf_lib.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.4/wafermap_clustering/models/clustering_performance.py` & `wafermap-clustering-0.2.5/wafermap_clustering/models/clustering_performance.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.4/wafermap_clustering/models/clustering_result.py` & `wafermap-clustering-0.2.5/wafermap_clustering/models/clustering_result.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.4/wafermap_clustering/wafermap_clustering.py` & `wafermap-clustering-0.2.5/wafermap_clustering/wafermap_clustering.py`

 * *Files 15% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             if autocreate_logger and logger is None
             else logger
         )
 
     def apply(
         self,
         klarf_path: Path,
-        output_path: Path = None,
+        output_directory: Path = None,
         klarf_format=KlarfFormat.BABY.value,
         clustering_mode=ClusteringMode.DBSCAN.value,
     ) -> List[ClusteringResult]:
 
         klarf_content, raw_content = Klarf.load_from_file_with_raw_content(
             filepath=klarf_path
         )
@@ -110,27 +110,35 @@
                 step_id=single_klarf.step_id,
                 wafer_id=single_klarf.wafer.id,
                 clusters=clusters,
                 clustered_defects=clustered_defects,
             )
 
             output_timestamp = None
+            output_filename = (
+                (
+                    output_directory
+                    / f"{single_klarf.lot_id}_{single_klarf.step_id}_{single_klarf.wafer.id}.000"
+                )
+                if output_directory is not None
+                else None
+            )
             match klarf_format:
-                case KlarfFormat.BABY.value if output_path is not None:
+                case KlarfFormat.BABY.value if output_directory is not None:
                     output_timestamp = klarf_lib.write_baby_klarf(
                         clustering_result=clustering_result,
                         attribute=self.config.attribute,
-                        output_filename=output_path,
+                        output_filename=output_filename,
                     )
-                case KlarfFormat.FULL.value if output_path is not None:
+                case KlarfFormat.FULL.value if output_directory is not None:
                     output_timestamp = klarf_lib.write_full_klarf(
                         raw_content=raw_content,
                         clustering_result=clustering_result,
                         attribute=self.config.attribute,
-                        output_filename=output_path,
+                        output_filename=output_filename,
                     )
 
             clustering_result.performance = ClusteringPerformance(
                 clustering_timestamp=round(clustering_timestamp, 3),
                 output_timestamp=round(output_timestamp, 3)
                 if output_timestamp is not None
                 else None,
```

### Comparing `wafermap-clustering-0.2.4/wafermap_clustering.egg-info/PKG-INFO` & `wafermap-clustering-0.2.5/wafermap_clustering.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.2.4
+Version: 0.2.5
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.4.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.5.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.2.4/wafermap_clustering.egg-info/SOURCES.txt` & `wafermap-clustering-0.2.5/wafermap_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

