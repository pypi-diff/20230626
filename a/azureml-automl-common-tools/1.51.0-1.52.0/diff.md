# Comparing `tmp/azureml_automl_common_tools-1.51.0-py3-none-any.whl.zip` & `tmp/azureml_automl_common_tools-1.52.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2160 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat      859 b- defN 23-May-24 03:34 azureml_automl_common_tools-1.51.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      746 b- defN 23-May-24 03:34 azureml_automl_common_tools-1.51.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-May-24 03:34 azureml_automl_common_tools-1.51.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-24 03:34 azureml_automl_common_tools-1.51.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      492 b- defN 23-May-24 03:34 azureml_automl_common_tools-1.51.0.dist-info/RECORD
-5 files, 2195 bytes uncompressed, 1222 bytes compressed:  44.3%
+Zip file size: 2172 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat      859 b- defN 23-Jun-26 15:40 azureml_automl_common_tools-1.52.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      778 b- defN 23-Jun-26 15:40 azureml_automl_common_tools-1.52.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-26 15:40 azureml_automl_common_tools-1.52.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-26 15:40 azureml_automl_common_tools-1.52.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      492 b- defN 23-Jun-26 15:40 azureml_automl_common_tools-1.52.0.dist-info/RECORD
+5 files, 2227 bytes uncompressed, 1234 bytes compressed:  44.6%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: azureml_automl_common_tools-1.51.0.dist-info/LICENSE.txt
+Filename: azureml_automl_common_tools-1.52.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: azureml_automl_common_tools-1.51.0.dist-info/METADATA
+Filename: azureml_automl_common_tools-1.52.0.dist-info/METADATA
 Comment: 
 
-Filename: azureml_automl_common_tools-1.51.0.dist-info/WHEEL
+Filename: azureml_automl_common_tools-1.52.0.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_automl_common_tools-1.51.0.dist-info/top_level.txt
+Filename: azureml_automl_common_tools-1.52.0.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_automl_common_tools-1.51.0.dist-info/RECORD
+Filename: azureml_automl_common_tools-1.52.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `azureml_automl_common_tools-1.51.0.dist-info/LICENSE.txt` & `azureml_automl_common_tools-1.52.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `azureml_automl_common_tools-1.51.0.dist-info/METADATA` & `azureml_automl_common_tools-1.52.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: azureml-automl-common-tools
-Version: 1.51.0
+Version: 1.52.0
 Summary: Internal metapackage used for Azure machine learning.
 Home-page: https://docs.microsoft.com/python/api/overview/azure/ml/?view=azure-ml-py
 Author: Microsoft Corp
 License: https://aka.ms/azureml-sdk-license
 Platform: UNKNOWN
-Requires-Python: >=3.7,<3.9
+Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/x-rst
 Requires-Dist: py-spy (==0.3.12)
 Requires-Dist: debugpy (~=1.6.3)
 Requires-Dist: ipykernel (~=6.0)
-Requires-Dist: tensorboard (~=2.11.0)
+Requires-Dist: tensorboard
 Requires-Dist: psutil (~=5.8.0)
 Requires-Dist: matplotlib (~=3.5.0)
 Requires-Dist: tqdm (~=4.62.0)
 Requires-Dist: py-cpuinfo (==5.0.0)
+Requires-Dist: torch-tb-profiler (~=0.4.0)
 
 The azureml-automl-common-tools is a metapackage that is used internally by Azure Machine Learning.
```

