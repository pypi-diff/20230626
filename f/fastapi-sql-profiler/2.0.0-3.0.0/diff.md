# Comparing `tmp/fastapi-sql-profiler-2.0.0.tar.gz` & `tmp/fastapi-sql-profiler-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-sql-profiler-2.0.0.tar", last modified: Mon Jun 26 02:11:53 2023, max compression
+gzip compressed data, was "fastapi-sql-profiler-3.0.0.tar", last modified: Mon Jun 26 06:34:48 2023, max compression
```

## Comparing `fastapi-sql-profiler-2.0.0.tar` & `fastapi-sql-profiler-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 sarvadhi1   (502) staff       (20)        0 2023-06-26 02:11:53.260400 fastapi-sql-profiler-2.0.0/
--rw-r--r--   0 sarvadhi1   (502) staff       (20)      611 2023-06-26 02:11:53.259860 fastapi-sql-profiler-2.0.0/PKG-INFO
--rw-r--r--   0 sarvadhi1   (502) staff       (20)     1110 2023-06-19 04:58:21.000000 fastapi-sql-profiler-2.0.0/README.md
-drwxr-xr-x   0 sarvadhi1   (502) staff       (20)        0 2023-06-26 02:11:53.248297 fastapi-sql-profiler-2.0.0/fastapi_sql_profiler/
--rw-r--r--   0 sarvadhi1   (502) staff       (20)       77 2023-06-23 11:17:08.000000 fastapi-sql-profiler-2.0.0/fastapi_sql_profiler/__init__.py
--rw-r--r--   0 sarvadhi1   (502) staff       (20)     2846 2023-06-23 11:02:00.000000 fastapi-sql-profiler-2.0.0/fastapi_sql_profiler/add_request.py
--rw-r--r--   0 sarvadhi1   (502) staff       (20)     1060 2023-06-21 06:53:09.000000 fastapi-sql-profiler-2.0.0/fastapi_sql_profiler/database.py
--rw-r--r--   0 sarvadhi1   (502) staff       (20)    10158 2023-06-23 11:10:06.000000 fastapi-sql-profiler-2.0.0/fastapi_sql_profiler/middleware.py
--rw-r--r--   0 sarvadhi1   (502) staff       (20)     1035 2023-06-23 10:30:16.000000 fastapi-sql-profiler-2.0.0/fastapi_sql_profiler/models.py
-drwxr-xr-x   0 sarvadhi1   (502) staff       (20)        0 2023-06-26 02:11:53.256502 fastapi-sql-profiler-2.0.0/fastapi_sql_profiler.egg-info/
--rw-r--r--   0 sarvadhi1   (502) staff       (20)      611 2023-06-26 02:11:53.000000 fastapi-sql-profiler-2.0.0/fastapi_sql_profiler.egg-info/PKG-INFO
--rw-r--r--   0 sarvadhi1   (502) staff       (20)      447 2023-06-26 02:11:53.000000 fastapi-sql-profiler-2.0.0/fastapi_sql_profiler.egg-info/SOURCES.txt
--rw-r--r--   0 sarvadhi1   (502) staff       (20)        1 2023-06-26 02:11:53.000000 fastapi-sql-profiler-2.0.0/fastapi_sql_profiler.egg-info/dependency_links.txt
--rw-r--r--   0 sarvadhi1   (502) staff       (20)       94 2023-06-26 02:11:53.000000 fastapi-sql-profiler-2.0.0/fastapi_sql_profiler.egg-info/requires.txt
--rw-r--r--   0 sarvadhi1   (502) staff       (20)       21 2023-06-26 02:11:53.000000 fastapi-sql-profiler-2.0.0/fastapi_sql_profiler.egg-info/top_level.txt
--rw-r--r--   0 sarvadhi1   (502) staff       (20)       90 2023-06-17 09:13:44.000000 fastapi-sql-profiler-2.0.0/pyproject.toml
--rw-r--r--   0 sarvadhi1   (502) staff       (20)       38 2023-06-26 02:11:53.260532 fastapi-sql-profiler-2.0.0/setup.cfg
--rw-r--r--   0 sarvadhi1   (502) staff       (20)      880 2023-06-26 01:56:21.000000 fastapi-sql-profiler-2.0.0/setup.py
-drwxr-xr-x   0 sarvadhi1   (502) staff       (20)        0 2023-06-26 02:11:53.257830 fastapi-sql-profiler-2.0.0/tests/
--rw-r--r--   0 sarvadhi1   (502) staff       (20)     3950 2023-06-23 12:57:41.000000 fastapi-sql-profiler-2.0.0/tests/test_sql_profiler.py
+drwxr-xr-x   0 sarvadhi1   (502) staff       (20)        0 2023-06-26 06:34:48.959242 fastapi-sql-profiler-3.0.0/
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)      611 2023-06-26 06:34:48.957584 fastapi-sql-profiler-3.0.0/PKG-INFO
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)     1847 2023-06-26 06:25:44.000000 fastapi-sql-profiler-3.0.0/README.md
+drwxr-xr-x   0 sarvadhi1   (502) staff       (20)        0 2023-06-26 06:34:48.790633 fastapi-sql-profiler-3.0.0/fastapi_sql_profiler/
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)       77 2023-06-23 11:17:08.000000 fastapi-sql-profiler-3.0.0/fastapi_sql_profiler/__init__.py
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)     2846 2023-06-23 11:02:00.000000 fastapi-sql-profiler-3.0.0/fastapi_sql_profiler/add_request.py
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)     1060 2023-06-21 06:53:09.000000 fastapi-sql-profiler-3.0.0/fastapi_sql_profiler/database.py
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)    10158 2023-06-23 11:10:06.000000 fastapi-sql-profiler-3.0.0/fastapi_sql_profiler/middleware.py
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)     1035 2023-06-23 10:30:16.000000 fastapi-sql-profiler-3.0.0/fastapi_sql_profiler/models.py
+drwxr-xr-x   0 sarvadhi1   (502) staff       (20)        0 2023-06-26 06:34:48.953112 fastapi-sql-profiler-3.0.0/fastapi_sql_profiler/templates/
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)     3449 2023-06-23 10:05:39.000000 fastapi-sql-profiler-3.0.0/fastapi_sql_profiler/templates/base.html
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)     4738 2023-06-23 11:02:52.000000 fastapi-sql-profiler-3.0.0/fastapi_sql_profiler/templates/request.html
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)     2178 2023-06-23 10:40:36.000000 fastapi-sql-profiler-3.0.0/fastapi_sql_profiler/templates/request_show.html
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)     2012 2023-06-23 10:35:46.000000 fastapi-sql-profiler-3.0.0/fastapi_sql_profiler/templates/sql_query.html
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)      987 2023-06-23 10:53:04.000000 fastapi-sql-profiler-3.0.0/fastapi_sql_profiler/templates/sql_query_detail.html
+drwxr-xr-x   0 sarvadhi1   (502) staff       (20)        0 2023-06-26 06:34:48.799426 fastapi-sql-profiler-3.0.0/fastapi_sql_profiler.egg-info/
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)      611 2023-06-26 06:34:48.000000 fastapi-sql-profiler-3.0.0/fastapi_sql_profiler.egg-info/PKG-INFO
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)      680 2023-06-26 06:34:48.000000 fastapi-sql-profiler-3.0.0/fastapi_sql_profiler.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)        1 2023-06-26 06:34:48.000000 fastapi-sql-profiler-3.0.0/fastapi_sql_profiler.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)       94 2023-06-26 06:34:48.000000 fastapi-sql-profiler-3.0.0/fastapi_sql_profiler.egg-info/requires.txt
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)       21 2023-06-26 06:34:48.000000 fastapi-sql-profiler-3.0.0/fastapi_sql_profiler.egg-info/top_level.txt
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)       90 2023-06-17 09:13:44.000000 fastapi-sql-profiler-3.0.0/pyproject.toml
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)       38 2023-06-26 06:34:48.959389 fastapi-sql-profiler-3.0.0/setup.cfg
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)      940 2023-06-26 06:32:36.000000 fastapi-sql-profiler-3.0.0/setup.py
+drwxr-xr-x   0 sarvadhi1   (502) staff       (20)        0 2023-06-26 06:34:48.955597 fastapi-sql-profiler-3.0.0/tests/
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)     3950 2023-06-23 12:57:41.000000 fastapi-sql-profiler-3.0.0/tests/test_sql_profiler.py
```

### Comparing `fastapi-sql-profiler-2.0.0/PKG-INFO` & `fastapi-sql-profiler-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sql-profiler
-Version: 2.0.0
+Version: 3.0.0
 Summary: Middleware for profiling and logging database queries in a Python web application
 Home-page: https://github.com/Sarvadhi-Solutions/fastapi-sql-profiler.git
 Author: Ganesh Sali
 Author-email: ganesh@sarvadhi.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `fastapi-sql-profiler-2.0.0/fastapi_sql_profiler/add_request.py` & `fastapi-sql-profiler-3.0.0/fastapi_sql_profiler/add_request.py`

 * *Files identical despite different names*

