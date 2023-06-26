# Comparing `tmp/Flask-Cors-3.0.9.tar.gz` & `tmp/Flask-Cors-4.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-Cors-3.0.9.tar", last modified: Sun Aug 30 21:48:44 2020, max compression
+gzip compressed data, was "Flask-Cors-4.0.0a0.tar", last modified: Mon Jun 26 01:19:10 2023, max compression
```

## Comparing `Flask-Cors-3.0.9.tar` & `Flask-Cors-4.0.0a0.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-30 21:48:44.000000 Flask-Cors-3.0.9/
--rw-rw-r--   0 travis    (2000) travis    (2000)      186 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-30 21:48:44.000000 Flask-Cors-3.0.9/examples/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3403 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/examples/view_based_example.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4920 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/examples/app_based_example.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3595 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/examples/blueprints_based_example.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-30 21:48:44.000000 Flask-Cors-3.0.9/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2543 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/docs/api.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     5580 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)     8223 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       90 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/docs/index.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-30 21:48:44.000000 Flask-Cors-3.0.9/Flask_Cors.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6387 2020-08-30 21:48:44.000000 Flask-Cors-3.0.9/Flask_Cors.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-08-30 21:48:44.000000 Flask-Cors-3.0.9/Flask_Cors.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2020-08-30 21:48:44.000000 Flask-Cors-3.0.9/Flask_Cors.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-08-30 21:48:44.000000 Flask-Cors-3.0.9/Flask_Cors.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)     1143 2020-08-30 21:48:44.000000 Flask-Cors-3.0.9/Flask_Cors.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       15 2020-08-30 21:48:44.000000 Flask-Cors-3.0.9/Flask_Cors.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       15 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     6387 2020-08-30 21:48:44.000000 Flask-Cors-3.0.9/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2020-08-30 21:48:44.000000 Flask-Cors-3.0.9/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1069 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-30 21:48:44.000000 Flask-Cors-3.0.9/flask_cors/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13894 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/flask_cors/core.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7585 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/flask_cors/extension.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4937 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/flask_cors/decorator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/flask_cors/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      791 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/flask_cors/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4214 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1959 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-30 21:48:44.000000 Flask-Cors-3.0.9/tests/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-30 21:48:44.000000 Flask-Cors-3.0.9/tests/extension/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13981 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/tests/extension/test_app_extension.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      310 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/tests/extension/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2905 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/tests/base_test.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-30 21:48:44.000000 Flask-Cors-3.0.9/tests/decorator/
--rw-rw-r--   0 travis    (2000) travis    (2000)      852 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/tests/decorator/test_duplicate_headers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3136 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/tests/decorator/test_vary_header.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7911 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/tests/decorator/test_exception_interception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4323 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/tests/decorator/test_allow_headers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8070 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/tests/decorator/test_origins.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2866 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/tests/decorator/test_options.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2591 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/tests/decorator/test_w3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2070 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/tests/decorator/test_credentials.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1843 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/tests/decorator/test_max_age.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      318 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/tests/decorator/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2162 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/tests/decorator/test_methods.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1335 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/tests/decorator/test_expose_headers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-30 21:48:44.000000 Flask-Cors-3.0.9/tests/core/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3124 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/tests/core/helper_tests.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      815 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/tests/core/test_override_headers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      316 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/tests/core/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2020-08-30 21:48:21.000000 Flask-Cors-3.0.9/tests/__init__.py
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

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Flask-Cors-3.0.9/examples/view_based_example.py` & `Flask-Cors-4.0.0a0/examples/view_based_example.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-3.0.9/examples/app_based_example.py` & `Flask-Cors-4.0.0a0/examples/app_based_example.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,12 +139,12 @@
         Date: Sat, 31 Jan 2015 22:25:22 GMT
     """
     raise Exception("example")
 
 @app.errorhandler(500)
 def server_error(e):
     logging.exception('An error occurred during a request. %s', e)
-    return "An internal error occured", 500
+    return "An internal error occurred", 500
 
 
 if __name__ == "__main__":
     app.run(debug=True)
```

### Comparing `Flask-Cors-3.0.9/examples/blueprints_based_example.py` & `Flask-Cors-4.0.0a0/examples/blueprints_based_example.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-3.0.9/docs/api.rst` & `Flask-Cors-4.0.0a0/docs/api.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 API Docs
 ==========
 
-This package exposes a Flask extension which by default enables CORS support on all routes, for all origins and methods. It allows parameterization of all CORS headers on a per-resource level. The package also contains a decorator, for those who prefer this approach.
+This package exposes a Flask extension which by default enables CORS support on all routes, for all origins and methods.
+It allows parameterization of all CORS headers on a per-resource level. The package also contains a decorator, for those who prefer this approach.
 
 Extension
 ~~~~~~~~~
 
-This is the suggested approach to enabling CORS. The default configuration
-will work well for most use cases.
+This is the suggested approach to enabling CORS.
+The default configuration will work well for most use cases.
 
 .. autoclass:: flask_cors.CORS
 
 Decorator
 ~~~~~~~~~
 
-If the `CORS` extension does not satisfy your needs, you may find the
-decorator useful. It shares options with the extension, and should be simple
-to use.
+If the `CORS` extension does not satisfy your needs, you may find the decorator useful.
+It shares options with the extension, and should be simple to use.
 
 .. autofunction:: flask_cors.cross_origin
 
 
 Using `CORS` with cookies
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
-By default, Flask-CORS does not allow cookies to be submitted across sites,
-since it has potential security implications. If you wish to enable cross-site
-cookies, you may wish to add some sort of
-`CSRF <http://en.wikipedia.org/wiki/Cross-site_request_forgery>`__
-protection to keep you and your users safe.
+By default, Flask-CORS does not allow cookies to be submitted across sites, since it has potential security implications.
+If you wish to enable cross-site cookies, you may wish to add some sort of `CSRF <http://en.wikipedia.org/wiki/Cross-site_request_forgery>`__ protection to keep you and your users safe.
 
-To allow cookies or authenticated requests to be made
-cross origins, simply set the `supports_credentials` option to `True`. E.G.
+To allow cookies or authenticated requests to be made cross origins, simply set the `supports_credentials` option to `True`. E.g.
 
 .. code:: python
 
 
     from flask import Flask, session
     from flask_cors import CORS
 
@@ -43,21 +39,25 @@
     CORS(app, supports_credentials=True)
 
     @app.route("/")
     def helloWorld():
       return "Hello, %s" % session['username']
 
 
-The above code enables Flask backend to accept cookies to be submitted from cross origin sites. But if you are sending Xhr requests (ajax calls) to a cross-origin server, by default chrome or any modern browser won't send cookies and session with the request. You should use ``withCredentials = True`` while sending Xhr request to enable that. You should keep in mind about the necessary security concerns. Related MDN doc: https://developer.mozilla.org/en-US/docs/Web/API/XMLHttpRequest/withCredentials
+The above code enables Flask backend to accept cookies to be submitted from cross origin sites.
+But if you are sending Xhr requests (ajax calls) to a cross-origin server, by default chrome or any modern browser won't send cookies and session with the request.
+You should use ``withCredentials = True`` while sending Xhr request to enable that.
+You should keep in mind about the necessary security concerns.
+Related MDN doc: https://developer.mozilla.org/en-US/docs/Web/API/XMLHttpRequest/withCredentials
 
 Using `CORS` with Blueprints
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Flask-CORS supports blueprints out of the box. Simply pass a `blueprint`
-instance to the CORS extension, and everything will just work.
+Flask-CORS supports blueprints out of the box.
+Simply pass a `blueprint` instance to the CORS extension, and everything will just work.
 
 .. literalinclude:: ../examples/blueprints_based_example.py
   :language: python
   :lines: 23-
 
 
 Examples
@@ -66,13 +66,13 @@
 Using the `CORS` extension
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^
 .. literalinclude:: ../examples/app_based_example.py
    :language: python
    :lines: 29-
 
 
-Using the `cross_origins` decorator
+Using the `cross_origin` decorator
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. literalinclude:: ../examples/view_based_example.py
    :language: python
    :lines: 27-
```

### Comparing `Flask-Cors-3.0.9/docs/Makefile` & `Flask-Cors-4.0.0a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-Cors-3.0.9/docs/conf.py` & `Flask-Cors-4.0.0a0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.intersphinx']
+extensions = ['sphinx.ext.autodoc', 'sphinx.ext.intersphinx', 'sphinxcontrib.httpdomain']
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
 
@@ -122,15 +122,15 @@
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
 #html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+#html_static_path = ['_static']
 
 # Add any extra paths that contain custom files (such as robots.txt or
 # .htaccess) here, relative to this directory. These files are copied
 # directly to the root of the documentation.
 #html_extra_path = []
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
```

### Comparing `Flask-Cors-3.0.9/Flask_Cors.egg-info/SOURCES.txt` & `Flask-Cors-4.0.0a0/Flask_Cors.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 Flask_Cors.egg-info/dependency_links.txt
 Flask_Cors.egg-info/not-zip-safe
 Flask_Cors.egg-info/requires.txt
 Flask_Cors.egg-info/top_level.txt
 docs/Makefile
 docs/api.rst
 docs/conf.py
+docs/configuration.rst
 docs/index.rst
+docs/requirements.txt
 examples/app_based_example.py
 examples/blueprints_based_example.py
 examples/view_based_example.py
 flask_cors/__init__.py
 flask_cors/core.py
 flask_cors/decorator.py
 flask_cors/extension.py
```

### Comparing `Flask-Cors-3.0.9/LICENSE` & `Flask-Cors-4.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Cors-3.0.9/flask_cors/core.py` & `Flask-Cors-4.0.0a0/flask_cors/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,38 +5,34 @@
     Core functionality shared between the extension and the decorator.
 
     :copyright: (c) 2016 by Cory Dolphin.
     :license: MIT, see LICENSE for more details.
 """
 import re
 import logging
