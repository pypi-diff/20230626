# Comparing `tmp/pypomes-0.1.2.tar.gz` & `tmp/pypomes-0.1.3.tar.gz`

## Comparing `pypomes-0.1.2.tar` & `pypomes-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pypomes-0.1.2/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/__init__.py
--rw-r--r--   0        0        0     7637 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/azure_pomes.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/crypto_pomes.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/datetime_pomes.py
--rw-r--r--   0        0        0    27531 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/dict_pomes.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/encoding_pomes.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/env_pomes.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/exception_pomes.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/file_pomes.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/json_pomes.py
--rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/list_pomes.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/logging_pomes.py
--rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/minio_pomes.py
--rw-r--r--   0        0        0    10963 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/postgres_pomes.py
--rw-r--r--   0        0        0     7331 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/soap_pomes.py
--rw-r--r--   0        0        0    12078 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/sqlserver_pomes.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/str_pomes.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pypomes-0.1.2/src/pypomes/xml_pomes.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pypomes-0.1.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.2/README.md
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 pypomes-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pypomes-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pypomes-0.1.3/requirements.txt
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/__init__.py
+-rw-r--r--   0        0        0     7701 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/azure_pomes.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/crypto_pomes.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/datetime_pomes.py
+-rw-r--r--   0        0        0    12078 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/db_pomes.py
+-rw-r--r--   0        0        0    27520 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/dict_pomes.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/encoding_pomes.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/env_pomes.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/exception_pomes.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/file_pomes.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/json_pomes.py
+-rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/list_pomes.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/logging_pomes.py
+-rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/minio_pomes.py
+-rw-r--r--   0        0        0     7331 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/soap_pomes.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/str_pomes.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pypomes-0.1.3/src/pypomes/xml_pomes.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pypomes-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes-0.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.3/README.md
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pypomes-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pypomes-0.1.3/PKG-INFO
```

### Comparing `pypomes-0.1.2/src/pypomes/azure_pomes.py` & `pypomes-0.1.3/src/pypomes/azure_pomes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from azure.storage.blob import BlobClient, BlobProperties # noqa
+from azure.storage.blob import BlobClient, BlobProperties
 from typing import Final
 import io
 import sys
 from env_pomes import APP_PREFIX, env_get_str
 from exception_pomes import exc_format
 
 # string de conexão com o Azure
