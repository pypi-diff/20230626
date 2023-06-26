# Comparing `tmp/orbit_database-1.0.0.tar.gz` & `tmp/orbit_database-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_database-1.0.0.tar", max compression
+gzip compressed data, was "orbit_database-1.0.1.tar", max compression
```

## Comparing `orbit_database-1.0.0.tar` & `orbit_database-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rwxr-xr-x   0        0        0     1087 2023-06-09 10:34:34.878082 orbit_database-1.0.0/LICENSE
--rw-r--r--   0        0        0     4506 2023-06-09 10:34:34.878082 orbit_database-1.0.0/README.md
--rw-r--r--   0        0        0       46 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/README.md
--rwxr-xr-x   0        0        0     1932 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/__init__.py
--rw-r--r--   0        0        0     6369 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/audit.py
--rwxr-xr-x   0        0        0     2473 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/bitmap.py
--rw-r--r--   0        0        0     3542 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/catalog.py
--rwxr-xr-x   0        0        0    10513 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/compression.py
--rwxr-xr-x   0        0        0     1880 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/cursor.py
--rwxr-xr-x   0        0        0    15912 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/database.py
--rwxr-xr-x   0        0        0     5360 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/decorators.py
--rwxr-xr-x   0        0        0    10044 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/doc.py
--rwxr-xr-x   0        0        0     1104 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/exceptions.py
--rwxr-xr-x   0        0        0     3322 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/filterresult.py
--rwxr-xr-x   0        0        0    10506 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/index.py
--rwxr-xr-x   0        0        0    15546 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/invertedwordindex.py
--rwxr-xr-x   0        0        0     2924 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/manager.py
--rwxr-xr-x   0        0        0    14240 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/metadata.py
--rwxr-xr-x   0        0        0     4432 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/objectid.py
--rwxr-xr-x   0        0        0     6864 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/serialiser.py
--rwxr-xr-x   0        0        0    41987 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/table.py
--rwxr-xr-x   0        0        0      387 2023-06-09 10:34:34.882082 orbit_database-1.0.0/orbit_database/types_.py
--rw-r--r--   0        0        0     1570 2023-06-09 10:34:34.886081 orbit_database-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5530 1970-01-01 00:00:00.000000 orbit_database-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1087 2023-06-09 10:34:34.878082 orbit_database-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4506 2023-06-09 10:34:34.878082 orbit_database-1.0.1/README.md
+-rw-r--r--   0        0        0       46 2023-06-09 10:34:34.882082 orbit_database-1.0.1/orbit_database/README.md
+-rwxr-xr-x   0        0        0     1932 2023-06-26 15:41:12.993580 orbit_database-1.0.1/orbit_database/__init__.py
+-rw-r--r--   0        0        0     6369 2023-06-09 10:34:34.882082 orbit_database-1.0.1/orbit_database/audit.py
+-rwxr-xr-x   0        0        0     2473 2023-06-09 10:34:34.882082 orbit_database-1.0.1/orbit_database/bitmap.py
+-rw-r--r--   0        0        0     3653 2023-06-17 15:47:18.989970 orbit_database-1.0.1/orbit_database/catalog.py
+-rwxr-xr-x   0        0        0    10513 2023-06-09 10:34:34.882082 orbit_database-1.0.1/orbit_database/compression.py
+-rwxr-xr-x   0        0        0     1880 2023-06-09 10:34:34.882082 orbit_database-1.0.1/orbit_database/cursor.py
+-rwxr-xr-x   0        0        0    15912 2023-06-09 10:34:34.882082 orbit_database-1.0.1/orbit_database/database.py
+-rwxr-xr-x   0        0        0     5360 2023-06-09 10:34:34.882082 orbit_database-1.0.1/orbit_database/decorators.py
+-rwxr-xr-x   0        0        0    10044 2023-06-09 10:34:34.882082 orbit_database-1.0.1/orbit_database/doc.py
+-rwxr-xr-x   0        0        0     1104 2023-06-09 10:34:34.882082 orbit_database-1.0.1/orbit_database/exceptions.py
+-rwxr-xr-x   0        0        0     3322 2023-06-09 10:34:34.882082 orbit_database-1.0.1/orbit_database/filterresult.py
+-rwxr-xr-x   0        0        0    10506 2023-06-09 10:34:34.882082 orbit_database-1.0.1/orbit_database/index.py
+-rwxr-xr-x   0        0        0    15546 2023-06-09 10:34:34.882082 orbit_database-1.0.1/orbit_database/invertedwordindex.py
+-rwxr-xr-x   0        0        0     2924 2023-06-09 10:34:34.882082 orbit_database-1.0.1/orbit_database/manager.py
+-rwxr-xr-x   0        0        0    14240 2023-06-09 10:34:34.882082 orbit_database-1.0.1/orbit_database/metadata.py
+-rwxr-xr-x   0        0        0     4432 2023-06-09 10:34:34.882082 orbit_database-1.0.1/orbit_database/objectid.py
+-rwxr-xr-x   0        0        0     6864 2023-06-09 10:34:34.882082 orbit_database-1.0.1/orbit_database/serialiser.py
+-rwxr-xr-x   0        0        0    42013 2023-06-09 11:19:48.579067 orbit_database-1.0.1/orbit_database/table.py
+-rwxr-xr-x   0        0        0      387 2023-06-09 10:34:34.882082 orbit_database-1.0.1/orbit_database/types_.py
+-rw-r--r--   0        0        0     1586 2023-06-26 15:41:22.697373 orbit_database-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5525 1970-01-01 00:00:00.000000 orbit_database-1.0.1/PKG-INFO
```

### Comparing `orbit_database-1.0.0/LICENSE` & `orbit_database-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.0/README.md` & `orbit_database-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.0/orbit_database/__init__.py` & `orbit_database-1.0.1/orbit_database/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #####################################################################################
 #
 #  Copyright (c) 2020 - Mad Penguin Consulting Ltd
 #
 #####################################################################################
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 
 from orbit_database.manager import Manager
 from orbit_database.database import Database
 from orbit_database.table import Table
 from orbit_database.filterresult import FilterResult, MatchResult
 from orbit_database.index import Index
 from orbit_database.doc import Doc, JournalType
