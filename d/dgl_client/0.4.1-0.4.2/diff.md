# Comparing `tmp/dgl_client-0.4.1.tar.gz` & `tmp/dgl_client-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgl_client-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dgl_client-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dgl_client-0.4.1.tar` & `dgl_client-0.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       62 2023-06-26 10:49:28.405914 dgl_client-0.4.1/.gitignore
--rw-r--r--   0        0        0     1599 2023-05-30 07:01:38.904624 dgl_client-0.4.1/README.md
--rw-r--r--   0        0        0       64 2023-06-23 15:01:32.864864 dgl_client-0.4.1/dgl_client/__init__.py
--rw-r--r--   0        0        0    10719 2023-06-26 10:05:24.809476 dgl_client-0.4.1/dgl_client/api_cli.py
--rw-r--r--   0        0        0        0 2023-06-22 08:43:15.967703 dgl_client-0.4.1/dgl_client/commands/__init__.py
--rw-r--r--   0        0        0     1667 2023-06-23 14:50:58.125182 dgl_client-0.4.1/dgl_client/commands/chat.py
--rw-r--r--   0        0        0     3092 2023-06-23 14:14:07.305950 dgl_client-0.4.1/dgl_client/commands/collections.py
--rw-r--r--   0        0        0     1593 2023-06-23 14:16:53.409030 dgl_client-0.4.1/dgl_client/commands/ls.py
--rw-r--r--   0        0        0     1008 2023-06-23 14:12:36.247808 dgl_client-0.4.1/dgl_client/commands/utils.py
--rw-r--r--   0        0        0     5011 2023-06-21 14:26:36.680782 dgl_client-0.4.1/dgl_client/main.py
--rw-r--r--   0        0        0     1448 2023-06-26 10:54:23.480112 dgl_client-0.4.1/dgl_client/main2.py
--rw-r--r--   0        0        0     2573 2023-06-22 13:02:00.540897 dgl_client-0.4.1/dgl_client/utils.py
--rw-r--r--   0        0        0     2033 2023-05-30 13:59:58.346248 dgl_client-0.4.1/notebook.ipynb
--rw-r--r--   0        0        0      484 2023-06-26 10:54:31.687382 dgl_client-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 14:22:35.775422 dgl_client-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0      784 2023-06-14 14:42:24.721364 dgl_client-0.4.1/tests/test_collections.py
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 dgl_client-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       62 2023-06-26 10:49:28.405914 dgl_client-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1599 2023-05-30 07:01:38.904624 dgl_client-0.4.2/README.md
+-rw-r--r--   0        0        0       64 2023-06-26 12:09:05.446349 dgl_client-0.4.2/dgl_client/__init__.py
+-rw-r--r--   0        0        0    10719 2023-06-26 10:05:24.809476 dgl_client-0.4.2/dgl_client/api_cli.py
+-rw-r--r--   0        0        0        0 2023-06-22 08:43:15.967703 dgl_client-0.4.2/dgl_client/commands/__init__.py
+-rw-r--r--   0        0        0     1667 2023-06-23 14:50:58.125182 dgl_client-0.4.2/dgl_client/commands/chat.py
+-rw-r--r--   0        0        0     3092 2023-06-23 14:14:07.305950 dgl_client-0.4.2/dgl_client/commands/collections.py
+-rw-r--r--   0        0        0     1593 2023-06-23 14:16:53.409030 dgl_client-0.4.2/dgl_client/commands/ls.py
+-rw-r--r--   0        0        0     1069 2023-06-26 11:06:25.569632 dgl_client-0.4.2/dgl_client/commands/utils.py
+-rw-r--r--   0        0        0     5011 2023-06-21 14:26:36.680782 dgl_client-0.4.2/dgl_client/main.py
+-rw-r--r--   0        0        0     1448 2023-06-26 10:54:23.480112 dgl_client-0.4.2/dgl_client/main2.py
+-rw-r--r--   0        0        0     2573 2023-06-22 13:02:00.540897 dgl_client-0.4.2/dgl_client/utils.py
+-rw-r--r--   0        0        0     2033 2023-05-30 13:59:58.346248 dgl_client-0.4.2/notebook.ipynb
+-rw-r--r--   0        0        0      484 2023-06-26 10:54:31.687382 dgl_client-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 14:22:35.775422 dgl_client-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0      784 2023-06-14 14:42:24.721364 dgl_client-0.4.2/tests/test_collections.py
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 dgl_client-0.4.2/PKG-INFO
```

### Comparing `dgl_client-0.4.1/README.md` & `dgl_client-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.1/dgl_client/api_cli.py` & `dgl_client-0.4.2/dgl_client/api_cli.py`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.1/dgl_client/commands/chat.py` & `dgl_client-0.4.2/dgl_client/commands/chat.py`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.1/dgl_client/commands/collections.py` & `dgl_client-0.4.2/dgl_client/commands/collections.py`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.1/dgl_client/commands/ls.py` & `dgl_client-0.4.2/dgl_client/commands/ls.py`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.1/dgl_client/commands/utils.py` & `dgl_client-0.4.2/dgl_client/commands/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 if "DGL_INF_ENDPOINT" in os.environ and os.environ["DGL_INF_ENDPOINT"]:
     DGL_INF_ENDPOINT = os.environ["DGL_INF_ENDPOINT"]
 
 DGL_BCK_ENDPOINT = "https://www.diglife.eu/"
 if "DGL_BCK_ENDPOINT" in os.environ and os.environ["DGL_BCK_ENDPOINT"]:
     DGL_BCK_ENDPOINT = os.environ["DGL_BCK_ENDPOINT"]    
 
-def get_inf_client(endpoint: str, inference_url: str) -> InferenceClient:
+def get_inf_client(endpoint: str = DGL_INF_ENDPOINT, inference_url: str="inference") -> InferenceClient:
   logger.info("Connecting to API Endpoint %s"%endpoint)
   client = APIClient(endpoint, inf_url=inference_url)    
   return client._inference
 
-def get_back_client(endpoint: str, inference_url: str) -> BackendClient:
+def get_back_client(endpoint: str = DGL_INF_ENDPOINT, inference_url: str = "api/v1") -> BackendClient:
   logger.info("Connecting to API Endpoint %s"%endpoint)
   client = APIClient(endpoint, inf_url=inference_url)    
   return client._backend
 
 def do_login(access_key, client):
   if access_key:
     return client.login(access_key)
```

### Comparing `dgl_client-0.4.1/dgl_client/main.py` & `dgl_client-0.4.2/dgl_client/main.py`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.1/dgl_client/main2.py` & `dgl_client-0.4.2/dgl_client/main2.py`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.1/dgl_client/utils.py` & `dgl_client-0.4.2/dgl_client/utils.py`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.1/notebook.ipynb` & `dgl_client-0.4.2/notebook.ipynb`

 * *Files identical despite different names*

### Comparing `dgl_client-0.4.1/tests/test_collections.py` & `dgl_client-0.4.2/tests/test_collections.py`

 * *Files identical despite different names*

