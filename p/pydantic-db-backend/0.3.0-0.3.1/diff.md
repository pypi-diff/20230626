# Comparing `tmp/pydantic_db_backend-0.3.0.tar.gz` & `tmp/pydantic_db_backend-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_db_backend-0.3.0.tar", max compression
+gzip compressed data, was "pydantic_db_backend-0.3.1.tar", max compression
```

## Comparing `pydantic_db_backend-0.3.0.tar` & `pydantic_db_backend-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       87 2023-06-14 17:15:43.151729 pydantic_db_backend-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-05-11 08:45:17.171212 pydantic_db_backend-0.3.0/pydantic_db_backend/__init__.py
--rw-r--r--   0        0        0     6072 2023-06-26 13:34:47.557755 pydantic_db_backend-0.3.0/pydantic_db_backend/backend.py
--rw-r--r--   0        0        0        0 2023-05-13 10:06:57.338481 pydantic_db_backend-0.3.0/pydantic_db_backend/backends/__init__.py
--rw-r--r--   0        0        0     5757 2023-06-26 13:43:26.341233 pydantic_db_backend-0.3.0/pydantic_db_backend/backends/couchdb.py
--rw-r--r--   0        0        0      100 2023-06-14 12:06:00.522425 pydantic_db_backend-0.3.0/pydantic_db_backend/backends/json_files.py
--rw-r--r--   0        0        0      701 2023-06-20 16:53:47.237618 pydantic_db_backend-0.3.0/pydantic_db_backend/exceptions/__init__.py
--rw-r--r--   0        0        0      577 2023-06-16 13:56:03.761606 pydantic_db_backend-0.3.0/pydantic_db_backend/utils.py
--rw-r--r--   0        0        0     1000 2023-06-26 13:47:04.847490 pydantic_db_backend-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 pydantic_db_backend-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-06-14 17:15:43.151729 pydantic_db_backend-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 08:45:17.171212 pydantic_db_backend-0.3.1/pydantic_db_backend/__init__.py
+-rw-r--r--   0        0        0     6072 2023-06-26 13:34:47.557755 pydantic_db_backend-0.3.1/pydantic_db_backend/backend.py
+-rw-r--r--   0        0        0        0 2023-05-13 10:06:57.338481 pydantic_db_backend-0.3.1/pydantic_db_backend/backends/__init__.py
+-rw-r--r--   0        0        0     5757 2023-06-26 13:43:26.341233 pydantic_db_backend-0.3.1/pydantic_db_backend/backends/couchdb.py
+-rw-r--r--   0        0        0      100 2023-06-14 12:06:00.522425 pydantic_db_backend-0.3.1/pydantic_db_backend/backends/json_files.py
+-rw-r--r--   0        0        0      701 2023-06-20 16:53:47.237618 pydantic_db_backend-0.3.1/pydantic_db_backend/exceptions/__init__.py
+-rw-r--r--   0        0        0      577 2023-06-16 13:56:03.761606 pydantic_db_backend-0.3.1/pydantic_db_backend/utils.py
+-rw-r--r--   0        0        0     1000 2023-06-26 13:58:04.262602 pydantic_db_backend-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 pydantic_db_backend-0.3.1/PKG-INFO
```

### Comparing `pydantic_db_backend-0.3.0/pydantic_db_backend/backend.py` & `pydantic_db_backend-0.3.1/pydantic_db_backend/backend.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.3.0/pydantic_db_backend/backends/couchdb.py` & `pydantic_db_backend-0.3.1/pydantic_db_backend/backends/couchdb.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.3.0/pydantic_db_backend/exceptions/__init__.py` & `pydantic_db_backend-0.3.1/pydantic_db_backend/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.3.0/pydantic_db_backend/utils.py` & `pydantic_db_backend-0.3.1/pydantic_db_backend/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_db_backend-0.3.0/pyproject.toml` & `pydantic_db_backend-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-db-backend"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = "^1.0.0"
```

### Comparing `pydantic_db_backend-0.3.0/PKG-INFO` & `pydantic_db_backend-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-db-backend
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: couchdb
```

