# Comparing `tmp/piicatcher-0.9.5.tar.gz` & `tmp/piicatcher-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/piicatcher-0.9.5.tar", last modified: Mon Mar 23 06:07:57 2020, max compression
+gzip compressed data, was "dist/piicatcher-0.9.6.tar", last modified: Mon Apr  6 07:11:04 2020, max compression
```

## Comparing `piicatcher-0.9.5.tar` & `piicatcher-0.9.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-03-23 06:07:57.000000 piicatcher-0.9.5/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       42 2020-03-23 06:06:53.000000 piicatcher-0.9.5/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4367 2020-03-23 06:07:57.000000 piicatcher-0.9.5/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3070 2020-03-23 06:06:53.000000 piicatcher-0.9.5/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-03-23 06:07:57.000000 piicatcher-0.9.5/piicatcher/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2020-03-23 06:06:53.000000 piicatcher-0.9.5/piicatcher/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-03-23 06:07:57.000000 piicatcher-0.9.5/piicatcher/catalog/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      184 2020-03-23 06:06:53.000000 piicatcher-0.9.5/piicatcher/catalog/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2143 2020-03-23 06:06:53.000000 piicatcher-0.9.5/piicatcher/catalog/db.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      510 2020-03-23 06:06:53.000000 piicatcher-0.9.5/piicatcher/catalog/file.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2985 2020-03-23 06:06:53.000000 piicatcher-0.9.5/piicatcher/catalog/glue.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      330 2020-03-23 06:06:53.000000 piicatcher-0.9.5/piicatcher/catalog/pii_type_field.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1899 2020-03-23 06:06:53.000000 piicatcher-0.9.5/piicatcher/command_line.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-03-23 06:07:57.000000 piicatcher-0.9.5/piicatcher/explorer/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-03-23 06:06:53.000000 piicatcher-0.9.5/piicatcher/explorer/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5038 2020-03-23 06:06:53.000000 piicatcher-0.9.5/piicatcher/explorer/aws.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10281 2020-03-23 06:06:53.000000 piicatcher-0.9.5/piicatcher/explorer/databases.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7785 2020-03-23 06:06:53.000000 piicatcher-0.9.5/piicatcher/explorer/explorer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4078 2020-03-23 06:06:53.000000 piicatcher-0.9.5/piicatcher/explorer/files.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4946 2020-03-23 06:06:53.000000 piicatcher-0.9.5/piicatcher/explorer/metadata.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3993 2020-03-23 06:06:53.000000 piicatcher-0.9.5/piicatcher/explorer/sqlite.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      177 2020-03-23 06:06:53.000000 piicatcher-0.9.5/piicatcher/log_mixin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      986 2020-03-23 06:06:53.000000 piicatcher-0.9.5/piicatcher/piitypes.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3322 2020-03-23 06:06:53.000000 piicatcher-0.9.5/piicatcher/scanner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      350 2020-03-23 06:06:53.000000 piicatcher-0.9.5/piicatcher/tokenizer.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-03-23 06:07:57.000000 piicatcher-0.9.5/piicatcher.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4367 2020-03-23 06:07:57.000000 piicatcher-0.9.5/piicatcher.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      768 2020-03-23 06:07:57.000000 piicatcher-0.9.5/piicatcher.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-03-23 06:07:57.000000 piicatcher-0.9.5/piicatcher.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2020-03-23 06:07:57.000000 piicatcher-0.9.5/piicatcher.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      189 2020-03-23 06:07:57.000000 piicatcher-0.9.5/piicatcher.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       11 2020-03-23 06:07:57.000000 piicatcher-0.9.5/piicatcher.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      212 2020-03-23 06:06:53.000000 piicatcher-0.9.5/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      108 2020-03-23 06:07:57.000000 piicatcher-0.9.5/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2474 2020-03-23 06:06:53.000000 piicatcher-0.9.5/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-04-06 07:11:04.000000 piicatcher-0.9.6/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       42 2020-04-06 07:10:07.000000 piicatcher-0.9.6/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4367 2020-04-06 07:11:04.000000 piicatcher-0.9.6/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3070 2020-04-06 07:10:07.000000 piicatcher-0.9.6/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-04-06 07:11:04.000000 piicatcher-0.9.6/piicatcher/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2020-04-06 07:10:07.000000 piicatcher-0.9.6/piicatcher/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-04-06 07:11:04.000000 piicatcher-0.9.6/piicatcher/catalog/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      184 2020-04-06 07:10:07.000000 piicatcher-0.9.6/piicatcher/catalog/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1948 2020-04-06 07:10:07.000000 piicatcher-0.9.6/piicatcher/catalog/db.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      510 2020-04-06 07:10:07.000000 piicatcher-0.9.6/piicatcher/catalog/file.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2985 2020-04-06 07:10:07.000000 piicatcher-0.9.6/piicatcher/catalog/glue.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      335 2020-04-06 07:10:07.000000 piicatcher-0.9.6/piicatcher/catalog/pii_type_field.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1899 2020-04-06 07:10:07.000000 piicatcher-0.9.6/piicatcher/command_line.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-04-06 07:11:04.000000 piicatcher-0.9.6/piicatcher/explorer/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-04-06 07:10:07.000000 piicatcher-0.9.6/piicatcher/explorer/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5038 2020-04-06 07:10:07.000000 piicatcher-0.9.6/piicatcher/explorer/aws.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10281 2020-04-06 07:10:07.000000 piicatcher-0.9.6/piicatcher/explorer/databases.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7785 2020-04-06 07:10:07.000000 piicatcher-0.9.6/piicatcher/explorer/explorer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4078 2020-04-06 07:10:07.000000 piicatcher-0.9.6/piicatcher/explorer/files.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4946 2020-04-06 07:10:07.000000 piicatcher-0.9.6/piicatcher/explorer/metadata.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3993 2020-04-06 07:10:07.000000 piicatcher-0.9.6/piicatcher/explorer/sqlite.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      177 2020-04-06 07:10:07.000000 piicatcher-0.9.6/piicatcher/log_mixin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      986 2020-04-06 07:10:07.000000 piicatcher-0.9.6/piicatcher/piitypes.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3322 2020-04-06 07:10:07.000000 piicatcher-0.9.6/piicatcher/scanner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      350 2020-04-06 07:10:07.000000 piicatcher-0.9.6/piicatcher/tokenizer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-04-06 07:11:04.000000 piicatcher-0.9.6/piicatcher.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4367 2020-04-06 07:11:03.000000 piicatcher-0.9.6/piicatcher.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      768 2020-04-06 07:11:03.000000 piicatcher-0.9.6/piicatcher.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-04-06 07:11:03.000000 piicatcher-0.9.6/piicatcher.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       60 2020-04-06 07:11:03.000000 piicatcher-0.9.6/piicatcher.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      189 2020-04-06 07:11:03.000000 piicatcher-0.9.6/piicatcher.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       11 2020-04-06 07:11:03.000000 piicatcher-0.9.6/piicatcher.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      212 2020-04-06 07:10:07.000000 piicatcher-0.9.6/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      108 2020-04-06 07:11:04.000000 piicatcher-0.9.6/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2474 2020-04-06 07:10:07.000000 piicatcher-0.9.6/setup.py
```

### Comparing `piicatcher-0.9.5/PKG-INFO` & `piicatcher-0.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: piicatcher
-Version: 0.9.5
+Version: 0.9.6
 Summary: Find PII data in databases
 Home-page: https://tokern.io/piicatcher
 Author: Tokern
 Author-email: piicatcher@tokern.io
 License: Apache 2.0
