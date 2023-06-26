# Comparing `tmp/fastapi-sql-profiler-4.0.0.tar.gz` & `tmp/fastapi-sql-profiler-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-sql-profiler-4.0.0.tar", last modified: Mon Jun 26 06:51:45 2023, max compression
+gzip compressed data, was "fastapi-sql-profiler-5.0.0.tar", last modified: Mon Jun 26 07:21:24 2023, max compression
```

## Comparing `fastapi-sql-profiler-4.0.0.tar` & `fastapi-sql-profiler-5.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sarvadhi1   (502) staff       (20)        0 2023-06-26 06:51:45.131178 fastapi-sql-profiler-4.0.0/
--rw-r--r--   0 sarvadhi1   (502) staff       (20)      611 2023-06-26 06:51:45.130230 fastapi-sql-profiler-4.0.0/PKG-INFO
--rw-r--r--   0 sarvadhi1   (502) staff       (20)     1847 2023-06-26 06:25:44.000000 fastapi-sql-profiler-4.0.0/README.md
-drwxr-xr-x   0 sarvadhi1   (502) staff       (20)        0 2023-06-26 06:51:45.011626 fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/
--rw-r--r--   0 sarvadhi1   (502) staff       (20)       77 2023-06-23 11:17:08.000000 fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/__init__.py
--rw-r--r--   0 sarvadhi1   (502) staff       (20)     2846 2023-06-23 11:02:00.000000 fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/add_request.py
--rw-r--r--   0 sarvadhi1   (502) staff       (20)     1060 2023-06-21 06:53:09.000000 fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/database.py
--rw-r--r--   0 sarvadhi1   (502) staff       (20)    10175 2023-06-26 06:44:43.000000 fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/middleware.py
--rw-r--r--   0 sarvadhi1   (502) staff       (20)     1035 2023-06-23 10:30:16.000000 fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/models.py
-drwxr-xr-x   0 sarvadhi1   (502) staff       (20)        0 2023-06-26 06:51:45.126889 fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/templates/
--rw-r--r--   0 sarvadhi1   (502) staff       (20)     3449 2023-06-23 10:05:39.000000 fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/templates/base.html
--rw-r--r--   0 sarvadhi1   (502) staff       (20)     4738 2023-06-23 11:02:52.000000 fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/templates/request.html
--rw-r--r--   0 sarvadhi1   (502) staff       (20)     2178 2023-06-23 10:40:36.000000 fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/templates/request_show.html
--rw-r--r--   0 sarvadhi1   (502) staff       (20)     2012 2023-06-23 10:35:46.000000 fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/templates/sql_query.html
--rw-r--r--   0 sarvadhi1   (502) staff       (20)      987 2023-06-23 10:53:04.000000 fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/templates/sql_query_detail.html
-drwxr-xr-x   0 sarvadhi1   (502) staff       (20)        0 2023-06-26 06:51:45.115320 fastapi-sql-profiler-4.0.0/fastapi_sql_profiler.egg-info/
--rw-r--r--   0 sarvadhi1   (502) staff       (20)      611 2023-06-26 06:51:44.000000 fastapi-sql-profiler-4.0.0/fastapi_sql_profiler.egg-info/PKG-INFO
--rw-r--r--   0 sarvadhi1   (502) staff       (20)      680 2023-06-26 06:51:44.000000 fastapi-sql-profiler-4.0.0/fastapi_sql_profiler.egg-info/SOURCES.txt
--rw-r--r--   0 sarvadhi1   (502) staff       (20)        1 2023-06-26 06:51:44.000000 fastapi-sql-profiler-4.0.0/fastapi_sql_profiler.egg-info/dependency_links.txt
--rw-r--r--   0 sarvadhi1   (502) staff       (20)       94 2023-06-26 06:51:44.000000 fastapi-sql-profiler-4.0.0/fastapi_sql_profiler.egg-info/requires.txt
--rw-r--r--   0 sarvadhi1   (502) staff       (20)       21 2023-06-26 06:51:44.000000 fastapi-sql-profiler-4.0.0/fastapi_sql_profiler.egg-info/top_level.txt
--rw-r--r--   0 sarvadhi1   (502) staff       (20)       90 2023-06-17 09:13:44.000000 fastapi-sql-profiler-4.0.0/pyproject.toml
--rw-r--r--   0 sarvadhi1   (502) staff       (20)       38 2023-06-26 06:51:45.132118 fastapi-sql-profiler-4.0.0/setup.cfg
--rw-r--r--   0 sarvadhi1   (502) staff       (20)      940 2023-06-26 06:50:59.000000 fastapi-sql-profiler-4.0.0/setup.py
-drwxr-xr-x   0 sarvadhi1   (502) staff       (20)        0 2023-06-26 06:51:45.128266 fastapi-sql-profiler-4.0.0/tests/
--rw-r--r--   0 sarvadhi1   (502) staff       (20)     3950 2023-06-23 12:57:41.000000 fastapi-sql-profiler-4.0.0/tests/test_sql_profiler.py
+drwxr-xr-x   0 sarvadhi1   (502) staff       (20)        0 2023-06-26 07:21:24.840467 fastapi-sql-profiler-5.0.0/
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)      611 2023-06-26 07:21:24.834275 fastapi-sql-profiler-5.0.0/PKG-INFO
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)     1834 2023-06-26 07:04:54.000000 fastapi-sql-profiler-5.0.0/README.md
+drwxr-xr-x   0 sarvadhi1   (502) staff       (20)        0 2023-06-26 07:21:24.738954 fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)       77 2023-06-23 11:17:08.000000 fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/__init__.py
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)     2846 2023-06-23 11:02:00.000000 fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/add_request.py
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)     1060 2023-06-21 06:53:09.000000 fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/database.py
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)    10175 2023-06-26 06:44:43.000000 fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/middleware.py
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)     1035 2023-06-23 10:30:16.000000 fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/models.py
+drwxr-xr-x   0 sarvadhi1   (502) staff       (20)        0 2023-06-26 07:21:24.829710 fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/templates/
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)     3449 2023-06-23 10:05:39.000000 fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/templates/base.html
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)     4738 2023-06-23 11:02:52.000000 fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/templates/request.html
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)     2440 2023-06-26 07:15:53.000000 fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/templates/request_show.html
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)     2012 2023-06-23 10:35:46.000000 fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/templates/sql_query.html
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)      987 2023-06-23 10:53:04.000000 fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/templates/sql_query_detail.html
+drwxr-xr-x   0 sarvadhi1   (502) staff       (20)        0 2023-06-26 07:21:24.766278 fastapi-sql-profiler-5.0.0/fastapi_sql_profiler.egg-info/
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)      611 2023-06-26 07:21:24.000000 fastapi-sql-profiler-5.0.0/fastapi_sql_profiler.egg-info/PKG-INFO
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)      680 2023-06-26 07:21:24.000000 fastapi-sql-profiler-5.0.0/fastapi_sql_profiler.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)        1 2023-06-26 07:21:24.000000 fastapi-sql-profiler-5.0.0/fastapi_sql_profiler.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)       94 2023-06-26 07:21:24.000000 fastapi-sql-profiler-5.0.0/fastapi_sql_profiler.egg-info/requires.txt
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)       21 2023-06-26 07:21:24.000000 fastapi-sql-profiler-5.0.0/fastapi_sql_profiler.egg-info/top_level.txt
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)       90 2023-06-17 09:13:44.000000 fastapi-sql-profiler-5.0.0/pyproject.toml
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)       38 2023-06-26 07:21:24.840642 fastapi-sql-profiler-5.0.0/setup.cfg
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)      940 2023-06-26 07:18:57.000000 fastapi-sql-profiler-5.0.0/setup.py
+drwxr-xr-x   0 sarvadhi1   (502) staff       (20)        0 2023-06-26 07:21:24.832332 fastapi-sql-profiler-5.0.0/tests/
+-rw-r--r--   0 sarvadhi1   (502) staff       (20)     3950 2023-06-23 12:57:41.000000 fastapi-sql-profiler-5.0.0/tests/test_sql_profiler.py
```

### Comparing `fastapi-sql-profiler-4.0.0/PKG-INFO` & `fastapi-sql-profiler-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sql-profiler
-Version: 4.0.0
+Version: 5.0.0
 Summary: Middleware for profiling and logging database queries in a Python web application
 Home-page: https://github.com/Sarvadhi-Solutions/fastapi-sql-profiler.git
 Author: Ganesh Sali
 Author-email: ganesh@sarvadhi.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `fastapi-sql-profiler-4.0.0/README.md` & `fastapi-sql-profiler-5.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## Database Query Profiling Middleware
 
 This project is a middleware implementation for profiling and logging database queries in a Python web application. It utilizes the Starlette framework and SQLAlchemy for interacting with the database.
 
 ## Features
 
-    * Profiles and logs database queries made within the web application.
+    * Logs database queries made within the web application.
     * Captures query execution times, query texts, and stack traces.
     * Stores query information in a database table along with request details.
     * Provides insights into query performance for debugging and optimization.
 
 ## Installation
 
 pip install fastapi-sql-profiler
```

