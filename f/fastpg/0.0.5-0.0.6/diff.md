# Comparing `tmp/fastpg-0.0.5.tar.gz` & `tmp/fastpg-0.0.6.tar.gz`

## Comparing `fastpg-0.0.5.tar` & `fastpg-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,12 @@
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 fastpg-0.0.5/Makefile
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fastpg-0.0.5/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fastpg-0.0.5/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastpg-0.0.5/.ruff_cache/content/16e9276ce601f9d4
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 fastpg-0.0.5/.ruff_cache/content/1ab6d1f4b669f5fa
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastpg-0.0.5/.ruff_cache/content/2f4daf4fe347aac7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastpg-0.0.5/.ruff_cache/content/454c8a0d424ee8b4
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastpg-0.0.5/.ruff_cache/content/55a4dd45d1da5c6d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fastpg-0.0.5/.ruff_cache/content/82b86688b82b071e
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastpg-0.0.5/.ruff_cache/content/e1f19352ed1a2f17
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 fastpg-0.0.5/src/fastpg/__init__.py
--rw-r--r--   0        0        0     8329 2020-02-02 00:00:00.000000 fastpg-0.0.5/src/fastpg/core.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fastpg-0.0.5/src/fastpg/exceptions.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 fastpg-0.0.5/src/fastpg/utils.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fastpg-0.0.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 fastpg-0.0.5/LICENSE
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 fastpg-0.0.5/README.md
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 fastpg-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 fastpg-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 fastpg-0.0.6/Makefile
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fastpg-0.0.6/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fastpg-0.0.6/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 fastpg-0.0.6/src/fastpg/__init__.py
+-rw-r--r--   0        0        0     9581 2020-02-02 00:00:00.000000 fastpg-0.0.6/src/fastpg/core.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fastpg-0.0.6/src/fastpg/exceptions.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 fastpg-0.0.6/src/fastpg/utils.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fastpg-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 fastpg-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 fastpg-0.0.6/README.md
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 fastpg-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 fastpg-0.0.6/PKG-INFO
```

### Comparing `fastpg-0.0.5/src/fastpg/core.py` & `fastpg-0.0.6/src/fastpg/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 from collections.abc import Mapping
 from contextlib import asynccontextmanager
-from typing import Any, Iterator, List, Optional, Sequence, Tuple
+from typing import Any, Iterator, List, Optional, Sequence, Tuple, cast
 
 import asyncpg
 from asyncpg.pgproto.pgproto import UUID
 
 from .utils import compile_query, compile_value
 
 
@@ -68,15 +68,15 @@
             dsn = f"postgresql://{user}:{password}@{host}:{port}/{database}"
         self.dsn = dsn
         self.kwargs = kwargs
 
         self._force_rollback = force_rollback
 
         self._pool: asyncpg.Pool | None = None
-        self._global_connection: Connection | None = None
+        self._global_connection: asyncpg.Connection | None = None
 
     async def connect(self):
         if self._force_rollback:
             assert self._global_connection is None, "Database already connected"
             self._global_connection = await asyncpg.connect(self.dsn, **self.kwargs)
             return
 
@@ -97,24 +97,26 @@
             self._pool.terminate()
         self._pool = None
 
     @asynccontextmanager
     async def connection(self):
         if self._force_rollback:
             assert self._global_connection is not None, "Database is not connected"
-            conn = Connection(self._global_connection)
+            conn = Connection(self.dsn)
+            conn._connection = self._global_connection
             async with conn.transaction(force_rollback=True):
                 try:
                     yield conn
                 finally:
                     return
 
         assert self._pool is not None, "Database is not connected"
         _conn = await self._pool.acquire()
-        conn = Connection(_conn)
+        conn = Connection(self.dsn)
+        conn._connection = _conn
         try:
             yield conn
         finally:
             await self._pool.release(conn._connection)
 
     async def execute(self, query: str, values: Optional[dict] = None):
         assert self._pool is not None, "Database is not connected"
@@ -152,20 +154,48 @@
         async with self.connection() as conn:
             return await conn.copy_records_to_table(
                 table_name, records=records, columns=columns
             )
 
 
 class Connection:
-    def __init__(self, connection):
-        self._connection = connection
+    def __init__(
+        self,
+        dsn: str | None = None,
+        *,
+        user: str | None = None,
+        password: str | None = None,
+        host: str | None = None,
+        port: int | None = None,
+        database: str | None = None,
+    ):
+        if dsn is None:
+            assert user is not None, "Missing user (no DSN provided)"
+            assert password is not None, "Missing password (no DSN provided)"
+            assert host is not None, "Missing host (no DSN provided)"
+            assert port is not None, "Missing port (no DSN provided)"
+            dsn = f"postgresql://{user}:{password}@{host}:{port}/{database}"
+        self.dsn = dsn
+        self._connection: asyncpg.Connection | None = None
+
+    async def connect(self):
+        assert self._connection is None, "Connection already connected"
+        self._connection = cast(asyncpg.Connection, await asyncpg.connect(self.dsn))
 
     async def close(self, *, timeout: float | None = None):
+        assert self._connection is not None, "Connection is not connected"
         await self._connection.close(timeout=timeout)
 
+    async def __aenter__(self):
+        await self.connect()
+        return self
+
+    async def __aexit__(self, exc_type, exc_value, traceback):
+        await self.close()
+
     async def execute(self, query: str, values: Optional[dict] = None):
         assert self._connection is not None, "Connection is not acquired"
         compiled_query, ordered_values = compile_query(query, values)
         return await self._connection.execute(compiled_query, *ordered_values)
 
     async def execute_many(self, query: str, values: List[dict]):
         assert self._connection is not None, "Connection is not acquired"
@@ -217,14 +247,15 @@
             table_name,
             records=[[compile_value(v) for v in rec] for rec in records],
             columns=columns,
         )
 
     @asynccontextmanager
     async def transaction(self, *, force_rollback: bool = False):
+        assert self._connection is not None, "Connection is not connected"
         transaction = self._connection.transaction()
         await transaction.start()
         try:
             yield transaction
         except:
             await transaction.rollback()
             raise
```

### Comparing `fastpg-0.0.5/src/fastpg/utils.py` & `fastpg-0.0.6/src/fastpg/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import json
 import re
 from enum import Enum
 from typing import List
 from uuid import UUID
 
 
-
 def compile_value(value):
     if isinstance(value, dict):
         return json.dumps(value)
     elif isinstance(value, UUID):
         return str(value)
     elif isinstance(value, Enum):
         return value.value
     else:
         return value
 
 
 def compile_query(query: str, values: dict | List[dict] | None = None):
-
     if type(values) is None:
         return query, tuple()
 
     compiled_query = query
     ordered_values = []
 
     if type(values) is dict:
```

### Comparing `fastpg-0.0.5/LICENSE` & `fastpg-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastpg-0.0.5/README.md` & `fastpg-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fastpg-0.0.5/pyproject.toml` & `fastpg-0.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastpg"
-version = "0.0.5"
+version = "0.0.6"
 description = "A fast Postgres client library for Python"
 readme = "README.md"
 requires-python = ">=3.10.4"
 license = { text = 'MIT' }
 authors = [{ name = "Wayde Gilliam", email = "waydegilliam@gmail.com" }]
 keywords = ["python", "postgres", "asyncio", "asyncpg"]
 classifiers = [
@@ -28,11 +28,11 @@
 dependencies = ["asyncpg==0.27.0"]
 
 [project.urls]
 Homepage = "https://github.com/waydegg/fastpg"
 Source = "https://github.com/waydegg/fastpg"
 
 [project.optional-dependencies]
-dev = ["ruff", "ipdb", "ipython"]
+dev = ["black", "isort", "ipdb", "ipython"]
 
 [tool.ruff]
 line-length = 88
```

### Comparing `fastpg-0.0.5/PKG-INFO` & `fastpg-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastpg
-Version: 0.0.5
+Version: 0.0.6
 Summary: A fast Postgres client library for Python
 Project-URL: Homepage, https://github.com/waydegg/fastpg
 Project-URL: Source, https://github.com/waydegg/fastpg
 Author-email: Wayde Gilliam <waydegilliam@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: asyncio,asyncpg,postgres,python
@@ -19,17 +19,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10.4
 Requires-Dist: asyncpg==0.27.0
 Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
 Requires-Dist: ipdb; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
-Requires-Dist: ruff; extra == 'dev'
+Requires-Dist: isort; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # fastpg
 
 [![PyPI version](https://badge.fury.io/py/fastpg.svg)](https://pypi.org/project/fastpg/)
 
 A fast Postgres client library for Python.
```

