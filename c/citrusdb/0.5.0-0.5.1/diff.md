# Comparing `tmp/citrusdb-0.5.0.tar.gz` & `tmp/citrusdb-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citrusdb-0.5.0.tar", last modified: Sat Jun 24 14:36:20 2023, max compression
+gzip compressed data, was "citrusdb-0.5.1.tar", last modified: Mon Jun 26 18:40:38 2023, max compression
```

## Comparing `citrusdb-0.5.0.tar` & `citrusdb-0.5.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.197616 citrusdb-0.5.0/
--rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.5.0/LICENSE
--rw-r--r--   0 debabrata   (501) staff       (20)     2411 2023-06-24 14:36:20.197492 citrusdb-0.5.0/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)     1828 2023-06-19 14:22:45.000000 citrusdb-0.5.0/README.md
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.193707 citrusdb-0.5.0/citrusdb/
--rw-r--r--   0 debabrata   (501) staff       (20)      281 2023-06-16 18:28:46.000000 citrusdb-0.5.0/citrusdb/__init__.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.194869 citrusdb-0.5.0/citrusdb/api/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.0/citrusdb/api/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     4017 2023-06-19 15:43:59.000000 citrusdb-0.5.0/citrusdb/api/index.py
--rw-r--r--   0 debabrata   (501) staff       (20)     6915 2023-06-24 14:09:55.000000 citrusdb-0.5.0/citrusdb/api/local.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.195028 citrusdb-0.5.0/citrusdb/db/
--rw-r--r--   0 debabrata   (501) staff       (20)     1252 2023-06-19 18:42:45.000000 citrusdb-0.5.0/citrusdb/db/__init__.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.195276 citrusdb-0.5.0/citrusdb/db/index/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.0/citrusdb/db/index/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1605 2023-06-12 11:56:56.000000 citrusdb-0.5.0/citrusdb/db/index/hnswlib.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.195695 citrusdb-0.5.0/citrusdb/db/postgres/
--rw-r--r--   0 debabrata   (501) staff       (20)     5421 2023-06-24 11:27:51.000000 citrusdb-0.5.0/citrusdb/db/postgres/db.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1722 2023-06-24 12:19:41.000000 citrusdb-0.5.0/citrusdb/db/postgres/queries.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1533 2023-06-19 15:14:26.000000 citrusdb-0.5.0/citrusdb/db/postgres/query_builder.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.196243 citrusdb-0.5.0/citrusdb/db/sqlite/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-12 11:56:56.000000 citrusdb-0.5.0/citrusdb/db/sqlite/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     4116 2023-06-24 14:15:18.000000 citrusdb-0.5.0/citrusdb/db/sqlite/db.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1708 2023-06-24 13:50:46.000000 citrusdb-0.5.0/citrusdb/db/sqlite/queries.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1382 2023-06-19 15:10:21.000000 citrusdb-0.5.0/citrusdb/db/sqlite/query_builder.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.196529 citrusdb-0.5.0/citrusdb/embedding/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.0/citrusdb/embedding/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)      402 2023-05-15 17:55:08.000000 citrusdb-0.5.0/citrusdb/embedding/openai.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.196930 citrusdb-0.5.0/citrusdb/utils/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-12 11:56:56.000000 citrusdb-0.5.0/citrusdb/utils/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)      236 2023-06-19 15:39:24.000000 citrusdb-0.5.0/citrusdb/utils/types.py
--rw-r--r--   0 debabrata   (501) staff       (20)      663 2023-06-12 11:56:56.000000 citrusdb-0.5.0/citrusdb/utils/utils.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.194439 citrusdb-0.5.0/citrusdb.egg-info/
--rw-r--r--   0 debabrata   (501) staff       (20)     2411 2023-06-24 14:36:20.000000 citrusdb-0.5.0/citrusdb.egg-info/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)      792 2023-06-24 14:36:20.000000 citrusdb-0.5.0/citrusdb.egg-info/SOURCES.txt
--rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-06-24 14:36:20.000000 citrusdb-0.5.0/citrusdb.egg-info/dependency_links.txt
--rw-r--r--   0 debabrata   (501) staff       (20)       79 2023-06-24 14:36:20.000000 citrusdb-0.5.0/citrusdb.egg-info/requires.txt
--rw-r--r--   0 debabrata   (501) staff       (20)       20 2023-06-24 14:36:20.000000 citrusdb-0.5.0/citrusdb.egg-info/top_level.txt
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-24 14:36:20.197309 citrusdb-0.5.0/cloud-temp/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 10:48:15.000000 citrusdb-0.5.0/cloud-temp/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     2248 2023-06-16 13:03:05.000000 citrusdb-0.5.0/cloud-temp/index.py
--rw-r--r--   0 debabrata   (501) staff       (20)     2826 2023-06-16 18:18:23.000000 citrusdb-0.5.0/cloud-temp/main-pg.py
--rw-r--r--   0 debabrata   (501) staff       (20)      724 2023-06-24 14:34:53.000000 citrusdb-0.5.0/pyproject.toml
--rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-06-24 14:36:20.197646 citrusdb-0.5.0/setup.cfg
--rw-r--r--   0 debabrata   (501) staff       (20)      964 2023-06-24 14:35:05.000000 citrusdb-0.5.0/setup.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.524660 citrusdb-0.5.1/
+-rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.5.1/LICENSE
+-rw-r--r--   0 debabrata   (501) staff       (20)     2411 2023-06-26 18:40:38.524540 citrusdb-0.5.1/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)     1828 2023-06-19 14:22:45.000000 citrusdb-0.5.1/README.md
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.521252 citrusdb-0.5.1/citrusdb/
+-rw-r--r--   0 debabrata   (501) staff       (20)      281 2023-06-16 18:28:46.000000 citrusdb-0.5.1/citrusdb/__init__.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.522228 citrusdb-0.5.1/citrusdb/api/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.1/citrusdb/api/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     4017 2023-06-19 15:43:59.000000 citrusdb-0.5.1/citrusdb/api/index.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     7418 2023-06-26 18:09:39.000000 citrusdb-0.5.1/citrusdb/api/local.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.522365 citrusdb-0.5.1/citrusdb/db/
+-rw-r--r--   0 debabrata   (501) staff       (20)     1282 2023-06-26 15:57:37.000000 citrusdb-0.5.1/citrusdb/db/__init__.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.522624 citrusdb-0.5.1/citrusdb/db/index/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.1/citrusdb/db/index/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1605 2023-06-12 11:56:56.000000 citrusdb-0.5.1/citrusdb/db/index/hnswlib.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.523025 citrusdb-0.5.1/citrusdb/db/postgres/
+-rw-r--r--   0 debabrata   (501) staff       (20)     6929 2023-06-26 18:09:32.000000 citrusdb-0.5.1/citrusdb/db/postgres/db.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1771 2023-06-26 17:28:44.000000 citrusdb-0.5.1/citrusdb/db/postgres/queries.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1533 2023-06-19 15:14:26.000000 citrusdb-0.5.1/citrusdb/db/postgres/query_builder.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.523466 citrusdb-0.5.1/citrusdb/db/sqlite/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-12 11:56:56.000000 citrusdb-0.5.1/citrusdb/db/sqlite/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     5250 2023-06-26 15:54:34.000000 citrusdb-0.5.1/citrusdb/db/sqlite/db.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1742 2023-06-26 15:16:54.000000 citrusdb-0.5.1/citrusdb/db/sqlite/queries.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1382 2023-06-19 15:10:21.000000 citrusdb-0.5.1/citrusdb/db/sqlite/query_builder.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.523691 citrusdb-0.5.1/citrusdb/embedding/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.1/citrusdb/embedding/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      402 2023-05-15 17:55:08.000000 citrusdb-0.5.1/citrusdb/embedding/openai.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.524032 citrusdb-0.5.1/citrusdb/utils/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-12 11:56:56.000000 citrusdb-0.5.1/citrusdb/utils/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      236 2023-06-19 15:39:24.000000 citrusdb-0.5.1/citrusdb/utils/types.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1018 2023-06-26 15:48:25.000000 citrusdb-0.5.1/citrusdb/utils/utils.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.521857 citrusdb-0.5.1/citrusdb.egg-info/
+-rw-r--r--   0 debabrata   (501) staff       (20)     2411 2023-06-26 18:40:38.000000 citrusdb-0.5.1/citrusdb.egg-info/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)      792 2023-06-26 18:40:38.000000 citrusdb-0.5.1/citrusdb.egg-info/SOURCES.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-06-26 18:40:38.000000 citrusdb-0.5.1/citrusdb.egg-info/dependency_links.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)       79 2023-06-26 18:40:38.000000 citrusdb-0.5.1/citrusdb.egg-info/requires.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)       20 2023-06-26 18:40:38.000000 citrusdb-0.5.1/citrusdb.egg-info/top_level.txt
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-06-26 18:40:38.524371 citrusdb-0.5.1/cloud-temp/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 10:48:15.000000 citrusdb-0.5.1/cloud-temp/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     2248 2023-06-16 13:03:05.000000 citrusdb-0.5.1/cloud-temp/index.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     2826 2023-06-16 18:18:23.000000 citrusdb-0.5.1/cloud-temp/main-pg.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      724 2023-06-26 18:39:30.000000 citrusdb-0.5.1/pyproject.toml
+-rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-06-26 18:40:38.524691 citrusdb-0.5.1/setup.cfg
+-rw-r--r--   0 debabrata   (501) staff       (20)      964 2023-06-26 18:39:42.000000 citrusdb-0.5.1/setup.py
```

### Comparing `citrusdb-0.5.0/LICENSE` & `citrusdb-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.0/PKG-INFO` & `citrusdb-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citrusdb
-Version: 0.5.0
+Version: 0.5.1
 Summary: open-source vector database. store and retrieve embeddings for your next project!
 Home-page: https://github.com/0xDebabrata/citrus
 Author: Debabrata Mondal
 Author-email: Debabrata Mondal <debabrata.js@protonmail.com>
 Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: citrusdb Version: 0.5.0 Summary: open-source vector
