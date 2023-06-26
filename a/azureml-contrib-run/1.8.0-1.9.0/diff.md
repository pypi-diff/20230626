# Comparing `tmp/azureml_contrib_run-1.8.0-py3-none-any.whl.zip` & `tmp/azureml_contrib_run-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 5094 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      251 b- defN 20-Jun-22 17:21 azureml/__init__.py
--rw-rw-rw-  2.0 fat      251 b- defN 20-Jun-22 17:21 azureml/contrib/__init__.py
--rw-rw-rw-  2.0 fat      659 b- defN 20-Jun-22 17:21 azureml/contrib/mlflow/__init__.py
--rw-rw-rw-  2.0 fat      221 b- defN 20-Jun-22 17:21 azureml/contrib/run/__init__.py
--rw-rw-rw-  2.0 fat       19 b- defN 20-Jun-22 17:21 azureml/contrib/run/_version.py
--rw-rw-rw-  2.0 fat      434 b- defN 20-Jun-22 17:21 azureml_contrib_run-1.8.0.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat     1021 b- defN 20-Jun-22 17:21 azureml_contrib_run-1.8.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1088 b- defN 20-Jun-22 17:21 azureml_contrib_run-1.8.0.dist-info/metadata.json
--rw-rw-rw-  2.0 fat        8 b- defN 20-Jun-22 17:21 azureml_contrib_run-1.8.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 20-Jun-22 17:21 azureml_contrib_run-1.8.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1344 b- defN 20-Jun-22 17:21 azureml_contrib_run-1.8.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat     1095 b- defN 20-Jun-22 17:21 azureml_contrib_run-1.8.0.dist-info/RECORD
-12 files, 6488 bytes uncompressed, 3230 bytes compressed:  50.2%
+Zip file size: 5092 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      251 b- defN 20-Jul-06 20:24 azureml/__init__.py
+-rw-rw-rw-  2.0 fat      251 b- defN 20-Jul-06 20:24 azureml/contrib/__init__.py
+-rw-rw-rw-  2.0 fat      659 b- defN 20-Jul-06 20:24 azureml/contrib/mlflow/__init__.py
+-rw-rw-rw-  2.0 fat      221 b- defN 20-Jul-06 20:24 azureml/contrib/run/__init__.py
+-rw-rw-rw-  2.0 fat       19 b- defN 20-Jul-06 20:25 azureml/contrib/run/_version.py
+-rw-rw-rw-  2.0 fat      434 b- defN 20-Jul-06 20:25 azureml_contrib_run-1.9.0.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat     1021 b- defN 20-Jul-06 20:25 azureml_contrib_run-1.9.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1088 b- defN 20-Jul-06 20:25 azureml_contrib_run-1.9.0.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat        8 b- defN 20-Jul-06 20:25 azureml_contrib_run-1.9.0.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 20-Jul-06 20:25 azureml_contrib_run-1.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1344 b- defN 20-Jul-06 20:25 azureml_contrib_run-1.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat     1095 b- defN 20-Jul-06 20:25 azureml_contrib_run-1.9.0.dist-info/RECORD
+12 files, 6488 bytes uncompressed, 3228 bytes compressed:  50.2%
```

## zipnote {}

```diff
@@ -9,29 +9,29 @@
 
 Filename: azureml/contrib/run/__init__.py
 Comment: 
 
 Filename: azureml/contrib/run/_version.py
 Comment: 
 
-Filename: azureml_contrib_run-1.8.0.dist-info/DESCRIPTION.rst
+Filename: azureml_contrib_run-1.9.0.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: azureml_contrib_run-1.8.0.dist-info/LICENSE.txt
+Filename: azureml_contrib_run-1.9.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: azureml_contrib_run-1.8.0.dist-info/metadata.json
+Filename: azureml_contrib_run-1.9.0.dist-info/metadata.json
 Comment: 
 
-Filename: azureml_contrib_run-1.8.0.dist-info/top_level.txt
+Filename: azureml_contrib_run-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_contrib_run-1.8.0.dist-info/WHEEL
+Filename: azureml_contrib_run-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_contrib_run-1.8.0.dist-info/METADATA
+Filename: azureml_contrib_run-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: azureml_contrib_run-1.8.0.dist-info/RECORD
+Filename: azureml_contrib_run-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## azureml/contrib/run/_version.py

```diff
@@ -1 +1 @@
-VERSION = "1.8.0"
+VERSION = "1.9.0"
```

## Comparing `azureml_contrib_run-1.8.0.dist-info/LICENSE.txt` & `azureml_contrib_run-1.9.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `azureml_contrib_run-1.8.0.dist-info/metadata.json` & `azureml_contrib_run-1.9.0.dist-info/metadata.json`

 * *Files 2% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'run_requires'": "{0: {'requires': ['azureml-mlflow (~=1.9.0)']}}", "'version'": "'1.9.0'"}*

```diff
@@ -35,14 +35,14 @@
     "license": "Proprietary https://aka.ms/azureml-preview-sdk-license ",
     "metadata_version": "2.0",
     "name": "azureml-contrib-run",
     "requires_python": ">=3.5,<4",
     "run_requires": [
         {
             "requires": [
-                "azureml-mlflow (~=1.8.0)"
+                "azureml-mlflow (~=1.9.0)"
             ]
         }
     ],
     "summary": "UNKNOWN",
-    "version": "1.8.0"
+    "version": "1.9.0"
 }
```

## Comparing `azureml_contrib_run-1.8.0.dist-info/METADATA` & `azureml_contrib_run-1.9.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: azureml-contrib-run
-Version: 1.8.0
+Version: 1.9.0
 Summary: UNKNOWN
 Home-page: https://docs.microsoft.com/en-us/azure/machine-learning/service/
 Author: Microsoft Corp
 License: Proprietary https://aka.ms/azureml-preview-sdk-license 
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.5,<4
 Description-Content-Type: text/x-rst
-Requires-Dist: azureml-mlflow (~=1.8.0)
+Requires-Dist: azureml-mlflow (~=1.9.0)
 
 Microsoft Azure Machine Learning Tracking server plugin for Python
 ===================================================================
 The azureml-contrib-run package used to contain the integration code of AzureML with Mlflow.
 We have now updated the library to integrate with Mlflow 1.0 and are now moving out of contrib.
 
 The azureml.contrib.mlflow integration is now deprecated for the latest bits:
```

