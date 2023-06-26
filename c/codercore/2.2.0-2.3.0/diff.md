# Comparing `tmp/codercore-2.2.0.tar.gz` & `tmp/codercore-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codercore-2.2.0.tar", last modified: Tue May 30 12:19:58 2023, max compression
+gzip compressed data, was "codercore-2.3.0.tar", last modified: Mon Jun 26 15:07:49 2023, max compression
```

## Comparing `codercore-2.2.0.tar` & `codercore-2.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:19:58.300785 codercore-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-30 12:19:58.300785 codercore-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 12:19:30.000000 codercore-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:19:58.296785 codercore-2.2.0/codercore/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-30 12:19:30.000000 codercore-2.2.0/codercore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:19:58.296785 codercore-2.2.0/codercore/db/
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-30 12:19:30.000000 codercore-2.2.0/codercore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-30 12:19:30.000000 codercore-2.2.0/codercore/db/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-30 12:19:30.000000 codercore-2.2.0/codercore/db/pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:19:58.300785 codercore-2.2.0/codercore/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-30 12:19:30.000000 codercore-2.2.0/codercore/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-30 12:19:30.000000 codercore-2.2.0/codercore/lib/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-30 12:19:30.000000 codercore-2.2.0/codercore/lib/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-30 12:19:30.000000 codercore-2.2.0/codercore/lib/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:19:58.300785 codercore-2.2.0/codercore/lib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:19:30.000000 codercore-2.2.0/codercore/lib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-30 12:19:30.000000 codercore-2.2.0/codercore/lib/schemas/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-30 12:19:30.000000 codercore-2.2.0/codercore/lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 12:19:30.000000 codercore-2.2.0/codercore/lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:19:58.300785 codercore-2.2.0/codercore/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:19:30.000000 codercore-2.2.0/codercore/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-30 12:19:30.000000 codercore-2.2.0/codercore/test/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-30 12:19:30.000000 codercore-2.2.0/codercore/test/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-30 12:19:30.000000 codercore-2.2.0/codercore/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:19:58.296785 codercore-2.2.0/codercore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-30 12:19:58.000000 codercore-2.2.0/codercore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-30 12:19:58.000000 codercore-2.2.0/codercore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:19:58.000000 codercore-2.2.0/codercore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-30 12:19:58.000000 codercore-2.2.0/codercore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 12:19:58.000000 codercore-2.2.0/codercore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-30 12:19:30.000000 codercore-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 12:19:58.300785 codercore-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:19:58.300785 codercore-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-30 12:19:30.000000 codercore-2.2.0/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:49.303639 codercore-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-26 15:07:49.303639 codercore-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 15:07:23.000000 codercore-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:49.299639 codercore-2.3.0/codercore/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:49.299639 codercore-2.3.0/codercore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/db/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/db/pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:49.303639 codercore-2.3.0/codercore/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/lib/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/lib/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/lib/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:49.303639 codercore-2.3.0/codercore/lib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/lib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/lib/schemas/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:49.303639 codercore-2.3.0/codercore/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/test/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/test/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-26 15:07:23.000000 codercore-2.3.0/codercore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:49.299639 codercore-2.3.0/codercore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-26 15:07:49.000000 codercore-2.3.0/codercore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-26 15:07:49.000000 codercore-2.3.0/codercore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:07:49.000000 codercore-2.3.0/codercore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-26 15:07:49.000000 codercore-2.3.0/codercore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 15:07:49.000000 codercore-2.3.0/codercore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-26 15:07:23.000000 codercore-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:07:49.303639 codercore-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:07:49.303639 codercore-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-26 15:07:23.000000 codercore-2.3.0/tests/test_types.py
```

### Comparing `codercore-2.2.0/codercore/db/__init__.py` & `codercore-2.3.0/codercore/db/__init__.py`

 * *Files identical despite different names*

### Comparing `codercore-2.2.0/codercore/db/pagination.py` & `codercore-2.3.0/codercore/db/pagination.py`

 * *Files identical despite different names*

### Comparing `codercore-2.2.0/codercore/lib/hash.py` & `codercore-2.3.0/codercore/lib/hash.py`

 * *Files identical despite different names*

### Comparing `codercore-2.2.0/codercore/lib/redis.py` & `codercore-2.3.0/codercore/lib/redis.py`

 * *Files identical despite different names*

### Comparing `codercore-2.2.0/codercore/lib/settings.py` & `codercore-2.3.0/codercore/lib/settings.py`

 * *Files identical despite different names*

### Comparing `codercore-2.2.0/codercore/test/fixtures.py` & `codercore-2.3.0/codercore/test/fixtures.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections.abc import AsyncIterator
+from contextlib import asynccontextmanager
 from typing import Awaitable, Callable
 
 from pytest import FixtureRequest
 from sqlalchemy import MetaData
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.orm import sessionmaker as sessionmaker_
 from sqlalchemy.pool import NullPool
@@ -67,23 +68,34 @@
             return
 
         drop_database(sync_db_connection_url)
 
     request.addfinalizer(cleanup)
 
 
-async def redis_connection_maker(
+@asynccontextmanager
+async def _redis_connection_maker(
     worker_id: str,
-) -> AsyncIterator[Callable[[], Awaitable[Redis]]]:
+) -> AsyncIterator[Awaitable[Redis]]:
     async def redis_connection() -> Redis:
         return connection.__wrapped__(db=int(worker_id[2:]), **EnvSettings.redis)
 
-    yield redis_connection
-    redis = await redis_connection()
-    await redis.flushdb()
-    await redis.close()
+    try:
+        conn = await redis_connection()
+        yield conn
+    finally:
+        await conn.flushdb()
+        await conn.close()
+
+
+async def redis_connection_maker(
+    worker_id: str,
+) -> Callable[[], AsyncIterator[Awaitable[Redis]]]:
+    return _redis_connection_maker
 
 
 async def redis_connection(
-    redis_connection_maker: Callable[[], Awaitable[Redis]]
+    redis_connection_maker: Callable[[], Awaitable[Redis]],
+    worker_id: str,
 ) -> Redis:
-    return await redis_connection_maker()
+    async with redis_connection_maker(worker_id) as conn:
+        return conn
```

### Comparing `codercore-2.2.0/codercore/test/pydantic.py` & `codercore-2.3.0/codercore/test/pydantic.py`

 * *Files identical despite different names*

### Comparing `codercore-2.2.0/codercore.egg-info/SOURCES.txt` & `codercore-2.3.0/codercore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codercore-2.2.0/pyproject.toml` & `codercore-2.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "codercore"
-version = "2.2.0"
+version = "2.3.0"
 description = "codercore"
 readme = "README.md"
 authors = [{ name = "Code R", email = "hello@coderstudio.dev" }]
 dependencies = [
     'asyncpg ~= 0.27',
     'asyncstdlib ~= 3.10',
     'bcrypt ~= 4.0',
@@ -31,15 +31,15 @@
 dev = [
     'black ~= 22.10',
     'flake8 ~= 6.0',
     'isort ~= 5.11',
 ]
 
 [tool.bumpver]
-current_version = "2.2.0"
+current_version = "2.3.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

