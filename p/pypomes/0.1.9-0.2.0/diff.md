# Comparing `tmp/pypomes-0.1.9.tar.gz` & `tmp/pypomes-0.2.0.tar.gz`

## Comparing `pypomes-0.1.9.tar` & `pypomes-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pypomes-0.1.9/requirements.txt
--rw-r--r--   0        0        0     4209 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/__init__.py
--rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/azure_pomes.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/crypto_pomes.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/datetime_pomes.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/db_pomes.py
--rw-r--r--   0        0        0    27585 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/dict_pomes.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/encoding_pomes.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/env_pomes.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/exception_pomes.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/file_pomes.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/json_pomes.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/list_pomes.py
--rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/logging_pomes.py
--rw-r--r--   0        0        0    10498 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/minio_pomes.py
--rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/soap_pomes.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/str_pomes.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pypomes-0.1.9/src/pypomes/xml_pomes.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pypomes-0.1.9/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes-0.1.9/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.9/README.md
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 pypomes-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pypomes-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 pypomes-0.2.0/requirements.txt
+-rw-r--r--   0        0        0     5354 2020-02-02 00:00:00.000000 pypomes-0.2.0/src/pypomes/__init__.py
+-rw-r--r--   0        0        0     7757 2020-02-02 00:00:00.000000 pypomes-0.2.0/src/pypomes/azure_pomes.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pypomes-0.2.0/src/pypomes/crypto_pomes.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes-0.2.0/src/pypomes/datetime_pomes.py
+-rw-r--r--   0        0        0    12131 2020-02-02 00:00:00.000000 pypomes-0.2.0/src/pypomes/db_pomes.py
+-rw-r--r--   0        0        0    27585 2020-02-02 00:00:00.000000 pypomes-0.2.0/src/pypomes/dict_pomes.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 pypomes-0.2.0/src/pypomes/email_pomes.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes-0.2.0/src/pypomes/encoding_pomes.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 pypomes-0.2.0/src/pypomes/env_pomes.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes-0.2.0/src/pypomes/exception_pomes.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes-0.2.0/src/pypomes/file_pomes.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes-0.2.0/src/pypomes/json_pomes.py
+-rw-r--r--   0        0        0    14123 2020-02-02 00:00:00.000000 pypomes-0.2.0/src/pypomes/ldap_pomes.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pypomes-0.2.0/src/pypomes/list_pomes.py
+-rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 pypomes-0.2.0/src/pypomes/logging_pomes.py
+-rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 pypomes-0.2.0/src/pypomes/minio_pomes.py
+-rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 pypomes-0.2.0/src/pypomes/soap_pomes.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes-0.2.0/src/pypomes/str_pomes.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pypomes-0.2.0/src/pypomes/xml_pomes.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pypomes-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes-0.2.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.2.0/README.md
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pypomes-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 pypomes-0.2.0/PKG-INFO
```

### Comparing `pypomes-0.1.9/src/pypomes/__init__.py` & `pypomes-0.2.0/src/pypomes/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .azure_pomes import (
+    AZURE_CONNECTION_STRING, AZURE_STORAGE_BUCKET,
     blob_exists, blob_retrieve, blob_store, blob_delete, blob_get_mimetype
 )
 from .crypto_pomes import (
-    crypto_hash
+    CRYPTO_HASH_ALGORITHM, crypto_hash
 )
 from .datetime_pomes import (
     DATE_FORMAT_STD, DATE_FORMAT_COMPACT, DATE_FORMAT_INV,
     DATETIME_FORMAT_STD, DATETIME_FORMAT_COMPACT, DATETIME_FORMAT_INV,
     date_reformat, date_parse, datetime_parse
 )
 from .db_pomes import (
@@ -15,14 +16,17 @@
     db_select_all, db_select_one, db_row_to_dict, db_exec_stored_procedure
 )
 from .dict_pomes import (
     dict_has_key_chain, dict_get_value, dict_set_value, dict_reduce,
     dict_listify, dict_transform, dict_merge, dict_coalesce, dict_get_key,
     dict_get_keys, dict_from_object, dict_from_form, dict_from_list, dict_replace_value, dict_pop_value
 )
