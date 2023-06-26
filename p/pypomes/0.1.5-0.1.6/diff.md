# Comparing `tmp/pypomes-0.1.5.tar.gz` & `tmp/pypomes-0.1.6.tar.gz`

## Comparing `pypomes-0.1.5.tar` & `pypomes-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pypomes-0.1.5/requirements.txt
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/__init__.py
--rw-r--r--   0        0        0     7703 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/azure_pomes.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/crypto_pomes.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/datetime_pomes.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/db_pomes.py
--rw-r--r--   0        0        0    27543 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/dict_pomes.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/encoding_pomes.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/env_pomes.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/exception_pomes.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/file_pomes.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/json_pomes.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/list_pomes.py
--rw-r--r--   0        0        0     4667 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/logging_pomes.py
--rw-r--r--   0        0        0    10458 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/minio_pomes.py
--rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/soap_pomes.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/str_pomes.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pypomes-0.1.5/src/pypomes/xml_pomes.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pypomes-0.1.5/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes-0.1.5/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.5/README.md
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pypomes-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pypomes-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pypomes-0.1.6/requirements.txt
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/__init__.py
+-rw-r--r--   0        0        0     7707 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/azure_pomes.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/crypto_pomes.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/datetime_pomes.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/db_pomes.py
+-rw-r--r--   0        0        0    27585 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/dict_pomes.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/encoding_pomes.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/env_pomes.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/exception_pomes.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/file_pomes.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/json_pomes.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/list_pomes.py
+-rw-r--r--   0        0        0     4667 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/logging_pomes.py
+-rw-r--r--   0        0        0    10458 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/minio_pomes.py
+-rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/soap_pomes.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/str_pomes.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 pypomes-0.1.6/src/pypomes/xml_pomes.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 pypomes-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes-0.1.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes-0.1.6/README.md
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pypomes-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 pypomes-0.1.6/PKG-INFO
```

### Comparing `pypomes-0.1.5/src/pypomes/__init__.py` & `pypomes-0.1.6/src/pypomes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,9 +98,9 @@
     soap_post, soap_post_zeep, soap_get_attachment, soap_get_dict, soap_get_cids, soap_build_envelope,
     # str_pomes
     str_between, str_split_on_mark, str_find_whitespace,
     # xml_pomes
     xml_to_dict, xml_normalize_keys
 ]
 
-__version__ = "0.1.5"
-__version_info__ = (0, 1, 5)
+__version__ = "0.1.6"
+__version_info__ = (0, 1, 6)
```

### Comparing `pypomes-0.1.5/src/pypomes/azure_pomes.py` & `pypomes-0.1.6/src/pypomes/azure_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from azure.storage.blob import BlobClient, BlobProperties
 from typing import Final
 import io
 import sys
 from .env_pomes import APP_PREFIX, env_get_str
-from .exception_pomes import exc_format
 
 # string de conexão com o Azure
 AZURE_CONNECTION_STRING: Final[str] = env_get_str(f"{APP_PREFIX}_AZURE_CONNECTION_STRING")
 
 #  nome do bucket no armazenamento Azure
 AZURE_STORAGE_BUCKET: Final[str] = env_get_str(f"{APP_PREFIX}_AZURE_STORAGE_BUCKET")
 
@@ -162,14 +161,15 @@
     """
     Formata e retorna a mensagem de erro correspondente à exceção levantada no acesso ao Azure.
 
     :param exception: A exceção levantada
     :return: A mensagem de erro formatada
     """
     # TODO
+    from .exception_pomes import exc_format
     return exc_format(exception, sys.exc_info())
 
 
 # testes do acesso ao Azure
 # if __name__ == "__main__":
 #
 #     # print errors
```

### Comparing `pypomes-0.1.5/src/pypomes/crypto_pomes.py` & `pypomes-0.1.6/src/pypomes/crypto_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.5/src/pypomes/datetime_pomes.py` & `pypomes-0.1.6/src/pypomes/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.5/src/pypomes/db_pomes.py` & `pypomes-0.1.6/src/pypomes/db_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.5/src/pypomes/dict_pomes.py` & `pypomes-0.1.6/src/pypomes/dict_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from flask import Request
 import inspect
 import types
-from .list_pomes import list_find_coupled, list_transform, list_unflatten
 
 
 def dict_has_key_chain(source: dict, key_chain: list[str]) -> bool:
     """
     Indicate the existence of an element in *source* pointed to by the nested keys chain
     *[keys[0]: ... :keys[n]*. The path up to he last key in the chain must point to an existing element.
     A given key may indicate the element's position within a *list*, using the format *<key>[<pos>]*.
@@ -571,14 +570,17 @@
 
     :param source: o dict de origem dos valores
     :param from_to_keys: a lista de tuplas contendo as sequências de chaves de origem e destino
     :param prefix_from: prefixo a ser acrescentado às chaves de origem
     :param prefix_to: prefixo a ser removido das chaves de destino
     :return: o novo dicionário
     """
+    # import the neeeded functions
+    from .list_pomes import list_find_coupled, list_transform, list_unflatten
+
     # inicializa a variável de retorno
     result: dict = {}
 
     # percorre o dicionário de origem
     for key, value in source.items():
 
         # define a cadeia de chaves de origem