+Metadata-Version: 2.1 Name: citrusdb Version: 0.5.1 Summary: open-source vector
 database. store and retrieve embeddings for your next project! Home-page:
 https://github.com/0xDebabrata/citrus Author: Debabrata Mondal Author-email:
 Debabrata Mondal
 js@protonmail.com> Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `citrusdb-0.5.0/README.md` & `citrusdb-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.0/citrusdb/api/index.py` & `citrusdb-0.5.1/citrusdb/api/index.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.0/citrusdb/api/local.py` & `citrusdb-0.5.1/citrusdb/api/local.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import enum
 import os
 import json
 from typing import Any, Dict, List, Optional
 from numpy import float32
 from numpy._typing import NDArray
 import shutil
 
@@ -27,15 +28,15 @@
         self._db = {}
         self.persist_directory = persist_directory
 
         if not(persist_directory) and os.path.isdir(self._TEMP_DIRECTORY):
             # Cleanup previous sqlite data
             shutil.rmtree(self._TEMP_DIRECTORY)
 
-        if persist_directory and database_type == "pg":
+        if persist_directory and (database_type == "pg" or database_type == "postgres"):
             self._SQLClient = PostgresDB(**kwargs)
         else:
             self._SQLClient = SQLiteDB(persist_directory if persist_directory else self._TEMP_DIRECTORY)
 
     def create_index(
         self,
         name: str,
@@ -176,37 +177,48 @@
 
     def query(
         self,
         index: str,
         documents: Optional[List[str]] = None,
         query_embeddings: Optional[NDArray[float32]] = None,
         k=1,
-        filters: Optional[List[Dict]] = None
+        filters: Optional[List[Dict]] = None,
+        include: List[str] = []
     ):
         allowed_ids = []
         if filters is not None:
             allowed_ids = self._SQLClient.filter_vectors(index, filters)
 
         filter_function = lambda label: label in allowed_ids
 
+        included_columns = {"id": True, "document": False, "metadata": False}
+        if "document" in include:
+            included_columns["document"] = True
+        if "metadata" in include:
+            included_columns["metadata"] = True
+
         flag = 1
         for key in self._db.keys():
             if key == index:
                 flag = 0
                 results, distances = self._db[key].query(
                     documents=documents,
                     query_embeddings=query_embeddings,
                     k=k,
                     filter_function=None if filters is None else filter_function
                 )
-                lolo_vector_ids = self._SQLClient.get_vector_ids_of_results(
+                elements = self._SQLClient.get_vector_ids_of_results(
                     name=index,
-                    results=results
+                    results=results,
+                    include=included_columns
                 )
-                return lolo_vector_ids, distances
+                for i, rows in enumerate(elements):
+                    for j, row in enumerate(rows):
+                        row["distance"] = distances[i][j]
+                return elements
 
         if flag:
             raise ValueError(f"Could not find index: {index}")
 
 
     def get_status(self, index: str):
         flag = 1
```

