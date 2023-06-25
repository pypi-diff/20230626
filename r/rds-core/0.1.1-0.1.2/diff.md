# Comparing `tmp/rds-core-0.1.1.tar.gz` & `tmp/rds-core-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rds-core-0.1.1.tar", last modified: Sun Jun 25 17:35:53 2023, max compression
+gzip compressed data, was "rds-core-0.1.2.tar", last modified: Sun Jun 25 23:00:54 2023, max compression
```

## Comparing `rds-core-0.1.1.tar` & `rds-core-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:35:53.117357 rds-core-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-25 17:35:35.000000 rds-core-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-25 17:35:53.117357 rds-core-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-25 17:35:35.000000 rds-core-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:35:53.113356 rds-core-0.1.1/rds_core/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-25 17:35:35.000000 rds-core-0.1.1/rds_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:35:53.113356 rds-core-0.1.1/rds_core/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-25 17:35:35.000000 rds-core-0.1.1/rds_core/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-06-25 17:35:35.000000 rds-core-0.1.1/rds_core/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-25 17:35:35.000000 rds-core-0.1.1/rds_core/cache/nocache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-25 17:35:35.000000 rds-core-0.1.1/rds_core/cache/search_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:35:53.117357 rds-core-0.1.1/rds_core/config/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-25 17:35:35.000000 rds-core-0.1.1/rds_core/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:35:53.117357 rds-core-0.1.1/rds_core/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-25 17:35:35.000000 rds-core-0.1.1/rds_core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-25 17:35:35.000000 rds-core-0.1.1/rds_core/helpers/cnes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-25 17:35:35.000000 rds-core-0.1.1/rds_core/helpers/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:35:53.117357 rds-core-0.1.1/rds_core/searchengine/
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-06-25 17:35:35.000000 rds-core-0.1.1/rds_core/searchengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:35:53.113356 rds-core-0.1.1/rds_core/transformers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:35:53.117357 rds-core-0.1.1/rds_core/transformers/fields/
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-25 17:35:35.000000 rds-core-0.1.1/rds_core/transformers/fields/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:35:53.117357 rds-core-0.1.1/rds_core/transformers/models/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-25 17:35:35.000000 rds-core-0.1.1/rds_core/transformers/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:35:53.113356 rds-core-0.1.1/rds_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-25 17:35:53.000000 rds-core-0.1.1/rds_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-25 17:35:53.000000 rds-core-0.1.1/rds_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:35:53.000000 rds-core-0.1.1/rds_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-25 17:35:53.000000 rds-core-0.1.1/rds_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 17:35:53.000000 rds-core-0.1.1/rds_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-25 17:35:53.117357 rds-core-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-25 17:35:35.000000 rds-core-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-25 23:00:35.000000 rds-core-0.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-25 23:00:54.301707 rds-core-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-25 23:00:35.000000 rds-core-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/rds_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/rds_core/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/cache/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/cache/search_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/rds_core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/rds_core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/helpers/cnes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/helpers/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/rds_core/searchengine/
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/searchengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/rds_core/transformers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/rds_core/transformers/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/transformers/fields/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/rds_core/transformers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-25 23:00:35.000000 rds-core-0.1.2/rds_core/transformers/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 23:00:54.301707 rds-core-0.1.2/rds_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-25 23:00:54.000000 rds-core-0.1.2/rds_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-25 23:00:54.000000 rds-core-0.1.2/rds_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 23:00:54.000000 rds-core-0.1.2/rds_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-25 23:00:54.000000 rds-core-0.1.2/rds_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 23:00:54.000000 rds-core-0.1.2/rds_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-25 23:00:54.301707 rds-core-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-25 23:00:35.000000 rds-core-0.1.2/setup.py
```

### Comparing `rds-core-0.1.1/PKG-INFO` & `rds-core-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: rds-core
-Version: 0.1.1
+Version: 0.1.2
 Summary: Framework para serviços do Rede de Dados em Saúde do LAIS
 Home-page: https://github.com/lais-huol/rds-core
 Author: Kelson da Costa Medeiros
 Author-email: kelson.medeiros@lais.huol.ufrn.br
 License: UNKNOWN
 Download-URL: https://github.com/lais-huol/rds-core/tags
