# Comparing `tmp/azureml_sdk-1.8.0-py3-none-any.whl.zip` & `tmp/azureml_sdk-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4370 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      991 b- defN 20-Jun-22 17:22 azureml_sdk-1.8.0.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat      859 b- defN 20-Jun-22 17:22 azureml_sdk-1.8.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     2232 b- defN 20-Jun-22 17:22 azureml_sdk-1.8.0.dist-info/metadata.json
--rw-rw-rw-  2.0 fat        1 b- defN 20-Jun-22 17:22 azureml_sdk-1.8.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 20-Jun-22 17:22 azureml_sdk-1.8.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     3594 b- defN 20-Jun-22 17:22 azureml_sdk-1.8.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      612 b- defN 20-Jun-22 17:22 azureml_sdk-1.8.0.dist-info/RECORD
-7 files, 8386 bytes uncompressed, 3282 bytes compressed:  60.9%
+Zip file size: 4368 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      991 b- defN 20-Jul-06 20:26 azureml_sdk-1.9.0.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat      859 b- defN 20-Jul-06 20:26 azureml_sdk-1.9.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     2233 b- defN 20-Jul-06 20:26 azureml_sdk-1.9.0.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat        1 b- defN 20-Jul-06 20:26 azureml_sdk-1.9.0.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 20-Jul-06 20:26 azureml_sdk-1.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     3595 b- defN 20-Jul-06 20:26 azureml_sdk-1.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      612 b- defN 20-Jul-06 20:26 azureml_sdk-1.9.0.dist-info/RECORD
+7 files, 8388 bytes uncompressed, 3280 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: azureml_sdk-1.8.0.dist-info/DESCRIPTION.rst
+Filename: azureml_sdk-1.9.0.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: azureml_sdk-1.8.0.dist-info/LICENSE.txt
+Filename: azureml_sdk-1.9.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: azureml_sdk-1.8.0.dist-info/metadata.json
+Filename: azureml_sdk-1.9.0.dist-info/metadata.json
 Comment: 
 
-Filename: azureml_sdk-1.8.0.dist-info/top_level.txt
+Filename: azureml_sdk-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_sdk-1.8.0.dist-info/WHEEL
+Filename: azureml_sdk-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_sdk-1.8.0.dist-info/METADATA
+Filename: azureml_sdk-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: azureml_sdk-1.8.0.dist-info/RECORD
+Filename: azureml_sdk-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `azureml_sdk-1.8.0.dist-info/DESCRIPTION.rst` & `azureml_sdk-1.9.0.dist-info/DESCRIPTION.rst`

 * *Files identical despite different names*

## Comparing `azureml_sdk-1.8.0.dist-info/LICENSE.txt` & `azureml_sdk-1.9.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `azureml_sdk-1.8.0.dist-info/metadata.json` & `azureml_sdk-1.9.0.dist-info/metadata.json`

 * *Files 20% similar despite different names*