### Comparing `citrusdb-0.5.0/citrusdb/db/__init__.py` & `citrusdb-0.5.1/citrusdb/db/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,16 +40,17 @@
     ) -> Optional[Tuple[int, str, int, int, int, int, int, bool]]:
         pass
 
     @abstractmethod
     def get_vector_ids_of_results(
         self,
         name: str,
-        results: List[List[int]]
-    ) -> List[IDs]:
+        results: List[List[int]],
+        include: Dict
+    ) -> List[List[Dict]]:
         pass
 
     @abstractmethod
     def insert_to_index(
         self,
         data
     ) -> List[int]:
```

### Comparing `citrusdb-0.5.0/citrusdb/db/index/hnswlib.py` & `citrusdb-0.5.1/citrusdb/db/index/hnswlib.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.0/citrusdb/db/postgres/db.py` & `citrusdb-0.5.1/citrusdb/db/sqlite/db.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,181 +1,178 @@
-from psycopg_pool import ConnectionPool
-from typing import Any, Dict, List, Optional, Tuple
+import os
+import sqlite3
+from typing import Dict, List, Optional, Tuple
+
 from citrusdb.db import BaseDB
-import citrusdb.db.postgres.queries as queries
-from citrusdb.db.postgres.query_builder import QueryBuilder
 from citrusdb.utils.types import IDs
