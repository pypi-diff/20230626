# Comparing `tmp/layerx-sdk-beta-1.0.9b1.tar.gz` & `tmp/layerx-sdk-beta-1.0.9b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layerx-sdk-beta-1.0.9b1.tar", last modified: Mon Mar 20 05:08:25 2023, max compression
+gzip compressed data, was "layerx-sdk-beta-1.0.9b2.tar", last modified: Mon Mar 20 05:15:53 2023, max compression
```

## Comparing `layerx-sdk-beta-1.0.9b1.tar` & `layerx-sdk-beta-1.0.9b2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2023-03-20 05:08:25.914662 layerx-sdk-beta-1.0.9b1/
--rw-r--r--   0 chathushka   (501) staff       (20)     5555 2023-03-20 05:08:25.914002 layerx-sdk-beta-1.0.9b1/PKG-INFO
--rw-r--r--   0 chathushka   (501) staff       (20)     5022 2022-11-29 07:30:24.000000 layerx-sdk-beta-1.0.9b1/README.md
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2023-03-20 05:08:25.890953 layerx-sdk-beta-1.0.9b1/layerx/
--rw-r--r--   0 chathushka   (501) staff       (20)    37482 2023-03-20 05:05:14.000000 layerx-sdk-beta-1.0.9b1/layerx/__init__.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2023-03-20 05:08:25.899190 layerx-sdk-beta-1.0.9b1/layerx/datalake/
--rw-r--r--   0 chathushka   (501) staff       (20)     7151 2023-03-20 05:03:28.000000 layerx-sdk-beta-1.0.9b1/layerx/datalake/__init__.py
--rw-r--r--   0 chathushka   (501) staff       (20)     8868 2023-03-20 05:03:28.000000 layerx-sdk-beta-1.0.9b1/layerx/datalake/annotation.py
--rw-r--r--   0 chathushka   (501) staff       (20)      686 2023-03-07 08:39:00.000000 layerx-sdk-beta-1.0.9b1/layerx/datalake/constants.py
--rw-r--r--   0 chathushka   (501) staff       (20)    14963 2023-03-20 05:03:28.000000 layerx-sdk-beta-1.0.9b1/layerx/datalake/datalakeinterface.py
--rw-r--r--   0 chathushka   (501) staff       (20)        0 2022-11-29 07:30:24.000000 layerx-sdk-beta-1.0.9b1/layerx/datalake/dataset.py
--rw-r--r--   0 chathushka   (501) staff       (20)     7560 2023-03-07 08:39:00.000000 layerx-sdk-beta-1.0.9b1/layerx/datalake/file_upload.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1453 2023-03-20 05:03:28.000000 layerx-sdk-beta-1.0.9b1/layerx/datalake/ground_truth.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1078 2023-03-20 05:03:28.000000 layerx-sdk-beta-1.0.9b1/layerx/datalake/keys.py
--rw-r--r--   0 chathushka   (501) staff       (20)     3514 2022-11-29 07:30:24.000000 layerx-sdk-beta-1.0.9b1/layerx/datalake/label.py
--rw-r--r--   0 chathushka   (501) staff       (20)      417 2022-11-29 07:30:24.000000 layerx-sdk-beta-1.0.9b1/layerx/datalake/logger.py
--rw-r--r--   0 chathushka   (501) staff       (20)      810 2023-03-20 05:03:28.000000 layerx-sdk-beta-1.0.9b1/layerx/datalake/model_run.py
--rw-r--r--   0 chathushka   (501) staff       (20)     1273 2023-02-03 11:39:52.000000 layerx-sdk-beta-1.0.9b1/layerx/datalake/query.py
--rw-r--r--   0 chathushka   (501) staff       (20)      924 2022-12-06 05:45:43.000000 layerx-sdk-beta-1.0.9b1/layerx/datalake/s3_interface.py
--rw-r--r--   0 chathushka   (501) staff       (20)     2936 2022-12-06 05:45:43.000000 layerx-sdk-beta-1.0.9b1/layerx/datalake/s3_upload.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2023-03-20 05:08:25.906163 layerx-sdk-beta-1.0.9b1/layerx/dataset/
--rw-r--r--   0 chathushka   (501) staff       (20)     2544 2023-03-03 05:29:54.000000 layerx-sdk-beta-1.0.9b1/layerx/dataset/__init__.py
--rw-r--r--   0 chathushka   (501) staff       (20)     3142 2023-02-23 11:01:24.000000 layerx-sdk-beta-1.0.9b1/layerx/dataset/dataset.py
--rw-r--r--   0 chathushka   (501) staff       (20)     5402 2023-02-23 11:01:24.000000 layerx-sdk-beta-1.0.9b1/layerx/dataset/datasetinterface.py
--rw-r--r--   0 chathushka   (501) staff       (20)      417 2023-02-03 11:12:42.000000 layerx-sdk-beta-1.0.9b1/layerx/dataset/logger.py
--rw-r--r--   0 chathushka   (501) staff       (20)    15497 2023-03-20 05:03:28.000000 layerx-sdk-beta-1.0.9b1/layerx/dataset/sync.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2023-03-20 05:08:25.909164 layerx-sdk-beta-1.0.9b1/layerx/studio/
--rw-r--r--   0 chathushka   (501) staff       (20)     2552 2023-03-20 05:05:14.000000 layerx-sdk-beta-1.0.9b1/layerx/studio/__init__.py
--rw-r--r--   0 chathushka   (501) staff       (20)      417 2023-01-12 10:23:52.000000 layerx-sdk-beta-1.0.9b1/layerx/studio/logger.py
--rw-r--r--   0 chathushka   (501) staff       (20)     3435 2023-03-20 05:05:14.000000 layerx-sdk-beta-1.0.9b1/layerx/studio/project.py
--rw-r--r--   0 chathushka   (501) staff       (20)     4897 2023-02-03 10:20:11.000000 layerx-sdk-beta-1.0.9b1/layerx/studio/studiointerface.py
-drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2023-03-20 05:08:25.912984 layerx-sdk-beta-1.0.9b1/layerx_sdk_beta.egg-info/
--rw-r--r--   0 chathushka   (501) staff       (20)     5555 2023-03-20 05:08:25.000000 layerx-sdk-beta-1.0.9b1/layerx_sdk_beta.egg-info/PKG-INFO
--rw-r--r--   0 chathushka   (501) staff       (20)      879 2023-03-20 05:08:25.000000 layerx-sdk-beta-1.0.9b1/layerx_sdk_beta.egg-info/SOURCES.txt
--rw-r--r--   0 chathushka   (501) staff       (20)        1 2023-03-20 05:08:25.000000 layerx-sdk-beta-1.0.9b1/layerx_sdk_beta.egg-info/dependency_links.txt
--rw-r--r--   0 chathushka   (501) staff       (20)       28 2023-03-20 05:08:25.000000 layerx-sdk-beta-1.0.9b1/layerx_sdk_beta.egg-info/requires.txt
--rw-r--r--   0 chathushka   (501) staff       (20)        7 2023-03-20 05:08:25.000000 layerx-sdk-beta-1.0.9b1/layerx_sdk_beta.egg-info/top_level.txt
--rw-r--r--   0 chathushka   (501) staff       (20)       38 2023-03-20 05:08:25.915058 layerx-sdk-beta-1.0.9b1/setup.cfg
--rw-r--r--   0 chathushka   (501) staff       (20)     1176 2023-03-20 05:08:09.000000 layerx-sdk-beta-1.0.9b1/setup.py
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2023-03-20 05:15:53.888677 layerx-sdk-beta-1.0.9b2/
+-rw-r--r--   0 chathushka   (501) staff       (20)     5555 2023-03-20 05:15:53.888113 layerx-sdk-beta-1.0.9b2/PKG-INFO
+-rw-r--r--   0 chathushka   (501) staff       (20)     5022 2022-11-29 07:30:24.000000 layerx-sdk-beta-1.0.9b2/README.md
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2023-03-20 05:15:53.867839 layerx-sdk-beta-1.0.9b2/layerx/
+-rw-r--r--   0 chathushka   (501) staff       (20)    39154 2023-03-20 05:10:13.000000 layerx-sdk-beta-1.0.9b2/layerx/__init__.py
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2023-03-20 05:15:53.874840 layerx-sdk-beta-1.0.9b2/layerx/datalake/
+-rw-r--r--   0 chathushka   (501) staff       (20)     7321 2023-03-20 05:10:13.000000 layerx-sdk-beta-1.0.9b2/layerx/datalake/__init__.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     8968 2023-03-20 05:10:13.000000 layerx-sdk-beta-1.0.9b2/layerx/datalake/annotation.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      686 2023-03-07 08:39:00.000000 layerx-sdk-beta-1.0.9b2/layerx/datalake/constants.py
+-rw-r--r--   0 chathushka   (501) staff       (20)    15121 2023-03-20 05:10:13.000000 layerx-sdk-beta-1.0.9b2/layerx/datalake/datalakeinterface.py
+-rw-r--r--   0 chathushka   (501) staff       (20)        0 2022-11-29 07:30:24.000000 layerx-sdk-beta-1.0.9b2/layerx/datalake/dataset.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     7560 2023-03-07 08:39:00.000000 layerx-sdk-beta-1.0.9b2/layerx/datalake/file_upload.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     1516 2023-03-20 05:10:13.000000 layerx-sdk-beta-1.0.9b2/layerx/datalake/ground_truth.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     1119 2023-03-20 05:10:13.000000 layerx-sdk-beta-1.0.9b2/layerx/datalake/keys.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     3514 2022-11-29 07:30:24.000000 layerx-sdk-beta-1.0.9b2/layerx/datalake/label.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      417 2022-11-29 07:30:24.000000 layerx-sdk-beta-1.0.9b2/layerx/datalake/logger.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      849 2023-03-20 05:10:13.000000 layerx-sdk-beta-1.0.9b2/layerx/datalake/model_run.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     1273 2023-02-03 11:39:52.000000 layerx-sdk-beta-1.0.9b2/layerx/datalake/query.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      924 2022-12-06 05:45:43.000000 layerx-sdk-beta-1.0.9b2/layerx/datalake/s3_interface.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     2936 2022-12-06 05:45:43.000000 layerx-sdk-beta-1.0.9b2/layerx/datalake/s3_upload.py
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2023-03-20 05:15:53.878873 layerx-sdk-beta-1.0.9b2/layerx/dataset/
+-rw-r--r--   0 chathushka   (501) staff       (20)     2544 2023-03-03 05:29:54.000000 layerx-sdk-beta-1.0.9b2/layerx/dataset/__init__.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     3142 2023-02-23 11:01:24.000000 layerx-sdk-beta-1.0.9b2/layerx/dataset/dataset.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     5402 2023-02-23 11:01:24.000000 layerx-sdk-beta-1.0.9b2/layerx/dataset/datasetinterface.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      417 2023-02-03 11:12:42.000000 layerx-sdk-beta-1.0.9b2/layerx/dataset/logger.py
+-rw-r--r--   0 chathushka   (501) staff       (20)    15582 2023-03-20 05:10:13.000000 layerx-sdk-beta-1.0.9b2/layerx/dataset/sync.py
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2023-03-20 05:15:53.883081 layerx-sdk-beta-1.0.9b2/layerx/studio/
+-rw-r--r--   0 chathushka   (501) staff       (20)     2552 2023-03-20 05:05:14.000000 layerx-sdk-beta-1.0.9b2/layerx/studio/__init__.py
+-rw-r--r--   0 chathushka   (501) staff       (20)      417 2023-01-12 10:23:52.000000 layerx-sdk-beta-1.0.9b2/layerx/studio/logger.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     3435 2023-03-20 05:05:14.000000 layerx-sdk-beta-1.0.9b2/layerx/studio/project.py
+-rw-r--r--   0 chathushka   (501) staff       (20)     4897 2023-02-03 10:20:11.000000 layerx-sdk-beta-1.0.9b2/layerx/studio/studiointerface.py
+drwxr-xr-x   0 chathushka   (501) staff       (20)        0 2023-03-20 05:15:53.886495 layerx-sdk-beta-1.0.9b2/layerx_sdk_beta.egg-info/
+-rw-r--r--   0 chathushka   (501) staff       (20)     5555 2023-03-20 05:15:53.000000 layerx-sdk-beta-1.0.9b2/layerx_sdk_beta.egg-info/PKG-INFO
+-rw-r--r--   0 chathushka   (501) staff       (20)      879 2023-03-20 05:15:53.000000 layerx-sdk-beta-1.0.9b2/layerx_sdk_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 chathushka   (501) staff       (20)        1 2023-03-20 05:15:53.000000 layerx-sdk-beta-1.0.9b2/layerx_sdk_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 chathushka   (501) staff       (20)       28 2023-03-20 05:15:53.000000 layerx-sdk-beta-1.0.9b2/layerx_sdk_beta.egg-info/requires.txt
+-rw-r--r--   0 chathushka   (501) staff       (20)        7 2023-03-20 05:15:53.000000 layerx-sdk-beta-1.0.9b2/layerx_sdk_beta.egg-info/top_level.txt
+-rw-r--r--   0 chathushka   (501) staff       (20)       38 2023-03-20 05:15:53.888974 layerx-sdk-beta-1.0.9b2/setup.cfg
+-rw-r--r--   0 chathushka   (501) staff       (20)     1203 2023-03-20 05:11:17.000000 layerx-sdk-beta-1.0.9b2/setup.py
```

### Comparing `layerx-sdk-beta-1.0.9b1/PKG-INFO` & `layerx-sdk-beta-1.0.9b2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layerx-sdk-beta
-Version: 1.0.9b1
+Version: 1.0.9b2
 Summary: LayerX Python SDK
 Author: LayerX
 Author-email: <support@layerx.ai>
 Keywords: python,datalake,datasetsync,ai,annotation,layerx,machine learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `layerx-sdk-beta-1.0.9b1/README.md` & `layerx-sdk-beta-1.0.9b2/README.md`

 * *Files identical despite different names*

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/__init__.py` & `layerx-sdk-beta-1.0.9b2/layerx/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,54 +6,58 @@
 
 
 class LayerxClient:
     """
     Python SDK of LayerX
     """
 