```

### Comparing `orbit_database-1.0.0/orbit_database/audit.py` & `orbit_database-1.0.1/orbit_database/audit.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.0/orbit_database/bitmap.py` & `orbit_database-1.0.1/orbit_database/bitmap.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.0/orbit_database/catalog.py` & `orbit_database-1.0.1/orbit_database/catalog.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 from lmdb import Transaction, NotFoundError
 from orbit_database.table import Table
 from orbit_database.doc import Doc
 from orbit_database.objectid import ObjectId
 from orbit_database.exceptions import NoSuchIndex
 from orbit_database.metadata import MetaData
 
+try:
+    from loguru import logger as log
+except Exception:
+    import logging as log
+
+
 class Catalog:
 
     @property
     def version (self):
         return self._version
 
     def __init__(self, version):
@@ -33,30 +39,30 @@
         if self._version == 2:
             self._table.delete(name, txn=txn)
 
     def drop_index (self, table_name, index_name, txn):
         if not table_name.startswith('@@') and self._version == 2:
             catalog = self._table.get(table_name, txn=txn)
             if not catalog or not catalog._indexes:
-                raise Exception(NotFoundError)
+                raise NotFoundError
             if index_name not in catalog._indexes:
-                raise Exception(NoSuchIndex)
+                raise NoSuchIndex
             catalog._indexes.pop(index_name)
             self._table.save(catalog, txn=txn)
 
     def indexes (self, name, txn):
         catalog = self._table.get(name, txn=txn)
         if catalog:
             for name in catalog._indexes or []:
                 yield name
 
     def ensure (self, table_name, index_name, iwx, txn):
         catalog = self._table.get(table_name, txn=txn)
         if not catalog:
-            raise Exception(NotFoundError)
+            raise NotFoundError
         if not catalog._indexes:
             catalog._indexes = {}
         if index_name not in catalog._indexes:
             if iwx:
                 catalog._indexes[index_name] = {
                     'iwx': True,
                     'lexicon': str(ObjectId()),
@@ -71,27 +77,30 @@
                 }
             self._table.save(catalog, txn=txn)
         return catalog
     
     def store_index (self, table_name, index_name, conf, txn=None):
         catalog = self._table.get(table_name, txn=txn)
         if not catalog:
-            raise Exception(NotFoundError)
+            raise NotFoundError
         if not catalog._indexes:
             catalog._indexes = {}
         catalog._indexes[index_name] = conf
         self._table.save(catalog, txn=txn)
 
     def get_metadata (self, table_name, index_name, txn=None):
         catalog = self._table.get(table_name, txn=txn)
         if not catalog:
-            raise Exception(NotFoundError)
+            raise NotFoundError
         if not catalog._indexes:
             catalog._indexes = {}
-        return catalog._indexes.get(index_name, {})
+        indexes = catalog._indexes.get(index_name)
+        if not indexes:
+            raise NotFoundError
+        return indexes
 
     def get_table_id (self, name, txn):
         doc = self._table.get(name)
         if not doc:
             doc = Doc({'id': str(ObjectId())}, oid=name)
             self._table.append(doc, txn=txn)
         return doc._id
```

### Comparing `orbit_database-1.0.0/orbit_database/compression.py` & `orbit_database-1.0.1/orbit_database/compression.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.0/orbit_database/cursor.py` & `orbit_database-1.0.1/orbit_database/cursor.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.0/orbit_database/database.py` & `orbit_database-1.0.1/orbit_database/database.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.0/orbit_database/decorators.py` & `orbit_database-1.0.1/orbit_database/decorators.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.0/orbit_database/doc.py` & `orbit_database-1.0.1/orbit_database/doc.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.0/orbit_database/exceptions.py` & `orbit_database-1.0.1/orbit_database/exceptions.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.0/orbit_database/filterresult.py` & `orbit_database-1.0.1/orbit_database/filterresult.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.0/orbit_database/index.py` & `orbit_database-1.0.1/orbit_database/index.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.0/orbit_database/invertedwordindex.py` & `orbit_database-1.0.1/orbit_database/invertedwordindex.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.0/orbit_database/manager.py` & `orbit_database-1.0.1/orbit_database/manager.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.0/orbit_database/metadata.py` & `orbit_database-1.0.1/orbit_database/metadata.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.0/orbit_database/objectid.py` & `orbit_database-1.0.1/orbit_database/objectid.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.0/orbit_database/serialiser.py` & `orbit_database-1.0.1/orbit_database/serialiser.py`

 * *Files identical despite different names*

### Comparing `orbit_database-1.0.0/orbit_database/table.py` & `orbit_database-1.0.1/orbit_database/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,16 +399,17 @@
         if self._database.index_version == 1:
             old_conf = self._meta.fetch_index(self.name, index_name, txn=transaction)
             if not old_conf._conf:
                 old_conf = {'key': Index.index_path(self.name, index_name)}
             else:
                 old_conf = old_conf._conf
         else:
-            old_conf = self._database._cat.get_metadata(self.name, index_name)
-            if not old_conf:
+            try:
+                old_conf = self._database._cat.get_metadata(self.name, index_name)
+            except NotFoundError:
                 old_conf = { 'key': str(ObjectId()) }
 
         new_conf = {
             'key': old_conf['key'],
             'dupsort': duplicates,
             'create': True,
             'func': func,
```

### Comparing `orbit_database-1.0.0/pyproject.toml` & `orbit_database-1.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit_database"
-version = "1.0.0"
+version = "1.0.1"
 description = "Database library for Python based on LMDB storage engine"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -20,15 +20,15 @@
 documentation = "https://gitlab.com/madpenguin/orbit-database"
 
 [project.urls]
 "Homepage" = "https://gitlab.com/madpenguin/orbit-database"
 "Bug Tracker" = "https://gitlab.com/madpenguin/orbit-database/-/issues"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.10"
 posix-ipc = "^1.1.1"
 lmdb = "^1.4.1"
 
 [tool.poetry.dev-dependencies]
 pipenv = "*"
 pytest = "*"
 pytest-cov = "*"
@@ -49,11 +49,12 @@
 pip = "^23.1"
 pytest-cov = "^4.0.0"
 coverage = "^7.2.3"
 coverage-badge = "^1.1.0"
 unittest2 = "^1.1.0"
 zstandard = "^0.21.0"
 python-snappy = "^0.6.1"
+tox = "^4.6.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `orbit_database-1.0.0/PKG-INFO` & `orbit_database-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: orbit-database
-Version: 1.0.0
+Version: 1.0.1
 Summary: Database library for Python based on LMDB storage engine
 Home-page: https://gitlab.com/madpenguin/orbit-database
 Keywords: database,nosql,lmdb
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