@@ -166,46 +166,46 @@
     :return: A mensagem de erro formatada
     """
     # TODO
     return exc_format(exception, sys.exc_info())
 
 
 # testes do acesso ao Azure
-if __name__ == "__main__":
-
-    # print errors
-    def __print_errors(errors: list[str], op):
-        if len(errors) > 0:
-            print(f"\nErrors in '{op}':")
-            for error in errors:
-                print(error)
-
-    errors: list[str] = []
-    content: bytes = b"This is the content of a sample text file."
-    file_path: str = "/temp/sample.txt"
-
-    # testa a verificação de existência do arquivo
-    exists: bool = blob_exists(errors, file_path)
-    __print_errors(errors, "blob_exists")
-    assert exists is not None, "Failed verifying file"
-
-    # testa armazenamento de arquivo
-    if not exists:
-        success = blob_store(errors, content, file_path)
-        __print_errors(errors, "blob_store")
-        assert success, "Failed storing file"
-
-    # testa recuperação do tipo do arquivo
-    mimetype: str = blob_get_mimetype(errors, file_path)
-    __print_errors(errors, "blob_get_mimetype")
-    assert mimetype is not None, "Failed retrieving file mimetype"
-
-    # testa recuperação do conteúdo do arquivo
-    retrieved: bytes = blob_retrieve(errors, file_path)
-    __print_errors(errors, "blob_retrieve")
-    assert retrieved is not None, "Failed retrieving file content"
-    print(f"Conteudo recuperado: {content}")
-
-    # testa a exclusão do arquivo
-    success = blob_delete(errors, file_path)
-    __print_errors(errors, "blob_delete")
-    assert success, "Failed Deleting file"
+# if __name__ == "__main__":
+#
+#     # print errors
+#     def __print_errors(errors: list[str], op):
+#         if len(errors) > 0:
+#             print(f"\nErrors in '{op}':")
+#             for error in errors:
+#                 print(error)
+#
+#     errors: list[str] = []
+#     content: bytes = b"This is the content of a sample text file."
+#     file_path: str = "/temp/sample.txt"
+#
+#     # testa a verificação de existência do arquivo
+#     exists: bool = blob_exists(errors, file_path)
+#     __print_errors(errors, "blob_exists")
+#     assert exists is not None, "Failed verifying file"
+#
+#     # testa armazenamento de arquivo
+#     if not exists:
+#         success = blob_store(errors, content, file_path)
+#         __print_errors(errors, "blob_store")
+#         assert success, "Failed storing file"
+#
+#     # testa recuperação do tipo do arquivo
+#     mimetype: str = blob_get_mimetype(errors, file_path)
+#     __print_errors(errors, "blob_get_mimetype")
+#     assert mimetype is not None, "Failed retrieving file mimetype"
+#
+#     # testa recuperação do conteúdo do arquivo
+#     retrieved: bytes = blob_retrieve(errors, file_path)
+#     __print_errors(errors, "blob_retrieve")
+#     assert retrieved is not None, "Failed retrieving file content"
+#     print(f"Conteudo recuperado: {content}")
+#
+#     # testa a exclusão do arquivo
+#     success = blob_delete(errors, file_path)
+#     __print_errors(errors, "blob_delete")
+#     assert success, "Failed Deleting file"
```

### Comparing `pypomes-0.1.2/src/pypomes/crypto_pomes.py` & `pypomes-0.1.3/src/pypomes/crypto_pomes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import hashlib
 import os
 from typing import Final
-from env_pomes import env_get_str
+from env_pomes import APP_PREFIX, env_get_str
 
-DEFAULT_HASH_ALGORITHM: Final[str] = env_get_str("PYPOMES_DEFAULT_HASH_ALGORITHM", "sha256")
+DEFAULT_HASH_ALGORITHM: Final[str] = env_get_str(f"{APP_PREFIX}_DEFAULT_HASH_ALGORITHM", "sha256")
 
 
 def crypto_hash(msg: str | bytes, alg: str = DEFAULT_HASH_ALGORITHM) -> bytes:
     """
     Compute the hash of *msg*, using the algorithm specified in *alg*.
     Return *None* if computing the hash not possible.
```

### Comparing `pypomes-0.1.2/src/pypomes/datetime_pomes.py` & `pypomes-0.1.3/src/pypomes/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.2/src/pypomes/dict_pomes.py` & `pypomes-0.1.3/src/pypomes/dict_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,22 +50,21 @@
             result = key in parent
 
     return result
 
 
 def dict_get_value(source: dict, key_chain: list[str]) -> any:
     """
-    Obtem o valor do elemento de *source* apontado pela cadeia de chaves aninhadas *[keys[0]: ... :keys[n]*.
-    O caminho até a última chave deve apontar para elementos existentes. Uma chave pode indicar a
-    posição do elemento dentro de uma lista, utilizando para tanto o formato *<key>[<pos>]*.
-    Retorna *None* se o valor procurado não for encontrado.
-
-    Note que o retorno do valor *None* pode não ser indicativo da ausência do elemento em *source*,
-    uma vez que esse elemento pode existir com o próprio valor *None*. Para certificar-se disso, use
-    a operação *dict_has_value*.
+    Obtain the value of the element in *source* pointed to by the nested keys chain *[keys[0]: ... :keys[n]*.
+    The path up to the last key in the chain must point to an existing element.
+    A given key may indicate the element's position within a *list*, using the format *<key>[<pos>]*.
+    Return *None* if the sought after value is not found.
+    Note that returning *None* might not be indicative of the absence of the element in *source*,
+    since that element might exist therein with the value *None*. To determine whether this is the case,
+    use the operation *dict_has_value*.
 
     :param source: o dict de referência
     :param key_chain: a cadeia de chaves
     :return: o valor obtido
     """
     # inicializa a variável de retorno
     result: any = source
