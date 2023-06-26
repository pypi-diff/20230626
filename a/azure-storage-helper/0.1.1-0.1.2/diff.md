# Comparing `tmp/azure_storage_helper-0.1.1.tar.gz` & `tmp/azure_storage_helper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_storage_helper-0.1.1.tar", max compression
+gzip compressed data, was "azure_storage_helper-0.1.2.tar", max compression
```

## Comparing `azure_storage_helper-0.1.1.tar` & `azure_storage_helper-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-06-23 06:04:39.516677 azure_storage_helper-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-06-23 06:04:51.606033 azure_storage_helper-0.1.1/README.md
--rw-r--r--   0        0        0      137 2023-06-23 06:18:18.233783 azure_storage_helper-0.1.1/azure/gen1/__init__.py
--rw-r--r--   0        0        0     9808 2023-06-23 06:18:18.238469 azure_storage_helper-0.1.1/azure/gen1/gen1.py
--rw-r--r--   0        0        0     2747 2023-06-26 04:48:47.058369 azure_storage_helper-0.1.1/azure/gen1/helper.py
--rw-r--r--   0        0        0      177 2023-06-23 06:18:18.248482 azure_storage_helper-0.1.1/azure/gen2/__init__.py
--rw-r--r--   0        0        0    16958 2023-06-23 06:18:18.251997 azure_storage_helper-0.1.1/azure/gen2/gen2.py
--rw-r--r--   0        0        0     2809 2023-06-26 04:48:53.986331 azure_storage_helper-0.1.1/azure/gen2/helper.py
--rw-r--r--   0        0        0      459 2023-06-26 04:49:07.714160 azure_storage_helper-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 azure_storage_helper-0.1.1/setup.py
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 azure_storage_helper-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-23 06:04:39.516677 azure_storage_helper-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-06-23 06:04:51.606033 azure_storage_helper-0.1.2/README.md
+-rw-r--r--   0        0        0      137 2023-06-23 06:18:18.233783 azure_storage_helper-0.1.2/azure/gen1/__init__.py
+-rw-r--r--   0        0        0    10215 2023-06-26 07:26:42.964073 azure_storage_helper-0.1.2/azure/gen1/gen1.py
+-rw-r--r--   0        0        0     2760 2023-06-26 07:26:51.109685 azure_storage_helper-0.1.2/azure/gen1/helper.py
+-rw-r--r--   0        0        0      177 2023-06-23 06:18:18.248482 azure_storage_helper-0.1.2/azure/gen2/__init__.py
+-rw-r--r--   0        0        0    17089 2023-06-26 07:26:13.491820 azure_storage_helper-0.1.2/azure/gen2/gen2.py
+-rw-r--r--   0        0        0     2822 2023-06-26 07:26:28.520023 azure_storage_helper-0.1.2/azure/gen2/helper.py
+-rw-r--r--   0        0        0      459 2023-06-26 07:28:12.292110 azure_storage_helper-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 azure_storage_helper-0.1.2/setup.py
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 azure_storage_helper-0.1.2/PKG-INFO
```

### Comparing `azure_storage_helper-0.1.1/azure/gen1/gen1.py` & `azure_storage_helper-0.1.2/azure/gen1/gen1.py`

 * *Files 3% similar despite different names*

```diff
@@ -280,14 +280,24 @@
         """Blob의 존재 유무를 반환합니다.
 
         Returns:
             bool: 해당 blob이 존재하면 `True`, 아니면 `False`를 반환.
         """
         return self.client.exists()
 
+    def delete(self, delete_snapshots: str = "include") -> None:
+        """현재 blob을 삭제합니다.
+
+        Args:
+            delete_snapshots (str, optional): 스냅샷 삭제 여부.\n
+            스냅샷만 삭제하고 blob은 남기고 싶다면 `delete_snapshots="only"`\n
+            Defaults to "include".\n
+        """
+        self.client.delete_blob(delete_snapshots=delete_snapshots)
+
     def __init(self) -> None:
         """인스턴스 초기화"""
         container_name, *others = self._sub_path.parts
         self._container = ContainerClient(container_name, self._storage)
         self._sub_path = Path("/".join(others))
 
     def __str__(self) -> str:
```

### Comparing `azure_storage_helper-0.1.1/azure/gen1/helper.py` & `azure_storage_helper-0.1.2/azure/gen1/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,25 +22,25 @@
         dict: YAML contents.
     """
     stream = blob.download()
     config = yaml.safe_load(stream)
     return config
 
 
-def load_csv(blob: BlobClient) -> DataFrame:
+def load_csv(blob: BlobClient, **kwargs) -> DataFrame:
     """CSV 파일을 읽어 DataFrame으로 반환합니다.
 
     Args:
         blob (BlobClient): BlobClient.
 
     Returns:
         DataFrame: Data.
     """
     stream = blob.download()
-    return pd.read_csv(stream, index_col=0, low_memory=False)
+    return pd.read_csv(stream, low_memory=False, **kwargs)
 
 
 def load_jobib(blob: BlobClient) -> Any:
     """joblib으로 저장된 객체를 불러옵니다.
 
     Args:
         blob (BlobClient): BlobClient.
@@ -55,15 +55,17 @@
         file.seek(os.SEEK_SET)
 
         obj = joblib.load(file.name)
 
     return obj
 
 
-def upload_to_csv(blob: BlobClient, data: DataFrame, encode: str = "utf-8", **kwargs):
+def upload_to_csv(
+    blob: BlobClient, data: DataFrame, encode: str = "utf-8", **kwargs
+):
     """DataFrame을 CSV 파일로 저장합니다.
 
     Args:
         blob (BlobClient): BlobClient.
         data (DataFrame): Data.
         encode (str): Encoding option.
         **kwargs : pandas.DataFrame.to_csv(**kwargs) e.g. index, header, ...
```

### Comparing `azure_storage_helper-0.1.1/azure/gen2/gen2.py` & `azure_storage_helper-0.1.2/azure/gen2/gen2.py`

 * *Files 1% similar despite different names*

```diff
@@ -496,14 +496,19 @@
         """
         try:
             self.client.create_file(**kwargs)
         except ResourceExistsError as err:
             if not exist_ok:
                 raise err
 
+    def delete(self, **kwargs) -> None:
+        """Blob을 삭제합니다.
+        """
+        self.client.delete_file(**kwargs)
+
     def __init(self) -> None:
         """인스턴스 초기화"""
         container_name, *others = self._sub_path.parts
         self._container = ContainerClient(container_name, self._storage)
         self._sub_path = Path("/".join(others))
 
     def __str__(self) -> str:
```

### Comparing `azure_storage_helper-0.1.1/azure/gen2/helper.py` & `azure_storage_helper-0.1.2/azure/gen2/helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,25 +22,25 @@
         dict: YAML contents.
     """
     stream = blob.download()
     config = yaml.safe_load(stream)
     return config
 
 
-def load_csv(blob: BlobClient) -> DataFrame:
+def load_csv(blob: BlobClient, **kwargs) -> DataFrame:
     """CSV 파일을 읽어 DataFrame으로 반환합니다.
 
     Args:
         blob (BlobClient): BlobClient.
 
     Returns:
         DataFrame: Data.
     """
     stream = blob.download()
-    return pd.read_csv(stream, index_col=0, low_memory=False)
+    return pd.read_csv(stream, low_memory=False, **kwargs)
 
 
 def load_jobib(blob: BlobClient) -> Any:
     """joblib으로 저장된 객체를 불러옵니다.
 
     Args:
         blob (BlobClient): BlobClient.
@@ -55,15 +55,17 @@
         file.seek(os.SEEK_SET)
 
         obj = joblib.load(file.name)
 
     return obj
 
 
-def upload_to_csv(blob: BlobClient, data: DataFrame, encode: str = "utf-8", **kwargs):
+def upload_to_csv(
+    blob: BlobClient, data: DataFrame, encode: str = "utf-8", **kwargs
+):
     """DataFrame을 CSV 파일로 저장합니다.
 
     Args:
         blob (BlobClient): BlobClient.
         data (DataFrame): Data.
         encode (str): Encoding option.
         **kwargs : pandas.DataFrame.to_csv(**kwargs) e.g. index, header, ...
```

### Comparing `azure_storage_helper-0.1.1/setup.py` & `azure_storage_helper-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'azure-storage-file-datalake>=12.9.1,<13.0.0',
  'joblib>=1.2.0,<2.0.0',
  'pandas>=1.5.2',
  'pyyaml>=6.0,<7.0']
 
 setup_kwargs = {
     'name': 'azure-storage-helper',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
     'long_description': '',
     'author': 'gbhwang',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `azure_storage_helper-0.1.1/PKG-INFO` & `azure_storage_helper-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-storage-helper
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: gbhwang
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

