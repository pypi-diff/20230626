# Comparing `tmp/sqlite-utils-3.9.tar.gz` & `tmp/sqlite-utils-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlite-utils-3.9.tar", last modified: Sat Jun 12 02:14:01 2021, max compression
+gzip compressed data, was "sqlite-utils-3.9.1.tar", last modified: Sun Jun 13 03:05:06 2021, max compression
```

## Comparing `sqlite-utils-3.9.tar` & `sqlite-utils-3.9.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-12 02:14:01.577057 sqlite-utils-3.9/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-06-12 02:13:54.000000 sqlite-utils-3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-06-12 02:13:54.000000 sqlite-utils-3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6060 2021-06-12 02:14:01.577057 sqlite-utils-3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4160 2021-06-12 02:13:54.000000 sqlite-utils-3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-12 02:14:01.573057 sqlite-utils-3.9/docs/
--rw-r--r--   0 runner    (1001) docker     (121)    43134 2021-06-12 02:13:54.000000 sqlite-utils-3.9/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)    44998 2021-06-12 02:13:54.000000 sqlite-utils-3.9/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1497 2021-06-12 02:13:54.000000 sqlite-utils-3.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    77455 2021-06-12 02:13:54.000000 sqlite-utils-3.9/docs/python-api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-12 02:14:01.577057 sqlite-utils-3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2021-06-12 02:13:54.000000 sqlite-utils-3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-12 02:14:01.573057 sqlite-utils-3.9/sqlite_utils/
--rw-r--r--   0 runner    (1001) docker     (121)      113 2021-06-12 02:13:54.000000 sqlite-utils-3.9/sqlite_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    49601 2021-06-12 02:13:54.000000 sqlite-utils-3.9/sqlite_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    79083 2021-06-12 02:13:54.000000 sqlite-utils-3.9/sqlite_utils/db.py
--rw-r--r--   0 runner    (1001) docker     (121)     3300 2021-06-12 02:13:54.000000 sqlite-utils-3.9/sqlite_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-12 02:14:01.573057 sqlite-utils-3.9/sqlite_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6060 2021-06-12 02:14:01.000000 sqlite-utils-3.9/sqlite_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2021-06-12 02:14:01.000000 sqlite-utils-3.9/sqlite_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-12 02:14:01.000000 sqlite-utils-3.9/sqlite_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-06-12 02:14:01.000000 sqlite-utils-3.9/sqlite_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      121 2021-06-12 02:14:01.000000 sqlite-utils-3.9/sqlite_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-06-12 02:14:01.000000 sqlite-utils-3.9/sqlite_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-12 02:14:01.577057 sqlite-utils-3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      444 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4055 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_analyze_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)      493 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_attach.py
--rw-r--r--   0 runner    (1001) docker     (121)    67315 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_column_affinity.py
--rw-r--r--   0 runner    (1001) docker     (121)      340 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_constructor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (121)    33957 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_create.py
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_create_view.py
--rw-r--r--   0 runner    (1001) docker     (121)      871 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (121)      784 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6099 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_enable_counts.py
--rw-r--r--   0 runner    (1001) docker     (121)     6230 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (121)     2159 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_extracts.py
--rw-r--r--   0 runner    (1001) docker     (121)    16411 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_fts.py
--rw-r--r--   0 runner    (1001) docker     (121)      930 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_get.py
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (121)     3592 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_insert_files.py
--rw-r--r--   0 runner    (1001) docker     (121)     7748 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_introspect.py
--rw-r--r--   0 runner    (1001) docker     (121)     2196 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_lookup.py
--rw-r--r--   0 runner    (1001) docker     (121)     7605 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_m2m.py
--rw-r--r--   0 runner    (1001) docker     (121)     1028 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_recreate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_register_function.py
--rw-r--r--   0 runner    (1001) docker     (121)     3180 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_rows.py
--rw-r--r--   0 runner    (1001) docker     (121)      888 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_sniff.py
--rw-r--r--   0 runner    (1001) docker     (121)      989 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_suggest_column_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2513 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_tracer.py
--rw-r--r--   0 runner    (1001) docker     (121)    11627 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     3241 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (121)     2083 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_upsert.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      721 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/test_wal.py
--rw-r--r--   0 runner    (1001) docker     (121)      109 2021-06-12 02:13:54.000000 sqlite-utils-3.9/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 03:05:06.187868 sqlite-utils-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6062 2021-06-13 03:05:06.187868 sqlite-utils-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4160 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 03:05:06.179868 sqlite-utils-3.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)    43375 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    44998 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1497 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    77455 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/docs/python-api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-13 03:05:06.187868 sqlite-utils-3.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2010 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 03:05:06.179868 sqlite-utils-3.9.1/sqlite_utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/sqlite_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49601 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/sqlite_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    79196 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/sqlite_utils/db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3300 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/sqlite_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 03:05:06.183868 sqlite-utils-3.9.1/sqlite_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6062 2021-06-13 03:05:05.000000 sqlite-utils-3.9.1/sqlite_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1176 2021-06-13 03:05:06.000000 sqlite-utils-3.9.1/sqlite_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-13 03:05:05.000000 sqlite-utils-3.9.1/sqlite_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-06-13 03:05:05.000000 sqlite-utils-3.9.1/sqlite_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2021-06-13 03:05:05.000000 sqlite-utils-3.9.1/sqlite_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-06-13 03:05:05.000000 sqlite-utils-3.9.1/sqlite_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-13 03:05:06.187868 sqlite-utils-3.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      444 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4055 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_analyze_tables.py
+-rw-r--r--   0 runner    (1001) docker     (121)      493 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_attach.py
+-rw-r--r--   0 runner    (1001) docker     (121)    67315 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1285 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_column_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (121)      340 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1467 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34169 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1435 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_create_view.py
+-rw-r--r--   0 runner    (1001) docker     (121)      871 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (121)      784 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6099 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_enable_counts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6230 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2159 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_extracts.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16411 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_fts.py
+-rw-r--r--   0 runner    (1001) docker     (121)      930 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1054 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3592 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_insert_files.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7748 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_introspect.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2196 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7605 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_m2m.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1028 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_recreate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1834 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_register_function.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3180 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_rows.py
+-rw-r--r--   0 runner    (1001) docker     (121)      888 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_sniff.py
+-rw-r--r--   0 runner    (1001) docker     (121)      989 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_suggest_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2513 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11627 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3241 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2295 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      721 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/test_wal.py
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2021-06-13 03:04:55.000000 sqlite-utils-3.9.1/tests/utils.py
```

### Comparing `sqlite-utils-3.9/LICENSE` & `sqlite-utils-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/PKG-INFO` & `sqlite-utils-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-utils
-Version: 3.9
+Version: 3.9.1
 Summary: CLI tool and Python utility functions for manipulating SQLite databases
 Home-page: https://github.com/simonw/sqlite-utils
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://sqlite-utils.datasette.io/en/stable/
 Project-URL: Changelog, https://sqlite-utils.datasette.io/en/stable/changelog.html
 Project-URL: Source code, https://github.com/simonw/sqlite-utils
