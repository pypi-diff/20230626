# Comparing `tmp/pysqlite3-0.5.0.tar.gz` & `tmp/pysqlite3-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysqlite3-0.5.0.tar", last modified: Tue Dec 13 22:13:46 2022, max compression
+gzip compressed data, was "dist/pysqlite3-0.5.1.tar", last modified: Mon Jun 26 01:49:41 2023, max compression
```

## Comparing `pysqlite3-0.5.0.tar` & `pysqlite3-0.5.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-12-13 22:13:46.000000 pysqlite3-0.5.0/
--rw-r--r--   0 charles   (1000) charles   (1000)      889 2018-08-16 18:40:45.000000 pysqlite3-0.5.0/LICENSE
--rw-r--r--   0 charles   (1000) charles   (1000)      128 2018-12-19 16:00:42.000000 pysqlite3-0.5.0/MANIFEST.in
--rw-r--r--   0 charles   (1000) charles   (1000)      757 2022-12-13 22:13:46.000000 pysqlite3-0.5.0/PKG-INFO
--rw-r--r--   0 charles   (1000) charles   (1000)     2158 2019-09-28 13:31:30.000000 pysqlite3-0.5.0/README.md
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-12-13 22:13:46.000000 pysqlite3-0.5.0/pysqlite3/
--rw-r--r--   0 charles   (1000) charles   (1000)     1019 2019-09-28 13:31:30.000000 pysqlite3-0.5.0/pysqlite3/__init__.py
--rw-r--r--   0 charles   (1000) charles   (1000)     2725 2019-09-28 13:31:30.000000 pysqlite3-0.5.0/pysqlite3/dbapi2.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-12-13 22:13:46.000000 pysqlite3-0.5.0/pysqlite3.egg-info/
--rw-r--r--   0 charles   (1000) charles   (1000)      757 2022-12-13 22:13:46.000000 pysqlite3-0.5.0/pysqlite3.egg-info/PKG-INFO
--rw-r--r--   0 charles   (1000) charles   (1000)      516 2022-12-13 22:13:46.000000 pysqlite3-0.5.0/pysqlite3.egg-info/SOURCES.txt
--rw-r--r--   0 charles   (1000) charles   (1000)        1 2022-12-13 22:13:46.000000 pysqlite3-0.5.0/pysqlite3.egg-info/dependency_links.txt
--rw-r--r--   0 charles   (1000) charles   (1000)       10 2022-12-13 22:13:46.000000 pysqlite3-0.5.0/pysqlite3.egg-info/top_level.txt
--rw-r--r--   0 charles   (1000) charles   (1000)      103 2022-12-13 22:13:46.000000 pysqlite3-0.5.0/setup.cfg
--rw-r--r--   0 charles   (1000) charles   (1000)     5625 2022-12-13 22:13:33.000000 pysqlite3-0.5.0/setup.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2022-12-13 22:13:46.000000 pysqlite3-0.5.0/src/
--rw-r--r--   0 charles   (1000) charles   (1000)    17814 2021-12-03 02:02:46.000000 pysqlite3-0.5.0/src/blob.c
--rw-r--r--   0 charles   (1000) charles   (1000)      580 2019-08-09 20:31:34.000000 pysqlite3-0.5.0/src/blob.h
--rw-r--r--   0 charles   (1000) charles   (1000)    12679 2020-10-23 14:03:32.000000 pysqlite3-0.5.0/src/cache.c
--rw-r--r--   0 charles   (1000) charles   (1000)     2357 2019-04-19 04:34:24.000000 pysqlite3-0.5.0/src/cache.h
--rw-r--r--   0 charles   (1000) charles   (1000)    61784 2022-09-21 18:12:03.000000 pysqlite3-0.5.0/src/connection.c
--rw-r--r--   0 charles   (1000) charles   (1000)     4713 2021-08-06 23:57:10.000000 pysqlite3-0.5.0/src/connection.h
--rw-r--r--   0 charles   (1000) charles   (1000)    29823 2021-08-06 23:57:10.000000 pysqlite3-0.5.0/src/cursor.c
--rw-r--r--   0 charles   (1000) charles   (1000)     2441 2019-04-19 04:34:24.000000 pysqlite3-0.5.0/src/cursor.h
--rw-r--r--   0 charles   (1000) charles   (1000)     4551 2019-04-19 04:34:24.000000 pysqlite3-0.5.0/src/microprotocols.c
--rw-r--r--   0 charles   (1000) charles   (1000)     2079 2019-04-19 04:34:24.000000 pysqlite3-0.5.0/src/microprotocols.h
--rw-r--r--   0 charles   (1000) charles   (1000)    18325 2021-08-23 15:47:03.000000 pysqlite3-0.5.0/src/module.c
--rw-r--r--   0 charles   (1000) charles   (1000)     1956 2019-08-09 20:31:34.000000 pysqlite3-0.5.0/src/module.h
--rw-r--r--   0 charles   (1000) charles   (1000)     4481 2022-09-21 18:12:03.000000 pysqlite3-0.5.0/src/prepare_protocol.c
--rw-r--r--   0 charles   (1000) charles   (1000)     1525 2019-04-19 04:34:24.000000 pysqlite3-0.5.0/src/prepare_protocol.h
--rw-r--r--   0 charles   (1000) charles   (1000)     9515 2019-09-28 13:31:30.000000 pysqlite3-0.5.0/src/row.c
--rw-r--r--   0 charles   (1000) charles   (1000)     1296 2019-04-19 04:34:24.000000 pysqlite3-0.5.0/src/row.h
--rw-r--r--   0 charles   (1000) charles   (1000)    17339 2021-08-04 19:08:01.000000 pysqlite3-0.5.0/src/statement.c
--rw-r--r--   0 charles   (1000) charles   (1000)     2080 2019-04-19 04:34:24.000000 pysqlite3-0.5.0/src/statement.h
--rw-r--r--   0 charles   (1000) charles   (1000)     4812 2021-05-14 15:12:08.000000 pysqlite3-0.5.0/src/util.c
--rw-r--r--   0 charles   (1000) charles   (1000)     1487 2021-05-14 15:08:25.000000 pysqlite3-0.5.0/src/util.h
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:49:41.000000 pysqlite3-0.5.1/
+-rw-r--r--   0 charles   (1000) charles   (1000)      889 2018-08-16 18:40:45.000000 pysqlite3-0.5.1/LICENSE
+-rw-r--r--   0 charles   (1000) charles   (1000)      128 2018-12-19 16:00:42.000000 pysqlite3-0.5.1/MANIFEST.in
+-rw-r--r--   0 charles   (1000) charles   (1000)      757 2023-06-26 01:49:41.000000 pysqlite3-0.5.1/PKG-INFO
+-rw-r--r--   0 charles   (1000) charles   (1000)     2158 2019-09-28 13:31:30.000000 pysqlite3-0.5.1/README.md
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:49:41.000000 pysqlite3-0.5.1/pysqlite3/
+-rw-r--r--   0 charles   (1000) charles   (1000)     1019 2019-09-28 13:31:30.000000 pysqlite3-0.5.1/pysqlite3/__init__.py
+-rw-r--r--   0 charles   (1000) charles   (1000)     2725 2019-09-28 13:31:30.000000 pysqlite3-0.5.1/pysqlite3/dbapi2.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:49:41.000000 pysqlite3-0.5.1/pysqlite3.egg-info/
+-rw-r--r--   0 charles   (1000) charles   (1000)      757 2023-06-26 01:49:41.000000 pysqlite3-0.5.1/pysqlite3.egg-info/PKG-INFO
+-rw-r--r--   0 charles   (1000) charles   (1000)      516 2023-06-26 01:49:41.000000 pysqlite3-0.5.1/pysqlite3.egg-info/SOURCES.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)        1 2023-06-26 01:49:41.000000 pysqlite3-0.5.1/pysqlite3.egg-info/dependency_links.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)       10 2023-06-26 01:49:41.000000 pysqlite3-0.5.1/pysqlite3.egg-info/top_level.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)      103 2023-06-26 01:49:41.000000 pysqlite3-0.5.1/setup.cfg
+-rw-r--r--   0 charles   (1000) charles   (1000)     5625 2023-06-26 01:49:18.000000 pysqlite3-0.5.1/setup.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:49:41.000000 pysqlite3-0.5.1/src/
+-rw-r--r--   0 charles   (1000) charles   (1000)    17814 2021-12-03 02:02:46.000000 pysqlite3-0.5.1/src/blob.c
+-rw-r--r--   0 charles   (1000) charles   (1000)      580 2019-08-09 20:31:34.000000 pysqlite3-0.5.1/src/blob.h
+-rw-r--r--   0 charles   (1000) charles   (1000)    12679 2020-10-23 14:03:32.000000 pysqlite3-0.5.1/src/cache.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     2357 2019-04-19 04:34:24.000000 pysqlite3-0.5.1/src/cache.h
+-rw-r--r--   0 charles   (1000) charles   (1000)    63395 2023-06-26 01:33:54.000000 pysqlite3-0.5.1/src/connection.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     4713 2021-08-06 23:57:10.000000 pysqlite3-0.5.1/src/connection.h
+-rw-r--r--   0 charles   (1000) charles   (1000)    30457 2023-01-11 19:31:06.000000 pysqlite3-0.5.1/src/cursor.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     2441 2019-04-19 04:34:24.000000 pysqlite3-0.5.1/src/cursor.h
+-rw-r--r--   0 charles   (1000) charles   (1000)     4551 2019-04-19 04:34:24.000000 pysqlite3-0.5.1/src/microprotocols.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     2079 2019-04-19 04:34:24.000000 pysqlite3-0.5.1/src/microprotocols.h
+-rw-r--r--   0 charles   (1000) charles   (1000)    18479 2023-04-28 22:49:31.000000 pysqlite3-0.5.1/src/module.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     1956 2019-08-09 20:31:34.000000 pysqlite3-0.5.1/src/module.h
+-rw-r--r--   0 charles   (1000) charles   (1000)     4481 2022-09-21 18:12:03.000000 pysqlite3-0.5.1/src/prepare_protocol.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     1525 2019-04-19 04:34:24.000000 pysqlite3-0.5.1/src/prepare_protocol.h
+-rw-r--r--   0 charles   (1000) charles   (1000)     9515 2019-09-28 13:31:30.000000 pysqlite3-0.5.1/src/row.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     1296 2019-04-19 04:34:24.000000 pysqlite3-0.5.1/src/row.h
+-rw-r--r--   0 charles   (1000) charles   (1000)    17400 2023-06-26 01:47:43.000000 pysqlite3-0.5.1/src/statement.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     2080 2019-04-19 04:34:24.000000 pysqlite3-0.5.1/src/statement.h
+-rw-r--r--   0 charles   (1000) charles   (1000)     4812 2021-05-14 15:12:08.000000 pysqlite3-0.5.1/src/util.c
+-rw-r--r--   0 charles   (1000) charles   (1000)     1487 2021-05-14 15:08:25.000000 pysqlite3-0.5.1/src/util.h
```

### Comparing `pysqlite3-0.5.0/LICENSE` & `pysqlite3-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/PKG-INFO` & `pysqlite3-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pysqlite3
-Version: 0.5.0
+Version: 0.5.1
 Summary: DB-API 2.0 interface for Sqlite 3.x
 Home-page: https://github.com/coleifer/pysqlite3
 Author: Charles Leifer
 Author-email: coleifer@gmail.com
 License: zlib/libpng
 Description: UNKNOWN
 Platform: ALL