+from .email_pomes import(
+    EMAIL_ACCOUNT, EMAIL_PWD, EMAIL_PORT, EMAIL_SERVER, email_send,
+)
 from .encoding_pomes import (
     encode_ascii_hex, decode_ascii_hex
 )
 from .env_pomes import (
     APP_PREFIX, env_get_str, env_get_int, env_get_bool, env_get_float
 )
 from .exception_pomes import (
@@ -30,14 +34,21 @@
 )
 from .file_pomes import (
     file_from_request
 )
 from .json_pomes import (
     jsonify_dict, jsonify_iterable
 )
+from .ldap_pomes import (
+    LDAP_BASE_DN, LDAP_BIND_DN, LDAP_BIND_PWD,
+    LDAP_SERVER_URI, LDAP_TIMEOUT, LDAP_TRACE_FILE, LDAP_TRACE_LEVEL,
+    ldap_init, ldap_bind, ldap_unbind, ldap_add_entry, ldap_search, ldap_delete_entry,
+    ldap_add_value, ldap_set_value, ldap_get_value, ldap_get_value_list, ldap_get_values,
+    ldap_get_values_lists, ldap_change_pwd, ldap_modify_user, ldap_modify_entry,
+)
 from .list_pomes import (
     list_compare, list_flatten, list_unflatten,
     list_find_coupled, list_elem_starting_with, list_transform,
 )
 from .logging_pomes import (
     LOGGING_ID, LOGGING_LEVEL, LOGGIN_FILE, LOGGING_MODE, PYPOMES_LOGGER,
     log_errors, logging_entries
@@ -56,42 +67,51 @@
 )
 from .xml_pomes import (
     xml_to_dict, xml_normalize_keys
 )
 
 __all__ = [
     # azure_pomes
+    AZURE_CONNECTION_STRING, AZURE_STORAGE_BUCKET,
     blob_exists, blob_retrieve, blob_store, blob_delete, blob_get_mimetype,
     # crypto_pomes
-    crypto_hash,
+    CRYPTO_HASH_ALGORITHM, crypto_hash,
     # datetime_pomes
     DATE_FORMAT_STD, DATE_FORMAT_COMPACT, DATE_FORMAT_INV,
     DATETIME_FORMAT_STD, DATETIME_FORMAT_COMPACT, DATETIME_FORMAT_INV,
     date_reformat, date_parse, datetime_parse,
     # db_pomes
     DB_HOST, DB_PWD, DB_NAME, DB_PORT, DB_USER, DB_DRIVER,
     db_delete, db_insert, db_update, db_connect, db_exists,
     db_select_all, db_select_one, db_row_to_dict, db_exec_stored_procedure,
     # dict_pomes
     dict_has_key_chain, dict_get_value, dict_set_value, dict_reduce,
     dict_listify, dict_transform, dict_merge, dict_coalesce, dict_get_key,
     dict_get_keys, dict_from_object, dict_from_form, dict_from_list, dict_replace_value, dict_pop_value,
+    # email_pomes
+    EMAIL_ACCOUNT, EMAIL_PWD, EMAIL_PORT, EMAIL_SERVER, email_send,
     # encoding_pomes
     encode_ascii_hex, decode_ascii_hex,
     # env_pomes
     APP_PREFIX, env_get_str, env_get_int, env_get_bool, env_get_float,
     # exception_pomes
     exc_format,
     # file_pomes
     file_from_request,
     # json_pomes
     jsonify_dict, jsonify_iterable,
     # list_pomes
     list_compare, list_flatten, list_unflatten,
     list_find_coupled, list_elem_starting_with, list_transform,
+    # ldap_pomes
+    LDAP_BASE_DN, LDAP_BIND_DN, LDAP_BIND_PWD,
+    LDAP_SERVER_URI, LDAP_TIMEOUT, LDAP_TRACE_FILE, LDAP_TRACE_LEVEL,
+    ldap_init, ldap_bind, ldap_unbind, ldap_add_entry, ldap_search, ldap_delete_entry,
+    ldap_add_value, ldap_set_value, ldap_get_value, ldap_get_value_list, ldap_get_values,
+    ldap_get_values_lists, ldap_change_pwd, ldap_modify_user, ldap_modify_entry,
     # logging_pomes
     LOGGING_ID, LOGGING_LEVEL, LOGGIN_FILE, LOGGING_MODE, PYPOMES_LOGGER,
     log_errors, logging_entries,
     # minio_pomes
     MINIO_BUCKET, MINIO_HOST, MINIO_ACCESS_KEY, MINIO_SECRET_KEY, MINIO_SECURE_ACCESS, MINIO_TEMP_PATH,
     minio_access, minio_file_store, minio_object_store, minio_object_stat,
     minio_object_delete, minio_objects_list, minio_object_retrieve, minio_object_exists,
@@ -100,9 +120,9 @@
     soap_post, soap_post_zeep, soap_get_attachment, soap_get_dict, soap_get_cids, soap_build_envelope,
     # str_pomes
     str_between, str_split_on_mark, str_find_whitespace,
     # xml_pomes
     xml_to_dict, xml_normalize_keys
 ]
 