+from citrusdb.utils.utils import convert_row_to_dict, ensure_valid_path
+import citrusdb.db.sqlite.queries as queries
+from citrusdb.db.sqlite.query_builder import QueryBuilder
 
 
-class PostgresDB(BaseDB):
-    _pool: ConnectionPool
+class SQLiteDB(BaseDB):
+    _con: sqlite3.Connection
 
     def __init__(
         self,
-        **kwargs: Dict[str, Any]
+        persist_directory: str,
     ):
-        # Setup connection pool
-        self._pool = ConnectionPool(kwargs=kwargs)
+        ensure_valid_path(persist_directory)
 
-        # Create index_manager and index_data table if they don't exist already
-        with self._pool.connection() as conn:
-            with conn.cursor() as cur:
-                cur.execute(queries.CREATE_INDEX_MANAGER_TABLE)
-                cur.execute(queries.CREATE_INDEX_DATA_TABLE)
-                conn.commit()
+        self._con = sqlite3.connect(
+            os.path.join(
+                persist_directory, "citrus.db"
+            )
+        )
+
+        cur = self._con.cursor()
+        cur.execute("PRAGMA foreign_keys = ON")    # Enable foreign keys
+        cur.executescript(f'''
+        BEGIN;
+        {queries.CREATE_INDEX_MANAGER_TABLE}
+        {queries.CREATE_INDEX_DATA_TABLE}
+        END;
+        ''')
+        cur.close()
 
     def create_index(
         self,
         name: str,
         max_elements: int,
         M: int,
         ef_construction: int,
         allow_replace_deleted: bool,
         dimensions: Optional[int] = 1536,
     ):
+        cur = self._con.cursor()
         ef = ef_construction
         parameters = (name, dimensions, max_elements, M, ef, ef_construction, allow_replace_deleted)
