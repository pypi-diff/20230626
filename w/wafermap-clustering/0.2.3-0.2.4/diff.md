# Comparing `tmp/wafermap-clustering-0.2.3.tar.gz` & `tmp/wafermap-clustering-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafermap-clustering-0.2.3.tar", last modified: Mon Jun 26 08:56:30 2023, max compression
+gzip compressed data, was "wafermap-clustering-0.2.4.tar", last modified: Mon Jun 26 09:23:19 2023, max compression
```

## Comparing `wafermap-clustering-0.2.3.tar` & `wafermap-clustering-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 08:56:30.990756 wafermap-clustering-0.2.3/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.2.3/LICENSE.txt
--rw-rw-rw-   0        0        0      568 2023-06-26 08:56:30.988738 wafermap-clustering-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.2.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-26 08:56:30.991256 wafermap-clustering-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      917 2023-06-26 08:51:49.000000 wafermap-clustering-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 08:56:30.920610 wafermap-clustering-0.2.3/tests/
--rw-rw-rw-   0        0        0     7900 2023-06-26 07:49:34.000000 wafermap-clustering-0.2.3/tests/test_clustering.py
-drwxrwxrwx   0        0        0        0 2023-06-26 08:56:30.923785 wafermap-clustering-0.2.3/wafermap_clustering/
-drwxrwxrwx   0        0        0        0 2023-06-26 08:56:30.960576 wafermap-clustering-0.2.3/wafermap_clustering/configs/
--rw-rw-rw-   0        0        0     4769 2023-06-26 07:52:53.000000 wafermap-clustering-0.2.3/wafermap_clustering/configs/config.py
--rw-rw-rw-   0        0        0     1275 2023-06-26 07:55:59.000000 wafermap-clustering-0.2.3/wafermap_clustering/configs/logging_config.py
-drwxrwxrwx   0        0        0        0 2023-06-26 08:56:30.966315 wafermap-clustering-0.2.3/wafermap_clustering/libs/
--rw-rw-rw-   0        0        0     4304 2023-04-06 09:28:27.000000 wafermap-clustering-0.2.3/wafermap_clustering/libs/klarf_lib.py
-drwxrwxrwx   0        0        0        0 2023-06-26 08:56:30.984455 wafermap-clustering-0.2.3/wafermap_clustering/models/
--rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.2.3/wafermap_clustering/models/clustered_defect.py
--rw-rw-rw-   0        0        0      521 2023-04-06 11:28:53.000000 wafermap-clustering-0.2.3/wafermap_clustering/models/clustering_performance.py
--rw-rw-rw-   0        0        0      763 2023-04-06 10:14:19.000000 wafermap-clustering-0.2.3/wafermap_clustering/models/clustering_result.py
--rw-rw-rw-   0        0        0      405 2023-03-31 19:52:57.000000 wafermap-clustering-0.2.3/wafermap_clustering/models/config.py
--rw-rw-rw-   0        0        0     5113 2023-06-26 07:56:19.000000 wafermap-clustering-0.2.3/wafermap_clustering/wafermap_clustering.py
-drwxrwxrwx   0        0        0        0 2023-06-26 08:56:30.951747 wafermap-clustering-0.2.3/wafermap_clustering.egg-info/
--rw-rw-rw-   0        0        0      568 2023-06-26 08:56:30.000000 wafermap-clustering-0.2.3/wafermap_clustering.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-06-26 08:56:30.000000 wafermap-clustering-0.2.3/wafermap_clustering.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 08:56:30.000000 wafermap-clustering-0.2.3/wafermap_clustering.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-26 08:56:30.000000 wafermap-clustering-0.2.3/wafermap_clustering.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-26 08:56:30.000000 wafermap-clustering-0.2.3/wafermap_clustering.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 09:23:19.249531 wafermap-clustering-0.2.4/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.2.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      568 2023-06-26 09:23:19.245945 wafermap-clustering-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 09:23:19.250531 wafermap-clustering-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      917 2023-06-26 09:21:35.000000 wafermap-clustering-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:23:19.182350 wafermap-clustering-0.2.4/tests/
+-rw-rw-rw-   0        0        0     7725 2023-06-26 09:12:45.000000 wafermap-clustering-0.2.4/tests/test_clustering.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:23:19.186890 wafermap-clustering-0.2.4/wafermap_clustering/
+drwxrwxrwx   0        0        0        0 2023-06-26 09:23:19.219071 wafermap-clustering-0.2.4/wafermap_clustering/configs/
+-rw-rw-rw-   0        0        0     3472 2023-06-26 09:19:26.000000 wafermap-clustering-0.2.4/wafermap_clustering/configs/config.py
+-rw-rw-rw-   0        0        0      913 2023-06-26 09:21:07.000000 wafermap-clustering-0.2.4/wafermap_clustering/configs/logging_config.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:23:19.224777 wafermap-clustering-0.2.4/wafermap_clustering/libs/
+-rw-rw-rw-   0        0        0     4304 2023-04-06 09:28:27.000000 wafermap-clustering-0.2.4/wafermap_clustering/libs/klarf_lib.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:23:19.241175 wafermap-clustering-0.2.4/wafermap_clustering/models/
+-rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.2.4/wafermap_clustering/models/clustered_defect.py
+-rw-rw-rw-   0        0        0      521 2023-04-06 11:28:53.000000 wafermap-clustering-0.2.4/wafermap_clustering/models/clustering_performance.py
+-rw-rw-rw-   0        0        0      763 2023-04-06 10:14:19.000000 wafermap-clustering-0.2.4/wafermap_clustering/models/clustering_result.py
+-rw-rw-rw-   0        0        0     5142 2023-06-26 09:20:09.000000 wafermap-clustering-0.2.4/wafermap_clustering/wafermap_clustering.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:23:19.210901 wafermap-clustering-0.2.4/wafermap_clustering.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-06-26 09:23:19.000000 wafermap-clustering-0.2.4/wafermap_clustering.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      582 2023-06-26 09:23:19.000000 wafermap-clustering-0.2.4/wafermap_clustering.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 09:23:19.000000 wafermap-clustering-0.2.4/wafermap_clustering.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-26 09:23:19.000000 wafermap-clustering-0.2.4/wafermap_clustering.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-26 09:23:19.000000 wafermap-clustering-0.2.4/wafermap_clustering.egg-info/top_level.txt
```

### Comparing `wafermap-clustering-0.2.3/LICENSE.txt` & `wafermap-clustering-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.3/PKG-INFO` & `wafermap-clustering-0.2.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.2.3
+Version: 0.2.4
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.3.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.4.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.2.3/setup.py` & `wafermap-clustering-0.2.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.2.3"
+version = "0.2.4"
 
 setup(
     name="wafermap-clustering",
     version=version,
     packages=[
         "wafermap_clustering",
         "wafermap_clustering.configs",
```

### Comparing `wafermap-clustering-0.2.3/tests/test_clustering.py` & `wafermap-clustering-0.2.4/tests/test_clustering.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 # MODULES
 from pathlib import Path
 from collections import Counter
 
 # UNITTEST
 import unittest
 
-# LIBS
+# WAFERMAP_CLUSTERING
 from wafermap_clustering.wafermap_clustering import Clustering
-from wafermap_clustering.models.config import DBSCANConfig, HDBSCANConfig
-
-# CONFIGS
 from wafermap_clustering.configs.config import (
     ClusteringMode,
     Config,
-    ClusteringConfig,
     KlarfFormat,
 )
 
-from wafermap_clustering.configs import logging_config
-
 ASSETS_PATH: Path = Path(__file__).parent / "assets"
 ASSETS_OUPUT_PATH: Path = ASSETS_PATH / "clustering" / "output"
 
 
 def compare_files(file1_path, file2_path):
     with open(file1_path, "r") as file1, open(file2_path, "r") as file2:
         for i, (line1, line2) in enumerate(zip(file1, file2)):
@@ -36,15 +30,15 @@
     def setUp(self) -> None:
         self.path_klarf_single_wafer = ASSETS_PATH / "J052SBN_8196_J052SBN-01.000"
         self.path_klarf_multi_wafers = ASSETS_PATH / "J237DTA_3236.000"
         self.path_klarf_single_wafer_large_klarf = ASSETS_PATH / "LARGE_KLARF.000"
 
         self.config = Config(
             platform="windows",
-            conf_path=Path(__file__).parent / "assets" / "conf" / "config.json",
+            conf_path=ASSETS_PATH / "conf" / "config.json",
         )
 
     def test_clustering_dbscan_single_wafer(self):
         # GIVEN
         expected_summary = [
             {
                 "result_timestamp": "02-23-21 06:10:02",
```

### Comparing `wafermap-clustering-0.2.3/wafermap_clustering/configs/config.py` & `wafermap-clustering-0.2.4/wafermap_clustering/configs/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 # MODULES
 import json
-import platform
 import os
 from enum import Enum
 from pathlib import Path
 from dataclasses import dataclass, field
 
-# MODELS
-from ..models.config import Config, ClusteringConfig, DBSCANConfig, HDBSCANConfig
-
 
 class KlarfFormat(Enum):
     BABY = "baby"
     FULL = "full"
 
 
 class ClusteringMode(Enum):
     DBSCAN = "dbscan"
     HDBSCAN = "hdbscan"
 
 
 @dataclass
+class DBSCANConfig:
+    min_samples: int
+    eps: int
+
+
+@dataclass
+class HDBSCANConfig:
+    min_samples: int
+    min_cluster_size: int
+
+
+@dataclass
+class ClusteringConfig:
+    dbscan: DBSCANConfig
+    hdbscan: HDBSCANConfig
+
+
+@dataclass
 class DirectoryConfig:
     root: str
     home: str
     logs: str
     tmp: str
 
 
@@ -97,47 +111,7 @@
                     if isinstance(value, (dict, list)):
                         traverse(value)
                     else:
                         obj[i] = replace_variable(value)
 
         traverse(replaced_config)
         return replaced_config
-
-
-"""
-def load_config(filepath: Path):
-    root_config, clustering_config, dbscan_config, hdbscan_config = {}, {}, {}, {}
-    if os.path.exists(filepath):
-        with open(filepath, encoding="utf-8") as json_data_file:
-            try:
-                root_config: dict = json.load(json_data_file)
-                clustering_config = root_config.get("clustering", {})
-                dbscan_config = clustering_config.get("dbscan", {})
-                hdbscan_config = clustering_config.get("hdbscan", {})
-            except Exception as ex:
-                print(f"Configuration file {filepath} is invalid: {ex}")
-                exit()
-
-    return Config(
-        platform=platform.system().lower(),
-        attribute=root_config.get("attribute", None),
-        clustering=ClusteringConfig(
-            dbscan=DBSCANConfig(
-                min_samples=dbscan_config.get("min_samples", None),
-                eps=dbscan_config.get("eps", None),
-            ),
-            hdbscan=HDBSCANConfig(
-                min_samples=hdbscan_config.get("min_samples", None),
-                min_cluster_size=hdbscan_config.get("eps", None),
-            ),
-        ),
-    )
-"""
-
-# CONFIGS_CLUSTERING_PATH = Path().parent / "config.json"
-# CONFIGS = load_config(filepath=CONFIGS_CLUSTERING_PATH)
-
-
-CONFIGS = Config(
-    platform=platform.system().lower(),
-    conf_path=Path(__file__).parent / "config.json",
-)
```

### Comparing `wafermap-clustering-0.2.3/wafermap_clustering/libs/klarf_lib.py` & `wafermap-clustering-0.2.4/wafermap_clustering/libs/klarf_lib.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.3/wafermap_clustering/models/clustering_performance.py` & `wafermap-clustering-0.2.4/wafermap_clustering/models/clustering_performance.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.3/wafermap_clustering/models/clustering_result.py` & `wafermap-clustering-0.2.4/wafermap_clustering/models/clustering_result.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.2.3/wafermap_clustering/wafermap_clustering.py` & `wafermap-clustering-0.2.4/wafermap_clustering/wafermap_clustering.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,39 +13,40 @@
 # HDBSCAN
 from hdbscan import HDBSCAN
 
 # KLARF_READER
 from klarf_reader.klarf import Klarf
 from klarf_reader.utils import klarf_convert
 
-from wafermap_clustering.configs.config import ClusteringMode, KlarfFormat
-from wafermap_clustering.models.clustering_performance import ClusteringPerformance
-
 # MODELS
-from .models.config import Config
 from .models.clustered_defect import ClusteredDefect
+from .models.clustering_performance import ClusteringPerformance
 from .models.clustering_result import ClusteringResult
 
 # LIBS
 from .libs import klarf_lib
 
 # CONFIGS
+from .configs.config import ClusteringMode, Config, KlarfFormat
 from .configs.logging_config import setup_logger
 
 
 class Clustering:
     def __init__(
         self,
         config: Config,
         logger: Logger = None,
         autocreate_logger: bool = False,
     ) -> None:
         self.config = config
         self.logger = (
-            setup_logger(name="clustering")
+            setup_logger(
+                name="clustering",
+                directory=Path(self.config.directories.logs),
+            )
             if autocreate_logger and logger is None
             else logger
         )
 
     def apply(
         self,
         klarf_path: Path,
```

### Comparing `wafermap-clustering-0.2.3/wafermap_clustering.egg-info/PKG-INFO` & `wafermap-clustering-0.2.4/wafermap_clustering.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.2.3
+Version: 0.2.4
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.3.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.2.4.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.2.3/wafermap_clustering.egg-info/SOURCES.txt` & `wafermap-clustering-0.2.4/wafermap_clustering.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 wafermap_clustering.egg-info/requires.txt
 wafermap_clustering.egg-info/top_level.txt
 wafermap_clustering/configs/config.py
 wafermap_clustering/configs/logging_config.py
 wafermap_clustering/libs/klarf_lib.py
 wafermap_clustering/models/clustered_defect.py
 wafermap_clustering/models/clustering_performance.py
-wafermap_clustering/models/clustering_result.py
-wafermap_clustering/models/config.py
+wafermap_clustering/models/clustering_result.py
```

