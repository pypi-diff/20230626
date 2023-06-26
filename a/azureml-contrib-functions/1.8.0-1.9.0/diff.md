# Comparing `tmp/azureml_contrib_functions-1.8.0-py3-none-any.whl.zip` & `tmp/azureml_contrib_functions-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6646 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      251 b- defN 20-Jun-22 17:21 azureml/__init__.py
--rw-rw-rw-  2.0 fat      251 b- defN 20-Jun-22 17:21 azureml/contrib/__init__.py
--rw-rw-rw-  2.0 fat     1776 b- defN 20-Jun-22 17:21 azureml/contrib/functions/__init__.py
--rw-rw-rw-  2.0 fat     8673 b- defN 20-Jun-22 17:21 azureml/contrib/functions/_package.py
--rw-rw-rw-  2.0 fat      158 b- defN 20-Jun-22 17:21 azureml_contrib_functions-1.8.0.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat     1021 b- defN 20-Jun-22 17:21 azureml_contrib_functions-1.8.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      655 b- defN 20-Jun-22 17:21 azureml_contrib_functions-1.8.0.dist-info/metadata.json
--rw-rw-rw-  2.0 fat        8 b- defN 20-Jun-22 17:21 azureml_contrib_functions-1.8.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 20-Jun-22 17:21 azureml_contrib_functions-1.8.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      553 b- defN 20-Jun-22 17:21 azureml_contrib_functions-1.8.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat     1059 b- defN 20-Jun-22 17:21 azureml_contrib_functions-1.8.0.dist-info/RECORD
-11 files, 14502 bytes uncompressed, 4818 bytes compressed:  66.8%
+Zip file size: 6647 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      251 b- defN 20-Jul-06 20:24 azureml/__init__.py
+-rw-rw-rw-  2.0 fat      251 b- defN 20-Jul-06 20:24 azureml/contrib/__init__.py
+-rw-rw-rw-  2.0 fat     1776 b- defN 20-Jul-06 20:24 azureml/contrib/functions/__init__.py
+-rw-rw-rw-  2.0 fat     8673 b- defN 20-Jul-06 20:24 azureml/contrib/functions/_package.py
+-rw-rw-rw-  2.0 fat      158 b- defN 20-Jul-06 20:25 azureml_contrib_functions-1.9.0.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat     1021 b- defN 20-Jul-06 20:25 azureml_contrib_functions-1.9.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      655 b- defN 20-Jul-06 20:25 azureml_contrib_functions-1.9.0.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat        8 b- defN 20-Jul-06 20:25 azureml_contrib_functions-1.9.0.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 20-Jul-06 20:25 azureml_contrib_functions-1.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      553 b- defN 20-Jul-06 20:25 azureml_contrib_functions-1.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat     1059 b- defN 20-Jul-06 20:25 azureml_contrib_functions-1.9.0.dist-info/RECORD
+11 files, 14502 bytes uncompressed, 4819 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -6,29 +6,29 @@
 
 Filename: azureml/contrib/functions/__init__.py
 Comment: 
 
 Filename: azureml/contrib/functions/_package.py
 Comment: 
 
-Filename: azureml_contrib_functions-1.8.0.dist-info/DESCRIPTION.rst
+Filename: azureml_contrib_functions-1.9.0.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: azureml_contrib_functions-1.8.0.dist-info/LICENSE.txt
+Filename: azureml_contrib_functions-1.9.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: azureml_contrib_functions-1.8.0.dist-info/metadata.json
+Filename: azureml_contrib_functions-1.9.0.dist-info/metadata.json
 Comment: 
 
-Filename: azureml_contrib_functions-1.8.0.dist-info/top_level.txt
+Filename: azureml_contrib_functions-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_contrib_functions-1.8.0.dist-info/WHEEL
+Filename: azureml_contrib_functions-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_contrib_functions-1.8.0.dist-info/METADATA
+Filename: azureml_contrib_functions-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: azureml_contrib_functions-1.8.0.dist-info/RECORD
+Filename: azureml_contrib_functions-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `azureml_contrib_functions-1.8.0.dist-info/LICENSE.txt` & `azureml_contrib_functions-1.9.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `azureml_contrib_functions-1.8.0.dist-info/metadata.json` & `azureml_contrib_functions-1.9.0.dist-info/metadata.json`

 * *Files 2% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9318181818181818%*

 * *Differences: {"'run_requires'": "{0: {'requires': ['azureml-core (~=1.9.0)']}}", "'version'": "'1.9.0'"}*

```diff
@@ -22,14 +22,14 @@
     "license": "Proprietary https://aka.ms/azureml-preview-sdk-license ",
     "metadata_version": "2.0",
     "name": "azureml-contrib-functions",
     "requires_python": ">=3.5,<4",
     "run_requires": [
         {
             "requires": [
-                "azureml-core (~=1.8.0)"
+                "azureml-core (~=1.9.0)"
             ]
         }
     ],
     "summary": "Azure Machine Learning Functions",
