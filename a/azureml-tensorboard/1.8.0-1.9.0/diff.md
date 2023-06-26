# Comparing `tmp/azureml_tensorboard-1.8.0-py3-none-any.whl.zip` & `tmp/azureml_tensorboard-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10709 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      251 b- defN 20-Jun-22 17:21 azureml/__init__.py
--rw-rw-rw-  2.0 fat      935 b- defN 20-Jun-22 17:21 azureml/tensorboard/__init__.py
--rw-rw-rw-  2.0 fat     5175 b- defN 20-Jun-22 17:21 azureml/tensorboard/export.py
--rw-rw-rw-  2.0 fat    11624 b- defN 20-Jun-22 17:21 azureml/tensorboard/tensorboard.py
--rw-rw-rw-  2.0 fat      703 b- defN 20-Jun-22 17:21 azureml_tensorboard-1.8.0.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat      859 b- defN 20-Jun-22 17:21 azureml_tensorboard-1.8.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1112 b- defN 20-Jun-22 17:21 azureml_tensorboard-1.8.0.dist-info/metadata.json
--rw-rw-rw-  2.0 fat        8 b- defN 20-Jun-22 17:21 azureml_tensorboard-1.8.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 20-Jun-22 17:21 azureml_tensorboard-1.8.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1646 b- defN 20-Jun-22 17:21 azureml_tensorboard-1.8.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat     1012 b- defN 20-Jun-22 17:21 azureml_tensorboard-1.8.0.dist-info/RECORD
-11 files, 23422 bytes uncompressed, 8979 bytes compressed:  61.7%
+Zip file size: 10209 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      251 b- defN 20-Jul-06 20:24 azureml/__init__.py
+-rw-rw-rw-  2.0 fat     1020 b- defN 20-Jul-06 20:24 azureml/tensorboard/__init__.py
+-rw-rw-rw-  2.0 fat     5190 b- defN 20-Jul-06 20:25 azureml/tensorboard/export.py
+-rw-rw-rw-  2.0 fat    11624 b- defN 20-Jul-06 20:25 azureml/tensorboard/tensorboard.py
+-rw-rw-rw-  2.0 fat       64 b- defN 20-Jul-06 20:25 azureml_tensorboard-1.9.0.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat      859 b- defN 20-Jul-06 20:25 azureml_tensorboard-1.9.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1112 b- defN 20-Jul-06 20:25 azureml_tensorboard-1.9.0.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat        8 b- defN 20-Jul-06 20:25 azureml_tensorboard-1.9.0.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 20-Jul-06 20:25 azureml_tensorboard-1.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1007 b- defN 20-Jul-06 20:25 azureml_tensorboard-1.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat     1012 b- defN 20-Jul-06 20:25 azureml_tensorboard-1.9.0.dist-info/RECORD
+11 files, 22244 bytes uncompressed, 8479 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -6,29 +6,29 @@
 
 Filename: azureml/tensorboard/export.py
 Comment: 
 
 Filename: azureml/tensorboard/tensorboard.py
 Comment: 
 
-Filename: azureml_tensorboard-1.8.0.dist-info/DESCRIPTION.rst
+Filename: azureml_tensorboard-1.9.0.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: azureml_tensorboard-1.8.0.dist-info/LICENSE.txt
+Filename: azureml_tensorboard-1.9.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: azureml_tensorboard-1.8.0.dist-info/metadata.json
+Filename: azureml_tensorboard-1.9.0.dist-info/metadata.json
 Comment: 
 
-Filename: azureml_tensorboard-1.8.0.dist-info/top_level.txt
+Filename: azureml_tensorboard-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_tensorboard-1.8.0.dist-info/WHEEL
+Filename: azureml_tensorboard-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_tensorboard-1.8.0.dist-info/METADATA
+Filename: azureml_tensorboard-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: azureml_tensorboard-1.8.0.dist-info/RECORD
+Filename: azureml_tensorboard-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## azureml/tensorboard/__init__.py

```diff
@@ -1,16 +1,16 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 """Contains modules and classes for exporting run history to TensorBoard logs and launching a TensorBoard instance.
 
 A Tensorboard instance enables you to visualize experiment performance and structure. For machine learning
-experiments that natively output Tensorboard logs, create a Tensorboard instance referencing your experiment's run
+experiments that natively output TensorBoard logs, create a Tensorboard instance referencing your experiment's run
 history. For Azure Machine Learning experiments and other machine learning frameworks that don't natively output
-Tensorboard logs, export your run history to Tensorboard log format before visualization. For more
-information about using Tensorboard, see
-https://docs.microsoft.com/azure/machine-learning/how-to-monitor-tensorboard.
+TensorBoard logs, export your run history to Tensorboard log format before visualization. For more
+information about using TensorBoard, see [Visualize experiment runs and metrics with TensorBoard and Azure
+Machine Learning](https://docs.microsoft.com/azure/machine-learning/how-to-monitor-tensorboard).
 """
 from .tensorboard import Tensorboard
 
 __all__ = ["Tensorboard"]
```

## azureml/tensorboard/export.py

```diff
@@ -89,15 +89,15 @@
         except AttributeError:
             # Otherwise, this is a run
             runs = [run_data]
             # Note: we assume this method is always scoped to a single project, as discussed with AK
             experiment = run_data.experiment
     if recursive:
         runs += [child for run in runs for child in run.get_children(recursive=True)]
-    client = ExperimentClient(experiment.workspace.service_context, experiment.name)
+    client = ExperimentClient(experiment.workspace.service_context, experiment.name, experiment.id)
 
     run_ids = [run.id for run in runs]
     all_metrics = client.get_metrics_by_run_ids(run_ids)
     run_id = None
     writer = None
     for run_metrics in all_metrics:
         old_run_id = run_id
```

## azureml/tensorboard/tensorboard.py

```diff
@@ -21,15 +21,15 @@
 except ImportError:
     from queue import Queue, Empty  # python 3.x
 
 module_logger = logging.getLogger(__name__)
 
 
 class Tensorboard(object):
-    """Represents a Tensorboard instance for visualizing experiment performance and structure.
+    """Represents a TensorBoard instance for visualizing experiment performance and structure.
 
     :param runs: An empty list or a list of one or more experiment :class:`azureml.core.run.Run` objects to
         attach to this Tensorboard instance.
     :type runs: list
     :param local_root: An optional local directory to store the run logs in.
     :type local_root: str
     :param port: The port to run this Tensorboard instance on.
```

## Comparing `azureml_tensorboard-1.8.0.dist-info/LICENSE.txt` & `azureml_tensorboard-1.9.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `azureml_tensorboard-1.8.0.dist-info/metadata.json` & `azureml_tensorboard-1.9.0.dist-info/metadata.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'run_requires'": "{0: {'requires': ['azureml-core (~=1.9.0)']}}", "'version'": "'1.9.0'"}*

```diff
@@ -36,14 +36,14 @@
     "license": "https://aka.ms/azureml-sdk-license",
     "metadata_version": "2.0",
     "name": "azureml-tensorboard",
     "requires_python": ">=3.5,<4",
     "run_requires": [
         {
             "requires": [
-                "azureml-core (~=1.8.0)"
+                "azureml-core (~=1.9.0)"
             ]
         }
     ],
     "summary": "UNKNOWN",
-    "version": "1.8.0"
+    "version": "1.9.0"
 }
```