### Pretty-printed

 * *Similarity: 0.946875%*

 * *Differences: {"'run_requires'": "{0: {'requires': ['azureml-accel-models (~=1.9.0)']}, 1: {'requires': "*

 * *                   "['azureml-contrib-notebook (~=1.9.0)', 'azureml-contrib-pipeline-steps "*

 * *                   "(~=1.9.0)', 'azureml-contrib-server (~=1.9.0)', 'azureml-contrib-services "*

 * *                   "(~=1.9.0)']}, 2: {'requires': ['azureml-contrib-notebook (~=1.9.0)', "*

 * *                   "'azureml-widgets (~=1.9.0)']}, 3: {'requires': ['azureml-contrib-services "*

 * *                   "(~=1.9.0)']}, 4: {'requi […]*

```diff
@@ -48,75 +48,75 @@
     "metadata_version": "2.0",
     "name": "azureml-sdk",
     "requires_python": ">=3.5,<4",
     "run_requires": [
         {
             "extra": "accel-models",
             "requires": [
-                "azureml-accel-models (~=1.8.0)"
+                "azureml-accel-models (~=1.9.0)"
             ]
         },
         {
             "extra": "contrib",
             "requires": [
-                "azureml-contrib-notebook (~=1.8.0)",
-                "azureml-contrib-pipeline-steps (~=1.8.0)",
-                "azureml-contrib-server (~=1.8.0)",
-                "azureml-contrib-services (~=1.8.0)"
+                "azureml-contrib-notebook (~=1.9.0)",
+                "azureml-contrib-pipeline-steps (~=1.9.0)",
+                "azureml-contrib-server (~=1.9.0)",
+                "azureml-contrib-services (~=1.9.0)"
             ]
         },
         {
             "extra": "notebooks",
             "requires": [
-                "azureml-contrib-notebook (~=1.8.0)",
-                "azureml-widgets (~=1.8.0)"
+                "azureml-contrib-notebook (~=1.9.0)",
+                "azureml-widgets (~=1.9.0)"
             ]
         },
         {
             "extra": "services",
             "requires": [
-                "azureml-contrib-services (~=1.8.0)"
+                "azureml-contrib-services (~=1.9.0)"
             ]
         },
         {
             "requires": [
-                "azureml-core (~=1.8.0)",
-                "azureml-dataprep[fuse] (<1.9.0a,>=1.8.0a)",
-                "azureml-pipeline (~=1.8.0)",
-                "azureml-train (~=1.8.0)",
-                "azureml-train-automl-client (~=1.8.0)"
+                "azureml-core (~=1.9.0)",
+                "azureml-dataprep[fuse] (<1.10.0a,>=1.9.0a)",
+                "azureml-pipeline (~=1.9.0)",
+                "azureml-train (~=1.9.0)",
+                "azureml-train-automl-client (~=1.9.0)"
             ]
         },
         {
             "extra": "explain",
             "requires": [
-                "azureml-explain-model (~=1.8.0)"
+                "azureml-explain-model (~=1.9.0)"
             ]
         },
         {
             "extra": "interpret",
             "requires": [
-                "azureml-interpret (~=1.8.0)"
+                "azureml-interpret (~=1.9.0)"
             ]
         },
         {
             "extra": "tensorboard",
             "requires": [
-                "azureml-tensorboard (~=1.8.0)"
+                "azureml-tensorboard (~=1.9.0)"
             ]
         },
         {
             "extra": "automl",
             "requires": [
-                "azureml-train-automl (~=1.8.0)"
+                "azureml-train-automl (~=1.9.0)"
             ]
         },
         {
             "extra": "automl_databricks",
             "requires": [
-                "azureml-train-automl (~=1.8.0)"
+                "azureml-train-automl (~=1.9.0)"
             ]
         }
     ],
     "summary": "Microsoft Azure Machine Learning Python SDK",
-    "version": "1.8.0"
+    "version": "1.9.0"
 }
```

## Comparing `azureml_sdk-1.8.0.dist-info/METADATA` & `azureml_sdk-1.9.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: azureml-sdk
-Version: 1.8.0
+Version: 1.9.0
 Summary: Microsoft Azure Machine Learning Python SDK
 Home-page: https://docs.microsoft.com/en-us/azure/machine-learning/service/
 Author: Microsoft Corp
 License: https://aka.ms/azureml-sdk-license
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -16,52 +16,52 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.5,<4
 Description-Content-Type: text/x-rst
-Provides-Extra: databricks
-Provides-Extra: services
-Provides-Extra: notebooks
-Provides-Extra: contrib
 Provides-Extra: explain
-Provides-Extra: automl_databricks
 Provides-Extra: tensorboard
+Provides-Extra: accel-models
 Provides-Extra: automl
+Provides-Extra: databricks
+Provides-Extra: automl_databricks
+Provides-Extra: services
+Provides-Extra: contrib
+Provides-Extra: notebooks
 Provides-Extra: interpret
+Requires-Dist: azureml-core (~=1.9.0)
+Requires-Dist: azureml-train (~=1.9.0)
+Requires-Dist: azureml-train-automl-client (~=1.9.0)
+Requires-Dist: azureml-pipeline (~=1.9.0)
+Requires-Dist: azureml-dataprep[fuse] (<1.10.0a,>=1.9.0a)
 Provides-Extra: accel-models
-Requires-Dist: azureml-core (~=1.8.0)
-Requires-Dist: azureml-train (~=1.8.0)
-Requires-Dist: azureml-train-automl-client (~=1.8.0)
-Requires-Dist: azureml-pipeline (~=1.8.0)
-Requires-Dist: azureml-dataprep[fuse] (<1.9.0a,>=1.8.0a)
-Provides-Extra: accel-models
-Requires-Dist: azureml-accel-models (~=1.8.0); extra == 'accel-models'
+Requires-Dist: azureml-accel-models (~=1.9.0); extra == 'accel-models'
 Provides-Extra: automl
-Requires-Dist: azureml-train-automl (~=1.8.0); extra == 'automl'
+Requires-Dist: azureml-train-automl (~=1.9.0); extra == 'automl'
 Provides-Extra: automl_databricks
-Requires-Dist: azureml-train-automl (~=1.8.0); extra == 'automl_databricks'
+Requires-Dist: azureml-train-automl (~=1.9.0); extra == 'automl_databricks'
 Provides-Extra: contrib
-Requires-Dist: azureml-contrib-pipeline-steps (~=1.8.0); extra == 'contrib'
-Requires-Dist: azureml-contrib-server (~=1.8.0); extra == 'contrib'
-Requires-Dist: azureml-contrib-services (~=1.8.0); extra == 'contrib'
-Requires-Dist: azureml-contrib-notebook (~=1.8.0); extra == 'contrib'
+Requires-Dist: azureml-contrib-pipeline-steps (~=1.9.0); extra == 'contrib'
+Requires-Dist: azureml-contrib-server (~=1.9.0); extra == 'contrib'
+Requires-Dist: azureml-contrib-services (~=1.9.0); extra == 'contrib'
+Requires-Dist: azureml-contrib-notebook (~=1.9.0); extra == 'contrib'
 Provides-Extra: databricks
 Provides-Extra: explain
-Requires-Dist: azureml-explain-model (~=1.8.0); extra == 'explain'
+Requires-Dist: azureml-explain-model (~=1.9.0); extra == 'explain'
 Provides-Extra: interpret
-Requires-Dist: azureml-interpret (~=1.8.0); extra == 'interpret'
+Requires-Dist: azureml-interpret (~=1.9.0); extra == 'interpret'
 Provides-Extra: notebooks
-Requires-Dist: azureml-widgets (~=1.8.0); extra == 'notebooks'
-Requires-Dist: azureml-contrib-notebook (~=1.8.0); extra == 'notebooks'
+Requires-Dist: azureml-widgets (~=1.9.0); extra == 'notebooks'
+Requires-Dist: azureml-contrib-notebook (~=1.9.0); extra == 'notebooks'
 Provides-Extra: services
-Requires-Dist: azureml-contrib-services (~=1.8.0); extra == 'services'
+Requires-Dist: azureml-contrib-services (~=1.9.0); extra == 'services'
 Provides-Extra: tensorboard
-Requires-Dist: azureml-tensorboard (~=1.8.0); extra == 'tensorboard'
+Requires-Dist: azureml-tensorboard (~=1.9.0); extra == 'tensorboard'
 
 What is the Azure Machine Learning SDK for Python?
 ==================================================
 
 The Azure Machine Learning SDK for Python is used by data scientists and AI developers 
 to build and run machine learning workflows upon the Azure Machine Learning service. 
 You can interact with the service in any Python environment, including Jupyter Notebooks
```

## Comparing `azureml_sdk-1.8.0.dist-info/RECORD` & `azureml_sdk-1.9.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-azureml_sdk-1.8.0.dist-info/DESCRIPTION.rst,sha256=Op4-82V6hE_OFSG4SduWhqcADZNLH0xHTtKN_QYx87U,991
-azureml_sdk-1.8.0.dist-info/LICENSE.txt,sha256=GBoIyZ-6vJ4xjRc8U3wTw4EfkuaEdVTm_gbr1Nm8uDI,859
-azureml_sdk-1.8.0.dist-info/METADATA,sha256=9T-hByrY3LFcSnItxZgJ1RZrAaDcieuq0UVDMaEYCqg,3594
-azureml_sdk-1.8.0.dist-info/RECORD,,
-azureml_sdk-1.8.0.dist-info/WHEEL,sha256=Vlaj2XNMTTJ893zWX-JvKeZUIs7q5E7d7Gise2Vouzc,97
-azureml_sdk-1.8.0.dist-info/metadata.json,sha256=sc74GBgXhHdEqyM3cxnXHKHbjqbPxvLBfE3LZoc4BAk,2232
-azureml_sdk-1.8.0.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+azureml_sdk-1.9.0.dist-info/DESCRIPTION.rst,sha256=Op4-82V6hE_OFSG4SduWhqcADZNLH0xHTtKN_QYx87U,991
+azureml_sdk-1.9.0.dist-info/LICENSE.txt,sha256=GBoIyZ-6vJ4xjRc8U3wTw4EfkuaEdVTm_gbr1Nm8uDI,859
+azureml_sdk-1.9.0.dist-info/METADATA,sha256=DpRU0ll8UU97utZ8IcaDpPZ6NURXehguGObLjPIpQnI,3595
+azureml_sdk-1.9.0.dist-info/RECORD,,
+azureml_sdk-1.9.0.dist-info/WHEEL,sha256=Vlaj2XNMTTJ893zWX-JvKeZUIs7q5E7d7Gise2Vouzc,97
+azureml_sdk-1.9.0.dist-info/metadata.json,sha256=d2CyUbPtOyj6iCYO4PcO4Y8iRYHaHDejICl4l9oDEXM,2233
+azureml_sdk-1.9.0.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
```