```

### Comparing `pysqlite3-0.5.0/README.md` & `pysqlite3-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/pysqlite3/__init__.py` & `pysqlite3-0.5.1/pysqlite3/__init__.py`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/pysqlite3/dbapi2.py` & `pysqlite3-0.5.1/pysqlite3/dbapi2.py`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/pysqlite3.egg-info/PKG-INFO` & `pysqlite3-0.5.1/pysqlite3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pysqlite3
-Version: 0.5.0
+Version: 0.5.1
 Summary: DB-API 2.0 interface for Sqlite 3.x
 Home-page: https://github.com/coleifer/pysqlite3
 Author: Charles Leifer
 Author-email: coleifer@gmail.com
 License: zlib/libpng
 Description: UNKNOWN
 Platform: ALL
```

### Comparing `pysqlite3-0.5.0/pysqlite3.egg-info/SOURCES.txt` & `pysqlite3-0.5.1/pysqlite3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/setup.py` & `pysqlite3-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from distutils import log
 from distutils.command.build_ext import build_ext
 from setuptools import Extension
 
 # If you need to change anything, it should be enough to change setup.cfg.
 
 PACKAGE_NAME = 'pysqlite3'
-VERSION = '0.5.0'
+VERSION = '0.5.1'
 
 # define sqlite sources
 sources = [os.path.join('src', source)
            for source in ["module.c", "connection.c", "cursor.c", "cache.c",
                           "microprotocols.c", "prepare_protocol.c",
                           "statement.c", "util.c", "row.c", "blob.c"]]
