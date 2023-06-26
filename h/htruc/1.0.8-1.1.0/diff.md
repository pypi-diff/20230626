# Comparing `tmp/htruc-1.0.8.tar.gz` & `tmp/htruc-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htruc-1.0.8.tar", last modified: Mon Jun 19 08:44:24 2023, max compression
+gzip compressed data, was "htruc-1.1.0.tar", last modified: Mon Jun 26 09:17:49 2023, max compression
```

## Comparing `htruc-1.0.8.tar` & `htruc-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:44:24.724958 htruc-1.0.8/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    16725 2023-06-19 07:16:39.000000 htruc-1.0.8/LICENSE.md
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1874 2023-06-19 08:44:24.724958 htruc-1.0.8/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1191 2022-06-20 10:01:21.000000 htruc-1.0.8/README.md
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:44:24.724958 htruc-1.0.8/htruc/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        0 2021-09-23 12:36:36.000000 htruc-1.0.8/htruc/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)    11544 2023-06-19 08:29:18.000000 htruc-1.0.8/htruc/catalog.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     8939 2023-06-19 08:19:51.000000 htruc-1.0.8/htruc/cli.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:44:24.724958 htruc-1.0.8/htruc/repos/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      118 2022-06-21 08:16:17.000000 htruc-1.0.8/htruc/repos/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      492 2022-02-04 15:30:28.000000 htruc-1.0.8/htruc/repos/_generic.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2537 2023-06-19 07:58:45.000000 htruc-1.0.8/htruc/repos/_github.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:44:24.724958 htruc-1.0.8/htruc/schemas/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1220 2022-06-20 10:01:21.000000 htruc-1.0.8/htruc/schemas/__init__.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1021 2022-06-20 10:01:21.000000 htruc-1.0.8/htruc/schemas/upgrade_path.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      130 2022-06-20 10:01:21.000000 htruc-1.0.8/htruc/types.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2390 2023-06-19 08:19:31.000000 htruc-1.0.8/htruc/utils.py
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     2882 2023-06-19 07:59:20.000000 htruc-1.0.8/htruc/validator.py
-drwxrwxr-x   0 thibault  (1000) thibault  (1000)        0 2023-06-19 08:44:24.724958 htruc-1.0.8/htruc.egg-info/
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     1874 2023-06-19 08:44:24.000000 htruc-1.0.8/htruc.egg-info/PKG-INFO
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      429 2023-06-19 08:44:24.000000 htruc-1.0.8/htruc.egg-info/SOURCES.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        1 2023-06-19 08:44:24.000000 htruc-1.0.8/htruc.egg-info/dependency_links.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       41 2023-06-19 08:44:24.000000 htruc-1.0.8/htruc.egg-info/entry_points.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)      176 2023-06-19 08:44:24.000000 htruc-1.0.8/htruc.egg-info/requires.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)        6 2023-06-19 08:44:24.000000 htruc-1.0.8/htruc.egg-info/top_level.txt
--rw-rw-r--   0 thibault  (1000) thibault  (1000)       38 2023-06-19 08:44:24.724958 htruc-1.0.8/setup.cfg
--rw-rw-r--   0 thibault  (1000) thibault  (1000)     3799 2023-06-19 08:29:31.000000 htruc-1.0.8/setup.py
+drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-06-26 09:17:49.221061 htruc-1.1.0/
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     2172 2023-06-26 09:17:49.221061 htruc-1.1.0/PKG-INFO
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     1191 2023-06-11 08:04:36.000000 htruc-1.1.0/README.md
+drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-06-26 09:17:49.221061 htruc-1.1.0/htruc/
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)        0 2023-06-11 08:04:36.000000 htruc-1.1.0/htruc/__init__.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)    11544 2023-06-26 09:08:41.000000 htruc-1.1.0/htruc/catalog.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     8939 2023-06-26 09:08:41.000000 htruc-1.1.0/htruc/cli.py
+drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-06-26 09:17:49.221061 htruc-1.1.0/htruc/repos/
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      118 2023-06-11 08:04:36.000000 htruc-1.1.0/htruc/repos/__init__.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      492 2023-06-11 08:04:36.000000 htruc-1.1.0/htruc/repos/_generic.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     2537 2023-06-26 09:08:41.000000 htruc-1.1.0/htruc/repos/_github.py
+drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-06-26 09:17:49.221061 htruc-1.1.0/htruc/schemas/
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     1375 2023-06-26 09:14:49.000000 htruc-1.1.0/htruc/schemas/__init__.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     1499 2023-06-26 09:13:32.000000 htruc-1.1.0/htruc/schemas/upgrade_path.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      130 2023-06-11 08:04:36.000000 htruc-1.1.0/htruc/types.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     2390 2023-06-26 09:08:41.000000 htruc-1.1.0/htruc/utils.py
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     2882 2023-06-26 09:08:41.000000 htruc-1.1.0/htruc/validator.py
+drwxrwxr-x   0 tclerice  (1000) tclerice  (1000)        0 2023-06-26 09:17:49.221061 htruc-1.1.0/htruc.egg-info/
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     2172 2023-06-26 09:17:49.000000 htruc-1.1.0/htruc.egg-info/PKG-INFO
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      418 2023-06-26 09:17:49.000000 htruc-1.1.0/htruc.egg-info/SOURCES.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)        1 2023-06-26 09:17:49.000000 htruc-1.1.0/htruc.egg-info/dependency_links.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)       41 2023-06-26 09:17:49.000000 htruc-1.1.0/htruc.egg-info/entry_points.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)      176 2023-06-26 09:17:49.000000 htruc-1.1.0/htruc.egg-info/requires.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)        6 2023-06-26 09:17:49.000000 htruc-1.1.0/htruc.egg-info/top_level.txt
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)       38 2023-06-26 09:17:49.221061 htruc-1.1.0/setup.cfg
+-rw-rw-r--   0 tclerice  (1000) tclerice  (1000)     3799 2023-06-26 09:17:28.000000 htruc-1.1.0/setup.py
```

### Comparing `htruc-1.0.8/PKG-INFO` & `htruc-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,57 @@
 Metadata-Version: 2.1
 Name: htruc
