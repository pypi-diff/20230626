# Comparing `tmp/pypomes-0.1.3.tar.gz` & `tmp/pypomes-0.1.4.tar.gz`

## Comparing `pypomes-0.1.3.tar` & `pypomes-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pypomes-0.1.3/requirements.txt
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/__init__.py
--rw-r--r--   0        0        0     7701 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/azure_pomes.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/crypto_pomes.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/datetime_pomes.py
--rw-r--r--   0        0        0    12078 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/db_pomes.py
--rw-r--r--   0        0        0    27520 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/dict_pomes.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/encoding_pomes.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/env_pomes.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/exception_pomes.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/file_pomes.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/json_pomes.py
--rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/list_pomes.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/logging_pomes.py
--rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/minio_pomes.py
--rw-r--r--   0        0        0     7331 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/soap_pomes.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/str_pomes.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/xml_pomes.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pypomes-0.1.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.3/README.md
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pypomes-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pypomes-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pypomes-0.1.4/requirements.txt
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/__init__.py
+-rw-r--r--   0        0        0     7701 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/azure_pomes.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/crypto_pomes.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/datetime_pomes.py
+-rw-r--r--   0        0        0    12078 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/db_pomes.py
+-rw-r--r--   0        0        0    27520 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/dict_pomes.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/encoding_pomes.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/env_pomes.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/exception_pomes.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/file_pomes.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/json_pomes.py
+-rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/list_pomes.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/logging_pomes.py
+-rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/minio_pomes.py
+-rw-r--r--   0        0        0     7331 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/soap_pomes.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/str_pomes.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/xml_pomes.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pypomes-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes-0.1.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.4/README.md
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pypomes-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pypomes-0.1.4/PKG-INFO
```

### Comparing `pypomes-0.1.3/src/pypomes/__init__.py` & `pypomes-0.1.4/src/pypomes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+from .env_pomes import (
+    APP_PREFIX, env_get_str, env_get_int, env_get_bool, env_get_float
+)
+from .exception_pomes import (
+    exc_format
+)
+from .str_pomes import (
+    str_between, str_split_on_mark, str_find_whitespace
+)
 from .azure_pomes import (
     blob_exists, blob_retrieve, blob_store, blob_delete, blob_get_mimetype
 )
 from .crypto_pomes import (
     crypto_hash
 )
 from .datetime_pomes import (
@@ -18,20 +27,14 @@
     dict_has_key_chain, dict_get_value, dict_set_value, dict_reduce,
     dict_listify, dict_transform, dict_merge, dict_coalesce, dict_get_key,
     dict_get_keys, dict_from_object, dict_from_form, dict_from_list, dict_replace_value, dict_pop_value
 )
 from .encoding_pomes import (
     encode_ascii_hex, decode_ascii_hex
 )
-from .env_pomes import (
-    APP_PREFIX, env_get_str, env_get_int, env_get_bool, env_get_float
-)
-from .exception_pomes import (
-    exc_format
-)
 from .file_pomes import (
     file_from_request
 )
 from .json_pomes import (
     jsonify_dict, jsonify_iterable
 )
 from .list_pomes import (
@@ -46,22 +49,25 @@
     minio_access, minio_file_store, minio_object_store, minio_object_stat,
     minio_object_delete, minio_objects_list, minio_object_retrieve, minio_object_exists,
     minio_object_tags_retrieve, minio_file_retrieve, minio_setup
 )
 from .soap_pomes import (
     soap_post, soap_post_zeep, soap_get_attachment, soap_get_dict, soap_get_cids, soap_build_envelope
 )
