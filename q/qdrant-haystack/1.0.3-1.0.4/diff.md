# Comparing `tmp/qdrant_haystack-1.0.3.tar.gz` & `tmp/qdrant_haystack-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_haystack-1.0.3.tar", max compression
+gzip compressed data, was "qdrant_haystack-1.0.4.tar", max compression
```

## Comparing `qdrant_haystack-1.0.3.tar` & `qdrant_haystack-1.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-06-09 11:42:00.938619 qdrant_haystack-1.0.3/LICENSE
--rw-r--r--   0        0        0     3160 2023-06-09 11:42:00.938619 qdrant_haystack-1.0.3/README.md
--rw-r--r--   0        0        0      764 2023-06-09 11:42:00.942620 qdrant_haystack-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      100 2023-06-09 11:42:00.942620 qdrant_haystack-1.0.3/src/qdrant_haystack/__init__.py
--rw-r--r--   0        0        0      107 2023-06-09 11:42:00.942620 qdrant_haystack-1.0.3/src/qdrant_haystack/document_stores/__init__.py
--rw-r--r--   0        0        0     2291 2023-06-09 11:42:00.942620 qdrant_haystack-1.0.3/src/qdrant_haystack/document_stores/converters.py
--rw-r--r--   0        0        0     8295 2023-06-09 11:42:00.942620 qdrant_haystack-1.0.3/src/qdrant_haystack/document_stores/filters.py
--rw-r--r--   0        0        0    20093 2023-06-09 11:42:00.942620 qdrant_haystack-1.0.3/src/qdrant_haystack/document_stores/qdrant.py
--rw-r--r--   0        0        0        0 2023-06-09 11:42:00.942620 qdrant_haystack-1.0.3/src/qdrant_haystack/utils.py
--rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 qdrant_haystack-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-26 16:33:42.874713 qdrant_haystack-1.0.4/LICENSE
+-rw-r--r--   0        0        0     3160 2023-06-26 16:33:42.874713 qdrant_haystack-1.0.4/README.md
+-rw-r--r--   0        0        0      764 2023-06-26 16:33:42.874713 qdrant_haystack-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-06-26 16:33:42.874713 qdrant_haystack-1.0.4/src/qdrant_haystack/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-26 16:33:42.874713 qdrant_haystack-1.0.4/src/qdrant_haystack/document_stores/__init__.py
+-rw-r--r--   0        0        0     2291 2023-06-26 16:33:42.874713 qdrant_haystack-1.0.4/src/qdrant_haystack/document_stores/converters.py
+-rw-r--r--   0        0        0     8295 2023-06-26 16:33:42.874713 qdrant_haystack-1.0.4/src/qdrant_haystack/document_stores/filters.py
+-rw-r--r--   0        0        0    20377 2023-06-26 16:33:42.874713 qdrant_haystack-1.0.4/src/qdrant_haystack/document_stores/qdrant.py
+-rw-r--r--   0        0        0        0 2023-06-26 16:33:42.874713 qdrant_haystack-1.0.4/src/qdrant_haystack/utils.py
+-rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 qdrant_haystack-1.0.4/PKG-INFO
```

### Comparing `qdrant_haystack-1.0.3/LICENSE` & `qdrant_haystack-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.3/README.md` & `qdrant_haystack-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.3/pyproject.toml` & `qdrant_haystack-1.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qdrant-haystack"
-version = "1.0.3"
+version = "1.0.4"
 description = "An integration of Qdrant ANN vector database backend with Haystack"
 authors = ["Kacper Łukawski <kacper.lukawski@qdrant.com>"]
 packages = [
     {include = "qdrant_haystack", from = "src"}
 ]
 readme = "README.md"
 license = "Apache 2.0"
```

### Comparing `qdrant_haystack-1.0.3/src/qdrant_haystack/document_stores/converters.py` & `qdrant_haystack-1.0.4/src/qdrant_haystack/document_stores/converters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.3/src/qdrant_haystack/document_stores/filters.py` & `qdrant_haystack-1.0.4/src/qdrant_haystack/document_stores/filters.py`

 * *Files identical despite different names*

### Comparing `qdrant_haystack-1.0.3/src/qdrant_haystack/document_stores/qdrant.py` & `qdrant_haystack-1.0.4/src/qdrant_haystack/document_stores/qdrant.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         write_consistency_factor: Optional[int] = None,
         on_disk_payload: Optional[bool] = None,
         hnsw_config: Optional[dict] = None,
         optimizers_config: Optional[dict] = None,
         wal_config: Optional[dict] = None,
         quantization_config: Optional[dict] = None,
         init_from: Optional[dict] = None,
+        wait_result_from_api: bool = True,
     ):
         super().__init__()
 
         self.client = qdrant_client.QdrantClient(
             location=location,
             url=url,
             port=port,
@@ -90,14 +91,15 @@
         self.write_consistency_factor = write_consistency_factor
         self.on_disk_payload = on_disk_payload
         self.hnsw_config = hnsw_config
         self.optimizers_config = optimizers_config
         self.wal_config = wal_config
         self.quantization_config = quantization_config
         self.init_from = init_from
+        self.wait_result_from_api = wait_result_from_api
 
         # Make sure the collection is properly set up
         self._set_up_collection(index, embedding_dim, recreate_index, similarity)
 
         self.embedding_dim = embedding_dim
         self.content_field = content_field
         self.name_field = name_field
@@ -310,14 +312,15 @@
                     field_map=self._create_document_field_map(),
                     fill_missing_embeddings=True,
                 )
 
                 response = self.client.upsert(
                     collection_name=index,
                     points=batch,
+                    wait=self.wait_result_from_api,
                 )
 
                 # TODO: handle errors in response
                 progress_bar.update(batch_size)
 
     def update_embeddings(
         self,
@@ -405,14 +408,15 @@
             embedding_field=self.embedding_field,
             embedding_dim=self.embedding_dim,
             field_map=self._create_document_field_map(),
         )
         self.client.upsert(
             collection_name=index,
             points=batch,
+            wait=self.wait_result_from_api,
         )
 
     def delete_documents(
         self,
         index: Optional[str] = None,
         ids: Optional[List[str]] = None,
         filters: Optional[FilterType] = None,
@@ -420,28 +424,30 @@
     ):
         index = index or self.index
         qdrant_filters = self.qdrant_filter_converter.convert(filters, ids)
 
         self.client.delete(
             collection_name=index,
             points_selector=qdrant_filters,
+            wait=self.wait_result_from_api,
         )
 
     def delete_all_documents(
         self,
         index: Optional[str] = None,
         filters: Optional[FilterType] = None,
         headers: Optional[Dict[str, str]] = None,
     ):
         index = index or self.index
         qdrant_filters = self.qdrant_filter_converter.convert(filters)
 
         self.client.delete(
             collection_name=index,
             points_selector=qdrant_filters,
+            wait=self.wait_result_from_api,
         )
 
     def delete_index(self, index: str):
         self.client.delete_collection(collection_name=index)
 
     def get_all_labels(
         self,
```

### Comparing `qdrant_haystack-1.0.3/PKG-INFO` & `qdrant_haystack-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdrant-haystack
-Version: 1.0.3
+Version: 1.0.4
 Summary: An integration of Qdrant ANN vector database backend with Haystack
 License: Apache 2.0
 Author: Kacper Łukawski
 Author-email: kacper.lukawski@qdrant.com
 Requires-Python: >=3.8.1,<=3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