+Description: É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias RDS, a exemplo RDS-RN e RDS-ES.
 Keywords: rds,cache,config,helper,searchengine
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.9
-License-File: LICENSE.md
-
-É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias RDS, a exemplo RDS-RN e RDS-ES.
-
+Requires-Python: >=3.8
```

### Comparing `rds-core-0.1.1/README.md` & `rds-core-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rds-core-0.1.1/rds_core/cache/__init__.py` & `rds-core-0.1.2/rds_core/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.1.1/rds_core/cache/base.py` & `rds-core-0.1.2/rds_core/cache/base.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.1.1/rds_core/cache/nocache.py` & `rds-core-0.1.2/rds_core/cache/nocache.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.1.1/rds_core/cache/search_engine.py` & `rds-core-0.1.2/rds_core/cache/search_engine.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.1.1/rds_core/helpers/__init__.py` & `rds-core-0.1.2/rds_core/helpers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,20 @@
         return v.lower() in TRUE_STRS
 
     raise ValueError("Boolean value expected.")
 
 
 def env(name, default=None, wrapped=False):
     result = getenv(name, default)
-    if wrapped and isinstance(result, str) and result[0:1] == "'" and result[-1:] == "'":
+    if (
+        wrapped
+        and isinstance(result, str)
+        and result[0:1] == "'"
+        and result[-1:] == "'"
+    ):
         return result[1:-1]
     return result
 
 
 def env_as_list(name, default="", delimiter=",", wrapped=False):
     result = env(name, default, wrapped)
     if result is None:
@@ -70,15 +75,17 @@
 
 
 def get_class(full_class_name: str) -> Any:
     module_name, class_name = full_class_name.rsplit(".", 1)
     return getattr(importlib.import_module(module_name), class_name)
 
 
-def instantiate_class(full_class_name: str, *args: List, **kwargs: Dict[str, Any]) -> Any:
+def instantiate_class(
+    full_class_name: str, *args: List, **kwargs: Dict[str, Any]
+) -> Any:
     Klass = get_class(full_class_name)
     return Klass(*args, **kwargs)
 
 
 def get_variable_by_pathname(full_class_name: str) -> Any:
     module_name, class_name = full_class_name.rsplit(".", 1)
     return getattr(importlib.import_module(module_name), class_name)
@@ -101,15 +108,15 @@
     ref = tmp.replace(".XX", "[0]")
     if tmp != ref:
         logger.warning("Warning: replaced '.XX' with [0]-th index")
     for key in ref.split("."):
         idstart = key.find("[")
         embedslist = 1 if idstart > 0 else 0
         if embedslist:
-            idx = int(key[idstart + 1 : key.find("]")])
+            idx = int(key[idstart + 1: key.find("]")])
             kyx = key[:idstart]
             try:
                 val = val[kyx][idx]
             except IndexError:
                 logger.warning(f"Index: x['{kyx}'][{idx}] does not exist.")
                 raise
         else:
```

### Comparing `rds-core-0.1.1/rds_core/helpers/http_client.py` & `rds-core-0.1.2/rds_core/helpers/http_client.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.1.1/rds_core/searchengine/__init__.py` & `rds-core-0.1.2/rds_core/searchengine/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 
 def create_index_if_not_exists(
     index: str,
     body: Union[dict, None] = None,
     params: Union[Dict[str, Any], None] = None,
     headers: Union[Dict[str, Any], None] = None,
-    alias: str = "default"
+    alias: str = "default",
 ) -> bool:
     """Cria um índice caso não exista. Retorna True se criou e False se não criou.
 
     Args:
         index (str): nome do índice a ser criado
         body (dict|None): corpo do índice
         params (dict|None): parametros
@@ -82,19 +82,21 @@
         return True
     except Exception as e:
         if getattr(e, "error", None) == "resource_already_exists_exception":
             return False
         raise e
 
 
-def delete_index_if_exists(index_name: str,
-                           params: Union[Dict[str, Any], None] = None,
-                           headers: Union[Dict[str, Any], None] = None,
-                           alias: str = "default",
-                           fail: bool = False) -> bool:
+def delete_index_if_exists(
+    index_name: str,
+    params: Union[Dict[str, Any], None] = None,
+    headers: Union[Dict[str, Any], None] = None,
+    alias: str = "default",
+    fail: bool = False,
+) -> bool:
     """Apaga um índice caso exista. Retorna True se apagou e False se não apagou.
 
     Args:
         index_name (str): nome do índice a ser criado
         params (Dict[str, Any] | None):
         headers (Dict[str, Any] | None): Union[Dict[str, Any], None] = None,
         alias (str): alias para o search engine
