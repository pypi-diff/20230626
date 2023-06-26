# Comparing `tmp/Flask-Cors-4.0.0.tar.gz` & `tmp/Flask-Cors-4.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Cors-4.0.0.tar", last modified: Mon Jun 26 05:38:34 2023, max compression
+gzip compressed data, was "Flask-Cors-4.0.0a0.tar", last modified: Mon Jun 26 01:19:10 2023, max compression
```

## Comparing `Flask-Cors-4.0.0.tar` & `Flask-Cors-4.0.0a0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:38:34.166286 Flask-Cors-4.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:38:34.162285 Flask-Cors-4.0.0/Flask_Cors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-06-26 05:38:34.000000 Flask-Cors-4.0.0/Flask_Cors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-26 05:38:34.000000 Flask-Cors-4.0.0/Flask_Cors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 05:38:34.000000 Flask-Cors-4.0.0/Flask_Cors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 05:38:33.000000 Flask-Cors-4.0.0/Flask_Cors.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 05:38:34.000000 Flask-Cors-4.0.0/Flask_Cors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 05:38:34.000000 Flask-Cors-4.0.0/Flask_Cors.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-06-26 05:38:34.166286 Flask-Cors-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:38:34.162285 Flask-Cors-4.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:38:34.162285 Flask-Cors-4.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/examples/app_based_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/examples/blueprints_based_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/examples/view_based_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:38:34.166286 Flask-Cors-4.0.0/flask_cors/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/flask_cors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14063 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/flask_cors/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/flask_cors/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/flask_cors/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/flask_cors/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 05:38:34.166286 Flask-Cors-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:38:34.166286 Flask-Cors-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/tests/base_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:38:34.166286 Flask-Cors-4.0.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/tests/core/helper_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/tests/core/test_override_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:38:34.166286 Flask-Cors-4.0.0/tests/decorator/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/tests/decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/tests/decorator/test_allow_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/tests/decorator/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/tests/decorator/test_duplicate_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/tests/decorator/test_exception_interception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/tests/decorator/test_expose_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/tests/decorator/test_max_age.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/tests/decorator/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/tests/decorator/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/tests/decorator/test_origins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/tests/decorator/test_vary_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/tests/decorator/test_w3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:38:34.166286 Flask-Cors-4.0.0/tests/extension/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/tests/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13982 2023-06-26 05:38:24.000000 Flask-Cors-4.0.0/tests/extension/test_app_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:19:10.163316 Flask-Cors-4.0.0a0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:19:10.163316 Flask-Cors-4.0.0a0/Flask_Cors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-26 01:19:10.000000 Flask-Cors-4.0.0a0/Flask_Cors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-26 01:19:10.000000 Flask-Cors-4.0.0a0/Flask_Cors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 01:19:10.000000 Flask-Cors-4.0.0a0/Flask_Cors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 01:19:10.000000 Flask-Cors-4.0.0a0/Flask_Cors.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 01:19:10.000000 Flask-Cors-4.0.0a0/Flask_Cors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 01:19:10.000000 Flask-Cors-4.0.0a0/Flask_Cors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-26 01:19:10.167316 Flask-Cors-4.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:19:10.163316 Flask-Cors-4.0.0a0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:19:10.163316 Flask-Cors-4.0.0a0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/examples/app_based_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/examples/blueprints_based_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/examples/view_based_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:19:10.163316 Flask-Cors-4.0.0a0/flask_cors/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/flask_cors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14063 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/flask_cors/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/flask_cors/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/flask_cors/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/flask_cors/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 01:19:10.167316 Flask-Cors-4.0.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:19:10.163316 Flask-Cors-4.0.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/base_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:19:10.163316 Flask-Cors-4.0.0a0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/core/helper_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/core/test_override_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:19:10.163316 Flask-Cors-4.0.0a0/tests/decorator/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_allow_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_duplicate_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_exception_interception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_expose_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_max_age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_origins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_vary_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/decorator/test_w3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:19:10.163316 Flask-Cors-4.0.0a0/tests/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13982 2023-06-26 01:19:00.000000 Flask-Cors-4.0.0a0/tests/extension/test_app_extension.py
```

### Comparing `Flask-Cors-4.0.0/Flask_Cors.egg-info/PKG-INFO` & `Flask-Cors-4.0.0a0/Flask_Cors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Cors
-Version: 4.0.0
+Version: 4.0.0a0
 Summary: A Flask extension adding a decorator for CORS support
 Home-page: https://github.com/corydolphin/flask-cors
 Author: Cory Dolphin
 Author-email: corydolphin@gmail.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `Flask-Cors-4.0.0/Flask_Cors.egg-info/SOURCES.txt` & `Flask-Cors-4.0.0a0/Flask_Cors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/LICENSE` & `Flask-Cors-4.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/PKG-INFO` & `Flask-Cors-4.0.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Cors
-Version: 4.0.0
+Version: 4.0.0a0
 Summary: A Flask extension adding a decorator for CORS support
 Home-page: https://github.com/corydolphin/flask-cors
 Author: Cory Dolphin
 Author-email: corydolphin@gmail.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
```

