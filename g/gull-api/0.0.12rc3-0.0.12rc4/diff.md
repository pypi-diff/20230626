# Comparing `tmp/gull_api-0.0.12rc3.tar.gz` & `tmp/gull_api-0.0.12rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gull_api-0.0.12rc3.tar", max compression
+gzip compressed data, was "gull_api-0.0.12rc4.tar", max compression
```

## Comparing `gull_api-0.0.12rc3.tar` & `gull_api-0.0.12rc4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2223 2023-06-26 00:57:36.810796 gull_api-0.0.12rc3/LICENSE
--rw-r--r--   0        0        0     2821 2023-06-26 00:57:36.810796 gull_api-0.0.12rc3/README.md
--rw-r--r--   0        0        0        0 2023-06-26 00:57:36.810796 gull_api-0.0.12rc3/gull_api/__init__.py
--rw-r--r--   0        0        0     1939 2023-06-26 00:57:36.810796 gull_api-0.0.12rc3/gull_api/db.py
--rw-r--r--   0        0        0     5637 2023-06-26 00:57:36.810796 gull_api-0.0.12rc3/gull_api/main.py
--rw-r--r--   0        0        0     1606 2023-06-26 00:57:36.918803 gull_api-0.0.12rc3/pyproject.toml
--rw-r--r--   0        0        0     4424 1970-01-01 00:00:00.000000 gull_api-0.0.12rc3/PKG-INFO
+-rw-r--r--   0        0        0     2223 2023-06-26 01:06:45.945275 gull_api-0.0.12rc4/LICENSE
+-rw-r--r--   0        0        0     2821 2023-06-26 01:06:45.945275 gull_api-0.0.12rc4/README.md
+-rw-r--r--   0        0        0        0 2023-06-26 01:06:45.945275 gull_api-0.0.12rc4/gull_api/__init__.py
+-rw-r--r--   0        0        0     1939 2023-06-26 01:06:45.945275 gull_api-0.0.12rc4/gull_api/db.py
+-rw-r--r--   0        0        0     5637 2023-06-26 01:06:45.945275 gull_api-0.0.12rc4/gull_api/main.py
+-rw-r--r--   0        0        0     1606 2023-06-26 01:06:46.049279 gull_api-0.0.12rc4/pyproject.toml
+-rw-r--r--   0        0        0     4424 1970-01-01 00:00:00.000000 gull_api-0.0.12rc4/PKG-INFO
```

### Comparing `gull_api-0.0.12rc3/LICENSE` & `gull_api-0.0.12rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `gull_api-0.0.12rc3/README.md` & `gull_api-0.0.12rc4/README.md`

 * *Files identical despite different names*

### Comparing `gull_api-0.0.12rc3/gull_api/db.py` & `gull_api-0.0.12rc4/gull_api/db.py`

 * *Files identical despite different names*

### Comparing `gull_api-0.0.12rc3/gull_api/main.py` & `gull_api-0.0.12rc4/gull_api/main.py`

 * *Files identical despite different names*

### Comparing `gull_api-0.0.12rc3/pyproject.toml` & `gull_api-0.0.12rc4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["poetry-core"]
 
 [tool.poetry]
 name = "gull-api"
-version = "0.0.12-rc.3"
+version = "0.0.12-rc.4"
 description = "A REST API for running Large Language Models"
 authors = ["Michael Becker <mdbecker@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/mdbecker/gull_api"
 repository = "https://github.com/mdbecker/gull_api"
 documentation = "https://github.com/mdbecker/gull_api/blob/main/README.md"
 readme = "README.md"
```

### Comparing `gull_api-0.0.12rc3/PKG-INFO` & `gull_api-0.0.12rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gull-api
-Version: 0.0.12rc3
+Version: 0.0.12rc4
 Summary: A REST API for running Large Language Models
 Home-page: https://github.com/mdbecker/gull_api
 License: MIT
 Keywords: api,artificial-intelligence,automation,bot,deep-learning,fastapi,GPT,language-models,large-language-models,machine-learning,microservices,natural-language-processing,NLP,openai,REST,text,text-generation,web-api
 Author: Michael Becker
 Author-email: mdbecker@gmail.com
 Requires-Python: >=3.10,<4.0
```

