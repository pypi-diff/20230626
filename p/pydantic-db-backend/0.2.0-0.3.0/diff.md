# Comparing `tmp/pydantic_db_backend-0.2.0.tar.gz` & `tmp/pydantic_db_backend-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_db_backend-0.2.0.tar", max compression
+gzip compressed data, was "pydantic_db_backend-0.3.0.tar", max compression
```

## Comparing `pydantic_db_backend-0.2.0.tar` & `pydantic_db_backend-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0        0 2023-05-11 08:45:05.171805 pydantic_db_backend-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-05-11 08:45:17.171212 pydantic_db_backend-0.2.0/pydantic_db_backend/__init__.py
--rw-r--r--   0        0        0     2550 2023-05-13 10:51:56.578404 pydantic_db_backend-0.2.0/pydantic_db_backend/backend.py
--rw-r--r--   0        0        0        0 2023-05-13 10:06:57.338481 pydantic_db_backend-0.2.0/pydantic_db_backend/backends/__init__.py
--rw-r--r--   0        0        0     2943 2023-05-13 10:05:18.402714 pydantic_db_backend-0.2.0/pydantic_db_backend/backends/couchdb.py
--rw-r--r--   0        0        0       92 2023-05-11 09:09:54.582757 pydantic_db_backend-0.2.0/pydantic_db_backend/backends/json_files.py
--rw-r--r--   0        0        0      566 2023-05-13 10:05:53.046645 pydantic_db_backend-0.2.0/pydantic_db_backend/utils.py
--rw-r--r--   0        0        0      724 2023-05-13 10:55:06.803914 pydantic_db_backend-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 pydantic_db_backend-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-06-14 17:15:43.151729 pydantic_db_backend-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-11 08:45:17.171212 pydantic_db_backend-0.3.0/pydantic_db_backend/__init__.py
+-rw-r--r--   0        0        0     6072 2023-06-26 13:34:47.557755 pydantic_db_backend-0.3.0/pydantic_db_backend/backend.py
+-rw-r--r--   0        0        0        0 2023-05-13 10:06:57.338481 pydantic_db_backend-0.3.0/pydantic_db_backend/backends/__init__.py
+-rw-r--r--   0        0        0     5757 2023-06-26 13:43:26.341233 pydantic_db_backend-0.3.0/pydantic_db_backend/backends/couchdb.py
+-rw-r--r--   0        0        0      100 2023-06-14 12:06:00.522425 pydantic_db_backend-0.3.0/pydantic_db_backend/backends/json_files.py
+-rw-r--r--   0        0        0      701 2023-06-20 16:53:47.237618 pydantic_db_backend-0.3.0/pydantic_db_backend/exceptions/__init__.py
+-rw-r--r--   0        0        0      577 2023-06-16 13:56:03.761606 pydantic_db_backend-0.3.0/pydantic_db_backend/utils.py
+-rw-r--r--   0        0        0     1000 2023-06-26 13:47:04.847490 pydantic_db_backend-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 pydantic_db_backend-0.3.0/PKG-INFO
```

### Comparing `pydantic_db_backend-0.2.0/pydantic_db_backend/utils.py` & `pydantic_db_backend-0.3.0/pydantic_db_backend/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from iso8601 import iso8601, ParseError
 
 
 def uid() -> str:
     return str(uuid4()).replace("-", "")
 
+_uid = uid
 
 def utcnow() -> datetime.datetime:
     return datetime.datetime.utcnow().replace(tzinfo=datetime.timezone.utc)
 
 
 def str_to_datetime_if_parseable(value: str) -> datetime.datetime | str:
     if len(value) < 8 or value.count('-') != 2:
```

### Comparing `pydantic_db_backend-0.2.0/pyproject.toml` & `pydantic_db_backend-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 [tool.poetry]
 name = "pydantic-db-backend"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Marco Bartel <bsimpson888@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = "^1.0.0"
 couchdb = { version = "^1.2", optional = true }
+pymongo = { version = "^3.13.0", optional = true }
 pydash = "^7.0.3"
 iso8601 = "^1.1.0"
 pydantic = "^1.10.7"
+coverage = "^7.2.7"
+webexception = "^1.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
+freezegun = "^1.2.2"
+couchdb = "^1.2"
+pymongo = "^3.13.0"
+pytest-mock = "^3.10.0"
+
 
 [tool.poetry.extras]
 couchdb = ["couchdb"]
+mongodb = ["pymongo"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q -s -v"
 testpaths = [
     "tests",
 ]
 log_cli = true
-log_cli_level = "INFO"
+log_cli_level = "debug"
+#log_cli_format = "[%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_cli_format = "[%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
```

### Comparing `pydantic_db_backend-0.2.0/PKG-INFO` & `pydantic_db_backend-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 Metadata-Version: 2.1
 Name: pydantic-db-backend
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: Marco Bartel
 Author-email: bsimpson888@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: couchdb
+Provides-Extra: mongodb
 Requires-Dist: couchdb (>=1.2,<2.0) ; extra == "couchdb"
+Requires-Dist: coverage (>=7.2.7,<8.0.0)
 Requires-Dist: iso8601 (>=1.1.0,<2.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pydash (>=7.0.3,<8.0.0)
+Requires-Dist: pymongo (>=3.13.0,<4.0.0) ; extra == "mongodb"
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: webexception (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
+# Testing
+
+### CouchDB
+
+http://localhost:5984/_utils/#
+
+- user: admin
+- passwd: pytest
```