-__version__ = "0.1.9"
-__version_info__ = (0, 1, 9)
+__version__ = "0.2.0"
+__version_info__ = (0, 2, 0)
```

### Comparing `pypomes-0.1.9/src/pypomes/azure_pomes.py` & `pypomes-0.2.0/src/pypomes/azure_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+# noinspection PyPackageRequirements
 from azure.storage.blob import BlobClient, BlobProperties
 from typing import Final
 import io
 import sys
 from .env_pomes import APP_PREFIX, env_get_str
 
 # string de conexão com o Azure
-AZURE_CONNECTION_STRING: Final[str] = env_get_str(f"{APP_PREFIX}_AZURE_CONNECTION_STRING")
+AZURE_CONNECTION_STRING: Final[str] = env_get_str(f"{APP_PREFIX}_AZURE_CONNECTION_STRING", None)
 
 #  nome do bucket no armazenamento Azure
-AZURE_STORAGE_BUCKET: Final[str] = env_get_str(f"{APP_PREFIX}_AZURE_STORAGE_BUCKET")
+AZURE_STORAGE_BUCKET: Final[str] = env_get_str(f"{APP_PREFIX}_AZURE_STORAGE_BUCKET", None)
 
 
 def blob_exists(errors: list[str], blob_path: str,
                 bucket_name: str = AZURE_STORAGE_BUCKET) -> bool:
     """
     Verifica a existência do arquivo apontado por *blob_path*, dentro de *bucket_name*.
```

### Comparing `pypomes-0.1.9/src/pypomes/crypto_pomes.py` & `pypomes-0.2.0/src/pypomes/crypto_pomes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import hashlib
 import os
 from typing import Final
 from .env_pomes import APP_PREFIX, env_get_str
 
-DEFAULT_HASH_ALGORITHM: Final[str] = env_get_str(f"{APP_PREFIX}_DEFAULT_HASH_ALGORITHM", "sha256")
+CRYPTO_HASH_ALGORITHM: Final[str] = env_get_str(f"{APP_PREFIX}_DEFAULT_HASH_ALGORITHM", "sha256")
 
 
-def crypto_hash(msg: str | bytes, alg: str = DEFAULT_HASH_ALGORITHM) -> bytes:
+def crypto_hash(msg: str | bytes, alg: str = CRYPTO_HASH_ALGORITHM) -> bytes:
     """
     Compute the hash of *msg*, using the algorithm specified in *alg*.
     Return *None* if computing the hash not possible.
 
     Supported algorithms: md5, blake2b, blake2s, sha1, sha224, sha256, sha384 sha512,
     sha3_224, sha3_256, sha3_384, sha3_512, shake_128, shake_256.