-    def __init__(self, api_key: str, secret: str, layerx_url: str) -> None:
+    def __init__(self, api_key:str, secret: str, layerx_url: str) -> None:
         _string_key_secret = f'{api_key}:{secret}'
         _key_secret_bytes = _string_key_secret.encode("ascii")
         _encoded_key_secret_bytes = base64.b64encode(_key_secret_bytes)
         self.encoded_key_secret = _encoded_key_secret_bytes.decode("ascii")
         self.layerx_url = layerx_url
 
     def upload_annoations_for_folder(
             self,
             collection_base_path: str,
             operation_unique_id: str,
             json_data_file_path: str,
             shape_type: str,
             is_normalized: bool,
-            is_model_run: bool
+            is_model_run: bool,
+            destination_project_id: str = None
     ):
         """
         Upload annotation data from a json file
         """
         # init datalake client
         _datalake_client = datalake.DatalakeClient(self.encoded_key_secret, self.layerx_url)
 
         if is_model_run:
             _datalake_client.upload_modelrun_from_json(
                 collection_base_path,
                 operation_unique_id,
                 json_data_file_path,
                 shape_type,
-                is_normalized
+                is_normalized,
+                destination_project_id
             )
         else:
             _datalake_client.upload_groundtruth_from_json(
                 collection_base_path,
                 operation_unique_id,
                 json_data_file_path,
                 shape_type,
-                is_normalized)
+                is_normalized,
+                destination_project_id)
 
     """
-    Download dataset """
+    Download dataset 
+    """
 
     def download_dataset(self, version_id: str, export_type: str, custom_download_path: str = None):
         # init dataset client
         _dataset_client = dataset.DatasetClient(self.encoded_key_secret, self.layerx_url, custom_download_path)
 
         # start download
         _dataset_client.download_dataset(version_id, export_type)
@@ -93,37 +97,41 @@
                 "is_success": False,
                 "collection_id": None
             }
 
         return _datalake_client.file_upload(path, collection_type, collection_name, meta_data_object, False)
 
     """
