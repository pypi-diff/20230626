# Comparing `tmp/databricks_sql_connector-2.6.3.dev1.tar.gz` & `tmp/databricks_sql_connector-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_sql_connector-2.6.3.dev1.tar", max compression
+gzip compressed data, was "databricks_sql_connector-2.7.0.tar", max compression
```

## Comparing `databricks_sql_connector-2.6.3.dev1.tar` & `databricks_sql_connector-2.7.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     4585 2023-06-21 21:04:46.601915 databricks_sql_connector-2.6.3.dev1/CHANGELOG.md
--rw-r--r--   0        0        0    11346 2023-06-14 20:24:08.166793 databricks_sql_connector-2.6.3.dev1/LICENSE
--rw-r--r--   0        0        0     2723 2023-06-14 20:24:08.167012 databricks_sql_connector-2.6.3.dev1/README.md
--rw-r--r--   0        0        0     1421 2023-06-21 22:01:35.095661 databricks_sql_connector-2.6.3.dev1/pyproject.toml
--rw-r--r--   0        0        0      295 2023-06-14 20:24:08.170343 databricks_sql_connector-2.6.3.dev1/src/databricks/__init__.py
--rw-r--r--   0        0        0     1273 2023-06-21 22:01:46.449876 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 20:24:08.170890 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/__init__.py
--rw-r--r--   0        0        0     4421 2023-06-21 18:47:10.955827 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/auth.py
--rw-r--r--   0        0        0     6192 2023-06-21 18:47:10.956342 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/authenticators.py
--rw-r--r--   0        0        0     3790 2023-06-21 18:47:10.956670 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/endpoint.py
--rw-r--r--   0        0        0     9499 2023-06-21 18:47:10.957158 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/oauth.py
--rw-r--r--   0        0        0     1201 2023-06-14 20:24:08.171709 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/oauth_http_handler.py
--rw-r--r--   0        0        0     5949 2023-06-14 20:24:08.171906 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/thrift_http_client.py
--rw-r--r--   0        0        0    36862 2023-06-14 20:24:08.172377 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/client.py
--rw-r--r--   0        0        0     2423 2023-06-14 20:24:08.172576 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/exc.py
--rw-r--r--   0        0        0        0 2023-06-14 20:24:08.172808 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/experimental/__init__.py
--rw-r--r--   0        0        0     2543 2023-06-21 18:47:10.957602 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/experimental/oauth_persistence.py
--rwxr-xr-x   0        0        0     8062 2023-06-14 20:24:08.173439 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
--rw-r--r--   0        0        0   136849 2023-06-14 20:24:08.175895 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
--rw-r--r--   0        0        0       49 2023-06-14 20:24:08.176090 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/TCLIService/__init__.py
--rw-r--r--   0        0        0     1307 2023-06-14 20:24:08.176221 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/TCLIService/constants.py
--rw-r--r--   0        0        0  2077276 2023-06-14 20:24:08.177855 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/TCLIService/ttypes.py
--rw-r--r--   0        0        0        0 2023-06-14 20:24:08.178096 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/__init__.py
--rw-r--r--   0        0        0    42976 2023-06-21 21:48:18.641419 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_backend.py
--rw-r--r--   0        0        0     6771 2023-06-14 20:24:08.178634 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/types.py
--rw-r--r--   0        0        0     6646 2023-06-14 20:24:08.178813 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/utils.py
--rw-r--r--   0        0        0       60 2023-06-14 20:24:08.179003 databricks_sql_connector-2.6.3.dev1/src/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     9761 2023-06-14 20:24:08.179220 databricks_sql_connector-2.6.3.dev1/src/databricks/sqlalchemy/dialect/__init__.py
--rw-r--r--   0        0        0      494 2023-06-14 20:24:08.179360 databricks_sql_connector-2.6.3.dev1/src/databricks/sqlalchemy/dialect/base.py
--rw-r--r--   0        0        0      792 2023-06-14 20:24:08.179497 databricks_sql_connector-2.6.3.dev1/src/databricks/sqlalchemy/dialect/compiler.py
--rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 databricks_sql_connector-2.6.3.dev1/PKG-INFO
+-rw-r--r--   0        0        0     4732 2023-06-26 21:46:34.551133 databricks_sql_connector-2.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11346 2023-06-26 21:46:34.551133 databricks_sql_connector-2.7.0/LICENSE
+-rw-r--r--   0        0        0     2723 2023-06-26 21:46:34.551133 databricks_sql_connector-2.7.0/README.md
+-rw-r--r--   0        0        0     1588 2023-06-26 21:47:10.389497 databricks_sql_connector-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0      295 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/__init__.py
+-rw-r--r--   0        0        0     1269 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/auth/__init__.py
+-rw-r--r--   0        0        0     4421 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/auth/auth.py
+-rw-r--r--   0        0        0     6192 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/auth/authenticators.py
+-rw-r--r--   0        0        0     3790 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/auth/endpoint.py
+-rw-r--r--   0        0        0     9499 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/auth/oauth.py
+-rw-r--r--   0        0        0     1201 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/auth/oauth_http_handler.py
+-rw-r--r--   0        0        0     5949 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/auth/thrift_http_client.py
+-rw-r--r--   0        0        0    37645 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/client.py
+-rw-r--r--   0        0        0     2423 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/exc.py
+-rw-r--r--   0        0        0        0 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/experimental/__init__.py
+-rw-r--r--   0        0        0     2543 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/experimental/oauth_persistence.py
+-rwxr-xr-x   0        0        0     8062 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
+-rw-r--r--   0        0        0   136849 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
+-rw-r--r--   0        0        0       49 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/TCLIService/__init__.py
+-rw-r--r--   0        0        0     1307 2023-06-26 21:46:34.555133 databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/TCLIService/constants.py
+-rw-r--r--   0        0        0  2077276 2023-06-26 21:46:34.563134 databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/TCLIService/ttypes.py
+-rw-r--r--   0        0        0        0 2023-06-26 21:46:34.563134 databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/__init__.py
+-rw-r--r--   0        0        0    43174 2023-06-26 21:46:34.563134 databricks_sql_connector-2.7.0/src/databricks/sql/thrift_backend.py
+-rw-r--r--   0        0        0     6771 2023-06-26 21:46:34.563134 databricks_sql_connector-2.7.0/src/databricks/sql/types.py
+-rw-r--r--   0        0        0     6646 2023-06-26 21:46:34.563134 databricks_sql_connector-2.7.0/src/databricks/sql/utils.py
+-rw-r--r--   0        0        0       60 2023-06-26 21:46:34.563134 databricks_sql_connector-2.7.0/src/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     9761 2023-06-26 21:46:34.563134 databricks_sql_connector-2.7.0/src/databricks/sqlalchemy/dialect/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-26 21:46:34.563134 databricks_sql_connector-2.7.0/src/databricks/sqlalchemy/dialect/base.py
+-rw-r--r--   0        0        0      792 2023-06-26 21:46:34.563134 databricks_sql_connector-2.7.0/src/databricks/sqlalchemy/dialect/compiler.py
+-rw-r--r--   0        0        0     4107 1970-01-01 00:00:00.000000 databricks_sql_connector-2.7.0/PKG-INFO
```

### Comparing `databricks_sql_connector-2.6.3.dev1/CHANGELOG.md` & `databricks_sql_connector-2.7.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Release History
 