### Comparing `fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/add_request.py` & `fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/add_request.py`

 * *Files identical despite different names*

### Comparing `fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/database.py` & `fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/database.py`

 * *Files identical despite different names*

### Comparing `fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/middleware.py` & `fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/models.py` & `fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/templates/base.html` & `fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/templates/base.html`

 * *Files identical despite different names*

### Comparing `fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/templates/request.html` & `fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/templates/request.html`

 * *Files identical despite different names*

### Comparing `fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/templates/request_show.html` & `fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/templates/request_show.html`

 * *Files 23% similar despite different names*

```diff
@@ -9,21 +9,21 @@
             <div class="card border-2 border-secondary shadow">
                 <div class="card-body">
                     <h5 class="card-title mb-2">
                         <span class="badge {% if request_info.method == 'GET' %}bg-success{% elif request_info.method == 'POST' %}bg-warning{% elif request_info.method == 'DELETE' %}bg-danger{% elif request_info.method == 'PUT' %}bg-info{% else %}bg-secondary{% endif %}">
                             {{ request_info.method }}
                         </span>
                     </h5>
-                    <div class="card-text">
+                    <div class="card-text" style="max-width: 200px; overflow: hidden; text-overflow: ellipsis; white-space: nowrap;">
                         <strong>Path:</strong> {{ request_info.path }}
                     </div>
-                    <div class="card-text">
-                        <strong>Time Taken:</strong> {{ request_info.time_taken }} ms overall
+                    <div class="card-text" style="max-width: 200px; overflow: hidden; text-overflow: ellipsis; white-space: nowrap;">
+                        <strong>Time Taken:</strong> {{ request_info.time_taken }} ms
                     </div>
-                    <div class="card-text">
+                    <div class="card-text" style="max-width: 200px; overflow: hidden; text-overflow: ellipsis; white-space: nowrap;">
                         <strong>Total Queries:</strong> {{ request_info.total_queries }} queries
                     </div>
                 </div>
             </div>
         </a>
     </div>
     {% endfor %}
```