@@ -101,14 +100,15 @@
 
 
 def dict_set_value(target: dict, key_chain: list[str], value: any):
     """
     Atribui ao elemento de *source*, apontado pela cadeia de chaves aninhadas *[keys[0]: ... :keys[n]*,
     o valor *value*. Caso o elemento final não exista, será criado com o valor especificado.
     Os elementos intermediários, caso não existam, serão criados com o valor de um *dict* vazio.
+
     Uma chave pode indicar a posição do elemento dentro de uma lista, utilizando para tanto
     o formato *<key>[<pos>]*, e nesse caso, o elemento deve existir.
 
     :param target: o dict de referência
     :param key_chain: a cadeia de chaves
     :param value: o valor a ser atribuído ao elemento
     """
```

### Comparing `pypomes-0.1.2/src/pypomes/encoding_pomes.py` & `pypomes-0.1.3/src/pypomes/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.2/src/pypomes/env_pomes.py` & `pypomes-0.1.3/src/pypomes/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.2/src/pypomes/exception_pomes.py` & `pypomes-0.1.3/src/pypomes/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.2/src/pypomes/file_pomes.py` & `pypomes-0.1.3/src/pypomes/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.2/src/pypomes/json_pomes.py` & `pypomes-0.1.3/src/pypomes/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.2/src/pypomes/list_pomes.py` & `pypomes-0.1.3/src/pypomes/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.2/src/pypomes/logging_pomes.py` & `pypomes-0.1.3/src/pypomes/logging_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from datetime_pomes import DATETIME_FORMAT_INV
 from env_pomes import APP_PREFIX, env_get_str
 
 LOGGING_ID: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_ID")
 LOGGIN_FILE: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_FILE")
 
 # define and configure the logger
-PYPOME_LOGGER: Final[logging.Logger] = logging.getLogger(LOGGING_ID)
+PYPOMES_LOGGER: Final[logging.Logger] = logging.getLogger(LOGGING_ID)
 
 match env_get_str(f"{APP_PREFIX}_LOGGING_LEVEL"):
     case "debug":
         LOGGING_LEVEL: Final[int] = logging.DEBUG
     case "info":
         LOGGING_LEVEL: Final[int] = logging.INFO
     case "warn":
@@ -29,16 +29,16 @@
 logging.basicConfig(level=LOGGING_LEVEL,
                     filename=LOGGIN_FILE,
                     filemode="a",
                     datefmt=DATETIME_FORMAT_INV,
                     style="{",
                     format="{asctime} {levelname:1.1} {thread:5d} "
                            "{module:20.20} {funcName:20.20} {lineno:3d} {message}")
-for handler in logging.root.handlers:
-    handler.addFilter(logging.Filter(LOGGING_ID))
+for _handler in logging.root.handlers:
+    _handler.addFilter(logging.Filter(LOGGING_ID))
 
 
 def logging_entries(errors: list[str], log_level: str, log_from: str, log_to: str) -> BytesIO:
 
     def get_level(level: str) -> int:
 
         result: int | None
