# Comparing `tmp/pypomes-0.1.4.tar.gz` & `tmp/pypomes-0.1.5.tar.gz`

## Comparing `pypomes-0.1.4.tar` & `pypomes-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pypomes-0.1.4/requirements.txt
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/__init__.py
--rw-r--r--   0        0        0     7701 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/azure_pomes.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/crypto_pomes.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/datetime_pomes.py
--rw-r--r--   0        0        0    12078 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/db_pomes.py
--rw-r--r--   0        0        0    27520 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/dict_pomes.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/encoding_pomes.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/env_pomes.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/exception_pomes.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/file_pomes.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/json_pomes.py
--rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/list_pomes.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/logging_pomes.py
--rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/minio_pomes.py
--rw-r--r--   0        0        0     7331 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/soap_pomes.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/str_pomes.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pypomes-0.1.4/src/pypomes/xml_pomes.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pypomes-0.1.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes-0.1.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.4/README.md
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pypomes-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pypomes-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pypomes-0.1.5/requirements.txt
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/__init__.py
+-rw-r--r--   0        0        0     7703 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/azure_pomes.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/crypto_pomes.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/datetime_pomes.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/db_pomes.py
+-rw-r--r--   0        0        0    27543 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/dict_pomes.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/encoding_pomes.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/env_pomes.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/exception_pomes.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/file_pomes.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/json_pomes.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/list_pomes.py
+-rw-r--r--   0        0        0     4667 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/logging_pomes.py
+-rw-r--r--   0        0        0    10458 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/minio_pomes.py
+-rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/soap_pomes.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/str_pomes.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/xml_pomes.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pypomes-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes-0.1.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.5/README.md
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pypomes-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pypomes-0.1.5/PKG-INFO
```

### Comparing `pypomes-0.1.4/src/pypomes/__init__.py` & `pypomes-0.1.5/src/pypomes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-from .env_pomes import (
-    APP_PREFIX, env_get_str, env_get_int, env_get_bool, env_get_float
-)
-from .exception_pomes import (
-    exc_format
-)
-from .str_pomes import (
-    str_between, str_split_on_mark, str_find_whitespace
-)
 from .azure_pomes import (
     blob_exists, blob_retrieve, blob_store, blob_delete, blob_get_mimetype
 )
 from .crypto_pomes import (
     crypto_hash
 )
 from .datetime_pomes import (
@@ -27,14 +18,20 @@
     dict_has_key_chain, dict_get_value, dict_set_value, dict_reduce,
     dict_listify, dict_transform, dict_merge, dict_coalesce, dict_get_key,
     dict_get_keys, dict_from_object, dict_from_form, dict_from_list, dict_replace_value, dict_pop_value
 )
 from .encoding_pomes import (
     encode_ascii_hex, decode_ascii_hex
 )
+from .env_pomes import (
+    APP_PREFIX, env_get_str, env_get_int, env_get_bool, env_get_float
+)
+from .exception_pomes import (
+    exc_format
+)
 from .file_pomes import (
     file_from_request
 )
 from .json_pomes import (
     jsonify_dict, jsonify_iterable
 )
 from .list_pomes import (
@@ -49,25 +46,22 @@
     minio_access, minio_file_store, minio_object_store, minio_object_stat,
     minio_object_delete, minio_objects_list, minio_object_retrieve, minio_object_exists,
     minio_object_tags_retrieve, minio_file_retrieve, minio_setup
 )
 from .soap_pomes import (
     soap_post, soap_post_zeep, soap_get_attachment, soap_get_dict, soap_get_cids, soap_build_envelope
 )
+from .str_pomes import (
+    str_between, str_split_on_mark, str_find_whitespace
+)
 from .xml_pomes import (
     xml_to_dict, xml_normalize_keys
 )
 
 __all__ = [
-    # env_pomes
-    APP_PREFIX, env_get_str, env_get_int, env_get_bool, env_get_float,
-    # exception_pomes
-    exc_format,
-    # str_pomes
-    str_between, str_split_on_mark, str_find_whitespace,
     # azure_pomes
     blob_exists, blob_retrieve, blob_store, blob_delete, blob_get_mimetype,
     # crypto_pomes
     crypto_hash,
     # datetime_pomes
     DATE_FORMAT_STD, DATE_FORMAT_COMPACT, DATE_FORMAT_INV,
     DATETIME_FORMAT_STD, DATETIME_FORMAT_COMPACT, DATETIME_FORMAT_INV,
@@ -78,14 +72,18 @@
     db_select_all, db_select_one, db_row_to_dict, db_exec_stored_procedure,
     # dict_pomes
     dict_has_key_chain, dict_get_value, dict_set_value, dict_reduce,
     dict_listify, dict_transform, dict_merge, dict_coalesce, dict_get_key,
     dict_get_keys, dict_from_object, dict_from_form, dict_from_list, dict_replace_value, dict_pop_value,
     # encoding_pomes
     encode_ascii_hex, decode_ascii_hex,
+    # env_pomes
+    APP_PREFIX, env_get_str, env_get_int, env_get_bool, env_get_float,
+    # exception_pomes
+    exc_format,
     # file_pomes
     file_from_request,
     # json_pomes
     jsonify_dict, jsonify_iterable,
     # list_pomes
     list_transform, list_compare, list_flatten, list_unflatten,
     list_find_coupled, list_elem_starting_with, str_split_on_mark,
@@ -94,13 +92,15 @@
     # minio_pomes
     MINIO_BUCKET, MINIO_HOST, MINIO_ACCESS_KEY, MINIO_SECRET_KEY, MINIO_SECURE_ACCESS, MINIO_TEMP_PATH,
     minio_access, minio_file_store, minio_object_store, minio_object_stat,
     minio_object_delete, minio_objects_list, minio_object_retrieve, minio_object_exists,
     minio_object_tags_retrieve, minio_file_retrieve, minio_setup,
     # soap_pomes
     soap_post, soap_post_zeep, soap_get_attachment, soap_get_dict, soap_get_cids, soap_build_envelope,
+    # str_pomes
+    str_between, str_split_on_mark, str_find_whitespace,
     # xml_pomes
     xml_to_dict, xml_normalize_keys
 ]
 