```

### Comparing `pysqlite3-0.5.0/src/blob.c` & `pysqlite3-0.5.1/src/blob.c`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/src/blob.h` & `pysqlite3-0.5.1/src/blob.h`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/src/cache.c` & `pysqlite3-0.5.1/src/cache.c`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/src/cache.h` & `pysqlite3-0.5.1/src/cache.h`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/src/connection.c` & `pysqlite3-0.5.1/src/connection.c`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,18 @@
 #endif
 #endif
 
 #if SQLITE_VERSION_NUMBER >= 3006011
 #define HAVE_BACKUP_API
 #endif
 
+#if SQLITE_VERSION_NUMBER >= 3014002
+#define HAVE_TRACE_V2
+#endif
+
 #if SQLITE_VERSION_NUMBER >= 3025000
 #define HAVE_WINDOW_FUNCTION
 #endif
 
 _Py_IDENTIFIER(cursor);
 
 static const char * const begin_statements[] = {
@@ -1188,24 +1192,68 @@
         Py_DECREF(ret);
     }
 
     PyGILState_Release(gilstate);
     return rc;
 }
 
+#ifdef HAVE_TRACE_V2
+static int _trace_callback(unsigned int type, void *ctx, void *stmt, void *sql)
+{
+    if (type != SQLITE_TRACE_STMT) {
+        return 0;
+    }
+
+    PyGILState_STATE gilstate = PyGILState_Ensure();
+    PyObject *py_statement = NULL;
+    const char *expanded_sql = sqlite3_expanded_sql((sqlite3_stmt *)stmt);
+    if (expanded_sql == NULL) {
+        sqlite3 *db = sqlite3_db_handle((sqlite3_stmt *)stmt);
+        if (sqlite3_errcode(db) == SQLITE_NOMEM) {
+            (void)PyErr_NoMemory();
+            goto exit;
+        }
+        PyErr_SetString(pysqlite_DataError, "Expanded SQL string exceeds the maximum string length");
+        if (_pysqlite_enable_callback_tracebacks) {
+            PyErr_Print();
+        } else {
+            PyErr_Clear();
+        }
+
+        py_statement = PyUnicode_FromString((const char *)sql);
+    } else {
+        py_statement = PyUnicode_FromString(expanded_sql);
+        sqlite3_free((void *)expanded_sql);
+    }
+
+    if (py_statement) {
+        PyObject *ret = PyObject_CallFunctionObjArgs((PyObject*)ctx, py_statement, NULL);
+        Py_DECREF(py_statement);
+        Py_XDECREF(ret);
+    }
+
+    if (PyErr_Occurred()) {
+        if (_pysqlite_enable_callback_tracebacks) {
+            PyErr_Print();
+        } else {
+            PyErr_Clear();
+        }
+    }
+exit:
+    PyGILState_Release(gilstate);
+    return 0;
+}
+#else
 static void _trace_callback(void* user_arg, const char* statement_string)
 {
     PyObject *py_statement = NULL;
     PyObject *ret = NULL;
 
-    PyGILState_STATE gilstate;
-
-    gilstate = PyGILState_Ensure();
-    py_statement = PyUnicode_DecodeUTF8(statement_string,
-            strlen(statement_string), "replace");
+    PyGILState_STATE gilstate = PyGILState_Ensure();
+    py_statement = PyUnicode_FromSTring(statement_string);
     if (py_statement) {
         ret = PyObject_CallFunctionObjArgs((PyObject*)user_arg, py_statement, NULL);
         Py_DECREF(py_statement);
     }
 
     if (ret) {
         Py_DECREF(ret);
@@ -1215,14 +1263,15 @@
         } else {
             PyErr_Clear();
         }
     }
 
     PyGILState_Release(gilstate);
 }
+#endif
 
 static PyObject* pysqlite_connection_set_authorizer(pysqlite_Connection* self, PyObject* args, PyObject* kwargs)
 {
     PyObject* authorizer_cb;
 
     static char *kwlist[] = { "authorizer_callback", NULL };
 
@@ -1296,18 +1345,26 @@
     if (!PyArg_ParseTupleAndKeywords(args, kwargs, "O:set_trace_callback",
                                       kwlist, &trace_callback)) {
         return NULL;
     }
 
     if (trace_callback == Py_None) {
         /* None clears the trace callback previously set */
+#ifdef HAVE_TRACE_V2
+        sqlite3_trace_v2(self->db, SQLITE_TRACE_STMT, NULL, (void*)0);
+#else
         sqlite3_trace(self->db, 0, (void*)0);
+#endif
         Py_XSETREF(self->function_pinboard_trace_callback, NULL);
     } else {
+#ifdef HAVE_TRACE_V2
+        sqlite3_trace_v2(self->db, SQLITE_TRACE_STMT, _trace_callback, trace_callback);
+#else
         sqlite3_trace(self->db, _trace_callback, trace_callback);
+#endif
         Py_INCREF(trace_callback);
         Py_XSETREF(self->function_pinboard_trace_callback, trace_callback);
     }
 
     Py_RETURN_NONE;
 }
```

