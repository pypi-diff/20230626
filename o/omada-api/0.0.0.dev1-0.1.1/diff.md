# Comparing `tmp/omada_api-0.0.0.dev1.tar.gz` & `tmp/omada_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omada_api-0.0.0.dev1.tar", max compression
+gzip compressed data, was "omada_api-0.1.1.tar", max compression
```

## Comparing `omada_api-0.0.0.dev1.tar` & `omada_api-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2023-06-19 12:07:46.539753 omada_api-0.0.0.dev1/LICENSE
--rw-r--r--   0        0        0     3686 2023-06-19 15:50:47.834469 omada_api-0.0.0.dev1/README.md
--rw-r--r--   0        0        0       77 2023-06-26 10:22:46.705093 omada_api-0.0.0.dev1/omada/__init__.py
--rw-r--r--   0        0        0      524 2023-06-26 10:23:33.952345 omada_api-0.0.0.dev1/omada/api_bindings.py
--rw-r--r--   0        0        0    12299 2023-06-26 11:41:57.804707 omada_api-0.0.0.dev1/omada/omada.py
--rw-r--r--   0        0        0     2115 2023-06-26 13:23:55.393160 omada_api-0.0.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     4703 1970-01-01 00:00:00.000000 omada_api-0.0.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-26 14:01:05.665513 omada_api-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3686 2023-06-26 14:01:05.665513 omada_api-0.1.1/README.md
+-rw-r--r--   0        0        0       77 2023-06-26 14:01:05.665513 omada_api-0.1.1/omada/__init__.py
+-rw-r--r--   0        0        0      524 2023-06-26 14:01:05.665513 omada_api-0.1.1/omada/api_bindings.py
+-rw-r--r--   0        0        0    12299 2023-06-26 14:01:05.665513 omada_api-0.1.1/omada/omada.py
+-rw-r--r--   0        0        0     2062 2023-06-26 14:01:13.693569 omada_api-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4698 1970-01-01 00:00:00.000000 omada_api-0.1.1/PKG-INFO
```

### Comparing `omada_api-0.0.0.dev1/LICENSE` & `omada_api-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omada_api-0.0.0.dev1/README.md` & `omada_api-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `omada_api-0.0.0.dev1/omada/api_bindings.py` & `omada_api-0.1.1/omada/api_bindings.py`

 * *Files identical despite different names*

### Comparing `omada_api-0.0.0.dev1/omada/omada.py` & `omada_api-0.1.1/omada/omada.py`

 * *Files identical despite different names*

### Comparing `omada_api-0.0.0.dev1/pyproject.toml` & `omada_api-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omada-api"
-version = "v0.0.0dev1"
+version = "v0.1.1"
 description = "A simple Python wrapper for the TP-Link Omada Software Controller API"
 authors = ["Ilja O <vrghost@gmail.com>", "Gregory Haberek <ghaberek@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "omada"}]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -21,19 +21,14 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.31.0"
 yarl = "^1.9.2"
 pydantic = "^1.10.9"
 
-[virtualenvs]
-create = false
-in-project = true
-
-
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 ruff = "^0.0.272"
 pytest-mock = "^3.11.1"
 pytest-local-badge = "^1.0.3"
```

### Comparing `omada_api-0.0.0.dev1/PKG-INFO` & `omada_api-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omada-api
-Version: 0.0.0.dev1
+Version: 0.1.1
 Summary: A simple Python wrapper for the TP-Link Omada Software Controller API
 License: MIT
 Keywords: tplink,omada,wrapper
 Author: Ilja O
 Author-email: vrghost@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