```

### Comparing `pypomes-0.1.5/src/pypomes/encoding_pomes.py` & `pypomes-0.1.6/src/pypomes/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.5/src/pypomes/env_pomes.py` & `pypomes-0.1.6/src/pypomes/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.5/src/pypomes/exception_pomes.py` & `pypomes-0.1.6/src/pypomes/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.5/src/pypomes/file_pomes.py` & `pypomes-0.1.6/src/pypomes/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.5/src/pypomes/json_pomes.py` & `pypomes-0.1.6/src/pypomes/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.5/src/pypomes/list_pomes.py` & `pypomes-0.1.6/src/pypomes/list_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from .dict_pomes import dict_transform
-from .str_pomes import str_split_on_mark
-
-
 def list_compare(list1: list[any], list2: list[any]) -> bool:
     """
     Compare o conteúdo de duas listas *list1* e *list2*, e retorna *True* se todos os elementos de *list1*
     estão em *list2*, e vice-versa, na mesma quantidade.
 
     :param list1: a primeira lista
     :param list2: a segunda lista
@@ -59,14 +55,17 @@
     - '.a.b'  -> ['', 'a', 'b']
     - 'x...y' -> ['x', '', '', 'y']
     - 'z'     -> ['z']
 
     :param source: string com elementos concatenados por "."
     :return: a lista de strings contendo os elementos da concatenação
     """
+    # import the needed function
+    from .str_pomes import str_split_on_mark
+
     return str_split_on_mark(source, ".")
 
 
 def list_find_coupled(coupled_elements: list[tuple[str, str]], primary_element: str) -> str:
     """
     Localiza em *coupled_elements* o elemento acoplado ao *primary_element* dado. Se *primary_element* contiver
     indicação de índice (denotado por *[<pos>]*), essa indicação é removida. Essa função é utilizada na transformação
@@ -111,14 +110,17 @@
     :param source: o dict de origem dos valores
     :param from_to_keys: a lista de tuplas contendo as sequências de chaves de origem e destino
     :param prefix_from: prefixo a ser acrescentado às chaves de origem
     :param prefix_to: prefixo a ser removido das chaves de destino
     :return: a nova lista
     """
 
+    # import the needed function
+    from .dict_pomes import dict_transform
+
     # inicializa a variável de retorno
     result: list[any] = []
 
     # percorre a lista de origem
     for inx, value in enumerate(source):
         if prefix_from is None:
             from_keys: None = None
```

### Comparing `pypomes-0.1.5/src/pypomes/logging_pomes.py` & `pypomes-0.1.6/src/pypomes/logging_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.5/src/pypomes/minio_pomes.py` & `pypomes-0.1.6/src/pypomes/minio_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.5/src/pypomes/soap_pomes.py` & `pypomes-0.1.6/src/pypomes/soap_pomes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from lxml import etree
 from zeep import Client
 import ast
 import json
 import requests
 
-from .json_pomes import jsonify_dict
-from .xml_pomes import xml_to_dict
-
 
 def soap_build_envelope(zeep_client: Client, service: str, payload: dict, file_path: str = None) -> bytes:
     """
     Constrói e retorna o envelope SOAP para um dado serviço. Esse envelope não contem os *headers*.
 
     :param zeep_client: o cliente zeep
     :param payload: os dados a serem enviados
@@ -71,14 +68,17 @@
     Encaminha a solicitação SOAP utilizando o pacote *zeep*, e retorna a resposta recebida.
 
     :param zeep_service: o serviço de referência
     :param payload: os dados a serem enviados
     :param file_path: Path to store the JSON corresponding to the returned response.
     :return: a resposta à solicitação
     """
+    # import the needed function
+    from .json_pomes import jsonify_dict
+
     # invoca o servico
     # ('response' é uma subclasse de dict - definida como retorno do 'zeep_service' no wsdl)
     response: any = zeep_service(**payload)
 
     # converte o conteúdo retornado em dict e o prepara para descarga em JSON
     result: dict = ast.literal_eval(str(response))
     jsonify_dict(result)
@@ -98,14 +98,18 @@
     Esse objeto é retornado em condições de ser descarregado em formato JSON.
 
     :param soap_response: o conteúdo retornado pela solicitação SOAP
     :param xml_path: Path to store the XML correspondinge to the returned response.
     :param json_path: Path to store the JSON correspondinge to the returned response.
     :return: o objeto com os dados de resposta à solicitação
     """
+    # import the needed functions
+    from .json_pomes import jsonify_dict
+    from .xml_pomes import xml_to_dict
+
     # restringe o conteúdo retornado ao conteúdo da tag soap:Body
     pos_1: int = soap_response.find(b"<soap:Body>") + 11
     pos_2: int = soap_response.find(b"</soap:Body>", pos_1)
     content: bytes = soap_response[pos_1:pos_2]
 
     # salva o conteúdo XML retornado em arquivo ?
     if xml_path is not None:
```

### Comparing `pypomes-0.1.5/src/pypomes/str_pomes.py` & `pypomes-0.1.6/src/pypomes/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.5/src/pypomes/xml_pomes.py` & `pypomes-0.1.6/src/pypomes/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.5/LICENSE` & `pypomes-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes-0.1.5/pyproject.toml` & `pypomes-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "xmltodict3>=0.0.4",
     "zeep>=4.2.1"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" },
 ]
 description = "A collection of Python pomes, pennyeach"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

