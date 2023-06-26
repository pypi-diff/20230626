# Comparing `tmp/ml-management-0.0.38.tar.gz` & `tmp/ml-management-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-management-0.0.38.tar", last modified: Fri Jun 23 12:33:17 2023, max compression
+gzip compressed data, was "dist/ml-management-0.0.39.tar", last modified: Mon Jun 26 13:30:57 2023, max compression
```

## Comparing `ml-management-0.0.38.tar` & `ml-management-0.0.39.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       18 2023-06-06 09:18:11.000000 ml-management-0.0.38/MANIFEST.in
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.973694 ml-management-0.0.38/ML_management/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/__init__.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.973694 ml-management-0.0.38/ML_management/collectors/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      120 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1092 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/collector_pattern.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      456 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/collector_pattern_to_methods_map.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1318 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/collectors.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.973694 ml-management-0.0.38/ML_management/collectors/dummy/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/dummy/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      463 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/dummy/dummy_collector.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.973694 ml-management-0.0.38/ML_management/collectors/s3/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/s3/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    10609 2023-06-20 12:45:17.000000 ml-management-0.0.38/ML_management/collectors/s3/s3collector.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/collectors/topic_markers/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/topic_markers/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)   331440 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/topic_markers/api_schema.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3167 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/collectors/topic_markers/topic_markers_collector.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/dataset_loader_template/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/dataset_loader_template/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2407 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/dataset_loader_template/dataset_loader_pattern.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      457 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/executor_template/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/executor_template/__init__.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/executor_template/default_executors/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/executor_template/default_executors/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      895 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/executor_template/default_executors/finetune_executor.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      843 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/executor_template/default_executors/test_executor.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      869 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/executor_template/default_executors/train_executor.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4566 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/executor_template/executor_pattern.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      402 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/executor_template/executor_pattern_to_methods_map.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      334 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/executor_template/upload_model_mode.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/mlmanagement/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      581 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/mlmanagement/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3392 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/mlmanagement/jsonschema_exceptions.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     5054 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/mlmanagement/jsonschema_inference.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    13677 2023-06-23 12:19:15.000000 ml-management-0.0.38/ML_management/mlmanagement/mlmanagement.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    10260 2023-06-23 12:16:04.000000 ml-management-0.0.38/ML_management/mlmanagement/mlmanager.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      201 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/mlmanagement/model_type.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     5001 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/mlmanagement/server_mlmanager_exceptions.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      316 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/mlmanagement/utils.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/models/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/models/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      949 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/models/model_type_to_methods_map.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/models/patterns/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/models/patterns/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4202 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/models/patterns/model_pattern.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      561 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/models/patterns/retrainable_model.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      445 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/models/patterns/torch_model.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      457 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/models/patterns/trainable_model.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/registry/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/registry/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2566 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/registry/exceptions.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     7556 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/registry/registry_manager.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/tests/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/tests/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3361 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/tests/test_jsonschema_inference.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     9275 2023-06-20 12:45:17.000000 ml-management-0.0.38/ML_management/tests/test_s3_dataset.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ML_management/uploader_data/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-06 09:18:11.000000 ml-management-0.0.38/ML_management/uploader_data/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1694 2023-06-20 12:45:17.000000 ml-management-0.0.38/ML_management/uploader_data/s3_uploader.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      367 2023-06-23 12:33:17.977694 ml-management-0.0.38/PKG-INFO
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       56 2023-06-06 09:18:11.000000 ml-management-0.0.38/README.md
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        7 2023-06-23 12:16:14.000000 ml-management-0.0.38/VERSION
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-23 12:33:17.977694 ml-management-0.0.38/ml_management.egg-info/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      367 2023-06-23 12:33:17.000000 ml-management-0.0.38/ml_management.egg-info/PKG-INFO
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2449 2023-06-23 12:33:17.000000 ml-management-0.0.38/ml_management.egg-info/SOURCES.txt
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        1 2023-06-23 12:33:17.000000 ml-management-0.0.38/ml_management.egg-info/dependency_links.txt
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      153 2023-06-23 12:33:17.000000 ml-management-0.0.38/ml_management.egg-info/requires.txt
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       14 2023-06-23 12:33:17.000000 ml-management-0.0.38/ml_management.egg-info/top_level.txt
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       38 2023-06-23 12:33:17.977694 ml-management-0.0.38/setup.cfg
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1052 2023-06-23 12:18:15.000000 ml-management-0.0.38/setup.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.366889 ml-management-0.0.39/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)       18 2022-11-15 15:35:02.000000 ml-management-0.0.39/MANIFEST.in
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.358888 ml-management-0.0.39/ML_management/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-08-01 13:04:47.000000 ml-management-0.0.39/ML_management/__init__.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.358888 ml-management-0.0.39/ML_management/collectors/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      120 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     1092 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/collector_pattern.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      456 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/collector_pattern_to_methods_map.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     1318 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/collectors.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.358888 ml-management-0.0.39/ML_management/collectors/dummy/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/dummy/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      463 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/dummy/dummy_collector.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.358888 ml-management-0.0.39/ML_management/collectors/s3/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/s3/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)    10609 2023-06-15 09:26:35.000000 ml-management-0.0.39/ML_management/collectors/s3/s3collector.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/collectors/topic_markers/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/topic_markers/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)   331440 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/topic_markers/api_schema.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     3167 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/topic_markers/topic_markers_collector.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/dataset_loader_template/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/dataset_loader_template/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     2407 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/dataset_loader_template/dataset_loader_pattern.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      457 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/executor_template/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/executor_template/__init__.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/executor_template/default_executors/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/executor_template/default_executors/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      895 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/executor_template/default_executors/finetune_executor.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      843 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/executor_template/default_executors/test_executor.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      869 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/executor_template/default_executors/train_executor.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     4566 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/executor_template/executor_pattern.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      402 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/executor_template/executor_pattern_to_methods_map.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      334 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/executor_template/upload_model_mode.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/mlmanagement/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      581 2022-09-29 11:08:30.000000 ml-management-0.0.39/ML_management/mlmanagement/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     3392 2023-03-13 16:12:20.000000 ml-management-0.0.39/ML_management/mlmanagement/jsonschema_exceptions.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     5054 2023-03-13 16:12:20.000000 ml-management-0.0.39/ML_management/mlmanagement/jsonschema_inference.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)    13677 2023-06-23 15:20:18.000000 ml-management-0.0.39/ML_management/mlmanagement/mlmanagement.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)    10260 2023-06-23 15:20:18.000000 ml-management-0.0.39/ML_management/mlmanagement/mlmanager.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      201 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/mlmanagement/model_type.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     5001 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/mlmanagement/server_mlmanager_exceptions.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      316 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/mlmanagement/utils.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/models/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-08-01 13:04:47.000000 ml-management-0.0.39/ML_management/models/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      949 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/models/model_type_to_methods_map.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/models/patterns/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/models/patterns/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     4202 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/models/patterns/model_pattern.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      561 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/models/patterns/retrainable_model.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      445 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/models/patterns/torch_model.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      457 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/models/patterns/trainable_model.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/registry/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-08-01 13:04:47.000000 ml-management-0.0.39/ML_management/registry/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     2566 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/registry/exceptions.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     7556 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/registry/registry_manager.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/tests/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-12-07 10:58:45.000000 ml-management-0.0.39/ML_management/tests/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     3361 2022-12-07 10:58:45.000000 ml-management-0.0.39/ML_management/tests/test_jsonschema_inference.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     9275 2023-06-15 09:26:35.000000 ml-management-0.0.39/ML_management/tests/test_s3_dataset.py
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/uploader_data/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/uploader_data/__init__.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     1694 2023-06-15 09:26:35.000000 ml-management-0.0.39/ML_management/uploader_data/s3_uploader.py
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      312 2023-06-26 13:30:57.366889 ml-management-0.0.39/PKG-INFO
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)       56 2022-08-01 13:04:47.000000 ml-management-0.0.39/README.md
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        7 2023-06-26 13:30:41.000000 ml-management-0.0.39/VERSION
+drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.366889 ml-management-0.0.39/ml_management.egg-info/
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      312 2023-06-26 13:30:57.000000 ml-management-0.0.39/ml_management.egg-info/PKG-INFO
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     2449 2023-06-26 13:30:57.000000 ml-management-0.0.39/ml_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)        1 2023-06-26 13:30:57.000000 ml-management-0.0.39/ml_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)      153 2023-06-26 13:30:57.000000 ml-management-0.0.39/ml_management.egg-info/requires.txt
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)       14 2023-06-26 13:30:57.000000 ml-management-0.0.39/ml_management.egg-info/top_level.txt
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)       38 2023-06-26 13:30:57.366889 ml-management-0.0.39/setup.cfg
+-rw-rw-r--   0 boeing    (1000) boeing    (1000)     1052 2023-06-23 15:20:18.000000 ml-management-0.0.39/setup.py
```

### Comparing `ml-management-0.0.38/ML_management/collectors/collector_pattern.py` & `ml-management-0.0.39/ML_management/collectors/collector_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/collectors/collectors.py` & `ml-management-0.0.39/ML_management/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/collectors/s3/s3collector.py` & `ml-management-0.0.39/ML_management/collectors/s3/s3collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/collectors/topic_markers/api_schema.py` & `ml-management-0.0.39/ML_management/collectors/topic_markers/api_schema.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/collectors/topic_markers/topic_markers_collector.py` & `ml-management-0.0.39/ML_management/collectors/topic_markers/topic_markers_collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/dataset_loader_template/dataset_loader_pattern.py` & `ml-management-0.0.39/ML_management/dataset_loader_template/dataset_loader_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/executor_template/default_executors/finetune_executor.py` & `ml-management-0.0.39/ML_management/executor_template/default_executors/finetune_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/executor_template/default_executors/test_executor.py` & `ml-management-0.0.39/ML_management/executor_template/default_executors/test_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/executor_template/default_executors/train_executor.py` & `ml-management-0.0.39/ML_management/executor_template/default_executors/train_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/executor_template/executor_pattern.py` & `ml-management-0.0.39/ML_management/executor_template/executor_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/mlmanagement/__init__.py` & `ml-management-0.0.39/ML_management/mlmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/mlmanagement/jsonschema_exceptions.py` & `ml-management-0.0.39/ML_management/mlmanagement/jsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/mlmanagement/jsonschema_inference.py` & `ml-management-0.0.39/ML_management/mlmanagement/jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/mlmanagement/mlmanagement.py` & `ml-management-0.0.39/ML_management/mlmanagement/mlmanagement.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/mlmanagement/mlmanager.py` & `ml-management-0.0.39/ML_management/mlmanagement/mlmanager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/mlmanagement/server_mlmanager_exceptions.py` & `ml-management-0.0.39/ML_management/mlmanagement/server_mlmanager_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/models/model_type_to_methods_map.py` & `ml-management-0.0.39/ML_management/models/model_type_to_methods_map.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/models/patterns/model_pattern.py` & `ml-management-0.0.39/ML_management/models/patterns/model_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/models/patterns/retrainable_model.py` & `ml-management-0.0.39/ML_management/models/patterns/retrainable_model.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/registry/exceptions.py` & `ml-management-0.0.39/ML_management/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/registry/registry_manager.py` & `ml-management-0.0.39/ML_management/registry/registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/tests/test_jsonschema_inference.py` & `ml-management-0.0.39/ML_management/tests/test_jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/tests/test_s3_dataset.py` & `ml-management-0.0.39/ML_management/tests/test_s3_dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ML_management/uploader_data/s3_uploader.py` & `ml-management-0.0.39/ML_management/uploader_data/s3_uploader.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/ml_management.egg-info/SOURCES.txt` & `ml-management-0.0.39/ml_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.38/setup.py` & `ml-management-0.0.39/setup.py`

 * *Files identical despite different names*