-Version: 1.0.8
+Version: 1.1.0
 Summary: HTRUC, a toolkit for HTR-United cataloging
 Home-page: https://github.com/htr-united/htrvc
 Author: Thibault Clérice
 License: MIT
+Description: 
+        <img src="./img/HTRUC.png" width=300 align=right>
+        
+        HTRUC
+        =====
+        
+        [![Test](https://github.com/HTR-United/HTRUC/actions/workflows/tests.yml/badge.svg)](https://github.com/HTR-United/HTRUC/actions/workflows/tests.yml)
+        
+        
+        Pronunced `EuchTruc` (*ce truc*), this contains most of the tooling for the catalog records: 
+        - Parses catalog records
+        - Test the validity of the catalog according to different schemas
+        - Builds agglomerated catalog records with optional dataviz
+        - Retrieve catalog information from all repositories of a user or an organization.
+        
+        ## Install 
+        
+        Either clone and run `python setup.py install` **or** use the pip version `pip install htruc`
+        
+        ## Use
+        
+        ### Testing a catalog record
+        
+        Simply run `htruc test YourYamlFile.yml`
+        
+        ### Upgrade a previously existing catalog record
+        
+        Run `htruc upgrade yourYamlFile.yml`
+        
+        ### Upgrade a previously existing catalog record to the newest schema
+        
+        Run `htruc upgrade yourYamlFile.yml`
+        
+        ### Upgrade metrics using [HTR-United Metadata Generator (HUMg)](https://github.com/HTR-United/htr-united-metadata-generator)
+        
+        Run `htruc update-volumes YourYamlFile.yml MetricFileFromHUMG.jons --inplace`
+        ---
+        
+        Logo by [Alix Chagué](https://alix-tz.github.io).
+        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-
-<img src="./img/HTRUC.png" width=300 align=right>
-
-HTRUC
-=====
-
-[![Test](https://github.com/HTR-United/HTRUC/actions/workflows/tests.yml/badge.svg)](https://github.com/HTR-United/HTRUC/actions/workflows/tests.yml)
-
-
-Pronunced `EuchTruc` (*ce truc*), this contains most of the tooling for the catalog records: 
-- Parses catalog records
-- Test the validity of the catalog according to different schemas
-- Builds agglomerated catalog records with optional dataviz
-- Retrieve catalog information from all repositories of a user or an organization.
-
-## Install 
-
-Either clone and run `python setup.py install` **or** use the pip version `pip install htruc`
-
-## Use
-
-### Testing a catalog record
-
-Simply run `htruc test YourYamlFile.yml`
-
-### Upgrade a previously existing catalog record
-
-Run `htruc upgrade yourYamlFile.yml`
-
-### Upgrade a previously existing catalog record to the newest schema
-
-Run `htruc upgrade yourYamlFile.yml`
-
-### Upgrade metrics using [HTR-United Metadata Generator (HUMg)](https://github.com/HTR-United/htr-united-metadata-generator)
-
-Run `htruc update-volumes YourYamlFile.yml MetricFileFromHUMG.jons --inplace`
----
-
-Logo by [Alix Chagué](https://alix-tz.github.io).
-
-
```

### Comparing `htruc-1.0.8/README.md` & `htruc-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `htruc-1.0.8/htruc/catalog.py` & `htruc-1.1.0/htruc/catalog.py`

 * *Files identical despite different names*

### Comparing `htruc-1.0.8/htruc/cli.py` & `htruc-1.1.0/htruc/cli.py`

 * *Files identical despite different names*

### Comparing `htruc-1.0.8/htruc/repos/_github.py` & `htruc-1.1.0/htruc/repos/_github.py`

 * *Files identical despite different names*

### Comparing `htruc-1.0.8/htruc/schemas/__init__.py` & `htruc-1.1.0/htruc/schemas/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from typing import Dict, Tuple, Callable, AnyStr, Iterable
-from htruc.schemas.upgrade_path import upgrade_2021_10_15_to_2022_04_15
+from htruc.schemas.upgrade_path import upgrade_2021_10_15_to_2022_04_15, upgrade_2022_04_15_to_2023_06_27
 from htruc.types import SchemaVersion, CatalogRecord
 
 
 # This Tuple is used to know which schema are supported
 UpgradeOrder: Tuple[SchemaVersion, ...] = (
     "https://htr-united.github.io/schema/2021-10-15/schema.json",
     "https://htr-united.github.io/schema/2022-04-15/schema.json",
+    "https://htr-united.github.io/schema/2023-06-27/schema.json",
 )
 
 UpgradeFunction: Dict[str, Callable[[CatalogRecord], CatalogRecord]] = {
-    UpgradeOrder[0]: upgrade_2021_10_15_to_2022_04_15
+    UpgradeOrder[0]: upgrade_2021_10_15_to_2022_04_15,
+    UpgradeOrder[1]: upgrade_2022_04_15_to_2023_06_27
 }
 
 
 def recursive_update(catalog_record: CatalogRecord) -> Tuple[CatalogRecord, Iterable[SchemaVersion]]:
     """ Automatically upgrade a schema
 
     :returns: The catalog record upgrade to the latest schema, with the list of upgrade it went through
```

### Comparing `htruc-1.0.8/htruc/schemas/upgrade_path.py` & `htruc-1.1.0/htruc/schemas/upgrade_path.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,7 +25,17 @@
     ]
     log(f"--> Automatically converted script to objects", verbose=verbose, use_log=use_log)
 
     catalog_record["production-software"] = "Unknown [Automatically filled]"
     log(f"--> Automatically upgraded with `production-software`=`Unknown`", verbose=verbose, use_log=use_log)
 
     return catalog_record
+
+
+def upgrade_2022_04_15_to_2023_06_27(catalog_record: CatalogRecord, verbose=True, use_log=False) -> CatalogRecord:
+    catalog_record["schema"] = "https://htr-united.github.io/schema/2023-06-27/schema.json"
+    log("Upgrading from 2022-04-15 to 2023-06-27", verbose=verbose, use_log=use_log)
+
+    catalog_record["automatically-aligned"] = False
+    log(f"--> Automatically set to False automatically-aligned flag", verbose=verbose, use_log=use_log)
+
+    return catalog_record
```

### Comparing `htruc-1.0.8/htruc/utils.py` & `htruc-1.1.0/htruc/utils.py`

 * *Files identical despite different names*

### Comparing `htruc-1.0.8/htruc/validator.py` & `htruc-1.1.0/htruc/validator.py`

 * *Files identical despite different names*

### Comparing `htruc-1.0.8/htruc.egg-info/PKG-INFO` & `htruc-1.1.0/htruc.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,57 @@
 Metadata-Version: 2.1
 Name: htruc
-Version: 1.0.8
+Version: 1.1.0
 Summary: HTRUC, a toolkit for HTR-United cataloging
 Home-page: https://github.com/htr-united/htrvc
 Author: Thibault Clérice
 License: MIT
+Description: 
+        <img src="./img/HTRUC.png" width=300 align=right>
+        
+        HTRUC
+        =====
+        
+        [![Test](https://github.com/HTR-United/HTRUC/actions/workflows/tests.yml/badge.svg)](https://github.com/HTR-United/HTRUC/actions/workflows/tests.yml)
+        
+        
+        Pronunced `EuchTruc` (*ce truc*), this contains most of the tooling for the catalog records: 
+        - Parses catalog records
+        - Test the validity of the catalog according to different schemas
+        - Builds agglomerated catalog records with optional dataviz
+        - Retrieve catalog information from all repositories of a user or an organization.
+        
+        ## Install 
+        
+        Either clone and run `python setup.py install` **or** use the pip version `pip install htruc`
+        
+        ## Use
+        
+        ### Testing a catalog record
+        
+        Simply run `htruc test YourYamlFile.yml`
+        
+        ### Upgrade a previously existing catalog record
+        
+        Run `htruc upgrade yourYamlFile.yml`
+        
+        ### Upgrade a previously existing catalog record to the newest schema
+        
+        Run `htruc upgrade yourYamlFile.yml`
+        
+        ### Upgrade metrics using [HTR-United Metadata Generator (HUMg)](https://github.com/HTR-United/htr-united-metadata-generator)
+        
+        Run `htruc update-volumes YourYamlFile.yml MetricFileFromHUMG.jons --inplace`
+        ---
+        
+        Logo by [Alix Chagué](https://alix-tz.github.io).
+        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-
-<img src="./img/HTRUC.png" width=300 align=right>
-
-HTRUC
-=====
-
-[![Test](https://github.com/HTR-United/HTRUC/actions/workflows/tests.yml/badge.svg)](https://github.com/HTR-United/HTRUC/actions/workflows/tests.yml)
-
-
-Pronunced `EuchTruc` (*ce truc*), this contains most of the tooling for the catalog records: 
-- Parses catalog records
-- Test the validity of the catalog according to different schemas
-- Builds agglomerated catalog records with optional dataviz
-- Retrieve catalog information from all repositories of a user or an organization.
-
-## Install 
-
-Either clone and run `python setup.py install` **or** use the pip version `pip install htruc`
-
-## Use
-
-### Testing a catalog record
-
-Simply run `htruc test YourYamlFile.yml`
-
-### Upgrade a previously existing catalog record
-
-Run `htruc upgrade yourYamlFile.yml`
-
-### Upgrade a previously existing catalog record to the newest schema
-
-Run `htruc upgrade yourYamlFile.yml`
-
-### Upgrade metrics using [HTR-United Metadata Generator (HUMg)](https://github.com/HTR-United/htr-united-metadata-generator)
-
-Run `htruc update-volumes YourYamlFile.yml MetricFileFromHUMG.jons --inplace`
----
-
-Logo by [Alix Chagué](https://alix-tz.github.io).
-
-
```

### Comparing `htruc-1.0.8/setup.py` & `htruc-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # Package meta-data.
 NAME = 'htruc'
 DESCRIPTION = 'HTRUC, a toolkit for HTR-United cataloging'
 URL = 'https://github.com/htr-united/htrvc'
 AUTHOR = 'Thibault Clérice'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = "1.0.8"
+VERSION = "1.1.0"
 
 # What packages are required for this module to be executed?
 
 with open(os.path.join(here, 'requirements.txt')) as f:
     REQUIRED = f.read().splitlines()
 
 # What packages are optional?
```

