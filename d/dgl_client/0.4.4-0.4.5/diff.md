# Comparing `tmp/dgl_client-0.4.4.tar.gz` & `tmp/dgl_client-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgl_client-0.4.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dgl_client-0.4.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dgl_client-0.4.4.tar` & `dgl_client-0.4.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       62 2023-06-26 10:49:28.405914 dgl_client-0.4.4/.gitignore
--rw-r--r--   0        0        0     1599 2023-05-30 07:01:38.904624 dgl_client-0.4.4/README.md
--rw-r--r--   0        0        0       64 2023-06-26 12:46:00.087700 dgl_client-0.4.4/dgl_client/__init__.py
--rw-r--r--   0        0        0    10693 2023-06-26 12:45:39.176607 dgl_client-0.4.4/dgl_client/api_cli.py
--rw-r--r--   0        0        0        0 2023-06-22 08:43:15.967703 dgl_client-0.4.4/dgl_client/commands/__init__.py
--rw-r--r--   0        0        0     1642 2023-06-26 12:41:45.269957 dgl_client-0.4.4/dgl_client/commands/chat.py
--rw-r--r--   0        0        0     3066 2023-06-26 12:41:24.632090 dgl_client-0.4.4/dgl_client/commands/collections.py
--rw-r--r--   0        0        0     1546 2023-06-26 12:41:31.795356 dgl_client-0.4.4/dgl_client/commands/ls.py
--rw-r--r--   0        0        0     1044 2023-06-26 12:41:37.515790 dgl_client-0.4.4/dgl_client/commands/utils.py
--rw-r--r--   0        0        0     5011 2023-06-21 14:26:36.680782 dgl_client-0.4.4/dgl_client/main.py
--rw-r--r--   0        0        0      920 2023-06-26 12:41:14.294495 dgl_client-0.4.4/dgl_client/main2.py
--rw-r--r--   0        0        0     2573 2023-06-22 13:02:00.540897 dgl_client-0.4.4/dgl_client/utils.py
--rw-r--r--   0        0        0     2033 2023-05-30 13:59:58.346248 dgl_client-0.4.4/notebook.ipynb
--rw-r--r--   0        0        0      498 2023-06-26 12:41:56.393164 dgl_client-0.4.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 14:22:35.775422 dgl_client-0.4.4/tests/__init__.py
--rw-r--r--   0        0        0      784 2023-06-14 14:42:24.721364 dgl_client-0.4.4/tests/test_collections.py
--rw-r--r--   0        0        0      383 1970-01-01 00:00:00.000000 dgl_client-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0       62 2023-06-26 10:49:28.405914 dgl_client-0.4.5/.gitignore
+-rw-r--r--   0        0        0     1599 2023-05-30 07:01:38.904624 dgl_client-0.4.5/README.md
+-rw-r--r--   0        0        0       64 2023-06-26 12:48:19.338411 dgl_client-0.4.5/dgl_client/__init__.py
+-rw-r--r--   0        0        0    10693 2023-06-26 12:45:39.176607 dgl_client-0.4.5/dgl_client/api_cli.py
+-rw-r--r--   0        0        0        0 2023-06-22 08:43:15.967703 dgl_client-0.4.5/dgl_client/commands/__init__.py
+-rw-r--r--   0        0        0     1642 2023-06-26 12:41:45.269957 dgl_client-0.4.5/dgl_client/commands/chat.py
+-rw-r--r--   0        0        0     3066 2023-06-26 12:41:24.632090 dgl_client-0.4.5/dgl_client/commands/collections.py
+-rw-r--r--   0        0        0     1566 2023-06-26 12:48:07.639757 dgl_client-0.4.5/dgl_client/commands/ls.py
+-rw-r--r--   0        0        0     1044 2023-06-26 12:41:37.515790 dgl_client-0.4.5/dgl_client/commands/utils.py
+-rw-r--r--   0        0        0     5011 2023-06-21 14:26:36.680782 dgl_client-0.4.5/dgl_client/main.py
+-rw-r--r--   0        0        0      920 2023-06-26 12:41:14.294495 dgl_client-0.4.5/dgl_client/main2.py
+-rw-r--r--   0        0        0     2573 2023-06-22 13:02:00.540897 dgl_client-0.4.5/dgl_client/utils.py
+-rw-r--r--   0        0        0     2033 2023-05-30 13:59:58.346248 dgl_client-0.4.5/notebook.ipynb
+-rw-r--r--   0        0        0      498 2023-06-26 12:41:56.393164 dgl_client-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 14:22:35.775422 dgl_client-0.4.5/tests/__init__.py
+-rw-r--r--   0        0        0      784 2023-06-14 14:42:24.721364 dgl_client-0.4.5/tests/test_collections.py
+-rw-r--r--   0        0        0      383 1970-01-01 00:00:00.000000 dgl_client-0.4.5/PKG-INFO
```

### Comparing `dgl_client-0.4.4/README.md` & `dgl_client-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.4/dgl_client/api_cli.py` & `dgl_client-0.4.5/dgl_client/api_cli.py`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.4/dgl_client/commands/chat.py` & `dgl_client-0.4.5/dgl_client/commands/chat.py`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.4/dgl_client/commands/collections.py` & `dgl_client-0.4.5/dgl_client/commands/collections.py`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.4/dgl_client/commands/ls.py` & `dgl_client-0.4.5/dgl_client/commands/ls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typer
 from rich import print
 from typing import Optional
 from loguru import logger
 from .utils import get_inf_client, do_login, DGL_INF_ENDPOINT
 
+app = typer.Typer()
 
 def list_models(client):
   available_models = client.get_available_models()
   logger.info("Available models %s"%str(available_models))
 
   available_wkf = client.get_available_workflows()
   logger.info("Available workflows %s"%str(available_wkf))
```

### Comparing `dgl_client-0.4.4/dgl_client/commands/utils.py` & `dgl_client-0.4.5/dgl_client/commands/utils.py`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.4/dgl_client/main.py` & `dgl_client-0.4.5/dgl_client/main.py`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.4/dgl_client/main2.py` & `dgl_client-0.4.5/dgl_client/main2.py`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.4/dgl_client/utils.py` & `dgl_client-0.4.5/dgl_client/utils.py`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.4/notebook.ipynb` & `dgl_client-0.4.5/notebook.ipynb`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.4/tests/test_collections.py` & `dgl_client-0.4.5/tests/test_collections.py`

 * *Files identical despite different names*