-__version__ = "0.1.4"
-__version_info__ = (0, 1, 4)
+__version__ = "0.1.5"
+__version_info__ = (0, 1, 5)
```

### Comparing `pypomes-0.1.4/src/pypomes/azure_pomes.py` & `pypomes-0.1.5/src/pypomes/azure_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from azure.storage.blob import BlobClient, BlobProperties
 from typing import Final
 import io
 import sys
-from env_pomes import APP_PREFIX, env_get_str
-from exception_pomes import exc_format
+from .env_pomes import APP_PREFIX, env_get_str
+from .exception_pomes import exc_format
 
 # string de conexão com o Azure
 AZURE_CONNECTION_STRING: Final[str] = env_get_str(f"{APP_PREFIX}_AZURE_CONNECTION_STRING")
 
 #  nome do bucket no armazenamento Azure
 AZURE_STORAGE_BUCKET: Final[str] = env_get_str(f"{APP_PREFIX}_AZURE_STORAGE_BUCKET")
```

### Comparing `pypomes-0.1.4/src/pypomes/crypto_pomes.py` & `pypomes-0.1.5/src/pypomes/crypto_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import hashlib
 import os
 from typing import Final
-from env_pomes import APP_PREFIX, env_get_str
+from .env_pomes import APP_PREFIX, env_get_str
 
 DEFAULT_HASH_ALGORITHM: Final[str] = env_get_str(f"{APP_PREFIX}_DEFAULT_HASH_ALGORITHM", "sha256")
 
 
 def crypto_hash(msg: str | bytes, alg: str = DEFAULT_HASH_ALGORITHM) -> bytes:
     """
     Compute the hash of *msg*, using the algorithm specified in *alg*.
```

### Comparing `pypomes-0.1.4/src/pypomes/datetime_pomes.py` & `pypomes-0.1.5/src/pypomes/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.4/src/pypomes/db_pomes.py` & `pypomes-0.1.5/src/pypomes/db_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # noinspection PyProtectedMember
 from pyodbc import connect, Connection, Row
 from typing import Final
-from env_pomes import APP_PREFIX, env_get_int, env_get_str
+from .env_pomes import APP_PREFIX, env_get_int, env_get_str
 
 # dados para acesso ao BD
 DB_DRIVER: Final[str] = env_get_str(f"{APP_PREFIX}_DB_DRIVER")
 DB_NAME: Final[str] = env_get_str(f"{APP_PREFIX}_DB_NAME")
 DB_HOST: Final[str] = env_get_str(f"{APP_PREFIX}_DB_HOST")
 DB_PORT: Final[int] = env_get_int(f"{APP_PREFIX}_DB_PORT")
 DB_PWD: Final[str] = env_get_str(f"{APP_PREFIX}_DB_PWD")
```

### Comparing `pypomes-0.1.4/src/pypomes/dict_pomes.py` & `pypomes-0.1.5/src/pypomes/dict_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from flask import Request
 import inspect
 import types
-import list_pomes
+from .list_pomes import list_find_coupled, list_transform, list_unflatten
 
 
 def dict_has_key_chain(source: dict, key_chain: list[str]) -> bool:
     """
     Indicate the existence of an element in *source* pointed to by the nested keys chain
     *[keys[0]: ... :keys[n]*. The path up to he last key in the chain must point to an existing element.
     A given key may indicate the element's position within a *list*, using the format *<key>[<pos>]*.
@@ -584,34 +584,34 @@
         # define a cadeia de chaves de origem
         if prefix_from is None:
             from_keys: str = key
         else:
             from_keys: str = f"{prefix_from}.{key}"
 
         # obtem a cadeia de chaves de destino
-        to_keys: str = list_pomes.list_find_coupled(from_to_keys, from_keys)
+        to_keys: str = list_find_coupled(from_to_keys, from_keys)
 
         # o destino foi definido ?
         if to_keys is not None:
             # sim, obtenha o valor de destino
             if isinstance(value, dict):
                 # valor é um dicionário, transforme-o
                 to_value: dict = dict_transform(value, from_to_keys, from_keys, to_keys)
             elif isinstance(value, list):
                 # valor é uma lista, transforme-a
-                to_value: list = list_pomes.list_transform(value, from_to_keys, from_keys, to_keys)
+                to_value: list = list_transform(value, from_to_keys, from_keys, to_keys)
             else:
                 # valor não é dicionário ou lista
                 to_value: any = value
 
             # o prefixo de destino foi definido e ocorre na cadeia de destino ?
             if prefix_to is not None and to_keys.startswith(prefix_to):
                 # sim, remova o prefixo
                 to_keys = to_keys[len(prefix_to)+1:]
-            to_keys_deep: list[str] = list_pomes.list_unflatten(to_keys)
+            to_keys_deep: list[str] = list_unflatten(to_keys)
 
             # atribui o valor transformado ao resultado
             dict_set_value(result, to_keys_deep, to_value)
 
     return result
```

### Comparing `pypomes-0.1.4/src/pypomes/encoding_pomes.py` & `pypomes-0.1.5/src/pypomes/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.4/src/pypomes/env_pomes.py` & `pypomes-0.1.5/src/pypomes/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.4/src/pypomes/exception_pomes.py` & `pypomes-0.1.5/src/pypomes/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.4/src/pypomes/file_pomes.py` & `pypomes-0.1.5/src/pypomes/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.4/src/pypomes/json_pomes.py` & `pypomes-0.1.5/src/pypomes/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.4/src/pypomes/list_pomes.py` & `pypomes-0.1.5/src/pypomes/list_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from str_pomes import str_split_on_mark
-from dict_pomes import dict_transform
+from .dict_pomes import dict_transform
+from .str_pomes import str_split_on_mark
 
 
 def list_compare(list1: list[any], list2: list[any]) -> bool:
     """
     Compare o conteúdo de duas listas *list1* e *list2*, e retorna *True* se todos os elementos de *list1*
     estão em *list2*, e vice-versa, na mesma quantidade.
```

### Comparing `pypomes-0.1.4/src/pypomes/logging_pomes.py` & `pypomes-0.1.5/src/pypomes/logging_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from datetime import datetime
 from dateutil import parser
 from io import BytesIO
 from typing import Final, TextIO
 import logging
 import os
 
-from datetime_pomes import DATETIME_FORMAT_INV
-from env_pomes import APP_PREFIX, env_get_str
+from .datetime_pomes import DATETIME_FORMAT_INV
+from .env_pomes import APP_PREFIX, env_get_str
 
 LOGGING_ID: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_ID")
 LOGGIN_FILE: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_FILE")
 
 # define and configure the logger
 PYPOMES_LOGGER: Final[logging.Logger] = logging.getLogger(LOGGING_ID)
```

### Comparing `pypomes-0.1.4/src/pypomes/minio_pomes.py` & `pypomes-0.1.5/src/pypomes/minio_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from minio import Minio
 from minio.datatypes import Object as MinioObject
 from minio.commonconfig import Tags
 from unidecode import unidecode
 import os
 import pickle
 import uuid
-from env_pomes import APP_PREFIX, env_get_bool, env_get_str
+from .env_pomes import APP_PREFIX, env_get_bool, env_get_str
 
 MINIO_BUCKET: Final[str] = env_get_str(f"{APP_PREFIX}_MINIO_BUCKET")
 MINIO_HOST: str = env_get_str(f"{APP_PREFIX}_MINIO_HOST")
 MINIO_ACCESS_KEY: str = env_get_str(f"{APP_PREFIX}_MINIO_ACCESS_KEY")
 MINIO_SECRET_KEY: str = env_get_str(f"{APP_PREFIX}_MINIO_SECRET_KEY")
 MINIO_SECURE_ACCESS: bool = env_get_bool(F"{APP_PREFIX}_MINIO_SECURE_ACCESS")
 MINIO_TEMP_PATH: str = env_get_str(F"{APP_PREFIX}_MINIO_TEMP_PATH")
```

### Comparing `pypomes-0.1.4/src/pypomes/soap_pomes.py` & `pypomes-0.1.5/src/pypomes/soap_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from lxml import etree
 from zeep import Client
 import ast
 import json
 import requests
 
-from json_pomes import jsonify_dict
-from xml_pomes import xml_to_dict
+from .json_pomes import jsonify_dict
+from .xml_pomes import xml_to_dict
 
 
 def soap_build_envelope(zeep_client: Client, service: str, payload: dict, file_path: str = None) -> bytes:
     """
     Constrói e retorna o envelope SOAP para um dado serviço. Esse envelope não contem os *headers*.
 
     :param zeep_client: o cliente zeep
```

### Comparing `pypomes-0.1.4/src/pypomes/str_pomes.py` & `pypomes-0.1.5/src/pypomes/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.4/src/pypomes/xml_pomes.py` & `pypomes-0.1.5/src/pypomes/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.4/LICENSE` & `pypomes-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.4/pyproject.toml` & `pypomes-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "xmltodict3>=0.0.4",
     "zeep>=4.2.1"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" },
 ]
 description = "A collection of Python pomes, pennyeach"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

