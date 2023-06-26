# Comparing `tmp/velour-client-0.4.0.tar.gz` & `tmp/velour-client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velour-client-0.4.0.tar", last modified: Tue Jun 13 18:45:19 2023, max compression
+gzip compressed data, was "velour-client-0.5.0.tar", last modified: Mon Jun 26 11:29:17 2023, max compression
```

## Comparing `velour-client-0.4.0.tar` & `velour-client-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:45:19.660563 velour-client-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-13 18:45:10.000000 velour-client-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-13 18:45:19.660563 velour-client-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 18:45:10.000000 velour-client-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-13 18:45:10.000000 velour-client-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 18:45:19.660563 velour-client-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-13 18:45:10.000000 velour-client-0.4.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:45:19.656563 velour-client-0.4.0/unit-tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-06-13 18:45:10.000000 velour-client-0.4.0/unit-tests/test_chariot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-13 18:45:10.000000 velour-client-0.4.0/unit-tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-13 18:45:10.000000 velour-client-0.4.0/unit-tests/test_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-13 18:45:10.000000 velour-client-0.4.0/unit-tests/test_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-13 18:45:10.000000 velour-client-0.4.0/unit-tests/test_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-06-13 18:45:10.000000 velour-client-0.4.0/unit-tests/test_yolo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:45:19.656563 velour-client-0.4.0/velour/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-13 18:45:10.000000 velour-client-0.4.0/velour/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28267 2023-06-13 18:45:10.000000 velour-client-0.4.0/velour/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-13 18:45:10.000000 velour-client-0.4.0/velour/data_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:45:19.656563 velour-client-0.4.0/velour/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)    14911 2023-06-13 18:45:10.000000 velour-client-0.4.0/velour/integrations/chariot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-13 18:45:10.000000 velour-client-0.4.0/velour/integrations/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-13 18:45:10.000000 velour-client-0.4.0/velour/integrations/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-13 18:45:10.000000 velour-client-0.4.0/velour/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-06-13 18:45:10.000000 velour-client-0.4.0/velour/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:45:19.660563 velour-client-0.4.0/velour_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-13 18:45:19.000000 velour-client-0.4.0/velour_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 18:45:19.000000 velour-client-0.4.0/velour_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 18:45:19.000000 velour-client-0.4.0/velour_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-13 18:45:19.000000 velour-client-0.4.0/velour_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 18:45:19.000000 velour-client-0.4.0/velour_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:29:17.770211 velour-client-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-26 11:29:08.000000 velour-client-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-26 11:29:17.770211 velour-client-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 11:29:08.000000 velour-client-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-26 11:29:08.000000 velour-client-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 11:29:17.770211 velour-client-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-26 11:29:08.000000 velour-client-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:29:17.770211 velour-client-0.5.0/unit-tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-06-26 11:29:08.000000 velour-client-0.5.0/unit-tests/test_chariot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-26 11:29:08.000000 velour-client-0.5.0/unit-tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-26 11:29:08.000000 velour-client-0.5.0/unit-tests/test_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-26 11:29:08.000000 velour-client-0.5.0/unit-tests/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-26 11:29:08.000000 velour-client-0.5.0/unit-tests/test_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-06-26 11:29:08.000000 velour-client-0.5.0/unit-tests/test_yolo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:29:17.770211 velour-client-0.5.0/velour/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-26 11:29:08.000000 velour-client-0.5.0/velour/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28757 2023-06-26 11:29:08.000000 velour-client-0.5.0/velour/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-26 11:29:08.000000 velour-client-0.5.0/velour/data_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:29:17.770211 velour-client-0.5.0/velour/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    14911 2023-06-26 11:29:08.000000 velour-client-0.5.0/velour/integrations/chariot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-26 11:29:08.000000 velour-client-0.5.0/velour/integrations/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-26 11:29:08.000000 velour-client-0.5.0/velour/integrations/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 11:29:08.000000 velour-client-0.5.0/velour/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-06-26 11:29:08.000000 velour-client-0.5.0/velour/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:29:17.770211 velour-client-0.5.0/velour_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-26 11:29:17.000000 velour-client-0.5.0/velour_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-26 11:29:17.000000 velour-client-0.5.0/velour_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 11:29:17.000000 velour-client-0.5.0/velour_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-26 11:29:17.000000 velour-client-0.5.0/velour_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 11:29:17.000000 velour-client-0.5.0/velour_client.egg-info/top_level.txt
```

### Comparing `velour-client-0.4.0/LICENSE` & `velour-client-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `velour-client-0.4.0/PKG-INFO` & `velour-client-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velour-client
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python client for the Velour evaluation store
 License: Copyright 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
```

### Comparing `velour-client-0.4.0/pyproject.toml` & `velour-client-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `velour-client-0.4.0/unit-tests/test_chariot.py` & `velour-client-0.5.0/unit-tests/test_chariot.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.4.0/unit-tests/test_client.py` & `velour-client-0.5.0/unit-tests/test_client.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.4.0/unit-tests/test_coco.py` & `velour-client-0.5.0/unit-tests/test_coco.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.4.0/unit-tests/test_data_types.py` & `velour-client-0.5.0/unit-tests/test_data_types.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.4.0/unit-tests/test_viz.py` & `velour-client-0.5.0/unit-tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.4.0/unit-tests/test_yolo.py` & `velour-client-0.5.0/unit-tests/test_yolo.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.4.0/velour/client.py` & `velour-client-0.5.0/velour/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,19 +384,37 @@
         self.name = name
 
     def finalize_inferences(self, dataset: DatasetBase) -> None:
         return self.client._requests_put_rel_host(
             f"models/{self.name}/inferences/{dataset.name}/finalize"
         ).json()
 
-    def evaluate_classification(self, dataset: DatasetBase) -> "EvalJob":
+    def evaluate_classification(
+        self, dataset: DatasetBase, group_by: str = None
+    ) -> "EvalJob":
+        """Start a classification evaluation job
+
+        Parameters
+        ----------
+        dataset
+            the dataset to evaluate against
+        group_by
+            optional name of metadatum to group the results by
+
+        Returns
+        -------
+        EvalJob
+            a job object that can be used to track the status of the job
+            and get the metrics of it upon completion
+        """
         payload = {
             "settings": {
                 "model_name": self.name,
                 "dataset_name": dataset.name,
+                "group_by": group_by,
             }
         }
 
         resp = self.client._requests_post_rel_host(
             "clf-metrics", json=payload
         ).json()
```

### Comparing `velour-client-0.4.0/velour/data_types.py` & `velour-client-0.5.0/velour/data_types.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.4.0/velour/integrations/chariot.py` & `velour-client-0.5.0/velour/integrations/chariot.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.4.0/velour/integrations/coco.py` & `velour-client-0.5.0/velour/integrations/coco.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.4.0/velour/integrations/yolo.py` & `velour-client-0.5.0/velour/integrations/yolo.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.4.0/velour/viz.py` & `velour-client-0.5.0/velour/viz.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.4.0/velour_client.egg-info/PKG-INFO` & `velour-client-0.5.0/velour_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velour-client
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python client for the Velour evaluation store
 License: Copyright 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
```

### Comparing `velour-client-0.4.0/velour_client.egg-info/SOURCES.txt` & `velour-client-0.5.0/velour_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

