# Comparing `tmp/pypomes-0.1.6.tar.gz` & `tmp/pypomes-0.1.7.tar.gz`

## Comparing `pypomes-0.1.6.tar` & `pypomes-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pypomes-0.1.6/requirements.txt
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/__init__.py
--rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/azure_pomes.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/crypto_pomes.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/datetime_pomes.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/db_pomes.py
--rw-r--r--   0        0        0    27585 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/dict_pomes.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/encoding_pomes.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/env_pomes.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/exception_pomes.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/file_pomes.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/json_pomes.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/list_pomes.py
--rw-r--r--   0        0        0     4667 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/logging_pomes.py
--rw-r--r--   0        0        0    10458 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/minio_pomes.py
--rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/soap_pomes.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/str_pomes.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/xml_pomes.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pypomes-0.1.6/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes-0.1.6/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.6/README.md
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pypomes-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pypomes-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pypomes-0.1.7/requirements.txt
+-rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/__init__.py
+-rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/azure_pomes.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/crypto_pomes.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/datetime_pomes.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/db_pomes.py
+-rw-r--r--   0        0        0    27585 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/dict_pomes.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/encoding_pomes.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/env_pomes.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/exception_pomes.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/file_pomes.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/json_pomes.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/list_pomes.py
+-rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/logging_pomes.py
+-rw-r--r--   0        0        0    10498 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/minio_pomes.py
+-rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/soap_pomes.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/str_pomes.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pypomes-0.1.7/src/pypomes/xml_pomes.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pypomes-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes-0.1.7/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.7/README.md
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pypomes-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pypomes-0.1.7/PKG-INFO
```

### Comparing `pypomes-0.1.6/src/pypomes/__init__.py` & `pypomes-0.1.7/src/pypomes/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,20 @@
 from .file_pomes import (
     file_from_request
 )
 from .json_pomes import (
     jsonify_dict, jsonify_iterable
 )
 from .list_pomes import (
-    list_transform, list_compare, list_flatten, list_unflatten,
-    list_find_coupled, list_elem_starting_with, str_split_on_mark
+    list_compare, list_flatten, list_unflatten,
+    list_find_coupled, list_elem_starting_with, list_transform,
 )
 from .logging_pomes import (
-    LOGGING_ID, LOGGING_LEVEL, LOGGIN_FILE, PYPOMES_LOGGER, log_errors, logging_entries
+    LOGGING_ID, LOGGING_LEVEL, LOGGIN_FILE, LOGGING_MODE, PYPOMES_LOGGER,
+    log_errors, logging_entries
 )
 from .minio_pomes import (
     MINIO_BUCKET, MINIO_HOST, MINIO_ACCESS_KEY, MINIO_SECRET_KEY, MINIO_SECURE_ACCESS, MINIO_TEMP_PATH,
     minio_access, minio_file_store, minio_object_store, minio_object_stat,
     minio_object_delete, minio_objects_list, minio_object_retrieve, minio_object_exists,
     minio_object_tags_retrieve, minio_file_retrieve, minio_setup
 )
@@ -81,26 +82,27 @@
     # exception_pomes
     exc_format,
     # file_pomes
     file_from_request,
     # json_pomes
     jsonify_dict, jsonify_iterable,
     # list_pomes
-    list_transform, list_compare, list_flatten, list_unflatten,
-    list_find_coupled, list_elem_starting_with, str_split_on_mark,
+    list_compare, list_flatten, list_unflatten,
+    list_find_coupled, list_elem_starting_with, list_transform,
     # logging_pomes
-    LOGGING_ID, LOGGING_LEVEL, LOGGIN_FILE, PYPOMES_LOGGER, log_errors, logging_entries,
+    LOGGING_ID, LOGGING_LEVEL, LOGGIN_FILE, LOGGING_MODE, PYPOMES_LOGGER,
+    log_errors, logging_entries,
     # minio_pomes
     MINIO_BUCKET, MINIO_HOST, MINIO_ACCESS_KEY, MINIO_SECRET_KEY, MINIO_SECURE_ACCESS, MINIO_TEMP_PATH,
     minio_access, minio_file_store, minio_object_store, minio_object_stat,
     minio_object_delete, minio_objects_list, minio_object_retrieve, minio_object_exists,
     minio_object_tags_retrieve, minio_file_retrieve, minio_setup,
     # soap_pomes
     soap_post, soap_post_zeep, soap_get_attachment, soap_get_dict, soap_get_cids, soap_build_envelope,
     # str_pomes
     str_between, str_split_on_mark, str_find_whitespace,
     # xml_pomes
     xml_to_dict, xml_normalize_keys
 ]
 
