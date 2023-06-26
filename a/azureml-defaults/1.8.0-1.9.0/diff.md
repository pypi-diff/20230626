# Comparing `tmp/azureml_defaults-1.8.0-py3-none-any.whl.zip` & `tmp/azureml_defaults-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2967 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat       92 b- defN 20-Jun-22 17:22 azureml_defaults-1.8.0.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat      859 b- defN 20-Jun-22 17:22 azureml_defaults-1.8.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      722 b- defN 20-Jun-22 17:22 azureml_defaults-1.8.0.dist-info/metadata.json
--rw-rw-rw-  2.0 fat        1 b- defN 20-Jun-22 17:22 azureml_defaults-1.8.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 20-Jun-22 17:22 azureml_defaults-1.8.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      692 b- defN 20-Jun-22 17:22 azureml_defaults-1.8.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      644 b- defN 20-Jun-22 17:22 azureml_defaults-1.8.0.dist-info/RECORD
-7 files, 3107 bytes uncompressed, 1809 bytes compressed:  41.8%
+Zip file size: 2966 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat       92 b- defN 20-Jul-06 20:26 azureml_defaults-1.9.0.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat      859 b- defN 20-Jul-06 20:26 azureml_defaults-1.9.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      723 b- defN 20-Jul-06 20:26 azureml_defaults-1.9.0.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat        1 b- defN 20-Jul-06 20:26 azureml_defaults-1.9.0.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 20-Jul-06 20:26 azureml_defaults-1.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      693 b- defN 20-Jul-06 20:26 azureml_defaults-1.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      644 b- defN 20-Jul-06 20:26 azureml_defaults-1.9.0.dist-info/RECORD
+7 files, 3109 bytes uncompressed, 1808 bytes compressed:  41.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: azureml_defaults-1.8.0.dist-info/DESCRIPTION.rst
+Filename: azureml_defaults-1.9.0.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: azureml_defaults-1.8.0.dist-info/LICENSE.txt
+Filename: azureml_defaults-1.9.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: azureml_defaults-1.8.0.dist-info/metadata.json
+Filename: azureml_defaults-1.9.0.dist-info/metadata.json
 Comment: 
 
-Filename: azureml_defaults-1.8.0.dist-info/top_level.txt
+Filename: azureml_defaults-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_defaults-1.8.0.dist-info/WHEEL
+Filename: azureml_defaults-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_defaults-1.8.0.dist-info/METADATA
+Filename: azureml_defaults-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: azureml_defaults-1.8.0.dist-info/RECORD
+Filename: azureml_defaults-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `azureml_defaults-1.8.0.dist-info/LICENSE.txt` & `azureml_defaults-1.9.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `azureml_defaults-1.8.0.dist-info/metadata.json` & `azureml_defaults-1.9.0.dist-info/metadata.json`

 * *Files 2% similar despite different names*

### Pretty-printed

 * *Similarity: 0.940909090909091%*

 * *Differences: {"'run_requires'": "{0: {'requires': {insert: [(1, 'azureml-core (~=1.9.0)'), (2, "*

 * *                   "'azureml-dataprep[fuse] (<1.10.0a,>=1.9.0a)')], delete: [2, 1]}}}",*

 * * "'version'": "'1.9.0'"}*

```diff
@@ -19,21 +19,21 @@
     "license": "https://aka.ms/azureml-sdk-license",
     "metadata_version": "2.0",
     "name": "azureml-defaults",
     "run_requires": [
         {
             "requires": [
                 "applicationinsights (>=0.11.7)",
-                "azureml-core (~=1.8.0)",
-                "azureml-dataprep[fuse] (<1.9.0a,>=1.8.0a)",
+                "azureml-core (~=1.9.0)",
+                "azureml-dataprep[fuse] (<1.10.0a,>=1.9.0a)",
                 "azureml-model-management-sdk (==1.0.1b6.post1)",
                 "configparser (==3.7.4)",
                 "flask (==1.0.3)",
                 "gunicorn (==19.9.0)",
                 "json-logging-py (==0.2)",
                 "werkzeug (==0.16.1)"
             ]
         }
     ],
     "summary": "UNKNOWN",
-    "version": "1.8.0"
+    "version": "1.9.0"
 }
```

## Comparing `azureml_defaults-1.8.0.dist-info/METADATA` & `azureml_defaults-1.9.0.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.0
 Name: azureml-defaults
-Version: 1.8.0
+Version: 1.9.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Microsoft Corp
 License: https://aka.ms/azureml-sdk-license
 Platform: UNKNOWN
 Description-Content-Type: text/x-rst
 Requires-Dist: azureml-model-management-sdk (==1.0.1b6.post1)
 Requires-Dist: configparser (==3.7.4)
 Requires-Dist: flask (==1.0.3)
 Requires-Dist: gunicorn (==19.9.0)
 Requires-Dist: json-logging-py (==0.2)
-Requires-Dist: azureml-core (~=1.8.0)
-Requires-Dist: azureml-dataprep[fuse] (<1.9.0a,>=1.8.0a)
+Requires-Dist: azureml-core (~=1.9.0)
+Requires-Dist: azureml-dataprep[fuse] (<1.10.0a,>=1.9.0a)
 Requires-Dist: applicationinsights (>=0.11.7)
 Requires-Dist: werkzeug (==0.16.1)
 
 The azureml-defaults is a metapackage that is used internally by Azure Machine Learning.
```