-    Download collection annotations
-    From datalake
-    @param collection_id - id of dataset version
-    @param model_id - Optional: id of the model (same operation_id given in upload annotations) 
-    if we need annotations for that specific model """
-
+    Deprecated
+    Download collection annotations from datalake
+    @param collection_id - id of collection
+    @param operation_id - Optional: id of the model (same operation_id given in upload annotations) - default: None
+    @param custom_download_path - Optional: custom download path for save downloaded files - default: None
+    """
     def download_annotations(self, collection_id: str, operation_id, custom_download_path: str = None):
+
+        print('This method is now deprecated and please switch to "download_collection" function as this will be removed in future')
         # init dataset client
         _dataset_client = dataset.DatasetClient(self.encoded_key_secret, self.layerx_url, custom_download_path)
 
         operation_id_list = []
-        operation_id_list.append(operation_id)
+        if operation_id != None:
+            operation_id_list.append(operation_id)
         annotation_type = "all"
         # start download
         _dataset_client.download_annotations(collection_id, annotation_type, operation_id_list)
 
     
     """
-    Download collection annotations
-    From datalake
-    @param collection_id - id of dataset version
-    @param model_id - Optional: id of the model (same operation_id given in upload annotations) 
-    if we need annotations for that specific model """
+    Download collection annotations from datalake
+    @param collection_id - id of collection
+    @param annotation_type - Optional: annotation category, can be given ("machine", "human" or "all") - default: "all"
+    @param operation_id_list - Optional: id list of the model or ground truth (same operation_id_list given in upload annotations) - default: []
+    @param custom_download_path - Optional: custom download path for save downloaded files - default: None
+    """
 
     def download_collection(self, collection_id: str, annotation_type = "all", operation_id_list = [], custom_download_path: str = None):
         # init dataset client
         _dataset_client = dataset.DatasetClient(self.encoded_key_secret, self.layerx_url, custom_download_path)
 
         # start download
         _dataset_client.download_annotations(collection_id, annotation_type, operation_id_list)
@@ -620,15 +628,19 @@
     @param query - query for search objects
     @param filter - filter for filter objects - { 
         "annotation_types": ["human", "raw", "machine"], 
         "from_date": "", "to_date": "" 
     }
     @param object_type - object_type for search objects
     @param object_list - object_list for search objects
-    @param split_info - dataset split infromation
+    @param split_info - dataset split information - {
+            "train": number,
+            "test": number,
+            "validation": number
+        }
     @param labels - dataset selected labels
     @param export_types - dataset selected export types
     """
     def __create_dataset(
         self, 
         dataset_name: str, 
         collection_id: str, 
@@ -646,15 +658,15 @@
             return {
                 "is_success": False,
                 "error": "Invalid dataset name"
             }
         if object_type.lower() == "image":
             object_type = ObjectType.IMAGE.value
         elif object_type.lower() == "image_collection":
-            object_type = 0
+            object_type = ObjectType.IMAGE_COLLECTION.value
         elif object_type.lower() == "dataset":
             object_type = ObjectType.DATASET.value
         else:
             print("Invalid content type - should be either 'image'")
             return {
                 "is_success": False,
                 "collection_id": None
@@ -685,32 +697,36 @@
             }
 
 
     """
     create dataset from search objects on collection
     @param dataset_name - name of the dataset
     @param collection_id - collection_id for search objects
+    @param split_info - dataset split information - {
+            "train": number,
+            "test": number,
+            "validation": number
+        }
+    @param labels - dataset selected labels
+    @param export_types - dataset selected export types
     @param query - query for search objects
     @param filter - filter for filter objects - { 
         "annotation_types": ["human", "raw", "machine"], 
         "from_date": "", "to_date": "" 
     }
-    @param split_info - dataset split infromation
-    @param labels - dataset selected labels
-    @param export_types - dataset selected export types
     """
     def create_dataset_from_collection(
         self, 
         dataset_name: str, 
         collection_id: str, 
-        query: str, 
-        filter,  
         split_info, 
-        labels, 
-        export_types):
+        labels = [], 
+        export_types = [],
+        query: str = "", 
+        filter = {}):
 
         if(collection_id == None):
             return {
                 "isSuccess": False,
                 "error": 'collection id must be provided'
             }
 