-        # Create new index entry to postgres db
-        with self._pool.connection() as conn:
-            with conn.cursor() as cur:
-                cur.execute(queries.INSERT_INDEX_TO_MANAGER, parameters)
-                conn.commit()
+        cur.execute(queries.INSERT_INDEX_TO_MANAGER, parameters)
+        self._con.commit()
+        cur.close()
 
     def delete_vectors_from_index(
         self,
         index_id: int,
         ids: IDs
     ):
-        """
-        Delete vectors with given list of IDs from specific index
-
-        index_id: ID of index where the elements belong
-        ids: List of IDs to be deleted
-        """
-
-        vector_ids = []
-        parameters = (tuple(ids), index_id)
-        with self._pool.connection() as conn:
-            with conn.cursor() as cur:
-                for vector_id in cur.execute(queries.DELETE_VECTORS_FROM_INDEX, parameters):
-                    vector_ids.append(vector_id)
-                conn.commit()
+        cur = self._con.cursor()
+        query = queries.DELETE_VECTORS_FROM_INDEX.format(", ".join("?" * len(ids)))
+        parameters = tuple(ids) + (index_id,)
+        cur.execute(query, parameters)
+
+        rows = cur.fetchall()
+        self._con.commit()
+        cur.close()
 
+        vector_ids = [row[0] for row in rows]
         return vector_ids
 
     def filter_vectors(self, index_name: str, filters: List[Dict]):
-        """
-        Get list of IDs of vectors that match filters.
-
-        index_name: Name of index where the elements belong
-        filters: List of filters to be applied
-        """
-
-        with self._pool.connection() as conn:
-            query_builder = QueryBuilder(conn)
-            res = query_builder.execute_query(index_name, filters)
-            allowed_ids = []
-            for row in res:
-                allowed_ids.append(row[0])
-            return allowed_ids
+        query_builder = QueryBuilder(self._con)
+        res = query_builder.execute_query(index_name, filters)
+        allowed_ids = []
+        for row in res:
+            allowed_ids.append(row[0])
+        return allowed_ids
 
     def get_indices(self):
         """
-        Get all index details
+        Fetch all index details from index_manager table.
+        Returns a list of tuples where each one corresponds to an index.
         """
-        with self._pool.connection() as conn:
-            with conn.cursor() as cur:
-                cur.execute(queries.GET_ALL_INDEX_DETAILS)
-                return cur.fetchall()
+
+        cur = self._con.cursor()
+        res = cur.execute(queries.GET_ALL_INDEX_DETAILS)
+        rows = res.fetchall()
+        cur.close()
+        return rows
 
     def get_index_details(
         self,
         name: str
     ) -> Optional[Tuple[int, str, int, int, int, int, int, bool]]:
-        """
-        Get specific index details
-
-        name: Name of index to fetch
-        """
+        cur = self._con.cursor()
         parameters = (name,)
-        with self._pool.connection() as conn:
-            with conn.cursor() as cur:
-                cur.execute(queries.GET_INDEX_DETAILS_BY_NAME, parameters)
-                return cur.fetchone()
+        res = cur.execute(queries.GET_INDEX_DETAILS_BY_NAME, parameters)
+        row = res.fetchone()
+        cur.close()
+        return row
 
     def get_vector_ids_of_results(
         self,
         name: str,
-        results: List[List[int]]
-    ):
-        """
-        Get user facing IDs of results
-
-        name: Name of index
-        results: List of list of integer HNSW labels
-        """
-        lolo_vector_ids = []
+        results: List[List[int]],
+        include: Dict
+    ) -> List[List[Dict]]:
+        cols = "id"
+        if include["document"]:
+            cols += ", text"
+            if include["metadata"]:
+                cols += ", metadata"
+        elif include["metadata"]:
+            cols += ", metadata"
 
+        returning_list = []
         index_details = self.get_index_details(name)
