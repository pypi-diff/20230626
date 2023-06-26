# Comparing `tmp/azureml_pipeline-1.8.0-py3-none-any.whl.zip` & `tmp/azureml_pipeline-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3663 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      597 b- defN 20-Jun-22 17:22 azureml_pipeline-1.8.0.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat      859 b- defN 20-Jun-22 17:22 azureml_pipeline-1.8.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1088 b- defN 20-Jun-22 17:22 azureml_pipeline-1.8.0.dist-info/metadata.json
--rw-rw-rw-  2.0 fat        1 b- defN 20-Jun-22 17:22 azureml_pipeline-1.8.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 20-Jun-22 17:22 azureml_pipeline-1.8.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1524 b- defN 20-Jun-22 17:22 azureml_pipeline-1.8.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      647 b- defN 20-Jun-22 17:22 azureml_pipeline-1.8.0.dist-info/RECORD
-7 files, 4813 bytes uncompressed, 2505 bytes compressed:  48.0%
+Zip file size: 3665 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      597 b- defN 20-Jul-06 20:26 azureml_pipeline-1.9.0.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat      859 b- defN 20-Jul-06 20:26 azureml_pipeline-1.9.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1088 b- defN 20-Jul-06 20:26 azureml_pipeline-1.9.0.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat        1 b- defN 20-Jul-06 20:26 azureml_pipeline-1.9.0.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 20-Jul-06 20:26 azureml_pipeline-1.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1524 b- defN 20-Jul-06 20:26 azureml_pipeline-1.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      647 b- defN 20-Jul-06 20:26 azureml_pipeline-1.9.0.dist-info/RECORD
+7 files, 4813 bytes uncompressed, 2507 bytes compressed:  47.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: azureml_pipeline-1.8.0.dist-info/DESCRIPTION.rst
+Filename: azureml_pipeline-1.9.0.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: azureml_pipeline-1.8.0.dist-info/LICENSE.txt
+Filename: azureml_pipeline-1.9.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: azureml_pipeline-1.8.0.dist-info/metadata.json
+Filename: azureml_pipeline-1.9.0.dist-info/metadata.json
 Comment: 
 
-Filename: azureml_pipeline-1.8.0.dist-info/top_level.txt
+Filename: azureml_pipeline-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_pipeline-1.8.0.dist-info/WHEEL
+Filename: azureml_pipeline-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_pipeline-1.8.0.dist-info/METADATA
+Filename: azureml_pipeline-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: azureml_pipeline-1.8.0.dist-info/RECORD
+Filename: azureml_pipeline-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `azureml_pipeline-1.8.0.dist-info/DESCRIPTION.rst` & `azureml_pipeline-1.9.0.dist-info/DESCRIPTION.rst`

 * *Files identical despite different names*

## Comparing `azureml_pipeline-1.8.0.dist-info/LICENSE.txt` & `azureml_pipeline-1.9.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `azureml_pipeline-1.8.0.dist-info/metadata.json` & `azureml_pipeline-1.9.0.dist-info/metadata.json`

 * *Files 9% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9318181818181818%*

 * *Differences: {"'run_requires'": "{0: {'requires': ['azureml-pipeline-core (~=1.9.0)', 'azureml-pipeline-steps "*

 * *                   "(~=1.9.0)']}}",*

 * * "'version'": "'1.9.0'"}*

```diff
@@ -34,15 +34,15 @@
     "generator": "bdist_wheel (0.30.0)",
     "license": "https://aka.ms/azureml-sdk-license",
     "metadata_version": "2.0",
     "name": "azureml-pipeline",
     "run_requires": [
         {
             "requires": [
-                "azureml-pipeline-core (~=1.8.0)",
-                "azureml-pipeline-steps (~=1.8.0)"
+                "azureml-pipeline-core (~=1.9.0)",
+                "azureml-pipeline-steps (~=1.9.0)"
             ]
         }
     ],
     "summary": "UNKNOWN",
-    "version": "1.8.0"
+    "version": "1.9.0"
 }
```

## Comparing `azureml_pipeline-1.8.0.dist-info/METADATA` & `azureml_pipeline-1.9.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: azureml-pipeline
-Version: 1.8.0
+Version: 1.9.0
 Summary: UNKNOWN
 Home-page: https://docs.microsoft.com/en-us/azure/machine-learning/service/
 Author: Microsoft Corp
 License: https://aka.ms/azureml-sdk-license
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -14,16 +14,16 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/x-rst
-Requires-Dist: azureml-pipeline-core (~=1.8.0)
-Requires-Dist: azureml-pipeline-steps (~=1.8.0)
+Requires-Dist: azureml-pipeline-core (~=1.9.0)
+Requires-Dist: azureml-pipeline-steps (~=1.9.0)
 
 Machine learning (ML) pipelines are used by data scientists to build, optimize, and manage their machine learning workflows. A typical pipeline involves a sequence of steps that cover the following areas:
 
  * Data preparation, such as normalizations and transformations
  * Model training, such as hyper parameter tuning and validation
  * Model deployment and evaluation
```

## Comparing `azureml_pipeline-1.8.0.dist-info/RECORD` & `azureml_pipeline-1.9.0.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-azureml_pipeline-1.8.0.dist-info/DESCRIPTION.rst,sha256=em67nE7x5nb5e5F-gdSnOpMgOfTnwJIknQhsoSocmPQ,597
-azureml_pipeline-1.8.0.dist-info/LICENSE.txt,sha256=GBoIyZ-6vJ4xjRc8U3wTw4EfkuaEdVTm_gbr1Nm8uDI,859
-azureml_pipeline-1.8.0.dist-info/METADATA,sha256=2eN70MkRF8sM2UOGqJUo6Rtm9iYPYGCyhSWIvC7QOyk,1524
-azureml_pipeline-1.8.0.dist-info/RECORD,,
-azureml_pipeline-1.8.0.dist-info/WHEEL,sha256=Vlaj2XNMTTJ893zWX-JvKeZUIs7q5E7d7Gise2Vouzc,97
-azureml_pipeline-1.8.0.dist-info/metadata.json,sha256=4WJXtZwCOJGRZWca7l3ArJqx9sta-oekTwx4WAsg-BM,1088
-azureml_pipeline-1.8.0.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+azureml_pipeline-1.9.0.dist-info/DESCRIPTION.rst,sha256=em67nE7x5nb5e5F-gdSnOpMgOfTnwJIknQhsoSocmPQ,597
+azureml_pipeline-1.9.0.dist-info/LICENSE.txt,sha256=GBoIyZ-6vJ4xjRc8U3wTw4EfkuaEdVTm_gbr1Nm8uDI,859
+azureml_pipeline-1.9.0.dist-info/METADATA,sha256=8ERHZscb-3Wp5ZCvmQS89wokNqEO4YArlVyCpKotLac,1524
+azureml_pipeline-1.9.0.dist-info/RECORD,,
+azureml_pipeline-1.9.0.dist-info/WHEEL,sha256=Vlaj2XNMTTJ893zWX-JvKeZUIs7q5E7d7Gise2Vouzc,97
+azureml_pipeline-1.9.0.dist-info/metadata.json,sha256=rv0kCFTTMyAvKKD2JvR9QrGi8ZtWfTOrGzPb1tIBy3w,1088
+azureml_pipeline-1.9.0.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
```