@@ -722,86 +738,94 @@
         if object_type == None:
             print('object type cannot find for collection id')
             return {
                 "isSuccess": False,
                 "error": 'object type cannot find for collection id'
             }
         if object_type == ObjectType.IMAGE_COLLECTION.value:
-            object_type = "image_collection"
+            object_type = "image"
         else:
             return {
                 "isSuccess": False,
                 "error": 'collection type is not acceptable for create dataset, only image collections are valid'
             }
 
         self.__create_dataset(dataset_name, collection_id, query, filter, object_type, [], split_info, labels, export_types)
 
     
 
     """
     create dataset from search objects on datalake
     @param dataset_name - name of the dataset
+    @param split_info - dataset split information - {
+            "train": number,
+            "test": number,
+            "validation": number
+        }
+    @param labels - dataset selected labels
+    @param export_types - dataset selected export types
+    @param content_type - content_type for search objects
     @param query - query for search objects
     @param filter - filter for filter objects - { 
         "annotation_types": ["human", "raw", "machine"], 
         "from_date": "", "to_date": "" 
     }
-    @param content_type - content_type for search objects
-    @param split_info - dataset split infromation
-    @param labels - dataset selected labels
-    @param export_types - dataset selected export types
     """
     def create_dataset_from_datalake(
         self, 
-        dataset_name: str, 
-        query: str, 
-        filter, 
-        content_type, 
-        split_info, 
-        labels, 
-        export_types):
+        dataset_name: str,
+        split_info,
+        labels = [], 
+        export_types = [],
+        item_type = "image",
+        query: str = "", 
+        filter = {}):
             