```

### Comparing `sqlite-utils-3.9/README.md` & `sqlite-utils-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/docs/changelog.rst` & `sqlite-utils-3.9.1/docs/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 ===========
  Changelog
 ===========
 
+.. _3.9.1:
+
+3.9.1 (2021-06-12)
+------------------
+
+- Fixed bug when using ``table.upsert_all()`` to create a table with only a single column that is treated as the primary key. (`#271 <https://github.com/simonw/sqlite-utils/issues/271>`__)
+
 .. _v3_9:
 
 3.9 (2021-06-11)
 ----------------
 
 - New ``sqlite-utils schema`` command showing the full SQL schema for a database, see :ref:`Showing the schema (CLI)<cli_schema>`. (`#268 <https://github.com/simonw/sqlite-utils/issues/268>`__)
 - ``db.schema`` introspection property exposing the same feature to the Python library, see :ref:`Showing the schema (Python library) <python_api_schema>`.
```

### Comparing `sqlite-utils-3.9/docs/cli.rst` & `sqlite-utils-3.9.1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/docs/index.rst` & `sqlite-utils-3.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/docs/python-api.rst` & `sqlite-utils-3.9.1/docs/python-api.rst`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/setup.py` & `sqlite-utils-3.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import io
 import os
 
-VERSION = "3.9"
+VERSION = "3.9.1"
 
 
 def get_long_description():
     with io.open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `sqlite-utils-3.9/sqlite_utils/cli.py` & `sqlite-utils-3.9.1/sqlite_utils/cli.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/sqlite_utils/db.py` & `sqlite-utils-3.9.1/sqlite_utils/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -1728,28 +1728,30 @@
                     table=self.name,
                     pks=", ".join(["[{}]".format(p) for p in pks]),
                     pk_placeholders=", ".join(["?" for p in pks]),
                 )
                 queries_and_params.append((sql, [record[col] for col in pks]))
                 # UPDATE [book] SET [name] = 'Programming' WHERE [id] = 1001;
                 set_cols = [col for col in all_columns if col not in pks]