@@ -114,15 +114,15 @@
 
     :param errors: a lista de erros
     :param output_dev: dispositivo de saída onde o erro deve ser impresso
     """
     # percorre a lista de erros
     for error in errors:
         # escreve o erro no log
-        PYPOME_LOGGER.error(error)
+        PYPOMES_LOGGER.error(error)
 
         # o dispositivo de saída foi definido ?
         if output_dev is not None:
             # sim, escreva o erro nesse dispositivo
             output_dev.write(error)
 
             # o dispositivo de saída é 'stderr' ou 'stdout' ?
```

### Comparing `pypomes-0.1.2/src/pypomes/minio_pomes.py` & `pypomes-0.1.3/src/pypomes/minio_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.2/src/pypomes/postgres_pomes.py` & `pypomes-0.1.3/src/pypomes/db_pomes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-from psycopg2 import connect
 # noinspection PyProtectedMember
-from psycopg2._psycopg import connection
-import os
+from pyodbc import connect, Connection, Row
+from typing import Final
 from env_pomes import APP_PREFIX, env_get_int, env_get_str
 
 # dados para acesso ao BD
-DB_HOST: str = env_get_str(f"{APP_PREFIX}_DB_HOST")
-DB_PORT: int = env_get_int(f"{APP_PREFIX}_DB_PORT")
-DB_NAME: str = os.environ[f"{APP_PREFIX}_DB_NAME"]
-DB_USER: str = os.environ[f"{APP_PREFIX}_DB_USER"]
-DB_PWD: str = os.environ[f"{APP_PREFIX}_DB_PWD"]
+DB_DRIVER: Final[str] = env_get_str(f"{APP_PREFIX}_DB_DRIVER")
+DB_NAME: Final[str] = env_get_str(f"{APP_PREFIX}_DB_NAME")
+DB_HOST: Final[str] = env_get_str(f"{APP_PREFIX}_DB_HOST")
+DB_PORT: Final[int] = env_get_int(f"{APP_PREFIX}_DB_PORT")
+DB_PWD: Final[str] = env_get_str(f"{APP_PREFIX}_DB_PWD")
+DB_USER: Final[str] = env_get_str(f"{APP_PREFIX}_DB_USER")
 
+CONNECTION_KWARGS: Final[str] = f"DRIVER={{{DB_DRIVER}}};SERVER={DB_HOST},{DB_PORT};" \
+                                f"DATABASE={DB_NAME};UID={DB_USER};PWD={DB_PWD};TrustServerCertificate=yes;"
 
-def db_connect(errors: list[str]) -> connection:
+
+def db_connect(errors: list[str]) -> Connection:
     """
-    Obtem e retorna uma conexão ao banco de dados, ou *None* se a conexão não pode ser obtida.
+    Obtém e retorna uma conexão ao banco de dados, ou *None* se a conexão não pode ser obtida.
 
     :param errors: lista a ser apensada com mensagem apropriada, em caso de erro
     :return: a conexão ao banco de dados
     """
     # inicializa a variável de retorno
-    result: connection | None = None
+    result: Connection | None = None
 
-    # obtem a conexão com o BD
+    # Obtém a conexão com o BD
     try:
-        result = connect(host=DB_HOST,
-                         port=DB_PORT,
-                         database=DB_NAME,
-                         user=DB_USER,
-                         password=DB_PWD)
+        result = connect(CONNECTION_KWARGS)
     except Exception as e:
         errors.append(__db_except_msg(e))
 
     return result
 
 
 def db_exists(errors: list[str], table: str, where_attrs: list[str], where_vals: tuple) -> bool:
@@ -43,94 +42,112 @@
 
     :param errors: lista a ser apensada com mensagem apropriada, em caso de erro
     :param table: a tabela a ser pesquisada
     :param where_attrs: os atributos para a busca
     :param where_vals: lista de valores a serem atribuídos aos atributos
     :return: True se não houve erro, e se pelo menos uma tupla existir
     """
-    sel_stmt: str = f"SELECT * FROM {table}" # noqa
+    sel_stmt: str = f"SELECT * FROM {table}"  # noqa
     if len(where_attrs) > 0:
-        sel_stmt += " WHERE " + "".join(f"{attr} = %s AND " for attr in where_attrs)[0:-5]
+        sel_stmt += " WHERE " + "".join(f"{attr} = ? AND " for attr in where_attrs)[0:-5]
     rec: tuple = db_select_one(errors, sel_stmt, where_vals)
     result: bool = None if len(errors) > 0 else rec is not None
 
     return result
 
 
 def db_select_one(errors: list[str], sel_stmt: str,
                   where_vals: tuple, required: bool = False) -> tuple:
     """
     Busca no banco de dados e retorna a primeira tupla que satisfaça o comando de busca *sel_stmt*.
     O comando pode opcionalmente conter critérios de busca, com valores respectivos fornecidos
     em *where_vals*. A lista de valores para um atributo com a cláusula *IN* deve estar contida
-    em tupla específica. Na hipóteese de erro, ou se a busca resultar vazia, *None* é retornado.
+    em tupla específica. Na hipótese de erro, ou se a busca resultar vazia, *None* é retornado.
 
     :param errors: lista a ser apensada com mensagem apropriada, em caso de erro
     :param sel_stmt: comando SELECT para a busca
     :param where_vals: lista de valores a serem associados aos critérios de busca
     :param required: define se busca vazia deve ser considerada erro
     :return: tupla contendo o resultado da busca, ou None se houve erro ou se a busca resultar vazia
     """
     # inicializa a variável de retorno
     result: tuple | None = None
 
     exc: bool = False
     try:
-        with connect(host=DB_HOST,
-                     port=DB_PORT,
-                     database=DB_NAME,
-                     user=DB_USER,
-                     password=DB_PWD) as conn:
+        with connect(CONNECTION_KWARGS) as conn:
             # obtem o cursor e executa a operação
             with conn.cursor() as cursor:
-                sel_stmt += " LIMIT 1"
-                cursor.execute(query=f"{sel_stmt};",
-                               vars=where_vals)
+                sel_stmt = sel_stmt.replace("SELECT", "SELECT TOP 1")
+                cursor.execute(sel_stmt, where_vals)
                 # obtem a primeira tupla retornada pelo SELECT (None se nenhuma foi retornada)
                 result = cursor.fetchone()
     except Exception as e:
         exc = True
         errors.append(__db_except_msg(e))
 
-    # o parâmetro 'required' foi definido e nenhum registro foi obtido ?
+    # o parâmetro 'required' foi definido e nenhum registro foi obtido?
     if required and not exc and result is None:
         # sim, reporte o erro
         errors.append(__db_required_msg(sel_stmt, where_vals))
 
     return result
 
 
+def db_exec_stored_procedure(errors: list[str], nm_proced: str, param_vals: tuple) -> list[Row]:
+    """
+    Executa o stored procedure no banco de dados com os parâmetros informados e retorna os erros que ocorrerem
+
+    :param errors: lista a ser apensada com mensagem apropriada, em caso de erro
+    :param nm_proced: nome do stored procedure
+    :param param_vals: lista de valores dos parâmetros
+    :return: lista de tuplas contendo o resultado da busca, ou [] se a busca resultar vazia
+    """
+    # inicializa a variável de retorno
+    result: list[Row] = []
+
+    try:
+        with connect(CONNECTION_KWARGS) as conn:
+            # obtém o cursor e executa a operação
+            with conn.cursor() as cursor:
+                sql = f"SET NOCOUNT ON; EXEC {nm_proced} {','.join(('?',) * len(param_vals))}"
+                cursor.execute(sql, param_vals)
+                # obtem as tuplas retornadas
+                for record in cursor:
+                    result.append(record)
+
+    except Exception as e:
+        errors.append(__db_except_msg(e))
+
+    return result
+
+
 def db_select_all(errors: list[str], sel_stmt: str,
-                  where_vals: tuple, required: bool = False) -> list[tuple]:
+                  where_vals: tuple, required: bool = False) -> list[Row]:
     """
-    Busca no banco de dados e retorna todas as tuplas que satifaçam o comando de busca *sele_stmt*.
+    Busca no banco de dados e retorna todas as tuplas que satisfaçam o comando de busca *sele_stmt*.
     O comando pode opcionalmente conter critérios de busca, com valores respectivos fornecidos
     em *where_vals*. A lista de valores para um atributo com a cláusula *IN* deve estar contida
     em tupla específica. Se a busca resultar vazia, uma lista vazia é retornado.
 
     :param errors: lista a ser apensada com mensagem apropriada, em caso de erro
     :param sel_stmt: comando SELECT para a busca
     :param where_vals: lista de valores a serem associados aos critérios de busca
     :param required: define se busca vazia deve ser considerada erro
-    :return: lista de tuplas contendo o resultado da busca, ou []  se a busca resultar vazia
+    :return: lista de tuplas contendo o resultado da busca, ou [] se a busca resultar vazia
     """
     # inicializa a variável de retorno