-        self.__create_dataset(dataset_name, None, query, filter, content_type, [], split_info, labels, export_types)
+        self.__create_dataset(dataset_name, None, query, filter, item_type, [], split_info, labels, export_types)
 
     
 
     """
     update dataset from search objects
     @param version_id - id of the base version
     @param collection_id - collection_id for search objects
     @param query - query for search objects
     @param filter - filter for filter objects - { 
         "annotation_types": ["human", "raw", "machine"], 
         "from_date": "", "to_date": "" 
     }
     @param object_type - object_type for search objects
     @param object_list - object_list for search objects
-    @param split_info - dataset split infromation
+    @param split_info - dataset split information - {
+            "train": number,
+            "test": number,
+            "validation": number
+        }
     @param labels - dataset selected labels
     @param export_types - dataset selected export types
-    @param is_new_version_requried - whether creating new version (True) or update existing version (False)
+    @param is_new_version_required - whether creating new version (True) or update existing version (False)
     """
     def __update_dataset_version(
         self, 
         version_id: str, 
         collection_id: str, 
         query: str, 
         filter, 
         object_type, 
         object_list, 
         split_info, 
         labels, 
         export_types,
-        is_new_version_requried):
+        is_new_version_required):
         print(f'create dataset - dataset version id: {version_id}')
 
         if object_type.lower() == "image":
             object_type = ObjectType.IMAGE.value
         elif object_type.lower() == "image_collection":
-            object_type = 0
+            object_type = ObjectType.IMAGE_COLLECTION.value
         elif object_type.lower() == "dataset":
             object_type = ObjectType.DATASET.value
         else:
             print("Invalid content type - should be either 'image'")
             return {
                 "is_success": False
             }
@@ -815,15 +839,15 @@
         response = _datalake_client.get_selection_id(collection_id, query, filter, object_type, object_list)
         print('selection id: ',response)
         get_selection_id_success = True
         if("isSuccess" in response):
             if(response["isSuccess"] == False):
                 get_selection_id_success = False
         if get_selection_id_success == True:
-            dataset_response = _dataset_client.update_dataset_version(version_id, response['selectionTag'], split_info, labels, export_types, is_new_version_requried)
+            dataset_response = _dataset_client.update_dataset_version(version_id, response['selectionTag'], split_info, labels, export_types, is_new_version_required)
             print('dataset_response: ',dataset_response)
             return dataset_response
         else:
             print('dataset_response: ',{
                 "isSuccess": False
             })
             return {
@@ -831,34 +855,38 @@
             }
 
 
     """
     update dataset from search objects on collection
     @param version_id - id of the base version
     @param collection_id - collection_id for search objects
+    @param split_info - dataset split information - {
+            "train": number,
+            "test": number,
+            "validation": number
+        }
+    @param labels - dataset selected labels
+    @param export_types - dataset selected export types
     @param query - query for search objects
     @param filter - filter for filter objects - { 
         "annotation_types": ["human", "raw", "machine"], 
         "from_date": "", "to_date": "" 
     }
-    @param split_info - dataset split infromation
-    @param labels - dataset selected labels
-    @param export_types - dataset selected export types
-    @param is_new_version_requried - whether creating new version (True) or update existing version (False)
+    @param is_new_version_required - whether creating new version (True) or update existing version (False)
     """
     def update_dataset_version_from_collection(
         self, 
         version_id: str, 
         collection_id: str, 
-        query: str, 
-        filter,  
         split_info, 
-        labels, 
-        export_types,
-        is_new_version_requried):
+        labels = [], 
+        export_types = [],
+        query: str = "", 
+        filter = {},
+        is_new_version_required = False):
 
         if(collection_id == None or collection_id == ""):
             return {
                 "isSuccess": False,
                 "error": 'collection id must be provided'
             }
         if(version_id == None or version_id == ""):
@@ -875,56 +903,60 @@
         if object_type == None:
             print('object type cannot find for collection id')
             return {
                 "isSuccess": False,
                 "error": 'object type cannot find for collection id'
             }
         if object_type == ObjectType.IMAGE_COLLECTION.value:
-            object_type = "image_collection"
+            object_type = "image"
         else:
             return {
                 "isSuccess": False,
                 "error": 'collection type is not acceptable for create dataset, only image collections are valid'
             }
 
-        self.__update_dataset_version(version_id, collection_id, query, filter, object_type, [], split_info, labels, export_types, is_new_version_requried)
+        self.__update_dataset_version(version_id, collection_id, query, filter, object_type, [], split_info, labels, export_types, is_new_version_required)
 
     
 
     """
     update dataset from search objects on datalake
     @param version_id - id of the base version
+    @param split_info - dataset split information - {
+            "train": number,
+            "test": number,
+            "validation": number
+        }
+    @param labels - dataset selected labels
+    @param export_types - dataset selected export types
+    @param item_type - content_type for search objects
     @param query - query for search objects
     @param filter - filter for filter objects - { 
         "annotation_types": ["human", "raw", "machine"], 
         "from_date": "", "to_date": "" 
     }
-    @param content_type - content_type for search objects
-    @param split_info - dataset split infromation
-    @param labels - dataset selected labels
-    @param export_types - dataset selected export types
-    @param is_new_version_requried - whether creating new version (True) or update existing version (False)
+    @param is_new_version_required - whether creating new version (True) or update existing version (False)
     """
     def update_dataset_version_from_datalake(
         self, 
-        version_id: str, 
-        query: str, 
-        filter, 
-        content_type, 
+        version_id: str,  
         split_info, 
-        labels, 
-        export_types,
-        is_new_version_requried):
+        labels = [], 
+        export_types = [],
+        item_type: str = "image",
+        query: str = "", 
+        filter = {},
+        is_new_version_required = False):
         
         if(version_id == None or version_id == ""):
             return {
                 "isSuccess": False,
                 "error": 'version id must be provided'
             }
-        self.__update_dataset_version(version_id, None, query, filter, content_type, [], split_info, labels, export_types, is_new_version_requried)
+        self.__update_dataset_version(version_id, None, query, filter, item_type, [], split_info, labels, export_types, is_new_version_required)
 
     
 
     """
     delete dataset version
     @param version_id - id of the deleting version
     """