### Comparing `fastapi-sql-profiler-2.0.0/fastapi_sql_profiler/database.py` & `fastapi-sql-profiler-3.0.0/fastapi_sql_profiler/database.py`

 * *Files identical despite different names*

### Comparing `fastapi-sql-profiler-2.0.0/fastapi_sql_profiler/middleware.py` & `fastapi-sql-profiler-3.0.0/fastapi_sql_profiler/middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi-sql-profiler-2.0.0/fastapi_sql_profiler/models.py` & `fastapi-sql-profiler-3.0.0/fastapi_sql_profiler/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-sql-profiler-2.0.0/fastapi_sql_profiler.egg-info/PKG-INFO` & `fastapi-sql-profiler-3.0.0/fastapi_sql_profiler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sql-profiler
-Version: 2.0.0
+Version: 3.0.0
 Summary: Middleware for profiling and logging database queries in a Python web application
 Home-page: https://github.com/Sarvadhi-Solutions/fastapi-sql-profiler.git
 Author: Ganesh Sali
 Author-email: ganesh@sarvadhi.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `fastapi-sql-profiler-2.0.0/setup.py` & `fastapi-sql-profiler-3.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from setuptools import setup
 
 setup(
     name='fastapi-sql-profiler',
-    version='2.0.0',
+    version='3.0.0',
     description='Middleware for profiling and logging database queries in a Python web application',
+    package_data={'fastapi_sql_profiler': ['templates/*']},
     author='Ganesh Sali',
     author_email='ganesh@sarvadhi.com',
     url="https://github.com/Sarvadhi-Solutions/fastapi-sql-profiler.git",
     install_requires=[
         "fastapi >= 0.97.0",
         "SQLAlchemy >= 2.0.16",
         "python-dotenv >= 1.0.0",
```

### Comparing `fastapi-sql-profiler-2.0.0/tests/test_sql_profiler.py` & `fastapi-sql-profiler-3.0.0/tests/test_sql_profiler.py`

 * *Files identical despite different names*