-    "version": "1.8.0"
+    "version": "1.9.0"
 }
```

## Comparing `azureml_contrib_functions-1.8.0.dist-info/METADATA` & `azureml_contrib_functions-1.9.0.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.0
 Name: azureml-contrib-functions
-Version: 1.8.0
+Version: 1.9.0
 Summary: Azure Machine Learning Functions
 Home-page: https://docs.microsoft.com/en-us/azure/machine-learning/service/
 Author: Microsoft Corp
 License: Proprietary https://aka.ms/azureml-preview-sdk-license 
 Platform: UNKNOWN
 Requires-Python: >=3.5,<4
 Description-Content-Type: text/x-rst
-Requires-Dist: azureml-core (~=1.8.0)
+Requires-Dist: azureml-core (~=1.9.0)
 
 AzureML Contrib Functions
 
 An experimental package to enable creation of Azure Functions applications from models registered with Azure Machine Learning.
```

## Comparing `azureml_contrib_functions-1.8.0.dist-info/RECORD` & `azureml_contrib_functions-1.9.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 azureml/__init__.py,sha256=n0xtZ3iWcoVg5Qognsb7InYAUVAK8s3iaVeHB5GOaNA,251
 azureml/contrib/__init__.py,sha256=n0xtZ3iWcoVg5Qognsb7InYAUVAK8s3iaVeHB5GOaNA,251
 azureml/contrib/functions/__init__.py,sha256=ZUOfXi4e_Vdzh_hwKBA5Sce0DBEscnQ51W0dPo6zhdA,1776
 azureml/contrib/functions/_package.py,sha256=oq_0OkuglzAdGUjsnNL30myHtVp8hM25zVymdpK6-fc,8673
-azureml_contrib_functions-1.8.0.dist-info/DESCRIPTION.rst,sha256=tY1uRX3C3IV01ny8aBujg6oML6gndf1mUtWeduYtYfU,158
-azureml_contrib_functions-1.8.0.dist-info/LICENSE.txt,sha256=FOfkEEz4uS7g278F9Rq12rqKF3lLyBUZhVpLetuZrTg,1021
-azureml_contrib_functions-1.8.0.dist-info/METADATA,sha256=To6QAPKiGeSxrKsVR10cRS9Hoo5UUQ4KGk8jXojmHPI,553
-azureml_contrib_functions-1.8.0.dist-info/RECORD,,
-azureml_contrib_functions-1.8.0.dist-info/WHEEL,sha256=Vlaj2XNMTTJ893zWX-JvKeZUIs7q5E7d7Gise2Vouzc,97
-azureml_contrib_functions-1.8.0.dist-info/metadata.json,sha256=3EU1oV9g5yGJDkevc3l9mnxPxGOwn5aiJUrMQ-NYPEo,655
-azureml_contrib_functions-1.8.0.dist-info/top_level.txt,sha256=ZOeEa0TAXo6i5wOjwBoqfIGEuxOcKuscGgNSpizqREY,8
+azureml_contrib_functions-1.9.0.dist-info/DESCRIPTION.rst,sha256=tY1uRX3C3IV01ny8aBujg6oML6gndf1mUtWeduYtYfU,158
+azureml_contrib_functions-1.9.0.dist-info/LICENSE.txt,sha256=FOfkEEz4uS7g278F9Rq12rqKF3lLyBUZhVpLetuZrTg,1021
+azureml_contrib_functions-1.9.0.dist-info/METADATA,sha256=ARzks7zBNJNeyqGJbVBX9Xuzif6lstmFGML9u9UdolU,553
+azureml_contrib_functions-1.9.0.dist-info/RECORD,,
+azureml_contrib_functions-1.9.0.dist-info/WHEEL,sha256=Vlaj2XNMTTJ893zWX-JvKeZUIs7q5E7d7Gise2Vouzc,97
+azureml_contrib_functions-1.9.0.dist-info/metadata.json,sha256=XKHIkTOUNEf70GRs33ZpuzE98CPShcfLr_xxbRJh_dI,655
+azureml_contrib_functions-1.9.0.dist-info/top_level.txt,sha256=ZOeEa0TAXo6i5wOjwBoqfIGEuxOcKuscGgNSpizqREY,8
```