-        if not(index_details):
-            return
-        index_id = index_details[0]
-
-        with self._pool.connection() as conn:
-            with conn.cursor() as cur:
-                data = ()
-                for ids in results:
-                    ids_tuple = tuple(ids)
-                    data = data + (ids_tuple, index_id)
-
-                cur.executemany(
-                    queries.GET_VECTOR_IDS_OF_RESULTS,
-                    data,                                       # type: ignore
-                    returning=True
-                )
-                while True:
-                    lolo_vector_ids.append(cur.fetchone())      # type: ignore
-                    if not cur.nextset():
-                        break;
+        index_id = index_details[0]                 # type: ignore
+
+        cur = self._con.cursor()
+        for ids in results:
+            query = queries.GET_VECTOR_IDS_OF_RESULTS.format(cols, ", ".join("?" * len(ids)))
+            parameters = ()
+            for id in ids:
+                parameters += (int(id),)
+            parameters += (index_id,)
+            res = cur.execute(query, parameters)
+            unordered_rows = res.fetchall()         # Rows not ordered according to similarity score
+
+            # Order rows according to order of id in ids list
+            ordered_rows = []
+            for id in ids:
+                low = 0; high = len(unordered_rows) - 1
+                while (low <= high):
+                    mid = low + (high - low)//2
+                    curr_vector_id = unordered_rows[mid][0]
+                    if curr_vector_id == id:
+                        ordered_rows.append(
+                            convert_row_to_dict(
+                                row=unordered_rows[mid],
+                                include=include
+                            )
+                        )
+                        break
+                    elif curr_vector_id < id:
+                        low = mid + 1
+                    else:
+                        high = mid - 1
 
-                conn.commit()
+            returning_list.append(ordered_rows)
+        cur.close()
 
-        return lolo_vector_ids
+        return returning_list
 
     def insert_to_index(
         self,
         data
     ):
-        """
-        Insert vectors to index
-
-        data: Tuple of tuples corresponding to each row
-        """
+        cur = self._con.cursor()
         vector_ids = []
-        with self._pool.connection() as conn:
-            with conn.cursor() as cur:
-                cur.executemany(queries.INSERT_DATA_TO_INDEX, data, returning=True)
-                while True:
-                    vector_ids.append(cur.fetchone()[0])        # type: ignore
-                    if not cur.nextset():
-                        break;
+        for row in data:
+            res = cur.execute(queries.INSERT_DATA_TO_INDEX, row)
+            vector_ids.append(res.fetchone()[0])
 
-                conn.commit()
+        self._con.commit()
+        cur.close()
 
         return vector_ids
 
     def update_ef(
         self,
         name: str,
         ef: int
     ):
-        """
-        Update ef for an index
-
-        name: Name of index to be updated
-        ef: New ef value
-        """
+        cur = self._con.cursor()
         parameters = (ef, name)
-        with self._pool.connection() as conn:
-            with conn.cursor() as cur:
-                cur.execute(queries.UPDATE_EF, parameters)
-                conn.commit()
+        cur.execute(queries.UPDATE_EF, parameters)
+        self._con.commit()
+        cur.close()
```

### Comparing `citrusdb-0.5.0/citrusdb/db/postgres/queries.py` & `citrusdb-0.5.1/citrusdb/db/postgres/queries.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     UNIQUE(id, index_id),
     FOREIGN KEY(index_id) REFERENCES index_manager(index_id) ON DELETE CASCADE
 );
 '''
 
 DELETE_VECTORS_FROM_INDEX = '''
 DELETE FROM index_data
-WHERE id IN %s AND index_id = %s
+WHERE id = ANY(%s) AND index_id = %s
 RETURNING vector_id
 '''
 
 GET_ALL_INDEX_DETAILS = '''
 SELECT index_id, name, dimensions, max_elements, m, ef, ef_construction, allow_replace_deleted
 FROM index_manager
 '''
@@ -38,17 +38,18 @@
 GET_INDEX_DETAILS_BY_NAME = '''
 SELECT index_id, name, dimensions, max_elements, m, ef, ef_construction, allow_replace_deleted
 FROM index_manager
 WHERE name = %s
 '''
 
 GET_VECTOR_IDS_OF_RESULTS = '''
-SELECT id
+SELECT vector_id, {}
 FROM index_data