```

### Comparing `pypomes-0.1.9/src/pypomes/datetime_pomes.py` & `pypomes-0.2.0/src/pypomes/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.9/src/pypomes/db_pomes.py` & `pypomes-0.2.0/src/pypomes/db_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # noinspection PyProtectedMember
 from pyodbc import connect, Connection, Row
 from typing import Final
 from .env_pomes import APP_PREFIX, env_get_int, env_get_str
 
 # dados para acesso ao BD
-DB_DRIVER: Final[str] = env_get_str(f"{APP_PREFIX}_DB_DRIVER")
-DB_NAME: Final[str] = env_get_str(f"{APP_PREFIX}_DB_NAME")
-DB_HOST: Final[str] = env_get_str(f"{APP_PREFIX}_DB_HOST")
-DB_PORT: Final[int] = env_get_int(f"{APP_PREFIX}_DB_PORT")
-DB_PWD: Final[str] = env_get_str(f"{APP_PREFIX}_DB_PWD")
-DB_USER: Final[str] = env_get_str(f"{APP_PREFIX}_DB_USER")
+DB_DRIVER: Final[str] = env_get_str(f"{APP_PREFIX}_DB_DRIVER", None)
+DB_NAME: Final[str] = env_get_str(f"{APP_PREFIX}_DB_NAME", None)
+DB_HOST: Final[str] = env_get_str(f"{APP_PREFIX}_DB_HOST", None)
+DB_PORT: Final[int] = env_get_int(f"{APP_PREFIX}_DB_PORT", None)
+DB_PWD: Final[str] = env_get_str(f"{APP_PREFIX}_DB_PWD", None)
+DB_USER: Final[str] = env_get_str(f"{APP_PREFIX}_DB_USER", None)
 
-CONNECTION_KWARGS: Final[str] = f"DRIVER={{{DB_DRIVER}}};SERVER={DB_HOST},{DB_PORT};" \
-                                f"DATABASE={DB_NAME};UID={DB_USER};PWD={DB_PWD};TrustServerCertificate=yes;"
+__CONNECTION_KWARGS: Final[str] = f"DRIVER={{{DB_DRIVER}}};SERVER={DB_HOST},{DB_PORT};" \
+                                  f"DATABASE={DB_NAME};UID={DB_USER};PWD={DB_PWD};TrustServerCertificate=yes;"
 
 
 def db_connect(errors: list[str]) -> Connection:
     """
     Obtém e retorna uma conexão ao banco de dados, ou *None* se a conexão não pode ser obtida.
 
     :param errors: lista a ser apensada com mensagem apropriada, em caso de erro
     :return: a conexão ao banco de dados
     """
     # inicializa a variável de retorno
     result: Connection | None = None
 
     # Obtém a conexão com o BD
     try:
-        result = connect(CONNECTION_KWARGS)
+        result = connect(__CONNECTION_KWARGS)
     except Exception as e:
         errors.append(__db_except_msg(e))
 
     return result
 
 
 def db_exists(errors: list[str], table: str, where_attrs: list[str], where_vals: tuple) -> bool:
@@ -70,15 +70,15 @@
     :return: tupla contendo o resultado da busca, ou None se houve erro ou se a busca resultar vazia
     """
     # inicializa a variável de retorno
     result: tuple | None = None
 
     exc: bool = False
     try:
-        with connect(CONNECTION_KWARGS) as conn:
+        with connect(__CONNECTION_KWARGS) as conn:
             # obtem o cursor e executa a operação
             with conn.cursor() as cursor:
                 sel_stmt = sel_stmt.replace("SELECT", "SELECT TOP 1")
                 cursor.execute(sel_stmt, where_vals)
                 # obtem a primeira tupla retornada pelo SELECT (None se nenhuma foi retornada)
                 result = cursor.fetchone()
     except Exception as e:
@@ -102,15 +102,15 @@
     :param param_vals: lista de valores dos parâmetros
     :return: lista de tuplas contendo o resultado da busca, ou [] se a busca resultar vazia
     """
     # inicializa a variável de retorno
     result: list[Row] = []
 
     try:
-        with connect(CONNECTION_KWARGS) as conn:
+        with connect(__CONNECTION_KWARGS) as conn:
             # obtém o cursor e executa a operação
             with conn.cursor() as cursor:
                 sql = f"SET NOCOUNT ON; EXEC {nm_proced} {','.join(('?',) * len(param_vals))}"
                 cursor.execute(sql, param_vals)
                 # obtem as tuplas retornadas
                 for record in cursor:
                     result.append(record)
@@ -136,15 +136,15 @@
     :return: lista de tuplas contendo o resultado da busca, ou [] se a busca resultar vazia
     """
     # inicializa a variável de retorno
     result: list[Row] = []
 
     exc: bool = False
     try:
-        with connect(CONNECTION_KWARGS) as conn:
+        with connect(__CONNECTION_KWARGS) as conn:
             # obtem o cursor e executa a operação
             with conn.cursor() as cursor:
                 cursor.execute(sel_stmt, where_vals)
                 # obtem as tuplas retornadas
                 for record in cursor:
                     result.append(record)
     except Exception as e:
@@ -167,15 +167,15 @@
     :param errors: lista a ser apensada com mensagem apropriada, em caso de erro
     :param insert_stmt: comando INSERT
     :param insert_vals: lista de valores a serem inseridos
     :return: o id da tupla inserida, ou None em caso de erro
     """
     result: int | None = None
     try:
-        with connect(CONNECTION_KWARGS) as conn:
+        with connect(__CONNECTION_KWARGS) as conn:
             with conn.cursor() as cursor:
                 insert_stmt = insert_stmt.replace("VALUES", "OUTPUT INSERTED.id VALUES")
                 cursor.execute(insert_stmt, insert_vals)
                 result = cursor.fetchone()[0]
     except Exception as e:
         errors.append(str(e))
 
