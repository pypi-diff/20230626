# Comparing `tmp/azureml_train_automl-1.8.0-py3-none-any.whl.zip` & `tmp/azureml_train_automl-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3423 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      169 b- defN 20-Jun-22 17:22 azureml_train_automl-1.8.0.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat      859 b- defN 20-Jun-22 17:22 azureml_train_automl-1.8.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1255 b- defN 20-Jun-22 17:22 azureml_train_automl-1.8.0.dist-info/metadata.json
--rw-rw-rw-  2.0 fat        1 b- defN 20-Jun-22 17:22 azureml_train_automl-1.8.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 20-Jun-22 17:22 azureml_train_automl-1.8.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1294 b- defN 20-Jun-22 17:22 azureml_train_automl-1.8.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      675 b- defN 20-Jun-22 17:22 azureml_train_automl-1.8.0.dist-info/RECORD
-7 files, 4350 bytes uncompressed, 2209 bytes compressed:  49.2%
+Zip file size: 3424 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      169 b- defN 20-Jul-06 20:26 azureml_train_automl-1.9.0.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat      859 b- defN 20-Jul-06 20:26 azureml_train_automl-1.9.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1256 b- defN 20-Jul-06 20:26 azureml_train_automl-1.9.0.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat        1 b- defN 20-Jul-06 20:26 azureml_train_automl-1.9.0.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 20-Jul-06 20:26 azureml_train_automl-1.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1295 b- defN 20-Jul-06 20:26 azureml_train_automl-1.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      675 b- defN 20-Jul-06 20:26 azureml_train_automl-1.9.0.dist-info/RECORD
+7 files, 4352 bytes uncompressed, 2210 bytes compressed:  49.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: azureml_train_automl-1.8.0.dist-info/DESCRIPTION.rst
+Filename: azureml_train_automl-1.9.0.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: azureml_train_automl-1.8.0.dist-info/LICENSE.txt
+Filename: azureml_train_automl-1.9.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: azureml_train_automl-1.8.0.dist-info/metadata.json
+Filename: azureml_train_automl-1.9.0.dist-info/metadata.json
 Comment: 
 
-Filename: azureml_train_automl-1.8.0.dist-info/top_level.txt
+Filename: azureml_train_automl-1.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_train_automl-1.8.0.dist-info/WHEEL
+Filename: azureml_train_automl-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_train_automl-1.8.0.dist-info/METADATA
+Filename: azureml_train_automl-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: azureml_train_automl-1.8.0.dist-info/RECORD
+Filename: azureml_train_automl-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `azureml_train_automl-1.8.0.dist-info/LICENSE.txt` & `azureml_train_automl-1.9.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `azureml_train_automl-1.8.0.dist-info/metadata.json` & `azureml_train_automl-1.9.0.dist-info/metadata.json`

 * *Files 19% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'run_requires'": "{0: {'requires': ['azureml-automl-core (~=1.9.0)', 'azureml-automl-runtime "*

 * *                   "(~=1.9.0)', 'azureml-dataprep[fuse,pandas] (<1.10.0a,>=1.9.0a)', "*

 * *                   "'azureml-train-automl-client (~=1.9.0)', 'azureml-train-automl-runtime "*

 * *                   "(~=1.9.0)']}}",*

 * * "'version'": "'1.9.0'"}*

```diff
@@ -35,18 +35,18 @@
     "license": "https://aka.ms/azureml-sdk-license",
     "metadata_version": "2.0",
     "name": "azureml-train-automl",
     "requires_python": ">=3.5,<4",
     "run_requires": [
         {
             "requires": [
-                "azureml-automl-core (~=1.8.0)",
-                "azureml-automl-runtime (~=1.8.0)",
-                "azureml-dataprep[fuse,pandas] (<1.9.0a,>=1.8.0a)",
-                "azureml-train-automl-client (~=1.8.0)",
-                "azureml-train-automl-runtime (~=1.8.0)"
+                "azureml-automl-core (~=1.9.0)",
+                "azureml-automl-runtime (~=1.9.0)",
+                "azureml-dataprep[fuse,pandas] (<1.10.0a,>=1.9.0a)",
+                "azureml-train-automl-client (~=1.9.0)",
+                "azureml-train-automl-runtime (~=1.9.0)"
             ]
         }
     ],
     "summary": "automl",
-    "version": "1.8.0"
+    "version": "1.9.0"
 }
```

## Comparing `azureml_train_automl-1.8.0.dist-info/RECORD` & `azureml_train_automl-1.9.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-azureml_train_automl-1.8.0.dist-info/DESCRIPTION.rst,sha256=uY32lxjEvP5QgN5MrOQv24YrzQkYgUuIevQVJ5x_SX0,169
-azureml_train_automl-1.8.0.dist-info/LICENSE.txt,sha256=GBoIyZ-6vJ4xjRc8U3wTw4EfkuaEdVTm_gbr1Nm8uDI,859
-azureml_train_automl-1.8.0.dist-info/METADATA,sha256=ABf1F33ynUYPaGes1jfdtr3_V3EGpZDQ4ve3DmmInkg,1294
-azureml_train_automl-1.8.0.dist-info/RECORD,,
-azureml_train_automl-1.8.0.dist-info/WHEEL,sha256=Vlaj2XNMTTJ893zWX-JvKeZUIs7q5E7d7Gise2Vouzc,97
-azureml_train_automl-1.8.0.dist-info/metadata.json,sha256=htUnzqHzCI5NgYhdn99jV8tb8CTftK1c16WGDbsxRq0,1255
-azureml_train_automl-1.8.0.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+azureml_train_automl-1.9.0.dist-info/DESCRIPTION.rst,sha256=uY32lxjEvP5QgN5MrOQv24YrzQkYgUuIevQVJ5x_SX0,169
+azureml_train_automl-1.9.0.dist-info/LICENSE.txt,sha256=GBoIyZ-6vJ4xjRc8U3wTw4EfkuaEdVTm_gbr1Nm8uDI,859
+azureml_train_automl-1.9.0.dist-info/METADATA,sha256=A_V4O5VUF7Dt3ToTn4vKGjptDrhohKZybdsrNpiq398,1295
+azureml_train_automl-1.9.0.dist-info/RECORD,,
+azureml_train_automl-1.9.0.dist-info/WHEEL,sha256=Vlaj2XNMTTJ893zWX-JvKeZUIs7q5E7d7Gise2Vouzc,97
+azureml_train_automl-1.9.0.dist-info/metadata.json,sha256=Q0FOywWGjXQYgXVCO12VJ1nH2rA4N-MDVFQw_0-X-y4,1256
+azureml_train_automl-1.9.0.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
```