-WHERE id IN %s AND index_id = %s
+WHERE vector_id = ANY(%s) AND index_id = %s
+ORDER BY vector_id ASC
 '''
 
 INSERT_DATA_TO_INDEX = '''
 INSERT INTO index_data
 (id, index_id, text, embedding, metadata)
 VALUES(%s, %s, %s, %s, %s)
 ON CONFLICT(id, index_id)
```

### Comparing `citrusdb-0.5.0/citrusdb/db/postgres/query_builder.py` & `citrusdb-0.5.1/citrusdb/db/postgres/query_builder.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.0/citrusdb/db/sqlite/queries.py` & `citrusdb-0.5.1/citrusdb/db/sqlite/queries.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,17 +38,18 @@
 GET_INDEX_DETAILS_BY_NAME = '''
 SELECT index_id, name, dimensions, max_elements, m, ef, ef_construction, allow_replace_deleted
 FROM index_manager
 WHERE name = ?
 '''
 
 GET_VECTOR_IDS_OF_RESULTS = '''
-SELECT id
+SELECT vector_id, {}
 FROM index_data
 WHERE vector_id IN ({}) AND index_id = ?
+ORDER BY vector_id ASC
 '''
 
 INSERT_DATA_TO_INDEX = '''
 INSERT INTO index_data
 (id, index_id, text, embedding, metadata)
 VALUES(?, ?, ?, ?, ?)
 ON CONFLICT(id, index_id)
```

### Comparing `citrusdb-0.5.0/citrusdb/db/sqlite/query_builder.py` & `citrusdb-0.5.1/citrusdb/db/sqlite/query_builder.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.0/citrusdb/utils/utils.py` & `citrusdb-0.5.1/citrusdb/utils/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 import os
-from typing import Optional
+from typing import Dict, Optional, Tuple
+
+def convert_row_to_dict(row: Tuple, include: Dict):
+    returning_dict = {"id": row[1]}
+    if include["document"]:
+        returning_dict["document"] = row[2]
+        if include["metadata"]:
+            returning_dict["metadata"] = row[3]
+    elif include["metadata"]:
+        returning_dict["metadata"] = row[2]
+
+    return returning_dict
 
 def ensure_valid_path(persist_directory: str, file_name: Optional[str] = None) -> bool:
     """
     Creates required directories if they do not exist.
 
     If only persist_directory is passed, returns True.
     When file_name is passed, function returns boolean based on whether the
```

### Comparing `citrusdb-0.5.0/citrusdb.egg-info/PKG-INFO` & `citrusdb-0.5.1/citrusdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citrusdb
-Version: 0.5.0
+Version: 0.5.1
 Summary: open-source vector database. store and retrieve embeddings for your next project!
 Home-page: https://github.com/0xDebabrata/citrus
 Author: Debabrata Mondal
 Author-email: Debabrata Mondal <debabrata.js@protonmail.com>
 Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: citrusdb Version: 0.5.0 Summary: open-source vector
+Metadata-Version: 2.1 Name: citrusdb Version: 0.5.1 Summary: open-source vector
 database. store and retrieve embeddings for your next project! Home-page:
 https://github.com/0xDebabrata/citrus Author: Debabrata Mondal Author-email:
 Debabrata Mondal
 js@protonmail.com> Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `citrusdb-0.5.0/citrusdb.egg-info/SOURCES.txt` & `citrusdb-0.5.1/citrusdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.0/cloud-temp/index.py` & `citrusdb-0.5.1/cloud-temp/index.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.0/cloud-temp/main-pg.py` & `citrusdb-0.5.1/cloud-temp/main-pg.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.0/pyproject.toml` & `citrusdb-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "citrusdb"
-version = "0.5.0"
+version = "0.5.1"
 
 authors = [
   { name="Debabrata Mondal", email="debabrata.js@protonmail.com" },
 ]
 description = "open-source vector database. store and retrieve embeddings for your next project!"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `citrusdb-0.5.0/setup.py` & `citrusdb-0.5.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="citrusdb",
-    version="0.5.0",
+    version="0.5.1",
     author="Debabrata Mondal",
     author_email="debabrata.js@protonmail.com",
     description="(distributed) vector database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/0xDebabrata/citrus",
     packages=(
```