-                sql2 = "UPDATE [{table}] SET {pairs} WHERE {wheres}".format(
-                    table=self.name,
-                    pairs=", ".join(
-                        "[{}] = {}".format(col, conversions.get(col, "?"))
-                        for col in set_cols
-                    ),
-                    wheres=" AND ".join("[{}] = ?".format(pk) for pk in pks),
-                )
-                queries_and_params.append(
-                    (
-                        sql2,
-                        [record[col] for col in set_cols] + [record[pk] for pk in pks],
+                if set_cols:
+                    sql2 = "UPDATE [{table}] SET {pairs} WHERE {wheres}".format(
+                        table=self.name,
+                        pairs=", ".join(
+                            "[{}] = {}".format(col, conversions.get(col, "?"))
+                            for col in set_cols
+                        ),
+                        wheres=" AND ".join("[{}] = ?".format(pk) for pk in pks),
+                    )
+                    queries_and_params.append(
+                        (
+                            sql2,
+                            [record[col] for col in set_cols]
+                            + [record[pk] for pk in pks],
+                        )
                     )
-                )
                 # We can populate .last_pk right here
                 if num_records_processed == 1:
                     self.last_pk = tuple(record[pk] for pk in pks)
                     if len(self.last_pk) == 1:
                         self.last_pk = self.last_pk[0]
 
         else:
```

### Comparing `sqlite-utils-3.9/sqlite_utils/utils.py` & `sqlite-utils-3.9.1/sqlite_utils/utils.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/sqlite_utils.egg-info/PKG-INFO` & `sqlite-utils-3.9.1/sqlite_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-utils
-Version: 3.9
+Version: 3.9.1
 Summary: CLI tool and Python utility functions for manipulating SQLite databases
 Home-page: https://github.com/simonw/sqlite-utils
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://sqlite-utils.datasette.io/en/stable/
 Project-URL: Changelog, https://sqlite-utils.datasette.io/en/stable/changelog.html
 Project-URL: Source code, https://github.com/simonw/sqlite-utils
```

### Comparing `sqlite-utils-3.9/sqlite_utils.egg-info/SOURCES.txt` & `sqlite-utils-3.9.1/sqlite_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_analyze_tables.py` & `sqlite-utils-3.9.1/tests/test_analyze_tables.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_cli.py` & `sqlite-utils-3.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_column_affinity.py` & `sqlite-utils-3.9.1/tests/test_column_affinity.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_conversions.py` & `sqlite-utils-3.9.1/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_create.py` & `sqlite-utils-3.9.1/tests/test_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -987,14 +987,21 @@
     assert 1 == fresh_db["t"].count
     fresh_db["t"].insert_all([])
     assert 1 == fresh_db["t"].count
     fresh_db["t"].insert_all([], replace=True)
     assert 1 == fresh_db["t"].count
 
 
+def test_insert_all_single_column(fresh_db):
+    table = fresh_db["table"]
+    table.insert_all([{"name": "Cleo"}], pk="name")
+    assert [{"name": "Cleo"}] == list(table.rows)
+    assert table.pks == ["name"]
+
+
 def test_create_with_a_null_column(fresh_db):
     record = {"name": "Name", "description": None}
     fresh_db["t"].insert(record)
     assert [record] == list(fresh_db["t"].rows)
 
 
 def test_create_with_nested_bytes(fresh_db):
```

### Comparing `sqlite-utils-3.9/tests/test_create_view.py` & `sqlite-utils-3.9.1/tests/test_create_view.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_delete.py` & `sqlite-utils-3.9.1/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_docs.py` & `sqlite-utils-3.9.1/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_enable_counts.py` & `sqlite-utils-3.9.1/tests/test_enable_counts.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_extract.py` & `sqlite-utils-3.9.1/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_extracts.py` & `sqlite-utils-3.9.1/tests/test_extracts.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_fts.py` & `sqlite-utils-3.9.1/tests/test_fts.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_get.py` & `sqlite-utils-3.9.1/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_hypothesis.py` & `sqlite-utils-3.9.1/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_insert_files.py` & `sqlite-utils-3.9.1/tests/test_insert_files.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_introspect.py` & `sqlite-utils-3.9.1/tests/test_introspect.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_lookup.py` & `sqlite-utils-3.9.1/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_m2m.py` & `sqlite-utils-3.9.1/tests/test_m2m.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_recreate.py` & `sqlite-utils-3.9.1/tests/test_recreate.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_register_function.py` & `sqlite-utils-3.9.1/tests/test_register_function.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_rows.py` & `sqlite-utils-3.9.1/tests/test_rows.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_sniff.py` & `sqlite-utils-3.9.1/tests/test_sniff.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_suggest_column_types.py` & `sqlite-utils-3.9.1/tests/test_suggest_column_types.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_tracer.py` & `sqlite-utils-3.9.1/tests/test_tracer.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_transform.py` & `sqlite-utils-3.9.1/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_update.py` & `sqlite-utils-3.9.1/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_upsert.py` & `sqlite-utils-3.9.1/tests/test_upsert.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,21 @@
     assert [
         {"id": 1, "name": "Cleo", "age": 5},
         {"id": 2, "name": "Nixie", "age": 5},
     ] == list(table.rows)
     assert table.last_pk is None
 
 
+def test_upsert_all_single_column(fresh_db):
+    table = fresh_db["table"]
+    table.upsert_all([{"name": "Cleo"}], pk="name")
+    assert [{"name": "Cleo"}] == list(table.rows)
+    assert table.pks == ["name"]
+
+
 def test_upsert_error_if_no_pk(fresh_db):
     table = fresh_db["table"]
     with pytest.raises(PrimaryKeyRequired):
         table.upsert_all([{"id": 1, "name": "Cleo"}])
     with pytest.raises(PrimaryKeyRequired):
         table.upsert({"id": 1, "name": "Cleo"})
```

### Comparing `sqlite-utils-3.9/tests/test_utils.py` & `sqlite-utils-3.9.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sqlite-utils-3.9/tests/test_wal.py` & `sqlite-utils-3.9.1/tests/test_wal.py`

 * *Files identical despite different names*

