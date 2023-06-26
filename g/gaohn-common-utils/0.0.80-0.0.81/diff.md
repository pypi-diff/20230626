# Comparing `tmp/gaohn-common-utils-0.0.80.tar.gz` & `tmp/gaohn-common-utils-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.80.tar", last modified: Thu Jun 22 09:11:35 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.81.tar", last modified: Mon Jun 26 07:19:07 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.80.tar` & `gaohn-common-utils-0.0.81.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:35.795432 gaohn-common-utils-0.0.80/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-22 09:11:35.795432 gaohn-common-utils-0.0.80/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:35.791432 gaohn-common-utils-0.0.80/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:35.791432 gaohn-common-utils-0.0.80/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:35.787432 gaohn-common-utils-0.0.80/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:35.791432 gaohn-common-utils-0.0.80/common_utils/cloud/gcp/database/
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/cloud/gcp/database/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:35.791432 gaohn-common-utils-0.0.80/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:35.791432 gaohn-common-utils-0.0.80/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/core/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:35.791432 gaohn-common-utils-0.0.80/common_utils/core/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/core/decorators/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/core/decorators/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:35.791432 gaohn-common-utils-0.0.80/common_utils/data_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/data_validator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/data_validator/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:35.787432 gaohn-common-utils-0.0.80/common_utils/experiment_tracking/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:35.795432 gaohn-common-utils-0.0.80/common_utils/experiment_tracking/promoter/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/experiment_tracking/promoter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/experiment_tracking/promoter/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:35.795432 gaohn-common-utils-0.0.80/common_utils/orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/orchestrator/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:35.787432 gaohn-common-utils-0.0.80/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:35.795432 gaohn-common-utils-0.0.80/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/versioning/dvc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/versioning/dvc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:35.795432 gaohn-common-utils-0.0.80/common_utils/versioning/git/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/versioning/git/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/common_utils/versioning/git/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:11:35.795432 gaohn-common-utils-0.0.80/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-22 09:11:35.000000 gaohn-common-utils-0.0.80/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-22 09:11:35.000000 gaohn-common-utils-0.0.80/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:11:35.000000 gaohn-common-utils-0.0.80/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-22 09:11:35.000000 gaohn-common-utils-0.0.80/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 09:11:35.000000 gaohn-common-utils-0.0.80/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-22 09:11:12.000000 gaohn-common-utils-0.0.80/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:11:35.795432 gaohn-common-utils-0.0.80/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:19:07.189830 gaohn-common-utils-0.0.81/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-26 07:19:07.189830 gaohn-common-utils-0.0.81/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:19:07.181830 gaohn-common-utils-0.0.81/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:19:07.181830 gaohn-common-utils-0.0.81/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:19:07.177830 gaohn-common-utils-0.0.81/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:19:07.181830 gaohn-common-utils-0.0.81/common_utils/cloud/gcp/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/cloud/gcp/database/bigquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:19:07.181830 gaohn-common-utils-0.0.81/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:19:07.185830 gaohn-common-utils-0.0.81/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/core/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:19:07.185830 gaohn-common-utils-0.0.81/common_utils/core/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/core/decorators/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/core/decorators/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:19:07.185830 gaohn-common-utils-0.0.81/common_utils/data_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/data_validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/data_validator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:19:07.177830 gaohn-common-utils-0.0.81/common_utils/experiment_tracking/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:19:07.185830 gaohn-common-utils-0.0.81/common_utils/experiment_tracking/promoter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/experiment_tracking/promoter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/experiment_tracking/promoter/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:19:07.185830 gaohn-common-utils-0.0.81/common_utils/orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/orchestrator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/orchestrator/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:19:07.181830 gaohn-common-utils-0.0.81/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:19:07.189830 gaohn-common-utils-0.0.81/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/versioning/dvc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/versioning/dvc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:19:07.189830 gaohn-common-utils-0.0.81/common_utils/versioning/git/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/versioning/git/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/common_utils/versioning/git/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:19:07.189830 gaohn-common-utils-0.0.81/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-26 07:19:07.000000 gaohn-common-utils-0.0.81/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-26 07:19:07.000000 gaohn-common-utils-0.0.81/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 07:19:07.000000 gaohn-common-utils-0.0.81/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-26 07:19:07.000000 gaohn-common-utils-0.0.81/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 07:19:07.000000 gaohn-common-utils-0.0.81/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-26 07:18:47.000000 gaohn-common-utils-0.0.81/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 07:19:07.189830 gaohn-common-utils-0.0.81/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.80/LICENSE` & `gaohn-common-utils-0.0.81/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.80/PKG-INFO` & `gaohn-common-utils-0.0.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.80
+Version: 0.0.81
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.80/README.md` & `gaohn-common-utils-0.0.81/README.md`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.80/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.81/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.80/common_utils/cloud/gcp/database/bigquery.py` & `gaohn-common-utils-0.0.81/common_utils/cloud/gcp/database/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.80/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.81/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.80/common_utils/core/base.py` & `gaohn-common-utils-0.0.81/common_utils/core/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.80/common_utils/core/common.py` & `gaohn-common-utils-0.0.81/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.80/common_utils/core/decorators/decorators.py` & `gaohn-common-utils-0.0.81/common_utils/core/decorators/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.80/common_utils/core/decorators/timer.py` & `gaohn-common-utils-0.0.81/common_utils/core/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.80/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.81/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.80/common_utils/core/logger.py` & `gaohn-common-utils-0.0.81/common_utils/core/logger.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.80/common_utils/data_validator/core.py` & `gaohn-common-utils-0.0.81/common_utils/data_validator/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.80/common_utils/experiment_tracking/promoter/base.py` & `gaohn-common-utils-0.0.81/common_utils/experiment_tracking/promoter/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.80/common_utils/experiment_tracking/promoter/core.py` & `gaohn-common-utils-0.0.81/common_utils/experiment_tracking/promoter/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.80/common_utils/versioning/dvc/core.py` & `gaohn-common-utils-0.0.81/common_utils/versioning/dvc/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.80/common_utils/versioning/git/core.py` & `gaohn-common-utils-0.0.81/common_utils/versioning/git/core.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.80/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.81/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.80
+Version: 0.0.81
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.80/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.81/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 common_utils/core/decorators/decorators.py
 common_utils/core/decorators/timer.py
 common_utils/data_validator/base.py
 common_utils/data_validator/core.py
 common_utils/experiment_tracking/promoter/base.py
 common_utils/experiment_tracking/promoter/core.py
 common_utils/orchestrator/base.py
+common_utils/orchestrator/core.py
 common_utils/versioning/dvc/base.py
 common_utils/versioning/dvc/core.py
 common_utils/versioning/git/base.py
 common_utils/versioning/git/core.py
 gaohn_common_utils.egg-info/PKG-INFO
 gaohn_common_utils.egg-info/SOURCES.txt
 gaohn_common_utils.egg-info/dependency_links.txt
```

### Comparing `gaohn-common-utils-0.0.80/pyproject.toml` & `gaohn-common-utils-0.0.81/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.80"
+version = "0.0.81"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