-from .str_pomes import (
-    str_between, str_split_on_mark, str_find_whitespace
-)
 from .xml_pomes import (
     xml_to_dict, xml_normalize_keys
 )
 
 __all__ = [
+    # env_pomes
+    APP_PREFIX, env_get_str, env_get_int, env_get_bool, env_get_float,
+    # exception_pomes
+    exc_format,
+    # str_pomes
+    str_between, str_split_on_mark, str_find_whitespace,
     # azure_pomes
     blob_exists, blob_retrieve, blob_store, blob_delete, blob_get_mimetype,
     # crypto_pomes
     crypto_hash,
     # datetime_pomes
     DATE_FORMAT_STD, DATE_FORMAT_COMPACT, DATE_FORMAT_INV,
     DATETIME_FORMAT_STD, DATETIME_FORMAT_COMPACT, DATETIME_FORMAT_INV,
@@ -72,18 +78,14 @@
     db_select_all, db_select_one, db_row_to_dict, db_exec_stored_procedure,
     # dict_pomes
     dict_has_key_chain, dict_get_value, dict_set_value, dict_reduce,
     dict_listify, dict_transform, dict_merge, dict_coalesce, dict_get_key,
     dict_get_keys, dict_from_object, dict_from_form, dict_from_list, dict_replace_value, dict_pop_value,
     # encoding_pomes
     encode_ascii_hex, decode_ascii_hex,
-    # env_pomes
-    APP_PREFIX, env_get_str, env_get_int, env_get_bool, env_get_float,
-    # execption_pomes
-    exc_format,
     # file_pomes
     file_from_request,
     # json_pomes
     jsonify_dict, jsonify_iterable,
     # list_pomes
     list_transform, list_compare, list_flatten, list_unflatten,
     list_find_coupled, list_elem_starting_with, str_split_on_mark,
@@ -92,15 +94,13 @@
     # minio_pomes
     MINIO_BUCKET, MINIO_HOST, MINIO_ACCESS_KEY, MINIO_SECRET_KEY, MINIO_SECURE_ACCESS, MINIO_TEMP_PATH,
     minio_access, minio_file_store, minio_object_store, minio_object_stat,
     minio_object_delete, minio_objects_list, minio_object_retrieve, minio_object_exists,
     minio_object_tags_retrieve, minio_file_retrieve, minio_setup,
     # soap_pomes
     soap_post, soap_post_zeep, soap_get_attachment, soap_get_dict, soap_get_cids, soap_build_envelope,
-    # str_pomes
-    str_between, str_split_on_mark, str_find_whitespace,
     # xml_pomes
     xml_to_dict, xml_normalize_keys
 ]
 
-__version__ = "0.1.3"
-__version_info__ = (0, 1, 3)
+__version__ = "0.1.4"
+__version_info__ = (0, 1, 4)
```

### Comparing `pypomes-0.1.3/src/pypomes/azure_pomes.py` & `pypomes-0.1.4/src/pypomes/azure_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.3/src/pypomes/crypto_pomes.py` & `pypomes-0.1.4/src/pypomes/crypto_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.3/src/pypomes/datetime_pomes.py` & `pypomes-0.1.4/src/pypomes/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.3/src/pypomes/db_pomes.py` & `pypomes-0.1.4/src/pypomes/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.3/src/pypomes/dict_pomes.py` & `pypomes-0.1.4/src/pypomes/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.3/src/pypomes/encoding_pomes.py` & `pypomes-0.1.4/src/pypomes/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.3/src/pypomes/env_pomes.py` & `pypomes-0.1.4/src/pypomes/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.3/src/pypomes/exception_pomes.py` & `pypomes-0.1.4/src/pypomes/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.3/src/pypomes/file_pomes.py` & `pypomes-0.1.4/src/pypomes/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.3/src/pypomes/json_pomes.py` & `pypomes-0.1.4/src/pypomes/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.3/src/pypomes/list_pomes.py` & `pypomes-0.1.4/src/pypomes/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.3/src/pypomes/logging_pomes.py` & `pypomes-0.1.4/src/pypomes/logging_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.3/src/pypomes/minio_pomes.py` & `pypomes-0.1.4/src/pypomes/minio_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.3/src/pypomes/soap_pomes.py` & `pypomes-0.1.4/src/pypomes/soap_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.3/src/pypomes/str_pomes.py` & `pypomes-0.1.4/src/pypomes/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.3/src/pypomes/xml_pomes.py` & `pypomes-0.1.4/src/pypomes/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.3/LICENSE` & `pypomes-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.3/pyproject.toml` & `pypomes-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "xmltodict3>=0.0.4",
     "zeep>=4.2.1"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" },
 ]
 description = "A collection of Python pomes, pennyeach"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