-__version__ = "0.1.6"
-__version_info__ = (0, 1, 6)
+__version__ = "0.1.7"
+__version_info__ = (0, 1, 7)
```

### Comparing `pypomes-0.1.6/src/pypomes/azure_pomes.py` & `pypomes-0.1.7/src/pypomes/azure_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.6/src/pypomes/crypto_pomes.py` & `pypomes-0.1.7/src/pypomes/crypto_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.6/src/pypomes/datetime_pomes.py` & `pypomes-0.1.7/src/pypomes/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.6/src/pypomes/db_pomes.py` & `pypomes-0.1.7/src/pypomes/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.6/src/pypomes/dict_pomes.py` & `pypomes-0.1.7/src/pypomes/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.6/src/pypomes/encoding_pomes.py` & `pypomes-0.1.7/src/pypomes/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.6/src/pypomes/env_pomes.py` & `pypomes-0.1.7/src/pypomes/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.6/src/pypomes/exception_pomes.py` & `pypomes-0.1.7/src/pypomes/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.6/src/pypomes/file_pomes.py` & `pypomes-0.1.7/src/pypomes/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.6/src/pypomes/json_pomes.py` & `pypomes-0.1.7/src/pypomes/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.6/src/pypomes/list_pomes.py` & `pypomes-0.1.7/src/pypomes/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.6/src/pypomes/logging_pomes.py` & `pypomes-0.1.7/src/pypomes/logging_pomes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from datetime import datetime
 from dateutil import parser
 from io import BytesIO
 from typing import Final, TextIO
 import logging
 import os
+import tempfile
 
 from .datetime_pomes import DATETIME_FORMAT_INV
 from .env_pomes import APP_PREFIX, env_get_str
 
-LOGGING_ID: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_ID")
-LOGGIN_FILE: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_FILE")
+LOGGING_ID: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_ID", f"{APP_PREFIX}")
+LOGGIN_FILE: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_FILE",
+                                      os.path.join(tempfile.gettempdir(), f"{APP_PREFIX}.log"))
+LOGGING_MODE: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_MODE", "a")
 
 # define and configure the logger
 PYPOMES_LOGGER: Final[logging.Logger] = logging.getLogger(LOGGING_ID)
 
 match env_get_str(f"{APP_PREFIX}_LOGGING_LEVEL"):
     case "debug":
         LOGGING_LEVEL: Final[int] = logging.DEBUG
@@ -24,15 +27,15 @@
     case "error":
         LOGGING_LEVEL: Final[int] = logging.ERROR
     case _:  # "critical"
         LOGGING_LEVEL: Final[int] = logging.CRITICAL
 
 logging.basicConfig(level=LOGGING_LEVEL,
                     filename=LOGGIN_FILE,
-                    filemode="a",
+                    filemode=LOGGING_MODE,
                     datefmt=DATETIME_FORMAT_INV,
                     style="{",
                     format="{asctime} {levelname:1.1} {thread:5d} "
                            "{module:20.20} {funcName:20.20} {lineno:3d} {message}")
 for _handler in logging.root.handlers:
     _handler.addFilter(logging.Filter(LOGGING_ID))
```

### Comparing `pypomes-0.1.6/src/pypomes/minio_pomes.py` & `pypomes-0.1.7/src/pypomes/minio_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from typing import Final, Iterator
 from minio import Minio
 from minio.datatypes import Object as MinioObject
 from minio.commonconfig import Tags
 from unidecode import unidecode
 import os
 import pickle
+import tempfile
 import uuid
 from .env_pomes import APP_PREFIX, env_get_bool, env_get_str
 
 MINIO_BUCKET: Final[str] = env_get_str(f"{APP_PREFIX}_MINIO_BUCKET")
 MINIO_HOST: str = env_get_str(f"{APP_PREFIX}_MINIO_HOST")
 MINIO_ACCESS_KEY: str = env_get_str(f"{APP_PREFIX}_MINIO_ACCESS_KEY")
 MINIO_SECRET_KEY: str = env_get_str(f"{APP_PREFIX}_MINIO_SECRET_KEY")
 MINIO_SECURE_ACCESS: bool = env_get_bool(F"{APP_PREFIX}_MINIO_SECURE_ACCESS")
-MINIO_TEMP_PATH: str = env_get_str(F"{APP_PREFIX}_MINIO_TEMP_PATH")
+MINIO_TEMP_PATH: str = env_get_str(F"{APP_PREFIX}_MINIO_TEMP_PATH", tempfile.gettempdir())
 
 
 def minio_setup(errors: list[str]) -> bool:
 
     result: bool = True
     try:
         # obtem o cliente MinIO
```

### Comparing `pypomes-0.1.6/src/pypomes/soap_pomes.py` & `pypomes-0.1.7/src/pypomes/soap_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.6/src/pypomes/str_pomes.py` & `pypomes-0.1.7/src/pypomes/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.6/src/pypomes/xml_pomes.py` & `pypomes-0.1.7/src/pypomes/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.6/LICENSE` & `pypomes-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.6/pyproject.toml` & `pypomes-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "xmltodict3>=0.0.4",
     "zeep>=4.2.1"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" },
 ]
 description = "A collection of Python pomes, pennyeach"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