### Comparing `Flask-Cors-4.0.0/README.rst` & `Flask-Cors-4.0.0a0/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/docs/Makefile` & `Flask-Cors-4.0.0a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/docs/api.rst` & `Flask-Cors-4.0.0a0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/docs/conf.py` & `Flask-Cors-4.0.0a0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/docs/configuration.rst` & `Flask-Cors-4.0.0a0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/examples/app_based_example.py` & `Flask-Cors-4.0.0a0/examples/app_based_example.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/examples/blueprints_based_example.py` & `Flask-Cors-4.0.0a0/examples/blueprints_based_example.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/examples/view_based_example.py` & `Flask-Cors-4.0.0a0/examples/view_based_example.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/flask_cors/__init__.py` & `Flask-Cors-4.0.0a0/flask_cors/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/flask_cors/core.py` & `Flask-Cors-4.0.0a0/flask_cors/core.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/flask_cors/decorator.py` & `Flask-Cors-4.0.0a0/flask_cors/decorator.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/flask_cors/extension.py` & `Flask-Cors-4.0.0a0/flask_cors/extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         # the app's configuration, the constructor, the kwargs to init_app, and
         # finally the options specified in the resources dictionary.
         resources = [
                      (pattern, get_cors_options(app, options, opts))
                      for (pattern, opts) in resources
                     ]
 
-        # Create a human-readable form of these resources by converting the compiled
+        # Create a human readable form of these resources by converting the compiled
         # regular expressions into strings.
         resources_human = {get_regexp_pattern(pattern): opts for (pattern,opts) in resources}
         LOG.debug("Configuring CORS with resources: %s", resources_human)
 
         cors_after_request = make_after_request_function(resources)
         app.after_request(cors_after_request)
```

### Comparing `Flask-Cors-4.0.0/setup.py` & `Flask-Cors-4.0.0a0/setup.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/tests/base_test.py` & `Flask-Cors-4.0.0a0/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/tests/core/helper_tests.py` & `Flask-Cors-4.0.0a0/tests/core/helper_tests.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/tests/core/test_override_headers.py` & `Flask-Cors-4.0.0a0/tests/core/test_override_headers.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/tests/decorator/test_allow_headers.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_allow_headers.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/tests/decorator/test_credentials.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_credentials.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/tests/decorator/test_duplicate_headers.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_duplicate_headers.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/tests/decorator/test_exception_interception.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_exception_interception.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/tests/decorator/test_expose_headers.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_expose_headers.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/tests/decorator/test_max_age.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_max_age.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/tests/decorator/test_methods.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_methods.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/tests/decorator/test_options.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_options.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/tests/decorator/test_origins.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_origins.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/tests/decorator/test_vary_header.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_vary_header.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/tests/decorator/test_w3.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_w3.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-4.0.0/tests/extension/test_app_extension.py` & `Flask-Cors-4.0.0a0/tests/extension/test_app_extension.py`

 * *Files identical despite different names*

