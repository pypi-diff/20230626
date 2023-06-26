# Comparing `tmp/azure_storage_helper-0.1.0.tar.gz` & `tmp/azure_storage_helper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_storage_helper-0.1.0.tar", max compression
+gzip compressed data, was "azure_storage_helper-0.1.1.tar", max compression
```

## Comparing `azure_storage_helper-0.1.0.tar` & `azure_storage_helper-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-06-23 06:04:39.516677 azure_storage_helper-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-06-23 06:04:51.606033 azure_storage_helper-0.1.0/README.md
--rw-r--r--   0        0        0      137 2023-06-23 06:18:18.233783 azure_storage_helper-0.1.0/azure/gen1/__init__.py
--rw-r--r--   0        0        0     9808 2023-06-23 06:18:18.238469 azure_storage_helper-0.1.0/azure/gen1/gen1.py
--rw-r--r--   0        0        0     2591 2023-06-23 06:18:18.239042 azure_storage_helper-0.1.0/azure/gen1/helper.py
--rw-r--r--   0        0        0      177 2023-06-23 06:18:18.248482 azure_storage_helper-0.1.0/azure/gen2/__init__.py
--rw-r--r--   0        0        0    16958 2023-06-23 06:18:18.251997 azure_storage_helper-0.1.0/azure/gen2/gen2.py
--rw-r--r--   0        0        0     2653 2023-06-23 06:18:18.252413 azure_storage_helper-0.1.0/azure/gen2/helper.py
--rw-r--r--   0        0        0      459 2023-06-23 06:15:11.622680 azure_storage_helper-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 azure_storage_helper-0.1.0/setup.py
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 azure_storage_helper-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-23 06:04:39.516677 azure_storage_helper-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-06-23 06:04:51.606033 azure_storage_helper-0.1.1/README.md
+-rw-r--r--   0        0        0      137 2023-06-23 06:18:18.233783 azure_storage_helper-0.1.1/azure/gen1/__init__.py
+-rw-r--r--   0        0        0     9808 2023-06-23 06:18:18.238469 azure_storage_helper-0.1.1/azure/gen1/gen1.py
+-rw-r--r--   0        0        0     2747 2023-06-26 04:48:47.058369 azure_storage_helper-0.1.1/azure/gen1/helper.py
+-rw-r--r--   0        0        0      177 2023-06-23 06:18:18.248482 azure_storage_helper-0.1.1/azure/gen2/__init__.py
+-rw-r--r--   0        0        0    16958 2023-06-23 06:18:18.251997 azure_storage_helper-0.1.1/azure/gen2/gen2.py
+-rw-r--r--   0        0        0     2809 2023-06-26 04:48:53.986331 azure_storage_helper-0.1.1/azure/gen2/helper.py
+-rw-r--r--   0        0        0      459 2023-06-26 04:49:07.714160 azure_storage_helper-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 azure_storage_helper-0.1.1/setup.py
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 azure_storage_helper-0.1.1/PKG-INFO
```

### Comparing `azure_storage_helper-0.1.0/azure/gen1/gen1.py` & `azure_storage_helper-0.1.1/azure/gen1/gen1.py`

 * *Files identical despite different names*

### Comparing `azure_storage_helper-0.1.0/azure/gen1/helper.py` & `azure_storage_helper-0.1.1/azure/gen1/helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -55,24 +55,26 @@
         file.seek(os.SEEK_SET)
 
         obj = joblib.load(file.name)
 
     return obj
 
 
-def upload_to_csv(blob: BlobClient, data: DataFrame):
+def upload_to_csv(blob: BlobClient, data: DataFrame, encode: str = "utf-8", **kwargs):
     """DataFrame을 CSV 파일로 저장합니다.
 
     Args:
         blob (BlobClient): BlobClient.
         data (DataFrame): Data.
+        encode (str): Encoding option.
+        **kwargs : pandas.DataFrame.to_csv(**kwargs) e.g. index, header, ...
     """
     blob.container.create(exist_ok=True)
 
-    stream = BytesIO(data.to_csv().encode("utf-8"))
+    stream = BytesIO(data.to_csv(**kwargs).encode(encode))
     blob.upload(stream)
 
 
 def upload_file(blob: BlobClient, local_path: str):
     """파일을 저장합니다.
 
     Args:
```

### Comparing `azure_storage_helper-0.1.0/azure/gen2/gen2.py` & `azure_storage_helper-0.1.1/azure/gen2/gen2.py`

 * *Files identical despite different names*

### Comparing `azure_storage_helper-0.1.0/azure/gen2/helper.py` & `azure_storage_helper-0.1.1/azure/gen2/helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,25 +55,27 @@
         file.seek(os.SEEK_SET)
 
         obj = joblib.load(file.name)
 
     return obj
 
 
-def upload_to_csv(blob: BlobClient, data: DataFrame):
+def upload_to_csv(blob: BlobClient, data: DataFrame, encode: str = "utf-8", **kwargs):
     """DataFrame을 CSV 파일로 저장합니다.
 
     Args:
         blob (BlobClient): BlobClient.
         data (DataFrame): Data.
+        encode (str): Encoding option.
+        **kwargs : pandas.DataFrame.to_csv(**kwargs) e.g. index, header, ...
     """
     blob.container.create(exist_ok=True)
     blob.create(exist_ok=True)
 
-    stream = BytesIO(data.to_csv().encode("utf-8"))
+    stream = BytesIO(data.to_csv(**kwargs).encode(encode))
     blob.upload(stream)
 
 
 def upload_file(blob: BlobClient, local_path: str):
     """파일을 저장합니다.
 
     Args:
```

### Comparing `azure_storage_helper-0.1.0/setup.py` & `azure_storage_helper-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'azure-storage-file-datalake>=12.9.1,<13.0.0',
  'joblib>=1.2.0,<2.0.0',
  'pandas>=1.5.2',
  'pyyaml>=6.0,<7.0']
 
 setup_kwargs = {
     'name': 'azure-storage-helper',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': '',
     'author': 'gbhwang',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `azure_storage_helper-0.1.0/PKG-INFO` & `azure_storage_helper-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-storage-helper
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: gbhwang
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

