# Comparing `tmp/fastapi_standalone_docs-0.1.1.tar.gz` & `tmp/fastapi_standalone_docs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_standalone_docs-0.1.1.tar", max compression
+gzip compressed data, was "fastapi_standalone_docs-0.1.2.tar", max compression
```

## Comparing `fastapi_standalone_docs-0.1.1.tar` & `fastapi_standalone_docs-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1064 2023-06-20 11:03:35.651240 fastapi_standalone_docs-0.1.1/LICENSE
--rw-r--r--   0        0        0     4618 2023-06-20 11:03:35.655240 fastapi_standalone_docs-0.1.1/README.md
--rw-r--r--   0        0        0       82 2023-06-20 11:03:35.655240 fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/__init__.py
--rw-r--r--   0        0        0     1828 2023-06-20 11:03:35.655240 fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/scripts.py
--rw-r--r--   0        0        0     2759 2023-06-20 11:03:35.655240 fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/standalone_docs.py
--rw-r--r--   0        0        0     1086 2023-06-20 11:03:35.655240 fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/static/fastapi/LICENSE
--rw-r--r--   0        0        0      412 2023-06-20 11:03:35.655240 fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/static/fastapi/favicon.png
--rw-r--r--   0        0        0     1174 2023-06-20 11:03:35.655240 fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/static/redoc/logo-mini.svg
--rw-r--r--   0        0        0  1042510 2023-06-20 11:03:35.663240 fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/static/redoc/redoc.standalone.js
--rw-r--r--   0        0        0     2628 2023-06-20 11:03:35.663240 fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/static/redoc/redoc.standalone.js.LICENSE.txt
--rw-r--r--   0        0        0    11358 2023-06-20 11:03:35.663240 fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/static/swagger/LICENSE
--rw-r--r--   0        0        0  1048219 2023-06-20 11:03:35.671240 fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/static/swagger/swagger-ui-bundle.js
--rw-r--r--   0        0        0   145206 2023-06-20 11:03:35.671240 fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/static/swagger/swagger-ui.css
--rw-r--r--   0        0        0        0 2023-06-20 11:03:35.671240 fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 11:03:35.671240 fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/tests/conftests.py
--rw-r--r--   0        0        0     6131 2023-06-20 11:03:35.671240 fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/tests/test_standalone_docs.py
--rw-r--r--   0        0        0      852 2023-06-20 11:03:35.671240 fastapi_standalone_docs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5313 1970-01-01 00:00:00.000000 fastapi_standalone_docs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-26 07:12:36.524958 fastapi_standalone_docs-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4618 2023-06-26 07:12:36.524958 fastapi_standalone_docs-0.1.2/README.md
+-rw-r--r--   0        0        0       82 2023-06-26 07:12:36.524958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/__init__.py
+-rw-r--r--   0        0        0     1828 2023-06-26 07:12:36.524958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/scripts.py
+-rw-r--r--   0        0        0     2759 2023-06-26 07:12:36.524958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/standalone_docs.py
+-rw-r--r--   0        0        0     1086 2023-06-26 07:12:36.524958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/fastapi/LICENSE
+-rw-r--r--   0        0        0      412 2023-06-26 07:12:36.524958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/fastapi/favicon.png
+-rw-r--r--   0        0        0     1174 2023-06-26 07:12:36.524958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/redoc/logo-mini.svg
+-rw-r--r--   0        0        0  1042510 2023-06-26 07:12:36.528958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/redoc/redoc.standalone.js
+-rw-r--r--   0        0        0     2628 2023-06-26 07:12:36.528958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/redoc/redoc.standalone.js.LICENSE.txt
+-rw-r--r--   0        0        0    11358 2023-06-26 07:12:36.528958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/swagger/LICENSE
+-rw-r--r--   0        0        0  1048219 2023-06-26 07:12:36.536958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/swagger/swagger-ui-bundle.js
+-rw-r--r--   0        0        0   145206 2023-06-26 07:12:36.536958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/swagger/swagger-ui.css
+-rw-r--r--   0        0        0        0 2023-06-26 07:12:36.536958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:12:36.536958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/tests/conftests.py
+-rw-r--r--   0        0        0     6131 2023-06-26 07:12:36.536958 fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/tests/test_standalone_docs.py
+-rw-r--r--   0        0        0      852 2023-06-26 07:12:36.536958 fastapi_standalone_docs-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5313 1970-01-01 00:00:00.000000 fastapi_standalone_docs-0.1.2/PKG-INFO
```

### Comparing `fastapi_standalone_docs-0.1.1/LICENSE` & `fastapi_standalone_docs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.1/README.md` & `fastapi_standalone_docs-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/scripts.py` & `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/scripts.py`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/standalone_docs.py` & `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/standalone_docs.py`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/static/fastapi/LICENSE` & `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/fastapi/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/static/redoc/logo-mini.svg` & `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/redoc/logo-mini.svg`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/static/redoc/redoc.standalone.js` & `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/redoc/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/static/redoc/redoc.standalone.js.LICENSE.txt` & `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/redoc/redoc.standalone.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/static/swagger/LICENSE` & `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/swagger/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/static/swagger/swagger-ui-bundle.js` & `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/swagger/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/static/swagger/swagger-ui.css` & `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/static/swagger/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.1/fastapi_standalone_docs/tests/test_standalone_docs.py` & `fastapi_standalone_docs-0.1.2/fastapi_standalone_docs/tests/test_standalone_docs.py`

 * *Files identical despite different names*

### Comparing `fastapi_standalone_docs-0.1.1/pyproject.toml` & `fastapi_standalone_docs-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "fastapi-standalone-docs"
-version = "0.1.1"
+version = "0.1.2"
 description = "Host FastAPI Swagger UI and ReDoc without third party CDNs"
 authors = ["IOXIO Ltd"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ioxiocom/fastapi-standalone-docs"
 packages = [{include = "fastapi_standalone_docs"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-fastapi = ">=0.95.2,<0.98.0"
+fastapi = ">=0.95.2,<0.99.0"
 
 [tool.poetry.scripts]
 update-fastapi-standalone-docs = { callable = "fastapi_standalone_docs.scripts:update_docs", extras = ["scripts"] }
 
 [tool.poetry.extras]
 scripts = []
```

### Comparing `fastapi_standalone_docs-0.1.1/PKG-INFO` & `fastapi_standalone_docs-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fastapi-standalone-docs
-Version: 0.1.1
+Version: 0.1.2
 Summary: Host FastAPI Swagger UI and ReDoc without third party CDNs
 Home-page: https://github.com/ioxiocom/fastapi-standalone-docs
 License: MIT
 Author: IOXIO Ltd
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: scripts
-Requires-Dist: fastapi (>=0.95.2,<0.98.0)
+Requires-Dist: fastapi (>=0.95.2,<0.99.0)
 Project-URL: Repository, https://github.com/ioxiocom/fastapi-standalone-docs
 Description-Content-Type: text/markdown
 
 # FastAPI Standalone Docs
 
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ioxiocom/fastapi-standalone-docs/publish.yaml)](https://github.com/ioxiocom/fastapi-standalone-docs/actions/workflows/publish.yaml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

