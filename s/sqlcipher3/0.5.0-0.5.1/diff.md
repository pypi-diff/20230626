# Comparing `tmp/sqlcipher3-0.5.0.tar.gz` & `tmp/sqlcipher3-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sqlcipher3-0.5.0.tar", last modified: Tue Dec 13 22:14:14 2022, max compression
+gzip compressed data, was "dist/sqlcipher3-0.5.1.tar", last modified: Mon Jun 26 01:50:15 2023, max compression
```

## Comparing `sqlcipher3-0.5.0.tar` & `sqlcipher3-0.5.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-12-13 22:14:14.000000 sqlcipher3-0.5.0/
--rw-r--r--   0 charles   (1000) charles   (1000)      889 2019-06-03 15:14:15.000000 sqlcipher3-0.5.0/LICENSE
--rw-r--r--   0 charles   (1000) charles   (1000)      128 2019-06-03 15:14:15.000000 sqlcipher3-0.5.0/MANIFEST.in
--rw-r--r--   0 charles   (1000) charles   (1000)      762 2022-12-13 22:14:14.000000 sqlcipher3-0.5.0/PKG-INFO
--rw-r--r--   0 charles   (1000) charles   (1000)     2122 2019-09-28 13:31:33.000000 sqlcipher3-0.5.0/README.md
--rw-r--r--   0 charles   (1000) charles   (1000)      103 2022-12-13 22:14:14.000000 sqlcipher3-0.5.0/setup.cfg
--rw-r--r--   0 charles   (1000) charles   (1000)     6442 2022-12-13 22:13:58.000000 sqlcipher3-0.5.0/setup.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-12-13 22:14:14.000000 sqlcipher3-0.5.0/sqlcipher3/
--rw-r--r--   0 charles   (1000) charles   (1000)     1020 2019-09-28 13:31:33.000000 sqlcipher3-0.5.0/sqlcipher3/__init__.py
--rw-r--r--   0 charles   (1000) charles   (1000)     2727 2019-09-28 13:31:33.000000 sqlcipher3-0.5.0/sqlcipher3/dbapi2.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-12-13 22:14:14.000000 sqlcipher3-0.5.0/sqlcipher3.egg-info/
--rw-r--r--   0 charles   (1000) charles   (1000)      762 2022-12-13 22:14:14.000000 sqlcipher3-0.5.0/sqlcipher3.egg-info/PKG-INFO
--rw-r--r--   0 charles   (1000) charles   (1000)      522 2022-12-13 22:14:14.000000 sqlcipher3-0.5.0/sqlcipher3.egg-info/SOURCES.txt
--rw-r--r--   0 charles   (1000) charles   (1000)        1 2022-12-13 22:14:14.000000 sqlcipher3-0.5.0/sqlcipher3.egg-info/dependency_links.txt
--rw-r--r--   0 charles   (1000) charles   (1000)       11 2022-12-13 22:14:14.000000 sqlcipher3-0.5.0/sqlcipher3.egg-info/top_level.txt
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-12-13 22:14:14.000000 sqlcipher3-0.5.0/src/
--rw-r--r--   0 charles   (1000) charles   (1000)    17810 2021-05-14 15:12:50.000000 sqlcipher3-0.5.0/src/blob.c
--rw-r--r--   0 charles   (1000) charles   (1000)      590 2019-08-09 20:31:54.000000 sqlcipher3-0.5.0/src/blob.h
--rw-r--r--   0 charles   (1000) charles   (1000)    12679 2020-11-08 02:22:30.000000 sqlcipher3-0.5.0/src/cache.c
--rw-r--r--   0 charles   (1000) charles   (1000)     2357 2019-06-03 15:14:15.000000 sqlcipher3-0.5.0/src/cache.h
--rw-r--r--   0 charles   (1000) charles   (1000)    61784 2022-09-21 18:11:46.000000 sqlcipher3-0.5.0/src/connection.c
--rw-r--r--   0 charles   (1000) charles   (1000)     4723 2021-08-06 23:58:58.000000 sqlcipher3-0.5.0/src/connection.h
--rw-r--r--   0 charles   (1000) charles   (1000)    29823 2021-08-06 23:58:58.000000 sqlcipher3-0.5.0/src/cursor.c
--rw-r--r--   0 charles   (1000) charles   (1000)     2441 2019-06-03 15:14:15.000000 sqlcipher3-0.5.0/src/cursor.h
--rw-r--r--   0 charles   (1000) charles   (1000)     4551 2019-06-03 15:14:15.000000 sqlcipher3-0.5.0/src/microprotocols.c
--rw-r--r--   0 charles   (1000) charles   (1000)     2079 2019-06-03 15:14:15.000000 sqlcipher3-0.5.0/src/microprotocols.h
--rw-r--r--   0 charles   (1000) charles   (1000)    18325 2021-08-23 15:49:07.000000 sqlcipher3-0.5.0/src/module.c
--rw-r--r--   0 charles   (1000) charles   (1000)     1956 2019-08-09 20:31:54.000000 sqlcipher3-0.5.0/src/module.h
--rw-r--r--   0 charles   (1000) charles   (1000)     4363 2022-09-21 18:11:46.000000 sqlcipher3-0.5.0/src/prepare_protocol.c
--rw-r--r--   0 charles   (1000) charles   (1000)     1525 2019-06-03 15:14:15.000000 sqlcipher3-0.5.0/src/prepare_protocol.h
--rw-r--r--   0 charles   (1000) charles   (1000)     9515 2019-09-28 13:31:33.000000 sqlcipher3-0.5.0/src/row.c
--rw-r--r--   0 charles   (1000) charles   (1000)     1296 2019-06-03 15:14:15.000000 sqlcipher3-0.5.0/src/row.h
--rw-r--r--   0 charles   (1000) charles   (1000)    17339 2019-07-23 18:05:13.000000 sqlcipher3-0.5.0/src/statement.c
--rw-r--r--   0 charles   (1000) charles   (1000)     2090 2019-06-03 15:14:15.000000 sqlcipher3-0.5.0/src/statement.h
--rw-r--r--   0 charles   (1000) charles   (1000)     4812 2021-05-14 15:12:50.000000 sqlcipher3-0.5.0/src/util.c
--rw-r--r--   0 charles   (1000) charles   (1000)     1497 2021-05-14 15:12:50.000000 sqlcipher3-0.5.0/src/util.h
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:50:15.000000 sqlcipher3-0.5.1/
+-rw-r--r--   0 charles   (1000) charles   (1000)      889 2019-06-03 15:14:15.000000 sqlcipher3-0.5.1/LICENSE
+-rw-r--r--   0 charles   (1000) charles   (1000)      128 2019-06-03 15:14:15.000000 sqlcipher3-0.5.1/MANIFEST.in
+-rw-r--r--   0 charles   (1000) charles   (1000)      762 2023-06-26 01:50:15.000000 sqlcipher3-0.5.1/PKG-INFO
+-rw-r--r--   0 charles   (1000) charles   (1000)     2122 2019-09-28 13:31:33.000000 sqlcipher3-0.5.1/README.md
+-rw-r--r--   0 charles   (1000) charles   (1000)      103 2023-06-26 01:50:15.000000 sqlcipher3-0.5.1/setup.cfg
+-rw-r--r--   0 charles   (1000) charles   (1000)     6442 2023-06-26 01:49:51.000000 sqlcipher3-0.5.1/setup.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:50:15.000000 sqlcipher3-0.5.1/sqlcipher3/
+-rw-r--r--   0 charles   (1000) charles   (1000)     1020 2019-09-28 13:31:33.000000 sqlcipher3-0.5.1/sqlcipher3/__init__.py
+-rw-r--r--   0 charles   (1000) charles   (1000)     2727 2019-09-28 13:31:33.000000 sqlcipher3-0.5.1/sqlcipher3/dbapi2.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:50:15.000000 sqlcipher3-0.5.1/sqlcipher3.egg-info/
+-rw-r--r--   0 charles   (1000) charles   (1000)      762 2023-06-26 01:50:15.000000 sqlcipher3-0.5.1/sqlcipher3.egg-info/PKG-INFO
+-rw-r--r--   0 charles   (1000) charles   (1000)      522 2023-06-26 01:50:15.000000 sqlcipher3-0.5.1/sqlcipher3.egg-info/SOURCES.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)        1 2023-06-26 01:50:15.000000 sqlcipher3-0.5.1/sqlcipher3.egg-info/dependency_links.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)       11 2023-06-26 01:50:15.000000 sqlcipher3-0.5.1/sqlcipher3.egg-info/top_level.txt
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:50:15.000000 sqlcipher3-0.5.1/src/
+-rw-r--r--   0 charles   (1000) charles   (1000)    17810 2021-05-14 15:12:50.000000 sqlcipher3-0.5.1/src/blob.c
+-rw-r--r--   0 charles   (1000) charles   (1000)      590 2019-08-09 20:31:54.000000 sqlcipher3-0.5.1/src/blob.h
+-rw-r--r--   0 charles   (1000) charles   (1000)    12679 2020-11-08 02:22:30.000000 sqlcipher3-0.5.1/src/cache.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     2357 2019-06-03 15:14:15.000000 sqlcipher3-0.5.1/src/cache.h
+-rw-r--r--   0 charles   (1000) charles   (1000)    61784 2022-09-21 18:11:46.000000 sqlcipher3-0.5.1/src/connection.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     4723 2021-08-06 23:58:58.000000 sqlcipher3-0.5.1/src/connection.h
+-rw-r--r--   0 charles   (1000) charles   (1000)    30457 2023-01-11 19:30:52.000000 sqlcipher3-0.5.1/src/cursor.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     2441 2019-06-03 15:14:15.000000 sqlcipher3-0.5.1/src/cursor.h
+-rw-r--r--   0 charles   (1000) charles   (1000)     4551 2019-06-03 15:14:15.000000 sqlcipher3-0.5.1/src/microprotocols.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     2079 2019-06-03 15:14:15.000000 sqlcipher3-0.5.1/src/microprotocols.h
+-rw-r--r--   0 charles   (1000) charles   (1000)    18479 2023-05-02 20:25:18.000000 sqlcipher3-0.5.1/src/module.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     1956 2019-08-09 20:31:54.000000 sqlcipher3-0.5.1/src/module.h
+-rw-r--r--   0 charles   (1000) charles   (1000)     4363 2022-09-21 18:11:46.000000 sqlcipher3-0.5.1/src/prepare_protocol.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     1525 2019-06-03 15:14:15.000000 sqlcipher3-0.5.1/src/prepare_protocol.h
+-rw-r--r--   0 charles   (1000) charles   (1000)     9515 2019-09-28 13:31:33.000000 sqlcipher3-0.5.1/src/row.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     1296 2019-06-03 15:14:15.000000 sqlcipher3-0.5.1/src/row.h
+-rw-r--r--   0 charles   (1000) charles   (1000)    17400 2023-06-26 01:47:13.000000 sqlcipher3-0.5.1/src/statement.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     2090 2019-06-03 15:14:15.000000 sqlcipher3-0.5.1/src/statement.h
+-rw-r--r--   0 charles   (1000) charles   (1000)     4812 2021-05-14 15:12:50.000000 sqlcipher3-0.5.1/src/util.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     1497 2021-05-14 15:12:50.000000 sqlcipher3-0.5.1/src/util.h
```

### Comparing `sqlcipher3-0.5.0/LICENSE` & `sqlcipher3-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/PKG-INFO` & `sqlcipher3-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sqlcipher3
-Version: 0.5.0
+Version: 0.5.1
 Summary: DB-API 2.0 interface for SQLCipher 3.x
 Home-page: https://github.com/coleifer/sqlcipher3
 Author: Charles Leifer
 Author-email: coleifer@gmail.com
 License: zlib/libpng
 Description: UNKNOWN
 Platform: ALL