@@ -990,38 +1022,41 @@
     """
     def attach_label_group_to_annotation_project(self, project_id, group_id):
         _studio_client = studio.StudioClient(self.encoded_key_secret, self.layerx_url)
         return _studio_client.project_set_label_group(project_id, group_id)
 
 
     """
+    Deprecated
     Download project annotations
     @param project_id - id of annotation project
-    @param task_status_list - (Optional): To filter by task status
-    @param is_annotated_only - (Optional): If True, then only the annotated images are downloaded
-    @param custom_download_path - (Optional): To download data to required location instead of current directory
+    @param task_status_list - (Optional): To filter by task status - default: []
+    @param is_annotated_only - (Optional): If True, then only the annotated images are downloaded - default: False
+    @param custom_download_path - (Optional): To download data to required location instead of current directory - default: None
     """
 
     def download_project_annotations(self, project_id, task_status_list: list = [], is_annotated_only: bool = False, custom_download_path: str = None):
+
+        print('This method is now deprecated and please switch to "download_annotation_projects" function as this will be removed in future')
         # init dataset client
         _dataset_client = dataset.DatasetClient(self.encoded_key_secret, self.layerx_url, custom_download_path)
 
         project_id_list = []
         project_id_list.append(project_id)
         # start download
         _dataset_client.download_annotations_for_project_v2(project_id_list, task_status_list, is_annotated_only)
 
     
 
     """
-    Download project annotations
+    Download multiple project annotations
     @param project_id_list - id list of annotation projects
-    @param task_status_list - (Optional): To filter by task status
-    @param is_annotated_only - (Optional): If True, then only the annotated images are downloaded
-    @param custom_download_path - (Optional): To download data to required location instead of current directory
+    @param task_status_list - (Optional): To filter by task status - default: []
+    @param is_annotated_only - (Optional): If True, then only the annotated images are downloaded - default: False
+    @param custom_download_path - (Optional): To download data to required location instead of current directory - default: None
     """
 
     def download_annotation_projects(self, project_id_list, task_status_list: list = [], is_annotated_only: bool = False, custom_download_path: str = None):
 
         if task_status_list == None:
             task_status_list = []
 
@@ -1030,13 +1065,14 @@
 
         # start download
         _dataset_client.download_annotations_for_project_v2(project_id_list, task_status_list, is_annotated_only)
 
 
     
     """
