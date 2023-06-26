# Comparing `tmp/flask-marshmallow-openapi-0.1.9.tar.gz` & `tmp/flask-marshmallow-openapi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-marshmallow-openapi-0.1.9.tar", last modified: Thu Jun 15 06:38:44 2023, max compression
+gzip compressed data, was "flask-marshmallow-openapi-0.2.0.tar", last modified: Mon Jun 26 06:32:58 2023, max compression
```

## Comparing `flask-marshmallow-openapi-0.1.9.tar` & `flask-marshmallow-openapi-0.2.0.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-15 06:38:44.593942 flask-marshmallow-openapi-0.1.9/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      135 2023-06-15 06:38:12.000000 flask-marshmallow-openapi-0.1.9/.bumpversion.cfg
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      709 2023-06-08 12:25:25.000000 flask-marshmallow-openapi-0.1.9/.gitignore
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)        5 2023-06-08 05:27:08.000000 flask-marshmallow-openapi-0.1.9/.python-version
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1065 2023-06-08 12:45:04.000000 flask-marshmallow-openapi-0.1.9/LICENSE
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      838 2023-06-09 19:55:49.000000 flask-marshmallow-openapi-0.1.9/MANIFEST.in
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-15 06:38:44.593942 flask-marshmallow-openapi-0.1.9/PKG-INFO
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     3648 2023-06-09 03:51:07.000000 flask-marshmallow-openapi-0.1.9/README.md
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     2699 2023-06-15 06:38:12.000000 flask-marshmallow-openapi-0.1.9/pyproject.toml
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       38 2023-06-15 06:38:44.593942 flask-marshmallow-openapi-0.1.9/setup.cfg
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-15 06:38:44.589941 flask-marshmallow-openapi-0.1.9/src/
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-15 06:38:44.589941 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      176 2023-06-15 06:38:12.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/__init__.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    13858 2023-06-15 06:33:38.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/decorators.py
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2199 2023-06-08 08:33:32.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/helpers.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)    11663 2023-06-09 04:04:07.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/middleware.py
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      641 2023-06-09 19:37:02.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/models.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-15 06:38:44.589941 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     8215 2023-06-15 06:34:03.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/redoc_favicon.png
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-15 06:38:44.593942 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      665 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      628 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      202 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/index.css
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      734 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/index.html
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2715 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      539 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045708 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   368781 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)  1045498 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   322863 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   145206 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)   256702 2023-06-08 05:32:51.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     3852 2023-06-09 04:04:07.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static_collector.py
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-15 06:38:44.593942 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/templates/
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)      648 2023-06-08 10:36:33.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      982 2023-06-15 06:37:48.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/templates/re_doc.jinja2
--rw-r--r--   0 tomislav  (1000) tomislav  (1000)     2435 2023-06-08 08:44:35.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
-drwxrwxr-x   0 tomislav  (1000) tomislav  (1000)        0 2023-06-15 06:38:44.589941 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi.egg-info/
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     4490 2023-06-15 06:38:44.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi.egg-info/PKG-INFO
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)     1706 2023-06-15 06:38:44.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-15 06:38:44.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)        1 2023-06-08 05:49:20.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi.egg-info/not-zip-safe
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)      428 2023-06-15 06:38:44.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi.egg-info/requires.txt
--rw-rw-r--   0 tomislav  (1000) tomislav  (1000)       26 2023-06-15 06:38:44.000000 flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:58.045611 flask-marshmallow-openapi-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-26 06:32:58.045611 flask-marshmallow-openapi-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 06:32:58.045611 flask-marshmallow-openapi-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:58.037611 flask-marshmallow-openapi-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:58.037611 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:58.037611 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/redoc_favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:58.045611 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1045708 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   368781 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1045498 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   322863 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js
+-rw-r--r--   0 runner    (1001) docker     (123)   145206 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)   256702 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:58.045611 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/templates/changelog.html.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/templates/re_doc.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-26 06:32:48.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:32:58.037611 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-26 06:32:58.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-26 06:32:58.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 06:32:58.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 06:32:57.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-26 06:32:58.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-26 06:32:58.000000 flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi.egg-info/top_level.txt
```

### Comparing `flask-marshmallow-openapi-0.1.9/.gitignore` & `flask-marshmallow-openapi-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/LICENSE` & `flask-marshmallow-openapi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/MANIFEST.in` & `flask-marshmallow-openapi-0.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/PKG-INFO` & `flask-marshmallow-openapi-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.1.9
+Version: 0.2.0
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flask-marshmallow-openapi-0.1.9/README.md` & `flask-marshmallow-openapi-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/pyproject.toml` & `flask-marshmallow-openapi-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel"]
 
 
 [project]
 name = "flask-marshmallow-openapi"
-version = "0.1.9"
+version = "0.2.0"
 description = "Flask + marshmallow + OpenAPI"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
@@ -40,14 +40,15 @@
     "ipython>=8.6.0",
     "black >= 22.1.0",
     "bump2version >= 1.0.1",
     "check-manifest >= 0.47",
     "isort >= 5.10.1",
     "pip-tools >= 6.5.1",
     "flask-shell-ipython>=0.5.1",