```

### Comparing `sqlcipher3-0.5.0/README.md` & `sqlcipher3-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/setup.py` & `sqlcipher3-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from distutils import log
 from distutils.command.build_ext import build_ext
 from setuptools import Extension
 
 # If you need to change anything, it should be enough to change setup.cfg.
 
 PACKAGE_NAME = 'sqlcipher3'
-VERSION = '0.5.0'
+VERSION = '0.5.1'
 
 # define sqlite sources
 sources = [os.path.join('src', source)
            for source in ["module.c", "connection.c", "cursor.c", "cache.c",
                           "microprotocols.c", "prepare_protocol.c",
                           "statement.c", "util.c", "row.c", "blob.c"]]
```

### Comparing `sqlcipher3-0.5.0/sqlcipher3/__init__.py` & `sqlcipher3-0.5.1/sqlcipher3/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/sqlcipher3/dbapi2.py` & `sqlcipher3-0.5.1/sqlcipher3/dbapi2.py`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/sqlcipher3.egg-info/PKG-INFO` & `sqlcipher3-0.5.1/sqlcipher3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sqlcipher3
-Version: 0.5.0
+Version: 0.5.1
 Summary: DB-API 2.0 interface for SQLCipher 3.x
 Home-page: https://github.com/coleifer/sqlcipher3
 Author: Charles Leifer
 Author-email: coleifer@gmail.com
 License: zlib/libpng
 Description: UNKNOWN
 Platform: ALL
```