-    result: list[tuple] = []
+    result: list[Row] = []
 
     exc: bool = False
     try:
-        with connect(host=DB_HOST,
-                     port=DB_PORT,
-                     database=DB_NAME,
-                     user=DB_USER,
-                     password=DB_PWD) as conn:
+        with connect(CONNECTION_KWARGS) as conn:
             # obtem o cursor e executa a operação
             with conn.cursor() as cursor:
-                cursor.execute(query=f"{sel_stmt};",
-                               vars=where_vals)
+                cursor.execute(sel_stmt, where_vals)
                 # obtem as tuplas retornadas
                 for record in cursor:
                     result.append(record)
     except Exception as e:
         exc = True
         errors.append(__db_except_msg(e))
 
@@ -141,115 +158,125 @@
 
     return result
 
 
 def db_insert(errors: list[str], insert_stmt: str, insert_vals: tuple) -> int:
     """
     Insere no banco de dados uma tupla com valores definidos em *insert_vals*.
+    Retorna o id da tupla inserida.
 
     :param errors: lista a ser apensada com mensagem apropriada, em caso de erro
     :param insert_stmt: comando INSERT
     :param insert_vals: lista de valores a serem inseridos
-    :return: o número de tuplas inseridas (0 ou 1), ou None em caso de erro
+    :return: o id da tupla inserida, ou None em caso de erro
     """
-    return __db_modify(errors, insert_stmt, insert_vals)
+    result: int | None = None
+    try:
+        with connect(CONNECTION_KWARGS) as conn:
+            with conn.cursor() as cursor:
+                insert_stmt = insert_stmt.replace("VALUES", "OUTPUT INSERTED.id VALUES")
+                cursor.execute(insert_stmt, insert_vals)
+                result = cursor.fetchone()[0]
+    except Exception as e:
+        errors.append(str(e))
+
+    return result
 
 
 def db_update(errors: list[str], update_stmt: str,
               update_vals: tuple, where_vals: tuple) -> int:
     """
     Atualiza uma ou mais tuplas no banco de dados, segundo as definições do comando
     *update_stmt*. Os valores para essa atualização estão em *update_vals*.
     Os valores para a seleção das tuplas a serem atualizadas estão em *where_vals*.
+    Retorna o número de tuplas modificadas.
 
     :param errors: lista a ser apensada com mensagem apropriada, em caso de erro
     :param update_stmt: comando UPDATE
     :param update_vals: lista de valores para a atualização
     :param where_vals: lista de valores para os critérios de seleção de tuplas
     :return: o número de tuplas atualizadas
     """
     values: tuple = update_vals + where_vals
     return __db_modify(errors, update_stmt, values)
 
 
 def db_delete(errors: list[str], delete_stmt: str, where_vals: tuple) -> int:
     """
     Exclui uma ou mais tuplas no banco de dados, segundo as definições do comando *delete_stmt*.
-    Os valores para a seleção das tuplas a serem excuídas estão em *where_vals*.
+    Os valores para a seleção das tuplas a serem excluídas estão em *where_vals*.
 
     :param errors: lista a ser apensada com mensagem apropriada, em caso de erro
     :param delete_stmt: comando DELETE
     :param where_vals: lista de valores para os critérios de seleção de tuplas
     :return: o número de tuplas excluídas
     """
     return __db_modify(errors, delete_stmt, where_vals)
 
 