-try:
-    # on python 3
-    from collections.abc import Iterable
-except ImportError:
-    # on python 2.7 and pypy
-    from collections import Iterable
+from collections.abc import Iterable
 from datetime import timedelta
-from six import string_types
 from flask import request, current_app
 from werkzeug.datastructures import Headers, MultiDict
 
 LOG = logging.getLogger(__name__)
 
 # Response Headers
 ACL_ORIGIN = 'Access-Control-Allow-Origin'
 ACL_METHODS = 'Access-Control-Allow-Methods'
 ACL_ALLOW_HEADERS = 'Access-Control-Allow-Headers'
 ACL_EXPOSE_HEADERS = 'Access-Control-Expose-Headers'
 ACL_CREDENTIALS = 'Access-Control-Allow-Credentials'
 ACL_MAX_AGE = 'Access-Control-Max-Age'
+ACL_RESPONSE_PRIVATE_NETWORK = 'Access-Control-Allow-Private-Network'
 
 # Request Header
 ACL_REQUEST_METHOD = 'Access-Control-Request-Method'
 ACL_REQUEST_HEADERS = 'Access-Control-Request-Headers'
+ACL_REQUEST_HEADER_PRIVATE_NETWORK = 'Access-Control-Request-Private-Network'
 
 ALL_METHODS = ['GET', 'HEAD', 'POST', 'OPTIONS', 'PUT', 'PATCH', 'DELETE']
 CONFIG_OPTIONS = ['CORS_ORIGINS', 'CORS_METHODS', 'CORS_ALLOW_HEADERS',
                   'CORS_EXPOSE_HEADERS', 'CORS_SUPPORTS_CREDENTIALS',
                   'CORS_MAX_AGE', 'CORS_SEND_WILDCARD',
                   'CORS_AUTOMATIC_OPTIONS', 'CORS_VARY_HEADER',
                   'CORS_RESOURCES', 'CORS_INTERCEPT_EXCEPTIONS',
@@ -76,15 +72,15 @@
             maybe_regex, _ = pair
             return len(get_regexp_pattern(maybe_regex))
 
         return sorted(resources,
                       key=pattern_length,
                       reverse=True)
 
-    elif isinstance(resources, string_types):
+    elif isinstance(resources, str):
         return [(re_fix(resources), {})]
 
     elif isinstance(resources, Iterable):
         return [(re_fix(r), {}) for r in resources]
 
     # Type of compiled regex is not part of the public API. Test for this
     # at runtime.
@@ -182,15 +178,19 @@
 
     for origin in origins_to_set:
         headers.add(ACL_ORIGIN, origin)
 
     headers[ACL_EXPOSE_HEADERS] = options.get('expose_headers')
 
     if options.get('supports_credentials'):
-        headers[ACL_CREDENTIALS] = 'true'  # case sensative
+        headers[ACL_CREDENTIALS] = 'true'  # case sensitive
+
+    if ACL_REQUEST_HEADER_PRIVATE_NETWORK in request_headers \
+            and request_headers.get(ACL_REQUEST_HEADER_PRIVATE_NETWORK) == 'true':
+        headers[ACL_RESPONSE_PRIVATE_NETWORK] = 'true'
 
     # This is a preflight request
     # http://www.w3.org/TR/cors/#resource-preflight-requests
     if request_method == 'OPTIONS':
         acl_request_method = request_headers.get(ACL_REQUEST_METHOD, '').upper()
 
         # If there is no Access-Control-Request-Method header or if parsing
@@ -219,15 +219,15 @@
             headers.add('Vary', 'Origin')
 
     return MultiDict((k, v) for k, v in headers.items() if v)
 
 
 def set_cors_headers(resp, options):
     """
-    Performs the actual evaluation of Flas-CORS options and actually
+    Performs the actual evaluation of Flask-CORS options and actually
     modifies the response object.
 
     This function is used both in the decorator and the after_request
     callback
     """
 
     # If CORS has already been evaluated via the decorator, skip
@@ -319,32 +319,31 @@
     A more flexible str function which intelligently handles stringifying
     strings, lists and other iterables. The results are lexographically sorted
     to ensure generated responses are consistent when iterables such as Set
     are used.
     """
     if obj is None:
         return None
-    elif(not isinstance(obj, string_types)
-            and isinstance(obj, Iterable)):
-        return ', '.join(str(item) for item in sorted(obj))
+    elif not isinstance(obj, str) and isinstance(obj, Iterable):
+        return ", ".join(str(item) for item in sorted(obj))
     else:
         return str(obj)
 
 
 def serialize_option(options_dict, key, upper=False):
     if key in options_dict:
         value = flexible_str(options_dict[key])
         options_dict[key] = value.upper() if upper else value
 
 
 def ensure_iterable(inst):
     """
     Wraps scalars or string types as a list, or returns the iterable instance.
     """
-    if isinstance(inst, string_types):
+    if isinstance(inst, str):
         return [inst]
     elif not isinstance(inst, Iterable):
         return [inst]
     else:
         return inst
 
 def sanitize_regex_param(param):
```

### Comparing `Flask-Cors-3.0.9/flask_cors/extension.py` & `Flask-Cors-4.0.0a0/flask_cors/extension.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,27 @@
     ~~~~
     Flask-CORS is a simple extension to Flask allowing you to support cross
     origin resource sharing (CORS) using a simple decorator.
 
     :copyright: (c) 2016 by Cory Dolphin.
     :license: MIT, see LICENSE for more details.
 """
+import logging
+from urllib.parse import unquote_plus
 from flask import request
-from .core import *
-try:
-    from urllib.parse import unquote_plus
-except ImportError:
-    from urllib import unquote_plus
+
+from .core import (
+    parse_resources,
+    get_cors_options,
+    get_regexp_pattern,
+    ACL_ORIGIN,
+    try_match,
+    set_cors_headers
+)
+
 
 LOG = logging.getLogger(__name__)
 
 class CORS(object):
     """
     Initializes Cross Origin Resource sharing for the application. The
     arguments are identical to :py:func:`cross_origin`, with the addition of a
@@ -57,15 +64,19 @@
         Default : Match all and apply app-level configuration
 
     :type resources: dict, iterable or string
 
     :param origins:
         The origin, or list of origins to allow requests from.
         The origin(s) may be regular expressions, case-sensitive strings,
-        or else an asterisk
+        or else an asterisk.
+
+        :note: origins must include the schema and the port (if not port 80),
+        e.g.,
+        `CORS(app, origins=["http://localhost:8000", "https://example.com"])`.
 
         Default : '*'
     :type origins: list, string or regex
 
     :param methods:
         The method or list of methods which the allowed origins are allowed to
         access for non-simple requests.
@@ -89,15 +100,15 @@
     :type allow_headers: list, string or regex
 
     :param supports_credentials:
         Allows users to make authenticated requests. If true, injects the
         `Access-Control-Allow-Credentials` header in responses. This allows
         cookies and credentials to be submitted across domains.
 
-        :note: This option cannot be used in conjuction with a '*' origin
+        :note: This option cannot be used in conjunction with a '*' origin
 
         Default : False
     :type supports_credentials: bool
 
     :param max_age:
         The maximum time for which this CORS request maybe cached. This value
         is set as the `Access-Control-Max-Age` header.
```

### Comparing `Flask-Cors-3.0.9/flask_cors/decorator.py` & `Flask-Cors-4.0.0a0/flask_cors/decorator.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,30 @@
     This unit exposes a single decorator which should be used to wrap a
     Flask route with. It accepts all parameters and options as
     the CORS extension.
 
     :copyright: (c) 2016 by Cory Dolphin.
     :license: MIT, see LICENSE for more details.
 """
+import logging
 from functools import update_wrapper
 from flask import make_response, request, current_app
-from .core import *
+
+from .core import get_cors_options, set_cors_headers, FLASK_CORS_EVALUATED
 
 LOG = logging.getLogger(__name__)
 
 def cross_origin(*args, **kwargs):
     """
     This function is the decorator which is used to wrap a Flask route with.
     In the simplest case, simply use the default parameters to allow all
     origins in what is the most permissive configuration. If this method
     modifies state or performs authentication which may be brute-forced, you
-    should add some degree of protection, such as Cross Site Forgery
-    Request protection.
+    should add some degree of protection, such as Cross Site Request Forgery
+    protection.
 
     :param origins:
         The origin, or list of origins to allow requests from.
         The origin(s) may be regular expressions, case-sensitive strings,
         or else an asterisk
 
         Default : '*'
@@ -55,15 +57,15 @@
     :type allow_headers: list, string or regex
 
     :param supports_credentials:
         Allows users to make authenticated requests. If true, injects the
         `Access-Control-Allow-Credentials` header in responses. This allows
         cookies and credentials to be submitted across domains.
 
-        :note: This option cannot be used in conjuction with a '*' origin
+        :note: This option cannot be used in conjunction with a '*' origin
 
         Default : False
     :type supports_credentials: bool
 
     :param max_age:
         The maximum time for which this CORS request maybe cached. This value
         is set as the `Access-Control-Max-Age` header.
```

### Comparing `Flask-Cors-3.0.9/flask_cors/__init__.py` & `Flask-Cors-4.0.0a0/flask_cors/__init__.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 
 # Set initial level to WARN. Users must manually enable logging for
 # flask_cors to see our logging.
 rootlogger = logging.getLogger(__name__)
 rootlogger.addHandler(NullHandler())
 
 if rootlogger.level == logging.NOTSET:
-    rootlogger.setLevel(logging.WARN)
+    rootlogger.setLevel(logging.WARN)
```

### Comparing `Flask-Cors-3.0.9/README.rst` & `Flask-Cors-4.0.0a0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 Flask-CORS
 ==========
 
 |Build Status| |Latest Version| |Supported Python versions|
 |License|
 
-A Flask extension for handling Cross Origin Resource Sharing (CORS),
-making cross-origin AJAX possible.
+A Flask extension for handling Cross Origin Resource Sharing (CORS), making cross-origin AJAX possible.
 
-This package has a simple philosophy, when you want to enable CORS, you
-wish to enable it for all use cases on a domain. This means no mucking
-around with different allowed headers, methods, etc. By default,
-submission of cookies across domains is disabled due to the security
-implications, please see the documentation for how to enable
-credential'ed requests, and please make sure you add some sort of
-`CSRF <http://en.wikipedia.org/wiki/Cross-site_request_forgery>`__
-protection before doing so!
+This package has a simple philosophy: when you want to enable CORS, you wish to enable it for all use cases on a domain. 
+This means no mucking around with different allowed headers, methods, etc. 
+
+By default, submission of cookies across domains is disabled due to the security implications. 
+Please see the documentation for how to enable credential'ed requests, and please make sure you add some sort of `CSRF <http://en.wikipedia.org/wiki/Cross-site_request_forgery>`__ protection before doing so!
 
 Installation
 ------------
 
 Install the extension with using pip, or easy\_install.
 
 .. code:: bash
 
     $ pip install -U flask-cors
 
 Usage
 -----
 
-This package exposes a Flask extension which by default enables CORS support on all routes, for all origins and methods. It allows parameterization of all CORS headers on a per-resource level. The package also contains a decorator, for those who prefer this approach.
+This package exposes a Flask extension which by default enables CORS support on all routes, for all origins and methods. 
+It allows parameterization of all CORS headers on a per-resource level. 
+The package also contains a decorator, for those who prefer this approach.
 
 Simple Usage
 ~~~~~~~~~~~~
 
-In the simplest case, initialize the Flask-Cors extension with default
-arguments in order to allow CORS for all domains on all routes. See the
-full list of options in the `documentation <https://flask-cors.corydolphin.com/en/latest/api.html#extension>`__.
+In the simplest case, initialize the Flask-Cors extension with default arguments in order to allow CORS for all domains on all routes. 
+See the full list of options in the `documentation <https://flask-cors.corydolphin.com/en/latest/api.html#extension>`__.
 
 .. code:: python
 
 
     from flask import Flask
     from flask_cors import CORS
 
@@ -49,82 +46,75 @@
     @app.route("/")
     def helloWorld():
       return "Hello, cross-origin-world!"
 
 Resource specific CORS
 ^^^^^^^^^^^^^^^^^^^^^^
 
-Alternatively, you can specify CORS options on a resource and origin
-level of granularity by passing a dictionary as the `resources` option,
-mapping paths to a set of options. See the
-full list of options in the `documentation <https://flask-cors.corydolphin.com/en/latest/api.html#extension>`__.
+Alternatively, you can specify CORS options on a resource and origin level of granularity by passing a dictionary as the `resources` option, mapping paths to a set of options. 
+See the full list of options in the `documentation <https://flask-cors.corydolphin.com/en/latest/api.html#extension>`__.
 
 .. code:: python
 
     app = Flask(__name__)
     cors = CORS(app, resources={r"/api/*": {"origins": "*"}})
 
     @app.route("/api/v1/users")
     def list_users():
       return "user example"
 
 Route specific CORS via decorator
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-This extension also exposes a simple decorator to decorate flask routes
-with. Simply add ``@cross_origin()`` below a call to Flask's
-``@app.route(..)`` to allow CORS on a given route. See the
-full list of options in the `decorator documentation <https://flask-cors.corydolphin.com/en/latest/api.html#decorator>`__.
+This extension also exposes a simple decorator to decorate flask routes with. 
+Simply add ``@cross_origin()`` below a call to Flask's ``@app.route(..)`` to allow CORS on a given route. 
+See the full list of options in the `decorator documentation <https://flask-cors.corydolphin.com/en/latest/api.html#decorator>`__.
 
 .. code:: python
 
     @app.route("/")
     @cross_origin()
     def helloWorld():
       return "Hello, cross-origin-world!"
 
 Documentation
 -------------
 
-For a full list of options, please see the full
-`documentation <https://flask-cors.corydolphin.com/en/latest/api.html>`__
+For a full list of options, please see the full `documentation <https://flask-cors.corydolphin.com/en/latest/api.html>`__
 
 Troubleshooting
 ---------------
 
-If things aren't working as you expect, enable logging to help understand
-what is going on under the hood, and why.
+If things aren't working as you expect, enable logging to help understand what is going on under the hood, and why.
 
 .. code:: python
 
     logging.getLogger('flask_cors').level = logging.DEBUG
 
 
 Tests
 -----
 
-A simple set of tests is included in ``test/``. To run, install nose,
-and simply invoke ``nosetests`` or ``python setup.py test`` to exercise
-the tests.
+A simple set of tests is included in ``test/``. 
+To run, install nose, and simply invoke ``nosetests`` or ``python setup.py test`` to exercise the tests.
+
+If nosetests does not work for you, due to it no longer working with newer python versions.
+You can use pytest to run the tests instead.
 
 Contributing
 ------------
 
-Questions, comments or improvements? Please create an issue on
-`Github <https://github.com/corydolphin/flask-cors>`__, tweet at
-`@corydolphin <https://twitter.com/corydolphin>`__ or send me an email.
-I do my best to include every contribution proposed in any way that I
-can.
+Questions, comments or improvements? 
+Please create an issue on `Github <https://github.com/corydolphin/flask-cors>`__, tweet at `@corydolphin <https://twitter.com/corydolphin>`__ or send me an email. 
+I do my best to include every contribution proposed in any way that I can.
 
 Credits
 -------
 
-This Flask extension is based upon the `Decorator for the HTTP Access
-Control <http://flask.pocoo.org/snippets/56/>`__ written by Armin
-Ronacher.
+This Flask extension is based upon the `Decorator for the HTTP Access Control <https://web.archive.org/web/20190128010149/http://flask.pocoo.org/snippets/56/>`__ written by Armin Ronacher.
 
 .. |Build Status| image:: https://api.travis-ci.org/corydolphin/flask-cors.svg?branch=master
    :target: https://travis-ci.org/corydolphin/flask-cors
 .. |Latest Version| image:: https://img.shields.io/pypi/v/Flask-Cors.svg
    :target: https://pypi.python.org/pypi/Flask-Cors/
 .. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/Flask-Cors.svg
    :target: https://img.shields.io/pypi/pyversions/Flask-Cors.svg
```

### Comparing `Flask-Cors-3.0.9/setup.py` & `Flask-Cors-4.0.0a0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,30 +29,27 @@
     long_description=open('README.rst').read(),
     packages=['flask_cors'],
     zip_safe=False,
     include_package_data=True,
     platforms='any',
     install_requires=install_requires,
     tests_require=[
-        'nose',
+        'pytest',
         'packaging'
     ],
-    test_suite='nose.collector',
+    test_suite='tests',
     classifiers=[
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ]
 )
```

### Comparing `Flask-Cors-3.0.9/tests/extension/test_app_extension.py` & `Flask-Cors-4.0.0a0/tests/extension/test_app_extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,16 +35,16 @@
             },
             r'/test_regex_mixed_list': {
                 'origins': ["http://example.com", r".*.otherexample.com"]
             },
             r'/test_send_wildcard_with_origin' : {
                 'send_wildcard':True
             },
-            re.compile('/test_compiled_subdomain_\w*'): {
-                'origins': re.compile("http://example\d+.com")
+            re.compile(r'/test_compiled_subdomain_\w*'): {
+                'origins': re.compile(r"http://example\d+.com")
             },
             r'/test_defaults':{}
         })
 
         @self.app.route('/test_defaults')
         def wildcard():
             return 'Welcome!'
@@ -158,15 +158,15 @@
         '''
         for sub in letters:
             domain = "http://%s.otherexample.com" % sub
             for resp in self.iter_responses('/test_regex_mixed_list',
                                             origin=domain):
                 self.assertEqual(domain, resp.headers.get(ACL_ORIGIN))
 
-        self.assertEquals("http://example.com",
+        self.assertEqual("http://example.com",
             self.get('/test_regex_mixed_list', origin='http://example.com').headers.get(ACL_ORIGIN))
 
 
 class AppExtensionList(FlaskCorsTestCase):
     def setUp(self):
         self.app = Flask(__name__)
         CORS(self.app, resources=[r'/test_exposed', r'/test_other_exposed'],
@@ -334,15 +334,15 @@
                 self.assertTrue(ACL_ORIGIN in resp.headers)
                 self.assertEqual(origin, resp.headers.get(ACL_ORIGIN))
 
 
 class AppExtensionCompiledRegexp(FlaskCorsTestCase):
     def test_compiled_regex(self):
         '''
-            Ensure we do not error if the user sepcifies an bad regular
+            Ensure we do not error if the user specifies an bad regular
             expression.
         '''
         import re
         self.app = Flask(__name__)
         CORS(self.app, resources=re.compile('/api/.*'))
 
         @self.app.route('/')
@@ -359,15 +359,15 @@
         for resp in self.iter_responses('/api/v1', origin='http://foo.com'):
             self.assertTrue(ACL_ORIGIN in resp.headers)
 
 
 class AppExtensionBadRegexp(FlaskCorsTestCase):
     def test_value_error(self):
         '''
-            Ensure we do not error if the user sepcifies an bad regular
+            Ensure we do not error if the user specifies an bad regular
             expression.
         '''
 
         self.app = Flask(__name__)
         CORS(self.app, resources="}")
 
         @self.app.route('/')
```

### Comparing `Flask-Cors-3.0.9/tests/base_test.py` & `Flask-Cors-4.0.0a0/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-3.0.9/tests/decorator/test_duplicate_headers.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_duplicate_headers.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-3.0.9/tests/decorator/test_vary_header.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_vary_header.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-3.0.9/tests/decorator/test_exception_interception.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_exception_interception.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         self.assertEqual(resp.status_code, 500)
         self.assertFalse(ACL_ORIGIN in resp.headers)
 
     def test_acl_exception_with_error_handler(self):
         '''
             If a 500 handler is setup by the user, responses should have
             CORS matching rules applied, regardless of whether or not
-            intercept_exceptions is enbaled.
+            intercept_exceptions is enabled.
         '''
         return_string = "Simple error handler"
 
         @self.app.errorhandler(404)
         @self.app.errorhandler(500)
         def catch_all_handler(error):
             '''
@@ -164,15 +164,15 @@
              })
         add_routes(self.app)
 
     def test_acl_exception_with_error_handler(self):
         '''
             If a 500 handler is setup by the user, responses should have
             CORS matching rules applied, regardless of whether or not
-            intercept_exceptions is enbaled.
+            intercept_exceptions is enabled.
         '''
         return_string = "Simple error handler"
 
         @self.app.errorhandler(404)
         @self.app.errorhandler(500)
         def catch_all_handler(error):
             '''
```

### Comparing `Flask-Cors-3.0.9/tests/decorator/test_allow_headers.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_allow_headers.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-3.0.9/tests/decorator/test_origins.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_origins.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         '''
         for sub in letters:
             domain = "http://%s.otherexample.com" % sub
             for resp in self.iter_responses('/test_regex_mixed_list',
                                             origin=domain):
                 self.assertEqual(domain, resp.headers.get(ACL_ORIGIN))
 
-        self.assertEquals("http://example.com",
+        self.assertEqual("http://example.com",
             self.get('/test_regex_mixed_list', origin='http://example.com').headers.get(ACL_ORIGIN))
 
     def test_multiple_protocols(self):
         import logging
         logging.getLogger('flask_cors').level = logging.DEBUG
         resp = self.get('test_multiple_protocols', origin='https://example.com')
         self.assertEqual('https://example.com', resp.headers.get(ACL_ORIGIN))
```

### Comparing `Flask-Cors-3.0.9/tests/decorator/test_options.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_options.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-3.0.9/tests/decorator/test_w3.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_w3.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-3.0.9/tests/decorator/test_credentials.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             return 'Open!'
 
     def test_credentials_supported(self):
         ''' The specified route should return the
             Access-Control-Allow-Credentials header.
         '''
         resp = self.get('/test_credentials_supported', origin='www.example.com')
-        self.assertEquals(resp.headers.get(ACL_CREDENTIALS), 'true')
+        self.assertEqual(resp.headers.get(ACL_CREDENTIALS), 'true')
 
     def test_default(self):
         ''' The default behavior should be to disallow credentials.
         '''
         resp = self.get('/test_default', origin='www.example.com')
         self.assertFalse(ACL_CREDENTIALS in resp.headers)
```

### Comparing `Flask-Cors-3.0.9/tests/decorator/test_max_age.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_max_age.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-3.0.9/tests/decorator/test_methods.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_methods.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-3.0.9/tests/decorator/test_expose_headers.py` & `Flask-Cors-4.0.0a0/tests/decorator/test_expose_headers.py`

 * *Files identical despite different names*

### Comparing `Flask-Cors-3.0.9/tests/core/helper_tests.py` & `Flask-Cors-4.0.0a0/tests/core/helper_tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -81,10 +81,10 @@
             [re.compile(r'/api/v1/.*'), '/foo', re.compile(r'/.*')]
         )
 
     def test_probably_regex(self):
         self.assertTrue(probably_regex("http://*.example.com"))
         self.assertTrue(probably_regex("*"))
         self.assertFalse(probably_regex("http://example.com"))
-        self.assertTrue(probably_regex("http://[\w].example.com"))
-        self.assertTrue(probably_regex("http://\w+.example.com"))
+        self.assertTrue(probably_regex(r"http://[\w].example.com"))
+        self.assertTrue(probably_regex(r"http://\w+.example.com"))
         self.assertTrue(probably_regex("https?://example.com"))
```

### Comparing `Flask-Cors-3.0.9/tests/core/test_override_headers.py` & `Flask-Cors-4.0.0a0/tests/core/test_override_headers.py`

 * *Files identical despite different names*