-## 2.6.x (Unreleased)
+## 2.7.x (Unreleased)
 
+## 2.7.0 (2023-06-26)
+
+- Fix: connector raised exception when calling close() on a closed Thrift session
+- Improve e2e test development ergonomics
 - Redact logged thrift responses by default
 - Add support for OAuth on Databricks Azure
 
 ## 2.6.2 (2023-06-14)
 
 - Fix: Retry GetOperationStatus requests for http errors
```

### Comparing `databricks_sql_connector-2.6.3.dev1/LICENSE` & `databricks_sql_connector-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.3.dev1/README.md` & `databricks_sql_connector-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.3.dev1/pyproject.toml` & `databricks_sql_connector-2.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-sql-connector"
-version = "2.6.3dev1"
+version = "2.7.0"
 description = "Databricks SQL Connector for Python"
 authors = ["Databricks <databricks-sql-connector-maintainers@databricks.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "databricks", from = "src"}]
 include = ["CHANGELOG.md"]
 
@@ -28,14 +28,15 @@
 alembic = "^1.0.11"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 mypy = "^0.950"
 pylint = ">=2.12.0"
 black = "^22.3.0"
+pytest-dotenv = "^0.5.2"
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/databricks/databricks-sql-python"
 "Bug Tracker" = "https://github.com/databricks/databricks-sql-python/issues"
 
 [tool.poetry.plugins."sqlalchemy.dialects"]
 "databricks" = "databricks.sqlalchemy:DatabricksDialect"
@@ -46,7 +47,18 @@
 
 [tool.mypy]
 ignore_missing_imports = "true"
 exclude = ['ttypes\.py$', 'TCLIService\.py$']
 
 [tool.black]
 exclude = '/(\.eggs|\.git|\.hg|\.mypy_cache|\.nox|\.tox|\.venv|\.svn|_build|buck-out|build|dist|thrift_api)/'
+
+[tool.pytest.ini_options]
+minversion = "6.0"
+log_cli = "false"
+log_cli_level = "INFO"
+testpaths = [
+    "tests"
+]
+env_files = [
+    "test.env"
+]
```

### Comparing `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/__init__.py` & `databricks_sql_connector-2.7.0/src/databricks/sql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 NUMBER = DBAPITypeObject(
     "boolean", "tinyint", "smallint", "int", "bigint", "float", "double", "decimal"
 )
 DATETIME = DBAPITypeObject("timestamp")
 DATE = DBAPITypeObject("date")
 ROWID = DBAPITypeObject()
 
-__version__ = "2.6.3dev1"
+__version__ = "2.7.0"
 USER_AGENT_NAME = "PyDatabricksSqlConnector"
 
 # These two functions are pyhive legacy
 Date = datetime.date
 Timestamp = datetime.datetime
```

### Comparing `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/auth.py` & `databricks_sql_connector-2.7.0/src/databricks/sql/auth/auth.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/authenticators.py` & `databricks_sql_connector-2.7.0/src/databricks/sql/auth/authenticators.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/endpoint.py` & `databricks_sql_connector-2.7.0/src/databricks/sql/auth/endpoint.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/oauth.py` & `databricks_sql_connector-2.7.0/src/databricks/sql/auth/oauth.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/oauth_http_handler.py` & `databricks_sql_connector-2.7.0/src/databricks/sql/auth/oauth_http_handler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/thrift_http_client.py` & `databricks_sql_connector-2.7.0/src/databricks/sql/auth/thrift_http_client.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/client.py` & `databricks_sql_connector-2.7.0/src/databricks/sql/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,15 +186,15 @@
             **kwargs,
         )
 
         self._session_handle = self.thrift_backend.open_session(
             session_configuration, catalog, schema
         )
         self.open = True