### Comparing `sqlcipher3-0.5.0/sqlcipher3.egg-info/SOURCES.txt` & `sqlcipher3-0.5.1/sqlcipher3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/src/blob.c` & `sqlcipher3-0.5.1/src/blob.c`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/src/blob.h` & `sqlcipher3-0.5.1/src/blob.h`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/src/cache.c` & `sqlcipher3-0.5.1/src/cache.c`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/src/cache.h` & `sqlcipher3-0.5.1/src/cache.h`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/src/connection.c` & `sqlcipher3-0.5.1/src/connection.c`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/src/connection.h` & `sqlcipher3-0.5.1/src/connection.h`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/src/cursor.c` & `sqlcipher3-0.5.1/src/cursor.c`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,23 @@
     }
     else {
         len = strlen(colname);
     }
     return PyUnicode_FromStringAndSize(colname, len);
 }
 
+static PyObject *
+_pysqlite_build_column_decltype(pysqlite_Cursor *self, const char *decltype)
+{
+    if (!decltype) {
+        Py_RETURN_NONE;
+    }
+    return PyUnicode_FromStringAndSize(decltype, strlen(decltype));
+}
+
 /*
  * Returns a row from the currently active SQLite statement
  *
  * Precondidition:
  * - sqlite3_step() has been called before and it returned SQLITE_ROW.
  */
 static PyObject *