@@ -139,20 +141,27 @@
 
 def index(
     index_name: str,
     body: Union[dict, None] = None,
     id: Any = None,
     params: Union[Dict[str, Any], None] = None,
     headers: Union[Dict[str, Any], None] = None,
-    alias: str = "default"
+    alias: str = "default",
 ) -> Union[Any, Any]:
     if not body:
         body = {}
-    return search_engine(alias).index(index=index_name, body=body, id=id, params=params, headers=headers)  # type: ignore
-
+    return search_engine(alias).index(
+        index=index_name,
+        body=body,
+        id=id,
+        params=params,
+        headers=headers,
+    )  # type: ignore
 
 
-def search_engine_healthy(params: Union[Dict[str, Any], None] = None,
-                          headers: Union[Dict[str, Any], None] = None,
-                          alias: str = "default") -> bool:
+def search_engine_healthy(
+    params: Union[Dict[str, Any], None] = None,
+    headers: Union[Dict[str, Any], None] = None,
+    alias: str = "default",
+) -> bool:
     print(search_engine(alias).ping)
     return search_engine(alias).ping(params=params, headers=headers)
```

### Comparing `rds-core-0.1.1/rds_core/transformers/fields/__init__.py` & `rds-core-0.1.2/rds_core/transformers/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.1.1/rds_core/transformers/models/__init__.py` & `rds-core-0.1.2/rds_core/transformers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.1.1/rds_core.egg-info/PKG-INFO` & `rds-core-0.1.2/rds_core.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: rds-core
-Version: 0.1.1
+Version: 0.1.2
 Summary: Framework para serviços do Rede de Dados em Saúde do LAIS
 Home-page: https://github.com/lais-huol/rds-core
 Author: Kelson da Costa Medeiros
 Author-email: kelson.medeiros@lais.huol.ufrn.br
 License: UNKNOWN
 Download-URL: https://github.com/lais-huol/rds-core/tags
+Description: É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias RDS, a exemplo RDS-RN e RDS-ES.
 Keywords: rds,cache,config,helper,searchengine
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.9
-License-File: LICENSE.md
-
-É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias RDS, a exemplo RDS-RN e RDS-ES.
-
+Requires-Python: >=3.8
```

### Comparing `rds-core-0.1.1/rds_core.egg-info/SOURCES.txt` & `rds-core-0.1.2/rds_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rds-core-0.1.1/setup.py` & `rds-core-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,37 +35,38 @@
 
 with open("requirements.txt", "w") as file1:
     for requirement in requirements:
         file1.write(f"{requirement}\n")
 
 setup(
     name="rds-core",
-    version="0.1.1",
+    version="0.1.2",
     description="Framework para serviços do Rede de Dados em Saúde do LAIS",
     long_description="É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o"
     " desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de"
     " Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias"
     " RDS, a exemplo RDS-RN e RDS-ES.",
     author="Kelson da Costa Medeiros",
     author_email="kelson.medeiros@lais.huol.ufrn.br",
     keywords=["rds", "cache", "config", "helper", "searchengine"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
+        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
         "Topic :: Software Development :: Libraries",
     ],
-    python_requires=">=3.9",
+    python_requires=">=3.8",
     install_requires=requirements,
     packages=[
         "rds_core",
         "rds_core.cache",
         "rds_core.config",
         "rds_core.helpers",
         "rds_core.searchengine",
```