-        logger.info("Successfully opened session " + str(self.get_session_id()))
+        logger.info("Successfully opened session " + str(self.get_session_id_hex()))
         self._cursors = []  # type: List[Cursor]
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
@@ -210,14 +210,17 @@
             except OperationalError as e:
                 # Close on best-effort basis.
                 logger.debug("Couldn't close unclosed connection: {}".format(e.message))
 
     def get_session_id(self):
         return self.thrift_backend.handle_to_id(self._session_handle)
 
+    def get_session_id_hex(self):
+        return self.thrift_backend.handle_to_hex_id(self._session_handle)
+
     def cursor(
         self,
         arraysize: int = DEFAULT_ARRAY_SIZE,
         buffer_size_bytes: int = DEFAULT_RESULT_BUFFER_SIZE_BYTES,
     ) -> "Cursor":
         """
         Return a new Cursor object using the connection.
@@ -240,15 +243,33 @@
         """Close the underlying session and mark all associated cursors as closed."""
         self._close()
 
     def _close(self, close_cursors=True) -> None:
         if close_cursors:
             for cursor in self._cursors:
                 cursor.close()
-        self.thrift_backend.close_session(self._session_handle)
+
+        logger.info(f"Closing session {self.get_session_id_hex()}")
+        if not self.open:
+            logger.debug("Session appears to have been closed already")
+
+        try:
+            self.thrift_backend.close_session(self._session_handle)
+        except DatabaseError as e:
+            if "Invalid SessionHandle" in str(e):
+                logger.warning(
+                    f"Attempted to close session that was already closed: {e}"
+                )
+            else:
+                logger.warning(
+                    f"Attempt to close session raised an exception at the server: {e}"
+                )
+        except Exception as e:
+            logger.error(f"Attempt to close session raised a local exception: {e}")
+
         self.open = False
 
     def commit(self):
         """No-op because Databricks does not support transactions"""
         pass
 
     def rollback(self):
```

### Comparing `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/exc.py` & `databricks_sql_connector-2.7.0/src/databricks/sql/exc.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/experimental/oauth_persistence.py` & `databricks_sql_connector-2.7.0/src/databricks/sql/experimental/oauth_persistence.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote` & `databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService.py` & `databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/TCLIService/TCLIService.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/TCLIService/constants.py` & `databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/TCLIService/constants.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/TCLIService/ttypes.py` & `databricks_sql_connector-2.7.0/src/databricks/sql/thrift_api/TCLIService/ttypes.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_backend.py` & `databricks_sql_connector-2.7.0/src/databricks/sql/thrift_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from decimal import Decimal
 import errno
 import logging
 import math
 import time
+import uuid
 import threading
 import lz4.frame
 from ssl import CERT_NONE, CERT_REQUIRED, create_default_context
 from typing import List, Union
 
 import pyarrow
 import thrift.transport.THttpClient
@@ -1017,7 +1018,12 @@
         logger.debug("Cancelling command {}".format(active_op_handle.operationId.guid))
         req = ttypes.TCancelOperationReq(active_op_handle)
         self.make_request(self._client.CancelOperation, req)
 
     @staticmethod
     def handle_to_id(session_handle):
         return session_handle.sessionId.guid
+
+    @staticmethod
+    def handle_to_hex_id(session_handle: TCLIService.TSessionHandle):
+        this_uuid = uuid.UUID(bytes=session_handle.sessionId.guid)
+        return str(this_uuid)
```

### Comparing `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/types.py` & `databricks_sql_connector-2.7.0/src/databricks/sql/types.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/utils.py` & `databricks_sql_connector-2.7.0/src/databricks/sql/utils.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.3.dev1/src/databricks/sqlalchemy/dialect/__init__.py` & `databricks_sql_connector-2.7.0/src/databricks/sqlalchemy/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.3.dev1/src/databricks/sqlalchemy/dialect/compiler.py` & `databricks_sql_connector-2.7.0/src/databricks/sqlalchemy/dialect/compiler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.3.dev1/PKG-INFO` & `databricks_sql_connector-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sql-connector
-Version: 2.6.3.dev1
+Version: 2.7.0
 Summary: Databricks SQL Connector for Python
 License: Apache-2.0
 Author: Databricks
 Author-email: databricks-sql-connector-maintainers@databricks.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