@@ -374,14 +383,15 @@
     PyObject* parameters = NULL;
     int i;
     int rc;
     PyObject* func_args;
     PyObject* result;
     int numcols;
     PyObject* column_name;
+    PyObject* column_decltype;
     PyObject* second_argument = NULL;
     sqlite_int64 lastrowid;
 
     if (!check_cursor(self)) {
         goto error;
     }
 
@@ -537,27 +547,36 @@
         if (self->description == Py_None && numcols > 0) {
             Py_SETREF(self->description, PyTuple_New(numcols));
             if (!self->description) {
                 goto error;
             }
             for (i = 0; i < numcols; i++) {
                 const char *colname;
+                const char *decltype;
                 colname = sqlite3_column_name(self->statement->st, i);
                 if (colname == NULL) {
                     PyErr_NoMemory();
                     goto error;
                 }
                 column_name = _pysqlite_build_column_name(self, colname);
                 if (!column_name) {
                     goto error;
                 }
-                PyObject *descriptor = PyTuple_Pack(7, column_name,
+                decltype = sqlite3_column_decltype(self->statement->st, i);
+                column_decltype = _pysqlite_build_column_decltype(self, decltype);
+                if (!column_decltype) {
+                    Py_DECREF(column_name);
+                    goto error;
+                }
+
+                PyObject *descriptor = PyTuple_Pack(7, column_name, column_decltype,
                                                     Py_None, Py_None, Py_None,
-                                                    Py_None, Py_None, Py_None);
+                                                    Py_None, Py_None);
                 Py_DECREF(column_name);
+                Py_DECREF(column_decltype);
                 if (descriptor == NULL) {
                     goto error;
                 }
                 PyTuple_SET_ITEM(self->description, i, descriptor);
             }
         }
