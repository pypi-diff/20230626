# Comparing `tmp/flask-migratepg-0.0.3.tar.gz` & `tmp/flask-migratepg-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-migratepg-0.0.3.tar", last modified: Sun Jun 25 17:23:11 2023, max compression
+gzip compressed data, was "flask-migratepg-0.0.4.tar", last modified: Mon Jun 26 10:02:53 2023, max compression
```

## Comparing `flask-migratepg-0.0.3.tar` & `flask-migratepg-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-25 17:23:11.833378 flask-migratepg-0.0.3/
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1504 2023-06-25 16:34:54.000000 flask-migratepg-0.0.3/LICENSE
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      553 2023-06-25 17:23:11.833378 flask-migratepg-0.0.3/PKG-INFO
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-25 16:49:01.000000 flask-migratepg-0.0.3/README.md
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      540 2023-06-25 17:22:38.000000 flask-migratepg-0.0.3/pyproject.toml
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       38 2023-06-25 17:23:11.833378 flask-migratepg-0.0.3/setup.cfg
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-25 17:23:11.831378 flask-migratepg-0.0.3/src/
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-25 17:23:11.832378 flask-migratepg-0.0.3/src/flask_migratepg/
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     2682 2023-06-25 17:21:23.000000 flask-migratepg-0.0.3/src/flask_migratepg/__init__.py
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-25 17:23:11.833378 flask-migratepg-0.0.3/src/flask_migratepg.egg-info/
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      553 2023-06-25 17:23:11.000000 flask-migratepg-0.0.3/src/flask_migratepg.egg-info/PKG-INFO
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      236 2023-06-25 17:23:11.000000 flask-migratepg-0.0.3/src/flask_migratepg.egg-info/SOURCES.txt
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)        1 2023-06-25 17:23:11.000000 flask-migratepg-0.0.3/src/flask_migratepg.egg-info/dependency_links.txt
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       16 2023-06-25 17:23:11.000000 flask-migratepg-0.0.3/src/flask_migratepg.egg-info/top_level.txt
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-26 10:02:53.594885 flask-migratepg-0.0.4/
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1504 2023-06-25 16:34:54.000000 flask-migratepg-0.0.4/LICENSE
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1770 2023-06-26 10:02:53.594885 flask-migratepg-0.0.4/PKG-INFO
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1185 2023-06-26 10:01:41.000000 flask-migratepg-0.0.4/README.md
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      566 2023-06-26 09:59:36.000000 flask-migratepg-0.0.4/pyproject.toml
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       38 2023-06-26 10:02:53.594885 flask-migratepg-0.0.4/setup.cfg
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-26 10:02:53.592885 flask-migratepg-0.0.4/src/
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-26 10:02:53.593885 flask-migratepg-0.0.4/src/flask_migratepg/
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     2729 2023-06-26 09:59:36.000000 flask-migratepg-0.0.4/src/flask_migratepg/__init__.py
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-26 10:02:53.594885 flask-migratepg-0.0.4/src/flask_migratepg.egg-info/
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1770 2023-06-26 10:02:53.000000 flask-migratepg-0.0.4/src/flask_migratepg.egg-info/PKG-INFO
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      236 2023-06-26 10:02:53.000000 flask-migratepg-0.0.4/src/flask_migratepg.egg-info/SOURCES.txt
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)        1 2023-06-26 10:02:53.000000 flask-migratepg-0.0.4/src/flask_migratepg.egg-info/dependency_links.txt
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       16 2023-06-26 10:02:53.000000 flask-migratepg-0.0.4/src/flask_migratepg.egg-info/top_level.txt
```

### Comparing `flask-migratepg-0.0.3/LICENSE` & `flask-migratepg-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-migratepg-0.0.3/pyproject.toml` & `flask-migratepg-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [project]
 name = "flask-migratepg"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Damien Bezborodov", email="dbezborodov@gmail.com" },
 ]
 description = "Simple migration command for Flask and Psycopg 3."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
+    "Framework :: Flask",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/bezborodow/flask-migratepg"
 "Bug Tracker" = "https://github.com/bezborodow/flask-migratepg/issues"
```

### Comparing `flask-migratepg-0.0.3/src/flask_migratepg/__init__.py` & `flask-migratepg-0.0.4/src/flask_migratepg/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,20 +13,21 @@
             finalise(cur, e.name)
 
 
 def migrate_py(conn, e):
     module_name = os.path.splitext(e.name)[0]
     spec = importlib.util.spec_from_file_location(module_name, e.path)
     module = importlib.util.module_from_spec(spec)
-    spec.loader.exec_module(module)
 
     with psycopg.ClientCursor(conn) as cur:
         if not begin(cur, e.name):
             return
-        module.migrate(conn)
+        spec.loader.exec_module(module)
+        if hasattr(module, 'migrate'):
+            module.migrate(conn)
         finalise(cur, e.name)
 
 
 def begin(cur, name):
     cur.execute('select true from migrations where filename = %s',
                 [ name ])
     if (cur.fetchone()):
```