-Download-URL: https://github.com/tokern/piicatcher/tarball/0.9.5
+Download-URL: https://github.com/tokern/piicatcher/tarball/0.9.6
 Description: [![CircleCI](https://circleci.com/gh/tokern/piicatcher.svg?style=svg)](https://circleci.com/gh/tokern/piicatcher)
         [![codecov](https://codecov.io/gh/tokern/piicatcher/branch/master/graph/badge.svg)](https://codecov.io/gh/tokern/piicatcher)
         [![PyPI](https://img.shields.io/pypi/v/piicatcher.svg)](https://pypi.python.org/pypi/piicatcher)
         [![image](https://img.shields.io/pypi/l/piicatcher.svg)](https://pypi.org/project/piicatcher/)
         [![image](https://img.shields.io/pypi/pyversions/piicatcher.svg)](https://pypi.org/project/piicatcher/)
         
         # PII Catcher for Files and Databases
```

### Comparing `piicatcher-0.9.5/README.md` & `piicatcher-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `piicatcher-0.9.5/piicatcher/catalog/db.py` & `piicatcher-0.9.6/piicatcher/catalog/db.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,21 +32,14 @@
 class DbFile(BaseModel):
     id = AutoField()
     full_path = CharField()
     mime_type = CharField()
     pii_types = PiiTypeField()
 
 
-def init_test(path):
-    database = SqliteDatabase(path)
-    database_proxy.initialize(database)
-    database_proxy.connect()
-    database_proxy.create_tables([DbSchemas, DbTables, DbColumns])
-
-
 def model_db_close():
     database_proxy.close()
 
 
 class DbStore(Store):
     @classmethod
     def setup_database(cls, catalog):
```

### Comparing `piicatcher-0.9.5/piicatcher/catalog/glue.py` & `piicatcher-0.9.6/piicatcher/catalog/glue.py`

 * *Files identical despite different names*

### Comparing `piicatcher-0.9.5/piicatcher/command_line.py` & `piicatcher-0.9.6/piicatcher/command_line.py`

 * *Files identical despite different names*

### Comparing `piicatcher-0.9.5/piicatcher/explorer/aws.py` & `piicatcher-0.9.6/piicatcher/explorer/aws.py`

 * *Files identical despite different names*

### Comparing `piicatcher-0.9.5/piicatcher/explorer/databases.py` & `piicatcher-0.9.6/piicatcher/explorer/databases.py`

 * *Files identical despite different names*

### Comparing `piicatcher-0.9.5/piicatcher/explorer/explorer.py` & `piicatcher-0.9.6/piicatcher/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `piicatcher-0.9.5/piicatcher/explorer/files.py` & `piicatcher-0.9.6/piicatcher/explorer/files.py`

 * *Files identical despite different names*

### Comparing `piicatcher-0.9.5/piicatcher/explorer/metadata.py` & `piicatcher-0.9.6/piicatcher/explorer/metadata.py`

 * *Files identical despite different names*

### Comparing `piicatcher-0.9.5/piicatcher/explorer/sqlite.py` & `piicatcher-0.9.6/piicatcher/explorer/sqlite.py`

 * *Files identical despite different names*

### Comparing `piicatcher-0.9.5/piicatcher/piitypes.py` & `piicatcher-0.9.6/piicatcher/piitypes.py`

 * *Files identical despite different names*

### Comparing `piicatcher-0.9.5/piicatcher/scanner.py` & `piicatcher-0.9.6/piicatcher/scanner.py`

 * *Files identical despite different names*

### Comparing `piicatcher-0.9.5/piicatcher.egg-info/PKG-INFO` & `piicatcher-0.9.6/piicatcher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: piicatcher
-Version: 0.9.5
+Version: 0.9.6
 Summary: Find PII data in databases
 Home-page: https://tokern.io/piicatcher
 Author: Tokern
 Author-email: piicatcher@tokern.io
 License: Apache 2.0
-Download-URL: https://github.com/tokern/piicatcher/tarball/0.9.5
+Download-URL: https://github.com/tokern/piicatcher/tarball/0.9.6
 Description: [![CircleCI](https://circleci.com/gh/tokern/piicatcher.svg?style=svg)](https://circleci.com/gh/tokern/piicatcher)
         [![codecov](https://codecov.io/gh/tokern/piicatcher/branch/master/graph/badge.svg)](https://codecov.io/gh/tokern/piicatcher)
         [![PyPI](https://img.shields.io/pypi/v/piicatcher.svg)](https://pypi.python.org/pypi/piicatcher)
         [![image](https://img.shields.io/pypi/l/piicatcher.svg)](https://pypi.org/project/piicatcher/)
         [![image](https://img.shields.io/pypi/pyversions/piicatcher.svg)](https://pypi.org/project/piicatcher/)
         
         # PII Catcher for Files and Databases
```

### Comparing `piicatcher-0.9.5/piicatcher.egg-info/SOURCES.txt` & `piicatcher-0.9.6/piicatcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piicatcher-0.9.5/setup.py` & `piicatcher-0.9.6/setup.py`

 * *Files identical despite different names*