```

### Comparing `sqlcipher3-0.5.0/src/cursor.h` & `sqlcipher3-0.5.1/src/cursor.h`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/src/microprotocols.c` & `sqlcipher3-0.5.1/src/microprotocols.c`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/src/microprotocols.h` & `sqlcipher3-0.5.1/src/microprotocols.h`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/src/module.c` & `sqlcipher3-0.5.1/src/module.c`

 * *Files 0% similar despite different names*

```diff
@@ -434,14 +434,20 @@
 
 PyMODINIT_FUNC PyInit__sqlite3(void)
 {
     PyObject *module, *dict;
     PyObject *tmp_obj;
     int i;
 
+    int rc = sqlite3_initialize();
+    if (rc != SQLITE_OK) {
+        PyErr_SetString(PyExc_ImportError, sqlite3_errstr(rc));
+        return NULL;
+    }
+
     module = PyModule_Create(&_sqlite3module);
 
     if (!module ||
         (pysqlite_row_setup_types() < 0) ||
         (pysqlite_cursor_setup_types() < 0) ||
         (pysqlite_connection_setup_types() < 0) ||
         (pysqlite_cache_setup_types() < 0) ||
```

### Comparing `sqlcipher3-0.5.0/src/module.h` & `sqlcipher3-0.5.1/src/module.h`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/src/prepare_protocol.c` & `sqlcipher3-0.5.1/src/prepare_protocol.c`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/src/prepare_protocol.h` & `sqlcipher3-0.5.1/src/prepare_protocol.h`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/src/row.c` & `sqlcipher3-0.5.1/src/row.c`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/src/row.h` & `sqlcipher3-0.5.1/src/row.h`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/src/statement.c` & `sqlcipher3-0.5.1/src/statement.c`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,16 @@
             /* DML iff statement is not a CREATE/DROP/BEGIN. */
             self->is_dml = (PyOS_strnicmp(p, "begin", 5) &&
                             PyOS_strnicmp(p, "create", 6) &&
                             PyOS_strnicmp(p, "drop", 4) &&
                             PyOS_strnicmp(p, "alter", 5) &&
                             PyOS_strnicmp(p, "analyze", 7) &&
                             PyOS_strnicmp(p, "reindex", 7) &&
-                            PyOS_strnicmp(p, "vacuum", 6));
+                            PyOS_strnicmp(p, "vacuum", 6) &&
+                            PyOS_strnicmp(p, "pragma", 6));
             break;
         }
     }
 
     self->db = connection->db;
 
     if (rc == SQLITE_OK && pysqlite_check_remaining_sql(tail)) {
```

### Comparing `sqlcipher3-0.5.0/src/statement.h` & `sqlcipher3-0.5.1/src/statement.h`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/src/util.c` & `sqlcipher3-0.5.1/src/util.c`

 * *Files identical despite different names*

### Comparing `sqlcipher3-0.5.0/src/util.h` & `sqlcipher3-0.5.1/src/util.h`

 * *Files identical despite different names*