-# modifica tabela no banco de dados e retorna o número de tuplas afetadas
+def db_row_to_dict(row):
+    """
+    Converts a pyodbc.Row object to a dictionary.
+
+    :param row: A pyodbc.Row object.
+    :return: A dictionary where keys are column names and values are the corresponding values in the row.
+    """
+    return {description[0]: row[i] for i, description in enumerate(row.cursor_description)}
+
+
 def __db_modify(errors: list[str], modify_stmt: str, bind_vals: tuple) -> int:
     """
     Modifica o banco de dados, inserindo, atualizando ou excluindo tuplas, segundo as
     definições do comando *modify_stmt*. Os valores para essa modificação, seguidos dos
     valores para a seleção das tuplas, estão em *bind_vals*.
 
     :param errors: lista a ser apensada com mensagem apropriada, em caso de erro
     :param modify_stmt: comando INSERT, UPDATE ou DELETE
     :param bind_vals: lista de valores para modificação e seleção de tuplas
     :return: o número de tuplas inseridas, atualizadas ou excluídas, ou None em caso de erro
     """
     result: int | None = None
 
     try:
-        with connect(host=DB_HOST,
-                     port=DB_PORT,
-                     database=DB_NAME,
-                     user=DB_USER,
-                     password=DB_PWD) as conn:
-            # obtem o sursor e executa a operação
+        with connect(CONNECTION_KWARGS) as conn:
+            # obtem o cursor e executa a operação
             with conn.cursor() as cursor:
-                cursor.execute(query=f"{modify_stmt};",
-                               vars=bind_vals)
+                cursor.execute(modify_stmt, bind_vals)
                 result = cursor.rowcount
                 conn.commit()
     except Exception as e:
         errors.append(__db_except_msg(e))
 
     return result
 
 
+# TODO
 def __db_except_msg(exception: Exception) -> str:
     """
     Formata e retorna a mensagem de erro correspondente à exceção levantada no acesso
     ao banco de dados.
 
-    :param exception: a exceção levantada
+    :param exception: A exceção levantada
     :return: A mensagem de erro formatada
     """
     exc_msg: str = f"{exception}"
-    pos: int = exc_msg.find("LINE 1")
-    if pos > 0:
-        exc_msg = exc_msg[:pos]
-    if hasattr(exception, "cursor") and hasattr(exception.cursor, "query"):
-        query: str = exception.cursor.query.decode()
-        exc_msg += f" ({query})"
-
     exc_msg = exc_msg.replace('"', "'") \
                      .replace('\n', " ") \
                      .replace('\t', " ") \
                      .replace("\\", "")
     result = f"Error accessing {DB_NAME} at {DB_HOST}: {exc_msg}"
 
     return result
 
 
 def __db_required_msg(sel_stmt: str, where_vals: tuple) -> str:
     """
     Formata e retorna a mensagem indicativa de busca vazia.
 
-    :param sel_stmt: o comando de busca utilizado
+    :param sel_stmt: O comando de busca utilizado
     :param where_vals: a lista de valores constituindo os critérios de busca
     :return: mensagem indicativa de busca vazia
     """
     stmt: str = sel_stmt.replace('"', "'") \
                         .replace('\n', " ") \
                         .replace('\t', " ") \
                         .replace("\\", "")
```

### Comparing `pypomes-0.1.2/src/pypomes/soap_pomes.py` & `pypomes-0.1.3/src/pypomes/soap_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.2/src/pypomes/str_pomes.py` & `pypomes-0.1.3/src/pypomes/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.2/src/pypomes/xml_pomes.py` & `pypomes-0.1.3/src/pypomes/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.2/LICENSE` & `pypomes-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.2/pyproject.toml` & `pypomes-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 [build-system]
 requires = [
     "hatchling",
     "asn1crypto>=1.5.1",
+    "azure-common>=1.1.28",
+    "azure-core>=1.26.4",
+    "azure-identity>=1.13.0",
+    "azure-storage-blob>=12.16.0",
     "cryptography>=41.0.1",
     "Flask>=2.3.2",
     "lxml>=4.9.2",
     "minio>=7.1.15",
     "psycopg2-binary>=2.9.6",
     "pyodbc>=4.0.39",
     "python-dateutil>=2.8.2",
     "requests>=2.31.0",
     "setuptools>=67.8.0",
     "Unidecode>=1.3.6",
+    "Werkzeug>=2.3.6",
     "wheel>=0.40.0",
     "xmltodict3>=0.0.4",
     "zeep>=4.2.1"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" },
 ]
 description = "A collection of Python pomes, pennyeach"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