### Comparing `fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/templates/sql_query.html` & `fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/templates/sql_query.html`

 * *Files identical despite different names*

### Comparing `fastapi-sql-profiler-4.0.0/fastapi_sql_profiler/templates/sql_query_detail.html` & `fastapi-sql-profiler-5.0.0/fastapi_sql_profiler/templates/sql_query_detail.html`

 * *Files identical despite different names*

### Comparing `fastapi-sql-profiler-4.0.0/fastapi_sql_profiler.egg-info/PKG-INFO` & `fastapi-sql-profiler-5.0.0/fastapi_sql_profiler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sql-profiler
-Version: 4.0.0
+Version: 5.0.0
 Summary: Middleware for profiling and logging database queries in a Python web application
 Home-page: https://github.com/Sarvadhi-Solutions/fastapi-sql-profiler.git
 Author: Ganesh Sali
 Author-email: ganesh@sarvadhi.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `fastapi-sql-profiler-4.0.0/fastapi_sql_profiler.egg-info/SOURCES.txt` & `fastapi-sql-profiler-5.0.0/fastapi_sql_profiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi-sql-profiler-4.0.0/setup.py` & `fastapi-sql-profiler-5.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='fastapi-sql-profiler',
-    version='4.0.0',
+    version='5.0.0',
     description='Middleware for profiling and logging database queries in a Python web application',
     package_data={'fastapi_sql_profiler': ['templates/*']},
     author='Ganesh Sali',
     author_email='ganesh@sarvadhi.com',
     url="https://github.com/Sarvadhi-Solutions/fastapi-sql-profiler.git",
     install_requires=[
         "fastapi >= 0.97.0",
```

### Comparing `fastapi-sql-profiler-4.0.0/tests/test_sql_profiler.py` & `fastapi-sql-profiler-5.0.0/tests/test_sql_profiler.py`

 * *Files identical despite different names*

