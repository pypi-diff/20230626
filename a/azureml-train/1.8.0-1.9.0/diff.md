# Comparing `tmp/azureml_train-1.8.0-py3-none-any.whl.zip` & `tmp/azureml_train-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3229 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      173 b- defN 20-Jun-22 17:22 azureml_train-1.8.0.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat      859 b- defN 20-Jun-22 17:22 azureml_train-1.8.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1118 b- defN 20-Jun-22 17:22 azureml_train-1.8.0.dist-info/metadata.json
--rw-rw-rw-  2.0 fat        1 b- defN 20-Jun-22 17:22 azureml_train-1.8.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 20-Jun-22 17:22 azureml_train-1.8.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1122 b- defN 20-Jun-22 17:22 azureml_train-1.8.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      626 b- defN 20-Jun-22 17:22 azureml_train-1.8.0.dist-info/RECORD
-7 files, 3996 bytes uncompressed, 2113 bytes compressed:  47.1%
+Zip file size: 3228 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      173 b- defN 20-Jul-06 20:26 azureml_train-1.9.0.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat      859 b- defN 20-Jul-06 20:26 azureml_train-1.9.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1118 b- defN 20-Jul-06 20:26 azureml_train-1.9.0.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat        1 b- defN 20-Jul-06 20:26 azureml_train-1.9.0.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 20-Jul-06 20:26 azureml_train-1.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1122 b- defN 20-Jul-06 20:26 azureml_train-1.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      626 b- defN 20-Jul-06 20:26 azureml_train-1.9.0.dist-info/RECORD
+7 files, 3996 bytes uncompressed, 2112 bytes compressed:  47.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: azureml_train-1.8.0.dist-info/DESCRIPTION.rst
+Filename: azureml_train-1.9.0.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: azureml_train-1.8.0.dist-info/LICENSE.txt
+Filename: azureml_train-1.9.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: azureml_train-1.8.0.dist-info/metadata.json
+Filename: azureml_train-1.9.0.dist-info/metadata.json
 Comment: 
 
-Filename: azureml_train-1.8.0.dist-info/top_level.txt
+Filename: azureml_train-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_train-1.8.0.dist-info/WHEEL
+Filename: azureml_train-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_train-1.8.0.dist-info/METADATA
+Filename: azureml_train-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: azureml_train-1.8.0.dist-info/RECORD
+Filename: azureml_train-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `azureml_train-1.8.0.dist-info/LICENSE.txt` & `azureml_train-1.9.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `azureml_train-1.8.0.dist-info/metadata.json` & `azureml_train-1.9.0.dist-info/metadata.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'run_requires'": "{0: {'requires': ['azureml-train-core (~=1.9.0)']}}", "'version'": "'1.9.0'"}*

```diff
@@ -36,14 +36,14 @@
     "license": "https://aka.ms/azureml-sdk-license",
     "metadata_version": "2.0",
     "name": "azureml-train",
     "requires_python": ">=3.5,<4",
     "run_requires": [
         {
             "requires": [
-                "azureml-train-core (~=1.8.0)"
+                "azureml-train-core (~=1.9.0)"
             ]
         }
     ],
     "summary": "UNKNOWN",
-    "version": "1.8.0"
+    "version": "1.9.0"
 }
```

## Comparing `azureml_train-1.8.0.dist-info/METADATA` & `azureml_train-1.9.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: azureml-train
-Version: 1.8.0
+Version: 1.9.0
 Summary: UNKNOWN
 Home-page: https://docs.microsoft.com/en-us/azure/machine-learning/service/
 Author: Microsoft Corp
 License: https://aka.ms/azureml-sdk-license
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -16,13 +16,13 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.5,<4
 Description-Content-Type: text/x-rst
-Requires-Dist: azureml-train-core (~=1.8.0)
+Requires-Dist: azureml-train-core (~=1.9.0)
 
 The azureml-train package provides estimators for training models using different deep learning frameworks and functionality for hyperparameter tuning using Azure cloud.
```