@@ -233,15 +233,15 @@
     :param modify_stmt: comando INSERT, UPDATE ou DELETE
     :param bind_vals: lista de valores para modificação e seleção de tuplas
     :return: o número de tuplas inseridas, atualizadas ou excluídas, ou None em caso de erro
     """
     result: int | None = None
 
     try:
-        with connect(CONNECTION_KWARGS) as conn:
+        with connect(__CONNECTION_KWARGS) as conn:
             # obtem o cursor e executa a operação
             with conn.cursor() as cursor:
                 cursor.execute(modify_stmt, bind_vals)
                 result = cursor.rowcount
                 conn.commit()
     except Exception as e:
         errors.append(__db_except_msg(e))
```

### Comparing `pypomes-0.1.9/src/pypomes/dict_pomes.py` & `pypomes-0.2.0/src/pypomes/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.9/src/pypomes/encoding_pomes.py` & `pypomes-0.2.0/src/pypomes/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.9/src/pypomes/env_pomes.py` & `pypomes-0.2.0/src/pypomes/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.9/src/pypomes/exception_pomes.py` & `pypomes-0.2.0/src/pypomes/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.9/src/pypomes/file_pomes.py` & `pypomes-0.2.0/src/pypomes/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.9/src/pypomes/json_pomes.py` & `pypomes-0.2.0/src/pypomes/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.9/src/pypomes/list_pomes.py` & `pypomes-0.2.0/src/pypomes/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.9/src/pypomes/logging_pomes.py` & `pypomes-0.2.0/src/pypomes/logging_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.9/src/pypomes/minio_pomes.py` & `pypomes-0.2.0/src/pypomes/minio_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from unidecode import unidecode
 import os
 import pickle
 import tempfile
 import uuid
 from .env_pomes import APP_PREFIX, env_get_bool, env_get_str
 
-MINIO_BUCKET: Final[str] = env_get_str(f"{APP_PREFIX}_MINIO_BUCKET")
-MINIO_HOST: str = env_get_str(f"{APP_PREFIX}_MINIO_HOST")
-MINIO_ACCESS_KEY: str = env_get_str(f"{APP_PREFIX}_MINIO_ACCESS_KEY")
-MINIO_SECRET_KEY: str = env_get_str(f"{APP_PREFIX}_MINIO_SECRET_KEY")
-MINIO_SECURE_ACCESS: bool = env_get_bool(F"{APP_PREFIX}_MINIO_SECURE_ACCESS")
-MINIO_TEMP_PATH: str = env_get_str(F"{APP_PREFIX}_MINIO_TEMP_PATH", tempfile.gettempdir())
+MINIO_BUCKET: Final[str] = env_get_str(f"{APP_PREFIX}_MINIO_BUCKET", None)
+MINIO_HOST: Final[str] = env_get_str(f"{APP_PREFIX}_MINIO_HOST", None)
+MINIO_ACCESS_KEY: Final[str] = env_get_str(f"{APP_PREFIX}_MINIO_ACCESS_KEY", None)
+MINIO_SECRET_KEY: Final[str] = env_get_str(f"{APP_PREFIX}_MINIO_SECRET_KEY", None)
+MINIO_SECURE_ACCESS: Final[bool] = env_get_bool(F"{APP_PREFIX}_MINIO_SECURE_ACCESS", None)
+MINIO_TEMP_PATH: Final[str] = env_get_str(F"{APP_PREFIX}_MINIO_TEMP_PATH", tempfile.gettempdir())
 
 
 def minio_setup(errors: list[str]) -> bool:
 
     result: bool = True
     try:
         # obtem o cliente MinIO
```

### Comparing `pypomes-0.1.9/src/pypomes/soap_pomes.py` & `pypomes-0.2.0/src/pypomes/soap_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.9/src/pypomes/str_pomes.py` & `pypomes-0.2.0/src/pypomes/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.9/src/pypomes/xml_pomes.py` & `pypomes-0.2.0/src/pypomes/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.9/LICENSE` & `pypomes-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.9/pyproject.toml` & `pypomes-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" },
 ]
 description = "A collection of Python pomes, pennyeach"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -27,18 +27,20 @@
     "cryptography>=41.0.1",
     "Flask>=2.3.2",
     "lxml>=4.9.2",
     "minio>=7.1.15",
     "psycopg2-binary>=2.9.6",
     "pyodbc>=4.0.39",
     "python-dateutil>=2.8.2",
+    "python-ldap>=3.4.0",
     "requests>=2.31.0",
     "setuptools>=67.8.0",
     "Unidecode>=1.3.6",
     "Werkzeug>=2.3.6",
     "wheel>=0.40.0",
     "xmltodict3>=0.0.4",
     "zeep>=4.2.1"
 ]
+
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes"
 "Bug Tracker" = "https://github.com/TheWiseCoder/PyPomes/issues"
```

### Comparing `pypomes-0.1.9/PKG-INFO` & `pypomes-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes
-Version: 0.1.9
+Version: 0.2.0
 Summary: A collection of Python pomes, pennyeach
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,15 @@
 Requires-Dist: cryptography>=41.0.1
 Requires-Dist: flask>=2.3.2
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: minio>=7.1.15
 Requires-Dist: psycopg2-binary>=2.9.6
 Requires-Dist: pyodbc>=4.0.39
 Requires-Dist: python-dateutil>=2.8.2
+Requires-Dist: python-ldap>=3.4.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: setuptools>=67.8.0
 Requires-Dist: unidecode>=1.3.6
 Requires-Dist: werkzeug>=2.3.6
 Requires-Dist: wheel>=0.40.0
 Requires-Dist: xmltodict3>=0.0.4
 Requires-Dist: zeep>=4.2.1
```