### Comparing `pysqlite3-0.5.0/src/connection.h` & `pysqlite3-0.5.1/src/connection.h`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/src/cursor.c` & `pysqlite3-0.5.1/src/cursor.c`

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

### Comparing `pysqlite3-0.5.0/src/cursor.h` & `pysqlite3-0.5.1/src/cursor.h`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/src/microprotocols.c` & `pysqlite3-0.5.1/src/microprotocols.c`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/src/microprotocols.h` & `pysqlite3-0.5.1/src/microprotocols.h`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/src/module.c` & `pysqlite3-0.5.1/src/module.c`

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

### Comparing `pysqlite3-0.5.0/src/module.h` & `pysqlite3-0.5.1/src/module.h`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/src/prepare_protocol.c` & `pysqlite3-0.5.1/src/prepare_protocol.c`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/src/prepare_protocol.h` & `pysqlite3-0.5.1/src/prepare_protocol.h`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/src/row.c` & `pysqlite3-0.5.1/src/row.c`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/src/row.h` & `pysqlite3-0.5.1/src/row.h`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/src/statement.c` & `pysqlite3-0.5.1/src/statement.c`

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

### Comparing `pysqlite3-0.5.0/src/statement.h` & `pysqlite3-0.5.1/src/statement.h`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/src/util.c` & `pysqlite3-0.5.1/src/util.c`

 * *Files identical despite different names*

### Comparing `pysqlite3-0.5.0/src/util.h` & `pysqlite3-0.5.1/src/util.h`

 * *Files identical despite different names*

