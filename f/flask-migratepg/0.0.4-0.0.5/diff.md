# Comparing `tmp/flask-migratepg-0.0.4.tar.gz` & `tmp/flask-migratepg-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-migratepg-0.0.4.tar", last modified: Mon Jun 26 10:02:53 2023, max compression
+gzip compressed data, was "flask-migratepg-0.0.5.tar", last modified: Mon Jun 26 10:07:01 2023, max compression
```

## Comparing `flask-migratepg-0.0.4.tar` & `flask-migratepg-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-26 10:02:53.594885 flask-migratepg-0.0.4/
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1504 2023-06-25 16:34:54.000000 flask-migratepg-0.0.4/LICENSE
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1770 2023-06-26 10:02:53.594885 flask-migratepg-0.0.4/PKG-INFO
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1185 2023-06-26 10:01:41.000000 flask-migratepg-0.0.4/README.md
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      566 2023-06-26 09:59:36.000000 flask-migratepg-0.0.4/pyproject.toml
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       38 2023-06-26 10:02:53.594885 flask-migratepg-0.0.4/setup.cfg
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-26 10:02:53.592885 flask-migratepg-0.0.4/src/
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-26 10:02:53.593885 flask-migratepg-0.0.4/src/flask_migratepg/
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     2729 2023-06-26 09:59:36.000000 flask-migratepg-0.0.4/src/flask_migratepg/__init__.py
-drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-26 10:02:53.594885 flask-migratepg-0.0.4/src/flask_migratepg.egg-info/
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1770 2023-06-26 10:02:53.000000 flask-migratepg-0.0.4/src/flask_migratepg.egg-info/PKG-INFO
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      236 2023-06-26 10:02:53.000000 flask-migratepg-0.0.4/src/flask_migratepg.egg-info/SOURCES.txt
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)        1 2023-06-26 10:02:53.000000 flask-migratepg-0.0.4/src/flask_migratepg.egg-info/dependency_links.txt
--rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       16 2023-06-26 10:02:53.000000 flask-migratepg-0.0.4/src/flask_migratepg.egg-info/top_level.txt
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-26 10:07:01.358400 flask-migratepg-0.0.5/
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1504 2023-06-25 16:34:54.000000 flask-migratepg-0.0.5/LICENSE
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1744 2023-06-26 10:07:01.358400 flask-migratepg-0.0.5/PKG-INFO
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1159 2023-06-26 10:05:55.000000 flask-migratepg-0.0.5/README.md
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      566 2023-06-26 10:06:48.000000 flask-migratepg-0.0.5/pyproject.toml
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       38 2023-06-26 10:07:01.358400 flask-migratepg-0.0.5/setup.cfg
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-26 10:07:01.357400 flask-migratepg-0.0.5/src/
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-26 10:07:01.357400 flask-migratepg-0.0.5/src/flask_migratepg/
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     2729 2023-06-26 09:59:36.000000 flask-migratepg-0.0.5/src/flask_migratepg/__init__.py
+drwxr-xr-x   0 dbezborodov  (1000) dbezborodov  (1000)        0 2023-06-26 10:07:01.358400 flask-migratepg-0.0.5/src/flask_migratepg.egg-info/
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)     1744 2023-06-26 10:07:01.000000 flask-migratepg-0.0.5/src/flask_migratepg.egg-info/PKG-INFO
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)      236 2023-06-26 10:07:01.000000 flask-migratepg-0.0.5/src/flask_migratepg.egg-info/SOURCES.txt
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)        1 2023-06-26 10:07:01.000000 flask-migratepg-0.0.5/src/flask_migratepg.egg-info/dependency_links.txt
+-rw-r--r--   0 dbezborodov  (1000) dbezborodov  (1000)       16 2023-06-26 10:07:01.000000 flask-migratepg-0.0.5/src/flask_migratepg.egg-info/top_level.txt
```

### Comparing `flask-migratepg-0.0.4/LICENSE` & `flask-migratepg-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-migratepg-0.0.4/PKG-INFO` & `flask-migratepg-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-migratepg
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple migration command for Flask and Psycopg 3.
 Author-email: Damien Bezborodov <dbezborodov@gmail.com>
 Project-URL: Homepage, https://github.com/bezborodow/flask-migratepg
 Project-URL: Bug Tracker, https://github.com/bezborodow/flask-migratepg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -52,9 +52,8 @@
 A Python migration can implement a method `migrate(conn)`. If this method is
 present, it will be called. An example of this:
 
 ````python
 def migrate(conn):
     cur = conn.cursor()
     # ...
-    cur.execute('commit')
 ````
```

### Comparing `flask-migratepg-0.0.4/README.md` & `flask-migratepg-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -37,9 +37,8 @@
 A Python migration can implement a method `migrate(conn)`. If this method is
 present, it will be called. An example of this:
 
 ````python
 def migrate(conn):
     cur = conn.cursor()
     # ...
-    cur.execute('commit')
 ````
```

### Comparing `flask-migratepg-0.0.4/pyproject.toml` & `flask-migratepg-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "flask-migratepg"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Damien Bezborodov", email="dbezborodov@gmail.com" },
 ]
 description = "Simple migration command for Flask and Psycopg 3."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `flask-migratepg-0.0.4/src/flask_migratepg/__init__.py` & `flask-migratepg-0.0.5/src/flask_migratepg/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-migratepg-0.0.4/src/flask_migratepg.egg-info/PKG-INFO` & `flask-migratepg-0.0.5/src/flask_migratepg.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-migratepg
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple migration command for Flask and Psycopg 3.
 Author-email: Damien Bezborodov <dbezborodov@gmail.com>
 Project-URL: Homepage, https://github.com/bezborodow/flask-migratepg
 Project-URL: Bug Tracker, https://github.com/bezborodow/flask-migratepg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -52,9 +52,8 @@
 A Python migration can implement a method `migrate(conn)`. If this method is
 present, it will be called. An example of this:
 
 ````python
 def migrate(conn):
     cur = conn.cursor()
     # ...
-    cur.execute('commit')
 ````
```