+    "inflection",
 ]
 # For dev machines and CI generating docs
 docs = [
     "furo",
     "myst-parser",
     "sphinx > 5.2.0",
     "sphinx_rtd_theme",
@@ -96,15 +97,15 @@
     "-pno:mock",
     "-pno:profiling",
     "-pno:random_order",
     # "--random-order",
     # "--random-order-bucket=class",
 ]
 
-python_classes = ["Describe*", "When_*", "describe_*", "when_*"]
+python_classes = ["Describe*", "When*", "describe_*", "when_*"]
 python_functions = ["it_*", "test_*", "then_*", "when_*"]
 python_files = ["test_*", "*_spec.py", "*_test.py"]
 spec_header_format = "{test_case}"
 filterwarnings = ["ignore::DeprecationWarning"]
 
 
 [tool.coverage.paths]
```

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/decorators.py` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/decorators.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/helpers.py` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/helpers.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/middleware.py` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 class OpenAPISettings:
     #: Name string displayed in various places in of API docs
     api_name: str
 
     #: Version string displayed in various places in of API docs
     api_version: str
 
-    #: Top level python package in which to search for marshmalow.Schema classes
+    #: Top level python package in which to search for marshmallow.Schema classes
     app_package_name: str
 
     #: Where to mount OpenAPI blueprint? Giving ie. "/v1" will create following docs
     #: routes: "/v1/re_doc", "/v1/swagger_ui", "/v1/docs/static", ...
     mounted_at: str = "/"
 
     #: Optional function that loads minimal OpenAPI specification and returns it as
@@ -146,16 +146,23 @@
 
             self._apispec = apispec.APISpec(
                 plugins=[MarshmallowPlugin()], **(initial_swagger_json)
             )
             for name, klass in helpers.all_schemas():
                 # apispec automatically registers all nested schema so we must prevent
                 # registering them ourselves because of DuplicateSchemaError
+                x_tags = getattr(klass.opts, "x_tags", None)
+
                 try:
-                    self._apispec.components.schema(name, schema=klass)
+                    if x_tags:
+                        self._apispec.components.schema(
+                            name, component={"x-tags": x_tags}, schema=klass
+                        )
+                    else:
+                        self._apispec.components.schema(name, schema=klass)
                 except DuplicateComponentNameError:
                     pass
 
             self._collect_endpoints_docs(app)
 
         app.register_blueprint(self.blueprint, url_prefix=str(full_url_prefix))
```

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/models.py` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/models.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/redoc_favicon.png` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/redoc_favicon.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/index.html` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/index.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-initializer.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle-core.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-es-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static/swagger_ui/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/static_collector.py` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/static_collector.py`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/templates/changelog.html.jinja2` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/templates/changelog.html.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/templates/re_doc.jinja2` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/templates/re_doc.jinja2`

 * *Files 27% similar despite different names*

```diff
@@ -18,13 +18,31 @@
       margin: 0;
       padding: 0;
     }
   </style>
 </head>
 
 <body>
-  <redoc spec-url="{{ swagger_json_path or url_for('open_api.swagger_json') }}" sort-operations-alphabetically="true"
-    sort-tags-alphabetically="true" sort-props-alphabetically="true" lazy-rendering="true"></redoc>
-  <script src="https://cdn.jsdelivr.net/npm/redoc@v2.0.0/bundles/redoc.standalone.js"></script>
+  <script src="https://cdn.redoc.ly/redoc/latest/bundles/redoc.standalone.js"> </script>
+
+  <div id="redoc-container"></div>
+
+  <script>
+    Redoc.init(
+      "{{ swagger_json_path or url_for('open_api.swagger_json') }}",
+      {
+        sortOperationsAlphabetically: true,
+        sortTagsAlphabetically: true,
+        sortPropsAlphabetically: true,
+        sortEnumValuesAlphabetically: true,
+        theme: {
+          openapi: {
+            schemaDefinitionsTagName: "Schemas",
+          },
+        },
+      },
+      document.getElementById("redoc-container")
+    );
+  </script>
 </body>
 
 </html>
```

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi/templates/swagger_ui.jinja2`

 * *Files identical despite different names*

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi.egg-info/PKG-INFO` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-marshmallow-openapi
-Version: 0.1.9
+Version: 0.2.0
 Summary: Flask + marshmallow + OpenAPI
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/flask-marshmallow-openapi
 Keywords: OpenAPI SwaggerUI ReDoc
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flask-marshmallow-openapi-0.1.9/src/flask_marshmallow_openapi.egg-info/SOURCES.txt` & `flask-marshmallow-openapi-0.2.0/src/flask_marshmallow_openapi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .bumpversion.cfg
 .gitignore
-.python-version
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/flask_marshmallow_openapi/__init__.py
 src/flask_marshmallow_openapi/decorators.py
 src/flask_marshmallow_openapi/helpers.py
```