-    wait untill job complete
+    Wait until job complete
+    @param job_id - id of the relevant job
     """
     def wait_for_job_complete(self, job_id: str):
         _datalake_client = datalake.DatalakeClient(self.encoded_key_secret, self.layerx_url)
         return _datalake_client.wait_for_job_complete(job_id)
```

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/datalake/__init__.py` & `layerx-sdk-beta-1.0.9b2/layerx/datalake/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,45 +33,47 @@
 
     def upload_modelrun_from_json(
             self,
             storage_base_path: str,
             model_id: str,
             file_path: str,
             annotation_geometry: str,
-            is_normalized: bool
+            is_normalized: bool,
+            dest_project_id: str
     ):
         datalake_logger.debug(f'upload_modelrun_from_json file_path={file_path}, '
                               f'annotation_geometry={annotation_geometry}')
         _model = ModelRun(client=self)
         if annotation_geometry == BOX_ANNOTATION:
-            _model.upload_modelrun_json(storage_base_path, model_id, file_path, BOX_ANNOTATION, is_normalized)
+            _model.upload_modelrun_json(storage_base_path, model_id, file_path, BOX_ANNOTATION, is_normalized, dest_project_id)
         elif annotation_geometry == POLYGON_ANNOTATION:
-            _model.upload_modelrun_json(storage_base_path, model_id, file_path, POLYGON_ANNOTATION, is_normalized)
+            _model.upload_modelrun_json(storage_base_path, model_id, file_path, POLYGON_ANNOTATION, is_normalized, dest_project_id)
         elif annotation_geometry == LINE_ANNOTATION:
-            _model.upload_modelrun_json(storage_base_path, model_id, file_path, LINE_ANNOTATION, is_normalized)
+            _model.upload_modelrun_json(storage_base_path, model_id, file_path, LINE_ANNOTATION, is_normalized, dest_project_id)
         else:
             datalake_logger.debug(f'unsupported annotation_geometry={annotation_geometry}')
 
     def upload_groundtruth_from_json(
             self,
             storage_base_path: str,
             operation_id: str,
             file_path: str,
             annotation_geometry: str,
-            is_normalized: bool
+            is_normalized: bool,
+            dest_project_id: str
     ):
         datalake_logger.debug(f'upload_groundtruth_from_json file_path={file_path}, '
                               f'annotation_geometry={annotation_geometry}')
         _groundTruth = GroundTruth(client=self)
         if annotation_geometry == BOX_ANNOTATION:
-            _groundTruth.upload_groundtruth_json(storage_base_path, operation_id, file_path, BOX_ANNOTATION, is_normalized)
+            _groundTruth.upload_groundtruth_json(storage_base_path, operation_id, file_path, BOX_ANNOTATION, is_normalized, dest_project_id)
         elif annotation_geometry == POLYGON_ANNOTATION:
-            _groundTruth.upload_groundtruth_json(storage_base_path, operation_id, file_path, POLYGON_ANNOTATION, is_normalized)
+            _groundTruth.upload_groundtruth_json(storage_base_path, operation_id, file_path, POLYGON_ANNOTATION, is_normalized, dest_project_id)
         elif annotation_geometry == LINE_ANNOTATION:
-            _groundTruth.upload_groundtruth_json(storage_base_path, operation_id, file_path, LINE_ANNOTATION, is_normalized)
+            _groundTruth.upload_groundtruth_json(storage_base_path, operation_id, file_path, LINE_ANNOTATION, is_normalized, dest_project_id)
         else:
             datalake_logger.debug(f'unsupported annotation_geometry={annotation_geometry}')
 
     def file_upload(self, path: str, collection_type, collection_name, meta_data_object, override):
         _upload = FileUpload(client=self)
         upload_res = _upload.file_upload_initiate(path, collection_type, collection_name, meta_data_object, override)
         return upload_res
```

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/datalake/annotation.py` & `layerx-sdk-beta-1.0.9b2/layerx/datalake/annotation.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,16 @@
     def upload_annotation_json(
             self,
             storage_base_path: str,
             operation_id: str,
             file_path: str,
             annotation_geometry: str,
             operation_mode: int,
-            is_normalized: bool
+            is_normalized: bool,
+            dest_project_id: str
     ):
 
         session_uuid = str(datetime.datetime.now().timestamp())
 
         # load json file
         f = open(file_path)
         annotation_data = json.load(f)
@@ -162,15 +163,16 @@
                     meta_updates_list,
                     OPERATION_TYPE_ANNOTATION,
                     operation_mode,
                     operation_id,
                     is_normalized,
                     session_uuid,
                     total_images_count,
-                    uploaded_images_count
+                    uploaded_images_count,
+                    dest_project_id
                 )
                 annotation_logger.debug(f'annotation data uploaded images count: {uploaded_images_count}')
 
                 meta_updates_list = []
 
         # call datalake operation data update API
         # this will handle final batch
@@ -180,15 +182,16 @@
             meta_updates_list,
             OPERATION_TYPE_ANNOTATION,
             operation_mode,
             operation_id,
             is_normalized,
             session_uuid,
             total_images_count,
-            uploaded_images_count
+            uploaded_images_count,
+            dest_project_id
         )
         annotation_logger.debug(f'annotation data uploaded images count: {uploaded_images_count}')
 
     def remove_collection_annotations(self, collection_id, model_run_id):
         session_uuid = str(datetime.datetime.now().timestamp())
         meta_update_response = self._client.datalake_interface.remove_modelrun_collection_annotation(collection_id, model_run_id, session_uuid)
         print('delete annotation status: ',meta_update_response)
```

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/datalake/constants.py` & `layerx-sdk-beta-1.0.9b2/layerx/datalake/constants.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/datalake/datalakeinterface.py` & `layerx-sdk-beta-1.0.9b2/layerx/datalake/datalakeinterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 
-from .keys import SESSION_ID, TOTAL_IMAGE_COUNT, UPLOADED_IMAGE_COUNT, USERNAME, LABELS, META_UPDATES_ARRAY, IS_NORMALIZED
+from .keys import DEST_PROJECT_ID, SESSION_ID, TOTAL_IMAGE_COUNT, UPLOADED_IMAGE_COUNT, USERNAME, LABELS, META_UPDATES_ARRAY, IS_NORMALIZED
 import requests
 
 
 class DatalakeInterface:
 
     def __init__(self, auth_token: str, dalalake_url: str):
         self.auth_token = auth_token
@@ -38,26 +38,29 @@
             response = requests.post(url=url, json=payload, headers=hed)
             return response.json()
         except requests.exceptions.RequestException as e:
             print("An exception occurred | find_datalake_label_references")
             print(e)
         
 
-    def upload_metadata_updates(self, meta_updates, operation_type, operation_mode, operation_id, is_normalized, session_id, total_images_count, uploaded_images_count):
+    def upload_metadata_updates(self, meta_updates, operation_type, operation_mode, operation_id, is_normalized, 
+                                session_id, total_images_count, uploaded_images_count, dest_project_id):
         hed = {'Authorization': 'Basic ' + self.auth_token}
         payload = {
             META_UPDATES_ARRAY: json.dumps(meta_updates),
             SESSION_ID : session_id,
             TOTAL_IMAGE_COUNT : total_images_count,
             UPLOADED_IMAGE_COUNT : uploaded_images_count
         }
 
         params = {
-            IS_NORMALIZED: is_normalized
+            IS_NORMALIZED: is_normalized,
         }
+        if dest_project_id != None:
+            params[DEST_PROJECT_ID] = dest_project_id
 
         url = f'{self.dalalake_url}/api/metadata/operationdata/{operation_type}/{operation_mode}/{operation_id}/update'
         print(url)
 
         try:
             response = requests.post(url=url, params=params, json=payload, headers=hed)
             return response.json()
```

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/datalake/file_upload.py` & `layerx-sdk-beta-1.0.9b2/layerx/datalake/file_upload.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/datalake/ground_truth.py` & `layerx-sdk-beta-1.0.9b2/layerx/datalake/ground_truth.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,24 +19,26 @@
 
     def upload_groundtruth_json(
             self,
             storage_base_path: str,
             operation_id: str,
             file_path: str,
             annotation_geometry: str,
-            is_normalized: bool
+            is_normalized: bool,
+            dest_project_id: str
     ):
         ground_truth_logger.debug(f'Started uploading ground truth data for model_id: {operation_id}')
         self.upload_annotation_json(
             storage_base_path,
             operation_id,
             file_path,
             annotation_geometry,
             OPERATION_MODE_HUMAN,
-            is_normalized
+            is_normalized,
+            dest_project_id
         )
         ground_truth_logger.debug(f'Finished uploading ground truth data for model_id: {operation_id}')
 
     def upload_coco(self, file_path: str):
         # load json file
         f = open(file_path)
         coco_data = json.load(f)
```

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/datalake/keys.py` & `layerx-sdk-beta-1.0.9b2/layerx/datalake/keys.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 COLOR = 'color'
 CONFIDENCE = 'confidence'
 DATA = 'data'
 DESCRIPTION = 'description'
 H = 'h'
 ID = 'id'
 IS_NORMALIZED = 'isNormalized'
+DEST_PROJECT_ID = 'destinationProjectId'
 IMAGE = 'image'
 IMAGES = 'images'
 IMG_FILES = 'imgFiles'
 IS_USER_ANNOTATED = 'isUserAnnotated'
 KEY = 'key'
 LABEL = 'label'
 LABEL_COLOR = 'labelColor'
```

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/datalake/label.py` & `layerx-sdk-beta-1.0.9b2/layerx/datalake/label.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/datalake/model_run.py` & `layerx-sdk-beta-1.0.9b2/layerx/datalake/model_run.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 model_logger = get_debug_logger('Model')
 
 
 class ModelRun(Annotation):
     def __init__(self, client: "DatalakeClient"):
         super().__init__(client)
 
-    def upload_modelrun_json(self, storage_base_path: str, model_id: str, file_path: str, annotation_geometry: str, is_normalized: bool):
+    def upload_modelrun_json(self, storage_base_path: str, model_id: str, file_path: str, annotation_geometry: str, is_normalized: bool, dest_project_id: str):
         model_logger.debug(f'Started uploading model run data for model_id: {model_id}')
-        self.upload_annotation_json(storage_base_path, model_id, file_path, annotation_geometry, OPERATION_MODE_AUTO, is_normalized)
+        self.upload_annotation_json(storage_base_path, model_id, file_path, annotation_geometry, OPERATION_MODE_AUTO, is_normalized, dest_project_id)
         model_logger.debug(f'Finished uploading model run data for model_id: {model_id}')
```

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/datalake/query.py` & `layerx-sdk-beta-1.0.9b2/layerx/datalake/query.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/datalake/s3_interface.py` & `layerx-sdk-beta-1.0.9b2/layerx/datalake/s3_interface.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/datalake/s3_upload.py` & `layerx-sdk-beta-1.0.9b2/layerx/datalake/s3_upload.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/dataset/__init__.py` & `layerx-sdk-beta-1.0.9b2/layerx/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/dataset/dataset.py` & `layerx-sdk-beta-1.0.9b2/layerx/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/dataset/datasetinterface.py` & `layerx-sdk-beta-1.0.9b2/layerx/dataset/datasetinterface.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/dataset/sync.py` & `layerx-sdk-beta-1.0.9b2/layerx/dataset/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,15 +245,15 @@
             self.json_file_name = response_data["rawFileName"]
             # Direct the response to download files
             self.initiate_download(response_data, page_no)
 
             # recursively call this again to get next page
             if(response_data['nextPage'] == True):
                 next_page_no = int(page_no)+1
-                self.get_all_pages(call_url, next_page_no)
+                self.get_all_pages(call_url, next_page_no, status_list, is_annotated_only, project_id_list, operation_id_list, annotation_type)
             print("Download Complete")
             if self.failed_downloads_present:
                 print(
                     "Unfortunately we failed to download everything, please retry to download missing items")
 
         else:
             print("No data recieved from remote for given group and/or version")
```

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/studio/__init__.py` & `layerx-sdk-beta-1.0.9b2/layerx/studio/__init__.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/studio/project.py` & `layerx-sdk-beta-1.0.9b2/layerx/studio/project.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-beta-1.0.9b1/layerx/studio/studiointerface.py` & `layerx-sdk-beta-1.0.9b2/layerx/studio/studiointerface.py`

 * *Files identical despite different names*

### Comparing `layerx-sdk-beta-1.0.9b1/layerx_sdk_beta.egg-info/PKG-INFO` & `layerx-sdk-beta-1.0.9b2/layerx_sdk_beta.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layerx-sdk-beta
-Version: 1.0.9b1
+Version: 1.0.9b2
 Summary: LayerX Python SDK
 Author: LayerX
 Author-email: <support@layerx.ai>
 Keywords: python,datalake,datasetsync,ai,annotation,layerx,machine learning
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `layerx-sdk-beta-1.0.9b1/layerx_sdk_beta.egg-info/SOURCES.txt` & `layerx-sdk-beta-1.0.9b2/layerx_sdk_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `layerx-sdk-beta-1.0.9b1/setup.py` & `layerx-sdk-beta-1.0.9b2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,35 @@
-from setuptools import setup, find_packages
 import codecs
 import os
 
+from setuptools import find_packages, setup
+
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.9-beta-1'
+VERSION = '1.0.9-beta-2'
 DESCRIPTION = 'LayerX Python SDK'
-LONG_DESCRIPTION = 'Python API Client to interact with layerx stack'
+LONG_DESCRIPTION = 'Python API Client to interact with LayerNext stack'
 
 # Setting up
 setup(
     name="layerx-sdk-beta",
     version=VERSION,
     author="LayerX",
     author_email="<support@layerx.ai>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
-    packages=find_packages(include=['layerx', 'layerx.datalake', 'layerx.dataset', 'layerx.studio']),
+    packages=find_packages(
+        include=['layerx', 'layerx.datalake', 'layerx.dataset', 'layerx.studio']),
     install_requires=['requests', 'uuid', 'python-dotenv'],
-    keywords=['python', 'datalake', 'datasetsync', 'ai', 'annotation', 'layerx', 'machine learning'],
+    keywords=['python', 'datalake', 'datasetsync', 'ai',
+              'annotation', 'layerx', 'machine learning'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

