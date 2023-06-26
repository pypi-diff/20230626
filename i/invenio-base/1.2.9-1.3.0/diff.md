# Comparing `tmp/invenio-base-1.2.9.tar.gz` & `tmp/invenio-base-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/invenio-base/invenio-base/dist/tmpakiwwrle/invenio-base-1.2.9.tar", last modified: Tue Feb 22 17:06:21 2022, max compression
+gzip compressed data, was "/home/runner/work/invenio-base/invenio-base/dist/.tmp-exghbyn1/invenio-base-1.3.0.tar", last modified: Mon Jun 26 07:00:49 2023, max compression
```

## Comparing `invenio-base-1.2.9.tar` & `invenio-base-1.3.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 17:06:21.000000 invenio-base-1.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-02-22 17:06:10.000000 invenio-base-1.2.9/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-02-22 17:06:10.000000 invenio-base-1.2.9/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-02-22 17:06:10.000000 invenio-base-1.2.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2860 2022-02-22 17:06:10.000000 invenio-base-1.2.9/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3705 2022-02-22 17:06:10.000000 invenio-base-1.2.9/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-02-22 17:06:10.000000 invenio-base-1.2.9/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-02-22 17:06:10.000000 invenio-base-1.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-02-22 17:06:10.000000 invenio-base-1.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4293 2022-02-22 17:06:21.000000 invenio-base-1.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-02-22 17:06:10.000000 invenio-base-1.2.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 17:06:21.000000 invenio-base-1.2.9/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7433 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10141 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6993 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-02-22 17:06:10.000000 invenio-base-1.2.9/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 17:06:21.000000 invenio-base-1.2.9/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2358 2022-02-22 17:06:10.000000 invenio-base-1.2.9/examples/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 17:06:21.000000 invenio-base-1.2.9/invenio_base/
--rw-r--r--   0 runner    (1001) docker     (121)     7332 2022-02-22 17:06:10.000000 invenio-base-1.2.9/invenio_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-02-22 17:06:10.000000 invenio-base-1.2.9/invenio_base/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9903 2022-02-22 17:06:10.000000 invenio-base-1.2.9/invenio_base/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     3082 2022-02-22 17:06:10.000000 invenio-base-1.2.9/invenio_base/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-02-22 17:06:10.000000 invenio-base-1.2.9/invenio_base/signals.py
--rw-r--r--   0 runner    (1001) docker     (121)     1196 2022-02-22 17:06:10.000000 invenio-base-1.2.9/invenio_base/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3919 2022-02-22 17:06:10.000000 invenio-base-1.2.9/invenio_base/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 17:06:21.000000 invenio-base-1.2.9/invenio_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4293 2022-02-22 17:06:20.000000 invenio-base-1.2.9/invenio_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-02-22 17:06:21.000000 invenio-base-1.2.9/invenio_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-22 17:06:20.000000 invenio-base-1.2.9/invenio_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-02-22 17:06:20.000000 invenio-base-1.2.9/invenio_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-22 17:06:19.000000 invenio-base-1.2.9/invenio_base.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-02-22 17:06:20.000000 invenio-base-1.2.9/invenio_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-02-22 17:06:21.000000 invenio-base-1.2.9/invenio_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-02-22 17:06:10.000000 invenio-base-1.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-02-22 17:06:10.000000 invenio-base-1.2.9/pytest.ini
--rwxr-xr-x   0 runner    (1001) docker     (121)      458 2022-02-22 17:06:10.000000 invenio-base-1.2.9/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-02-22 17:06:21.000000 invenio-base-1.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-02-22 17:06:10.000000 invenio-base-1.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 17:06:21.000000 invenio-base-1.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-02-22 17:06:10.000000 invenio-base-1.2.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    11862 2022-02-22 17:06:10.000000 invenio-base-1.2.9/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     5292 2022-02-22 17:06:10.000000 invenio-base-1.2.9/tests/test_cmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-02-22 17:06:10.000000 invenio-base-1.2.9/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-02-22 17:06:10.000000 invenio-base-1.2.9/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3817 2022-02-22 17:06:10.000000 invenio-base-1.2.9/tests/test_wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:00:49.000000 invenio-base-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-26 07:00:35.000000 invenio-base-1.3.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      641 2023-06-26 07:00:35.000000 invenio-base-1.3.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-26 07:00:35.000000 invenio-base-1.3.0/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-26 07:00:35.000000 invenio-base-1.3.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3439 2023-06-26 07:00:35.000000 invenio-base-1.3.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3705 2023-06-26 07:00:35.000000 invenio-base-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-06-26 07:00:35.000000 invenio-base-1.3.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-06-26 07:00:35.000000 invenio-base-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-06-26 07:00:35.000000 invenio-base-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4870 2023-06-26 07:00:49.000000 invenio-base-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-06-26 07:00:35.000000 invenio-base-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:00:49.000000 invenio-base-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7433 2023-06-26 07:00:35.000000 invenio-base-1.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-06-26 07:00:35.000000 invenio-base-1.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-26 07:00:35.000000 invenio-base-1.3.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-26 07:00:35.000000 invenio-base-1.3.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     9981 2023-06-26 07:00:35.000000 invenio-base-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-26 07:00:35.000000 invenio-base-1.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-26 07:00:35.000000 invenio-base-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-26 07:00:35.000000 invenio-base-1.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-26 07:00:35.000000 invenio-base-1.3.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6993 2023-06-26 07:00:35.000000 invenio-base-1.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-26 07:00:35.000000 invenio-base-1.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      261 2023-06-26 07:00:35.000000 invenio-base-1.3.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:00:49.000000 invenio-base-1.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)     2369 2023-06-26 07:00:35.000000 invenio-base-1.3.0/examples/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:00:49.000000 invenio-base-1.3.0/invenio_base/
+-rw-r--r--   0 runner    (1001) docker     (122)     7895 2023-06-26 07:00:35.000000 invenio-base-1.3.0/invenio_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      384 2023-06-26 07:00:35.000000 invenio-base-1.3.0/invenio_base/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11038 2023-06-26 07:00:35.000000 invenio-base-1.3.0/invenio_base/app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3007 2023-06-26 07:00:35.000000 invenio-base-1.3.0/invenio_base/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)      976 2023-06-26 07:00:35.000000 invenio-base-1.3.0/invenio_base/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1196 2023-06-26 07:00:35.000000 invenio-base-1.3.0/invenio_base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3924 2023-06-26 07:00:35.000000 invenio-base-1.3.0/invenio_base/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:00:49.000000 invenio-base-1.3.0/invenio_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4870 2023-06-26 07:00:49.000000 invenio-base-1.3.0/invenio_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-06-26 07:00:49.000000 invenio-base-1.3.0/invenio_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 07:00:49.000000 invenio-base-1.3.0/invenio_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-06-26 07:00:49.000000 invenio-base-1.3.0/invenio_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-26 07:00:48.000000 invenio-base-1.3.0/invenio_base.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-26 07:00:49.000000 invenio-base-1.3.0/invenio_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-06-26 07:00:49.000000 invenio-base-1.3.0/invenio_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-26 07:00:35.000000 invenio-base-1.3.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (122)      479 2023-06-26 07:00:35.000000 invenio-base-1.3.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-06-26 07:00:49.000000 invenio-base-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-06-26 07:00:35.000000 invenio-base-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-26 07:00:49.000000 invenio-base-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-06-26 07:00:35.000000 invenio-base-1.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11776 2023-06-26 07:00:35.000000 invenio-base-1.3.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4985 2023-06-26 07:00:35.000000 invenio-base-1.3.0/tests/test_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1044 2023-06-26 07:00:35.000000 invenio-base-1.3.0/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1261 2023-06-26 07:00:35.000000 invenio-base-1.3.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3819 2023-06-26 07:00:35.000000 invenio-base-1.3.0/tests/test_wsgi.py
```

### Comparing `invenio-base-1.2.9/.editorconfig` & `invenio-base-1.3.0/.editorconfig`

 * *Files 20% similar despite different names*

```diff
@@ -11,24 +11,14 @@
 [*]
 indent_style = space
 end_of_line = lf
 insert_final_newline = true
 trim_trailing_whitespace = true
 charset = utf-8
 
-# Python files
-[*.py]
-indent_size = 4
-# isort plugin configuration
-skip = .eggs
-known_first_party = invenio_base
-known_third_party = flask
-multi_line_output = 2
-default_section = THIRDPARTY
-
 # RST files (used by sphinx)
 [*.rst]
 indent_size = 4
 
 # CSS, HTML, JS, JSON, YML
 [*.{css,html,js,json,yml}]
 indent_size = 2
```

### Comparing `invenio-base-1.2.9/AUTHORS.rst` & `invenio-base-1.3.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.9/CHANGES.rst` & `invenio-base-1.3.0/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,40 @@
 ..
     This file is part of Invenio.
-    Copyright (C) 2015-2018 CERN.
+    Copyright (C) 2015-2023 CERN.
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 1.3.0 (released 2023-06-23)
+
+- Adds finalize_app_entry_points to overcome ``before_(app_)_first_request``
+  deprecation in Flask>=2.3.0
+
+Version 1.2.15 (released 2023-05-02)
+
+- Pins Werkzeug<2.3.0 due to removed deprecations (for example ``Authoriation`` headers
+  parsing issues).
+
+Version 1.2.14 (released 2023-04-26)
+
+- Pins Flask<2.3.0 due to removed deprecations (for example
+  `before_(app_)first_request`).
+
+Version 1.2.11 (released 2022-03-29)
+
+- Adds a compatibility layer for Werkzeug v2.1.
+
+Version 1.2.10 (released 2022-03-29)
+
+- Adds support for Flask v2.1
+
 Version 1.2.9 (released 2022-02-22)
 
 - Fixes issue with duplicate entry points during tests due to pytest
   modifying the sys.path.
 
 Version 1.2.8 (released 2022-02-21)
```

### Comparing `invenio-base-1.2.9/CONTRIBUTING.rst` & `invenio-base-1.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.9/LICENSE` & `invenio-base-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.9/MANIFEST.in` & `invenio-base-1.3.0/MANIFEST.in`

 * *Files 18% similar despite different names*

```diff
@@ -26,7 +26,8 @@
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs Makefile
 recursive-include examples *.py
 recursive-include tests *.html
 recursive-include tests *.js
 recursive-include tests *.py
+include .git-blame-ignore-revs
```

### Comparing `invenio-base-1.2.9/PKG-INFO` & `invenio-base-1.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: invenio-base
-Version: 1.2.9
+Version: 1.3.0
 Summary: "Base package for building Invenio application factories."
 Home-page: https://github.com/inveniosoftware/invenio-base
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Keywords: invenio
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: tests
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ..
     This file is part of Invenio.
     Copyright (C) 2015-2018 CERN.
@@ -40,22 +40,45 @@
 
 Base package for building Invenio application factories.
 
 Further documentation is available on https://invenio-base.readthedocs.io/
 
 ..
     This file is part of Invenio.
-    Copyright (C) 2015-2018 CERN.
+    Copyright (C) 2015-2023 CERN.
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 1.3.0 (released 2023-06-23)
+
+- Adds finalize_app_entry_points to overcome ``before_(app_)_first_request``
+  deprecation in Flask>=2.3.0
+
+Version 1.2.15 (released 2023-05-02)
+
+- Pins Werkzeug<2.3.0 due to removed deprecations (for example ``Authoriation`` headers
+  parsing issues).
+
+Version 1.2.14 (released 2023-04-26)
+
+- Pins Flask<2.3.0 due to removed deprecations (for example
+  `before_(app_)first_request`).
+
+Version 1.2.11 (released 2022-03-29)
+
+- Adds a compatibility layer for Werkzeug v2.1.
+
+Version 1.2.10 (released 2022-03-29)
+
+- Adds support for Flask v2.1
+
 Version 1.2.9 (released 2022-02-22)
 
 - Fixes issue with duplicate entry points during tests due to pytest
   modifying the sys.path.
 
 Version 1.2.8 (released 2022-02-21)
 
@@ -127,9 +150,7 @@
   with the signature create_blueprint(app), that will create and return a
   blueprint. This allows moving dynamic blueprint creation from the extension
   initialization phase to the blueprint registration phase.
 
 Version 1.0.0 (released 2018-03-23)
 
 - Initial public release.
-
-
```

### Comparing `invenio-base-1.2.9/README.rst` & `invenio-base-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.9/docs/Makefile` & `invenio-base-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.9/docs/conf.py` & `invenio-base-1.3.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,14 @@
 # Copyright (C) 2015-2018 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Sphinx configuration."""
 
-import os
-
-import sphinx.environment
-
 from invenio_base import __version__
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
@@ -44,17 +40,17 @@
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
-project = u"Invenio-Base"
-copyright = u"2015, CERN"
-author = u"CERN"
+project = "Invenio-Base"
+copyright = "2015, CERN"
+author = "CERN"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 
@@ -62,15 +58,15 @@
 release = __version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 # today = ''
 # Else, today_fmt is used as the format for a strftime call.
 # today_fmt = '%B %d, %Y'
 
@@ -113,18 +109,16 @@
     "description": "Base package for building Invenio application factories.",
     "github_user": "inveniosoftware",
     "github_repo": "invenio-base",
     "github_button": False,
     "github_banner": True,
     "show_powered_by": False,
     "extra_nav_links": {
-        "invenio-base@GitHub":
-        "https://github.com/inveniosoftware/invenio-base",
-        "invenio-base@PyPI":
-        "https://pypi.python.org/pypi/invenio-base/",
+        "invenio-base@GitHub": "https://github.com/inveniosoftware/invenio-base",
+        "invenio-base@PyPI": "https://pypi.python.org/pypi/invenio-base/",
     },
 }
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 
 # Theme options are theme-specific and customize the look and feel of a theme
@@ -240,19 +234,15 @@
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc,
-     "invenio-base.tex",
-     u"invenio-base Documentation",
-     u"CERN",
-     "manual"),
+    (master_doc, "invenio-base.tex", "invenio-base Documentation", "CERN", "manual"),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -272,34 +262,30 @@
 # latex_domain_indices = True
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [(master_doc,
-              "invenio-base",
-              u"invenio-base Documentation",
-              [author],
-              1)]
+man_pages = [(master_doc, "invenio-base", "invenio-base Documentation", [author], 1)]
 
 # If true, show URL addresses after external links.
 # man_show_urls = False
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (
         master_doc,
         "invenio-base",
-        u"Invenio-Base Documentation",
+        "Invenio-Base Documentation",
         author,
         "invenio-base",
         "Base package for building Invenio application factories.",
         "Miscellaneous",
     ),
 ]
 
@@ -315,13 +301,12 @@
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 # texinfo_no_detailmenu = False
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     "python": ("https://docs.python.org/2.7/", None),
-    "Invenio-Config": ("https://invenio-config.readthedocs.io/en/latest/",
-                       None),
+    "Invenio-Config": ("https://invenio-config.readthedocs.io/en/latest/", None),
 }
 
 # Autodoc configuraton.
 autoclass_content = "both"
```

### Comparing `invenio-base-1.2.9/docs/index.rst` & `invenio-base-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.9/docs/make.bat` & `invenio-base-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.9/examples/app.py` & `invenio-base-1.3.0/examples/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,68 +20,73 @@
 
 
 # sphinxdoc-example-config-begin
 class Config(object):
     """Example configuration."""
 
     DEBUG = True
-    SECRET_KEY = 'CHANGE_ME'
+    SECRET_KEY = "CHANGE_ME"
 
 
 def config_loader(app, **kwargs):
     """Custom config loader."""
     app.config.from_object(Config)
     app.config.update(**kwargs)
+
+
 # sphinxdoc-example-config-end
 
 
 # sphinxdoc-example-paths-begin
-env_prefix = 'APP'
+env_prefix = "APP"
 
 
 def instance_path():
     """Instance path for Invenio.
 
     Defaults to ``<env_prefix>_INSTANCE_PATH`` or if environment variable is not
     set ``<sys.prefix>/var/<app_name>-instance``.
     """
-    return os.getenv(env_prefix + '_INSTANCE_PATH') or \
-        os.path.join(sys.prefix, 'var', 'example-instance')
+    return os.getenv(env_prefix + "_INSTANCE_PATH") or os.path.join(
+        sys.prefix, "var", "example-instance"
+    )
 
 
 def static_folder():
     """Static folder path.
 
     Defaults to ``<env_prefix>_STATIC_FOLDER`` or if environment variable is not
     set ``<sys.prefix>/var/<app_name>-instance/static``.
     """
-    return os.getenv(env_prefix + '_STATIC_FOLDER') or \
-        os.path.join(instance_path(), 'static')
+    return os.getenv(env_prefix + "_STATIC_FOLDER") or os.path.join(
+        instance_path(), "static"
+    )
+
 
 # sphinxdoc-example-paths-end
 
 
 # sphinxdoc-example-factories-begin
 create_api = create_app_factory(
-    'example',
+    "example",
     config_loader=config_loader,
-    blueprint_entry_points=['invenio_base.api_blueprints'],
-    extension_entry_points=['invenio_base.api_apps'],
-    converter_entry_points=['invenio_base.api_converters'],
+    blueprint_entry_points=["invenio_base.api_blueprints"],
+    extension_entry_points=["invenio_base.api_apps"],
+    converter_entry_points=["invenio_base.api_converters"],
     instance_path=instance_path,
 )
 
 
 create_app = create_app_factory(
-    'example',
+    "example",
     config_loader=config_loader,
-    blueprint_entry_points=['invenio_base.blueprints'],
-    extension_entry_points=['invenio_base.apps'],
-    converter_entry_points=['invenio_base.converters'],
-    wsgi_factory=create_wsgi_factory({'/api': create_api}),
+    blueprint_entry_points=["invenio_base.blueprints"],
+    extension_entry_points=["invenio_base.apps"],
+    converter_entry_points=["invenio_base.converters"],
+    wsgi_factory=create_wsgi_factory({"/api": create_api}),
     instance_path=instance_path,
     static_folder=static_folder,
 )
 # sphinxdoc-example-factories-end
 
 # sphinxdoc-example-objects-begin
 app = application = create_app()
```

### Comparing `invenio-base-1.2.9/invenio_base/__init__.py` & `invenio-base-1.3.0/invenio_base/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -233,15 +233,33 @@
    $ inveniomanage instance migrate_secret_key --help
    ...
 """
 
 from .app import create_app_factory, create_cli
 from .wsgi import create_wsgi_factory
 
-__version__ = '1.2.9'
+# Monkey patch Werkzeug 2.1
+# Flask-Login uses the safe_str_cmp method which has been removed in Werkzeug
+# 2.1. Flask-Login v0.6.0 (yet to be released at the time of writing) fixes the
+# issue. Once we depend on Flask-Login v0.6.0 as the minimal version in
+# Flask-Security-Invenio/Invenio-Accounts we can remove this patch again.
+try:
+    # Werkzeug <2.1
+    from werkzeug import security
+
+    security.safe_str_cmp
+except AttributeError:
+    # Werkzeug >=2.1
+    import hmac
+
+    from werkzeug import security
+
+    security.safe_str_cmp = hmac.compare_digest
+
+__version__ = "1.3.0"
 
 __all__ = (
-    '__version__',
-    'create_app_factory',
-    'create_cli',
-    'create_wsgi_factory',
+    "__version__",
+    "create_app_factory",
+    "create_cli",
+    "create_wsgi_factory",
 )
```

### Comparing `invenio-base-1.2.9/invenio_base/app.py` & `invenio-base-1.3.0/invenio_base/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
 # Copyright (C) 2015-2018 CERN.
 # Copyright (C) 2022 RERO.
+# Copyright (C) 2023 Graz University of Technology.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Invenio application factory."""
-
 import logging
 import os.path
 import sys
 import warnings
 
 import click
 from flask import Flask
 from flask.cli import FlaskGroup
 from flask.helpers import get_debug_flag
 from importlib_metadata import entry_points as iter_entry_points
 
 from .signals import app_created, app_loaded
 
 
-def create_app_factory(app_name, config_loader=None,
-                       extension_entry_points=None, extensions=None,
-                       blueprint_entry_points=None, blueprints=None,
-                       converter_entry_points=None, converters=None,
-                       wsgi_factory=None, **app_kwargs):
+def create_app_factory(
+    app_name,
+    config_loader=None,
+    extension_entry_points=None,
+    extensions=None,
+    blueprint_entry_points=None,
+    blueprints=None,
+    converter_entry_points=None,
+    converters=None,
+    finalize_app_entry_points=None,
+    wsgi_factory=None,
+    **app_kwargs,
+):
     """Create a Flask application factory.
 
     The application factory will load Flask extensions and blueprints specified
     using both entry points and directly in the arguments. Loading order of
     entry points are not guaranteed and can happen in any order.
 
     :param app_name: Flask application name.
@@ -47,14 +55,16 @@
     :param blueprints: List of Blueprints that will be registered on the
         Flask application.
     :param converter_entry_points: List of entry points, which specifies
         Werkzeug URL map converters that will be added to
         ``app.url_map.converters``.
     :param converters: Map of Werkzeug URL map converter classes that will
         be added to ``app.url_map.converters``.
+    :param finalize_app_entry_points: List of entry points, which specifies
+        the functions to finalize the app.
     :param wsgi_factory: A callable that will be passed the Flask application
         object in order to overwrite the default WSGI application (e.g. to
         install ``DispatcherMiddleware``).
     :param app_kwargs: Keyword arguments passed to :py:meth:`base_app`.
         `instance_path` and `static_folder` can be passed as callables.
     :returns: Flask application factory.
 
@@ -78,23 +88,24 @@
     .. code-block:: python
 
        def my_wsgi_factory(app):
            return DispatcherMiddleware(app.wsgi_app, {'/api': api_app})
 
     .. versionadded: 1.0.0
     """
+
     def _create_app(**kwargs):
-        for k in ('instance_path', 'root_path', 'static_folder'):
+        for k in ("instance_path", "root_path", "static_folder"):
             if k in app_kwargs and callable(app_kwargs[k]):
                 app_kwargs[k] = app_kwargs[k]()
 
         app = base_app(app_name, **app_kwargs)
         app_created.send(_create_app, app=app)
 
-        debug = kwargs.get('debug')
+        debug = kwargs.get("debug")
         if debug is not None:
             app.debug = debug
 
         # Load configuration
         if config_loader:
             config_loader(app, **kwargs)
 
@@ -115,14 +126,19 @@
         # Load blueprints
         blueprint_loader(
             app,
             entry_points=blueprint_entry_points,
             modules=blueprints,
         )
 
+        finalize_app_loader(
+            app,
+            entry_points=finalize_app_entry_points,
+        )
+
         app_loaded.send(_create_app, app=app)
 
         # Replace WSGI application using factory if provided (e.g. to install
         # WSGI middleware).
         if wsgi_factory:
             app.wsgi_app = wsgi_factory(app, **kwargs)
 
@@ -135,46 +151,75 @@
     """Create CLI for ``inveniomanage`` command.
 
     :param create_app: Flask application factory.
     :returns: Click command group.
 
     .. versionadded: 1.0.0
     """
-    def create_cli_app(info):
+
+    # Flask 2.0 removed support for passing script_info argument. Below
+    # function is thus
+    def create_cli_app(*args):
         """Application factory for CLI app.
 
         Internal function for creating the CLI. When invoked via
         ``inveniomanage`` FLASK_APP must be set.
         """
         if create_app is None:
-            # Fallback to normal Flask behavior
-            info.create_app = None
-            app = info.load_app()
+            # This part is only used for the "inveniomanage" command.
+            if len(args) == 0:
+                # Flask v2
+                # Create a barebones Flask application.
+                app = Flask("inveniomanage")
+            else:
+                # Flask v1
+                # Fallback to normal Flask behavior
+                info = args[0]
+                info.create_app = None
+                app = info.load_app()
         else:
             app = create_app(debug=get_debug_flag())
         return app
 
     @click.group(cls=FlaskGroup, create_app=create_cli_app)
     def cli(**params):
         """Command Line Interface for Invenio."""
         pass
 
     return cli
 
 
+def finalize_app_loader(app, entry_points=None):
+    """Run functions before of the first request.
+
+    This loader is the last possible position where it is possible to configure the app.
+
+    NOTE: it replaces the before_first_request decorator of flask <2.3.0
+
+    :param entry_points: List of entry points providing to Flask extensions.
+
+    .. versionadded: 2.0.0
+    """
+
+    def loader_init_func(func):
+        with app.app_context():
+            func(app)
+
+    _loader(app, loader_init_func, entry_points=entry_points)
+
+
 def app_loader(app, entry_points=None, modules=None):
     """Run default application loader.
 
     :param entry_points: List of entry points providing to Flask extensions.
     :param modules: List of Flask extensions.
 
     .. versionadded: 1.0.0
     """
-    _loader(app, lambda ext: ext(app), entry_points=entry_points,
-            modules=modules)
+    _loader(app, lambda ext: ext(app), entry_points=entry_points, modules=modules)
 
 
 def blueprint_loader(app, entry_points=None, modules=None):
     """Run default blueprint loader.
 
     The value of any entry_point or module passed can be either an instance of
     ``flask.Blueprint`` or a callable accepting a ``flask.Flask`` application
@@ -182,15 +227,15 @@
     ``flask.Blueprint``.
 
     :param entry_points: List of entry points providing to Blueprints.
     :param modules: List of Blueprints.
 
     .. versionadded: 1.0.0
     """
-    url_prefixes = app.config.get('BLUEPRINTS_URL_PREFIXES', {})
+    url_prefixes = app.config.get("BLUEPRINTS_URL_PREFIXES", {})
 
     def loader_init_func(bp_or_func):
         bp = bp_or_func(app) if callable(bp_or_func) else bp_or_func
         app.register_blueprint(bp, url_prefix=url_prefixes.get(bp.name))
 
     _loader(app, loader_init_func, entry_points=entry_points, modules=modules)
 
@@ -205,16 +250,15 @@
     """
     if entry_points:
         for entry_point in entry_points:
             for ep in set(iter_entry_points(group=entry_point)):
                 try:
                     app.url_map.converters[ep.name] = ep.load()
                 except Exception:
-                    app.logger.error(
-                        f'Failed to initialize entry point: {ep}')
+                    app.logger.error(f"Failed to initialize entry point: {ep}")
                     raise
 
     if modules:
         app.url_map.converters.update(**modules)
 
 
 def _loader(app, init_func, entry_points=None, modules=None):
@@ -227,29 +271,35 @@
     """
     if entry_points:
         for entry_point in entry_points:
             for ep in set(iter_entry_points(group=entry_point)):
                 try:
                     init_func(ep.load())
                 except Exception:
-                    app.logger.error(
-                        f'Failed to initialize entry point: {ep}')
+                    app.logger.error(f"Failed to initialize entry point: {ep}")
                     raise
     if modules:
         for m in modules:
             try:
                 init_func(m)
             except Exception:
-                app.logger.error(f'Failed to initialize module: {m}')
+                app.logger.error(f"Failed to initialize module: {m}")
                 raise
 
 
-def base_app(import_name, instance_path=None, static_folder=None,
-             static_url_path='/static', template_folder='templates',
-             instance_relative_config=True, root_path=None, app_class=Flask):
+def base_app(
+    import_name,
+    instance_path=None,
+    static_folder=None,
+    static_url_path="/static",
+    template_folder="templates",
+    instance_relative_config=True,
+    root_path=None,
+    app_class=Flask,
+):
     """Invenio base application factory.
 
     If the instance folder does not exists, it will be created.
 
     :param import_name: The name of the application package.
     :param env_prefix: Environment variable prefix.
     :param instance_path: Instance path for Flask application.
@@ -273,17 +323,15 @@
     )
 
     # Create instance path if it doesn't exists
     try:
         if instance_path and not os.path.exists(instance_path):
             os.makedirs(instance_path)
     except Exception:  # pragma: no cover
-        app.logger.exception(
-            f'Failed to create instance folder: "{instance_path}"'
-        )
+        app.logger.exception(f'Failed to create instance folder: "{instance_path}"')
 
     return app
 
 
 def configure_warnings():
     """Configure warnings by routing warnings to the logging system.
 
@@ -294,9 +342,9 @@
     if not sys.warnoptions:
         # Route warnings through python logging
         logging.captureWarnings(True)
 
         # DeprecationWarning is by default hidden, hence we force the
         # 'default' behavior on deprecation warnings which is not to hide
         # errors.
-        warnings.simplefilter('default', DeprecationWarning)
-        warnings.simplefilter('ignore', PendingDeprecationWarning)
+        warnings.simplefilter("default", DeprecationWarning)
+        warnings.simplefilter("ignore", PendingDeprecationWarning)
```

### Comparing `invenio-base-1.2.9/invenio_base/cli.py` & `invenio-base-1.3.0/invenio_base/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,84 +17,82 @@
 
 
 @click.group()
 def instance():
     """Instance commands."""
 
 
-@instance.command('entrypoints')
+@instance.command("entrypoints")
 @click.option(
-    '-e', '--entry-point', default=None, metavar='ENTRY_POINT',
-    help='Entry point group name (e.g. invenio_base.apps)')
+    "-e",
+    "--entry-point",
+    default=None,
+    metavar="ENTRY_POINT",
+    help="Entry point group name (e.g. invenio_base.apps)",
+)
 def list_entrypoints(entry_point):
     """List defined entry points."""
     found_entry_points = {}
     for dist in working_set:
         # for dist in importlib_metadata.distributions:
         entry_map = dist.get_entry_map()
         for group_name, entry_points in entry_map.items():
             # Filter entry points
-            if entry_point is None and \
-               not group_name.startswith('invenio'):
+            if entry_point is None and not group_name.startswith("invenio"):
                 continue
-            if entry_point is not None and \
-               entry_point != group_name:
+            if entry_point is not None and entry_point != group_name:
                 continue
 
             # Store entry points.
             if group_name not in found_entry_points:
                 found_entry_points[group_name] = []
             for ep in entry_points.values():
                 found_entry_points[group_name].append(str(ep))
 
     for ep_group in sorted(found_entry_points.keys()):
-        click.secho(f'{ep_group}', fg='green')
+        click.secho(f"{ep_group}", fg="green")
         for ep in sorted(found_entry_points[ep_group]):
-            click.echo(f'  {ep}')
+            click.echo(f"  {ep}")
 
 
-@instance.command('migrate-secret-key')
-@click.option('--old-key', required=True)
+@instance.command("migrate-secret-key")
+@click.option("--old-key", required=True)
 @with_appcontext
 def migrate_secret_key(old_key):
     """Call entry points exposed for the SECRET_KEY change."""
-    if 'SECRET_KEY' not in current_app.config or \
-            current_app.config['SECRET_KEY'] is None:
-        raise click.ClickException(
-            'SECRET_KEY is not set in the configuration.')
+    if (
+        "SECRET_KEY" not in current_app.config
+        or current_app.config["SECRET_KEY"] is None
+    ):
+        raise click.ClickException("SECRET_KEY is not set in the configuration.")
 
     migrators = []
-    for ep in set(
-        importlib_metadata.entry_points().get('invenio_base.secret_key', [])
-    ):
+    for ep in set(importlib_metadata.entry_points().get("invenio_base.secret_key", [])):
         try:
             migrators.append(ep.load())
         except Exception:
-            raise click.ClickException(
-                f'Failed to initialize entry point: {ep}'
-            )
+            raise click.ClickException(f"Failed to initialize entry point: {ep}")
 
     if migrators:
         for m in migrators:
             try:
                 m(old_key=old_key)
             except Exception:
                 raise click.ClickException(
-                    f'Failed to perform migration of secret key {old_key}'
+                    f"Failed to perform migration of secret key {old_key}"
                 )
-        click.secho('Successfully changed secret key.', fg='green')
+        click.secho("Successfully changed secret key.", fg="green")
     else:
         raise click.ClickException(
-            f'Failed to perform migration of secret key {old_key}'
+            f"Failed to perform migration of secret key {old_key}"
         )
 
 
 def generate_secret_key():
     """Generate secret key."""
     import random
     import string
 
     rng = random.SystemRandom()
-    return ''.join(
-        rng.choice(string.ascii_letters + string.digits)
-        for dummy in range(0, 256)
+    return "".join(
+        rng.choice(string.ascii_letters + string.digits) for dummy in range(0, 256)
     )
```

### Comparing `invenio-base-1.2.9/invenio_base/signals.py` & `invenio-base-1.3.0/invenio_base/signals.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 
 """Signals for application creation."""
 
 from blinker import Namespace
 
 _signals = Namespace()
 
-app_created = _signals.signal('app-created')
+app_created = _signals.signal("app-created")
 """Signal sent when the base Flask application have been created.
 
 Parameters:
 - ``sender`` - the application factory function.
 - ``app`` - the Flask application instance.
 
 Example receiver:
 
 .. code-block:: python
 
    def receiver(sender, app=None, **kwargs):
        # ...
 """
 
-app_loaded = _signals.signal('app-loaded')
+app_loaded = _signals.signal("app-loaded")
 """Signal sent when the Flask application have been fully loaded.
 
 Parameters:
 - ``sender`` - the application factory function.
 - ``app`` - the Flask application instance.
 
 Example receiver:
```

### Comparing `invenio-base-1.2.9/invenio_base/utils.py` & `invenio-base-1.3.0/invenio_base/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-base-1.2.9/invenio_base/wsgi.py` & `invenio-base-1.3.0/invenio_base/wsgi.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 
 import warnings
 
 # They were moved in the same version so they can be in one try/except
 try:
     from werkzeug.middleware.dispatcher import DispatcherMiddleware
     from werkzeug.middleware.proxy_fix import ProxyFix
+
     WERKZEUG_GTE_014 = False
 except ImportError:
     from werkzeug.contrib.fixers import ProxyFix
     from werkzeug.wsgi import DispatcherMiddleware
+
     WERKZEUG_GTE_014 = True
 
 
 def create_wsgi_factory(mounts_factories):
     """Create a WSGI application factory.
 
     Usage example:
@@ -31,20 +33,21 @@
        wsgi_factory = create_wsgi_factory({'/api': create_api})
 
     :param mounts_factories: Dictionary of mount points per application
         factory.
 
     .. versionadded:: 1.0.0
     """
+
     def create_wsgi(app, **kwargs):
         mounts = {
-            mount: factory(**kwargs)
-            for mount, factory in mounts_factories.items()
+            mount: factory(**kwargs) for mount, factory in mounts_factories.items()
         }
         return DispatcherMiddleware(app.wsgi_app, mounts)
+
     return create_wsgi
 
 
 def wsgi_proxyfix(factory=None):
     """Fix Flask environment according to ``X-Forwarded-_`` headers.
 
     .. note::
@@ -93,23 +96,27 @@
     .. versionadded:: 1.2.0
 
     .. deprecated:: 1.2
 
        The ``WSGI_PROXIES`` configuration is deprecated and it will be removed,
        use ``PROXYFIX_CONFIG`` instead.
     """
+
     def create_wsgi(app, **kwargs):
         wsgi_app = factory(app, **kwargs) if factory else app.wsgi_app
-        num_proxies = app.config.get('WSGI_PROXIES')
-        proxy_config = app.config.get('PROXYFIX_CONFIG')
+        num_proxies = app.config.get("WSGI_PROXIES")
+        proxy_config = app.config.get("PROXYFIX_CONFIG")
         if proxy_config and not WERKZEUG_GTE_014:
             return ProxyFix(wsgi_app, **proxy_config)
         elif num_proxies:
-            warnings.warn('The WSGI_PROXIES configuration is deprecated and '
-                          'it will be removed, use PROXYFIX_CONFIG instead',
-                          PendingDeprecationWarning)
+            warnings.warn(
+                "The WSGI_PROXIES configuration is deprecated and "
+                "it will be removed, use PROXYFIX_CONFIG instead",
+                PendingDeprecationWarning,
+            )
             if WERKZEUG_GTE_014:
                 return ProxyFix(wsgi_app, num_proxies=num_proxies)
             else:
                 return ProxyFix(wsgi_app, x_for=num_proxies)
         return wsgi_app
+
     return create_wsgi
```

### Comparing `invenio-base-1.2.9/invenio_base.egg-info/PKG-INFO` & `invenio-base-1.3.0/invenio_base.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: invenio-base
-Version: 1.2.9
+Version: 1.3.0
 Summary: "Base package for building Invenio application factories."
 Home-page: https://github.com/inveniosoftware/invenio-base
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Keywords: invenio
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: tests
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ..
     This file is part of Invenio.
     Copyright (C) 2015-2018 CERN.
@@ -40,22 +40,45 @@
 
 Base package for building Invenio application factories.
 
 Further documentation is available on https://invenio-base.readthedocs.io/
 
 ..
     This file is part of Invenio.
-    Copyright (C) 2015-2018 CERN.
+    Copyright (C) 2015-2023 CERN.
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 1.3.0 (released 2023-06-23)
+
+- Adds finalize_app_entry_points to overcome ``before_(app_)_first_request``
+  deprecation in Flask>=2.3.0
+
+Version 1.2.15 (released 2023-05-02)
+
+- Pins Werkzeug<2.3.0 due to removed deprecations (for example ``Authoriation`` headers
+  parsing issues).
+
+Version 1.2.14 (released 2023-04-26)
+
+- Pins Flask<2.3.0 due to removed deprecations (for example
+  `before_(app_)first_request`).
+
+Version 1.2.11 (released 2022-03-29)
+
+- Adds a compatibility layer for Werkzeug v2.1.
+
+Version 1.2.10 (released 2022-03-29)
+
+- Adds support for Flask v2.1
+
 Version 1.2.9 (released 2022-02-22)
 
 - Fixes issue with duplicate entry points during tests due to pytest
   modifying the sys.path.
 
 Version 1.2.8 (released 2022-02-21)
 
@@ -127,9 +150,7 @@
   with the signature create_blueprint(app), that will create and return a
   blueprint. This allows moving dynamic blueprint creation from the extension
   initialization phase to the blueprint registration phase.
 
 Version 1.0.0 (released 2018-03-23)
 
 - Initial public release.
-
-
```

### Comparing `invenio-base-1.2.9/invenio_base.egg-info/SOURCES.txt` & `invenio-base-1.3.0/invenio_base.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 .dockerignore
 .editorconfig
+.git-blame-ignore-revs
 AUTHORS.rst
 CHANGES.rst
 CONTRIBUTING.rst
 INSTALL.rst
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
-pytest.ini
 run-tests.sh
 setup.cfg
 setup.py
 docs/Makefile
 docs/api.rst
 docs/authors.rst
 docs/changes.rst
```

### Comparing `invenio-base-1.2.9/setup.cfg` & `invenio-base-1.3.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -11,27 +11,28 @@
 url = https://github.com/inveniosoftware/invenio-base
 classifiers = 
 	Development Status :: 5 - Production/Stable
 
 [options]
 include_package_data = True
 packages = find:
-python_requires = >=3.6
+python_requires = >=3.7
 zip_safe = False
 install_requires = 
 	blinker>=1.4
-	Flask>=1.1.4,<3.0.0
+	Flask>=1.1.4,<2.3.0
 	itsdangerous>=1.1.0,<2.1.0
-	MarkupSafe>=2.0
-	Werkzeug>=1.0.1,<3.0
+	MarkupSafe>=0.23
+	Werkzeug>=1.0.1,<2.3.0
 	importlib-metadata>=4.4
 	importlib-resources>=5.0
 
 [options.extras_require]
 tests = 
+	pytest-black>=0.3.0,<0.3.10
 	pytest-invenio>=1.4.2
 	sphinx>=4.2.0
 
 [options.entry_points]
 console_scripts = 
 	inveniomanage = invenio_base.__main__:cli
 flask.commands = 
@@ -42,13 +43,25 @@
 build-dir = docs/_build
 all_files = 1
 
 [bdist_wheel]
 universal = 1
 
 [pydocstyle]
-add_ignore = D401
+add_ignore = D401, D202
+
+[isort]
+profile = black
+
+[check-manifest]
+ignore = 
+	*-requirements.txt
+
+[tool:pytest]
+addopts = --black --isort --pydocstyle --doctest-glob="*.rst" --doctest-modules --cov=invenio_base --cov-report=term-missing
+testpaths = docs tests invenio_base
+filterwarnings = ignore::pytest.PytestDeprecationWarning
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `invenio-base-1.2.9/tests/test_app.py` & `invenio-base-1.3.0/tests/test_app.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,35 +18,42 @@
 import pytest
 from click.testing import CliRunner
 from flask import Blueprint, Flask, current_app
 from importlib_metadata import EntryPoint
 from werkzeug.routing import BaseConverter
 
 from invenio_base import __version__
-from invenio_base.app import _loader, app_loader, base_app, blueprint_loader, \
-    configure_warnings, converter_loader, create_app_factory, create_cli
+from invenio_base.app import (
+    _loader,
+    app_loader,
+    base_app,
+    blueprint_loader,
+    configure_warnings,
+    converter_loader,
+    create_app_factory,
+    create_cli,
+)
 from invenio_base.cli import generate_secret_key
 
 try:
     from werkzeug.middleware.dispatcher import DispatcherMiddleware
 except ImportError:
     from werkzeug.wsgi import DispatcherMiddleware
 
 
 class ListConverter(BaseConverter):
     """Simple list converter."""
 
     def to_python(self, value):
         """Return Python object."""
-        return value.split('+')
+        return value.split("+")
 
     def to_url(self, values):
         """Return string."""
-        return '+'.join(BaseConverter.to_url(value)
-                        for value in values)
+        return "+".join(BaseConverter.to_url(value) for value in values)
 
 
 #
 # Mock helpers
 #
 class MockLoggingHandler(logging.Handler):
     """Mock logging handler to check for expected logs."""
@@ -59,41 +66,48 @@
     def emit(self, record):
         """Emit log record by saving message to internal list."""
         self.messages[record.levelname.lower()].append(record.getMessage())
 
     def reset(self):
         """Reset internal list of messages."""
         self.messages = {
-            'debug': [],
-            'info': [],
-            'warning': [],
-            'error': [],
-            'critical': [],
+            "debug": [],
+            "info": [],
+            "warning": [],
+            "error": [],
+            "critical": [],
         }
 
 
 class MockEntryPoint(EntryPoint):
     """Mocking of entrypoint."""
 
     def load(self):
         """Mock load entry point."""
-        if self.name == 'fail':
+        if self.name == "fail":
             raise Exception("Fail")
         return self.name
 
 
 def _mock_entry_points(group=None):
     data = dict(
-        entrypoint1=[MockEntryPoint('ep1.e1', 'ep1.e1', 'ep1.e1'),
-                     MockEntryPoint('ep1.e2', 'ep1.e2', 'ep1.e2'), ],
-        entrypoint2=[MockEntryPoint('ep2.e1', 'ep2.e1', 'ep2.e1'),
-                     MockEntryPoint('ep2.e2', 'ep2.e2', 'ep2.e2'), ],
-        entrypoint3=[MockEntryPoint('fail', 'ep3.e1', 'ep3.e1'), ],
-        entrypoint4=[MockEntryPoint(
-            'mylist', 'test_app:ListConverter', 'mylist'), ],
+        entrypoint1=[
+            MockEntryPoint("ep1.e1", "ep1.e1", "ep1.e1"),
+            MockEntryPoint("ep1.e2", "ep1.e2", "ep1.e2"),
+        ],
+        entrypoint2=[
+            MockEntryPoint("ep2.e1", "ep2.e1", "ep2.e1"),
+            MockEntryPoint("ep2.e2", "ep2.e2", "ep2.e2"),
+        ],
+        entrypoint3=[
+            MockEntryPoint("fail", "ep3.e1", "ep3.e1"),
+        ],
+        entrypoint4=[
+            MockEntryPoint("mylist", "test_app:ListConverter", "mylist"),
+        ],
     )
     names = data.keys() if group is None else [group]
     for key in names:
         for entry_point in data[key]:
             yield entry_point
 
 
@@ -103,312 +117,314 @@
 def test_version():
     """Test version."""
     assert __version__
 
 
 def test_configure_warnings():
     """Test warnings configuration."""
-    logger = logging.getLogger('py.warnings')
+    logger = logging.getLogger("py.warnings")
     handler = MockLoggingHandler()
     logger.addHandler(handler)
 
     # Warnings not routed through logging
     warnings.warn("Test")
-    assert handler.messages['warning'] == []
+    assert handler.messages["warning"] == []
 
     # Warnings through logging
     configure_warnings()
     warnings.warn("A warning")
-    assert "A warning" in handler.messages['warning'][0]
+    assert "A warning" in handler.messages["warning"][0]
 
     handler.reset()
     warnings.warn("Pending deprecation", PendingDeprecationWarning)
     warnings.warn("Deprecation", DeprecationWarning)
-    assert len(handler.messages['warning']) == 1
+    assert len(handler.messages["warning"]) == 1
 
     handler.reset()
     warnings.simplefilter("always")
     warnings.warn("Pending deprecation", PendingDeprecationWarning)
     warnings.warn("Deprecation", DeprecationWarning)
-    assert len(handler.messages['warning']) == 2
+    assert len(handler.messages["warning"]) == 2
     warnings.resetwarnings()
 
 
-@patch('invenio_base.app.iter_entry_points', _mock_entry_points)
+@patch("invenio_base.app.iter_entry_points", _mock_entry_points)
 def test_loader():
     """Test loader."""
     app = Flask(__name__)
     found = []
     _loader(app, lambda x: found.append(x), entry_points=None, modules=None)
     assert found == []
 
     # Modules
     found = []
-    _loader(app, lambda x: found.append(x), modules=['a', 'b'])
-    assert found == ['a', 'b']
+    _loader(app, lambda x: found.append(x), modules=["a", "b"])
+    assert found == ["a", "b"]
 
     # Entry points
     found = []
-    _loader(
-        app,
-        lambda x: found.append(x), entry_points=['entrypoint1', 'entrypoint2'])
-    assert sorted(found) == ['ep1.e1', 'ep1.e2', 'ep2.e1', 'ep2.e2']
+    _loader(app, lambda x: found.append(x), entry_points=["entrypoint1", "entrypoint2"])
+    assert sorted(found) == ["ep1.e1", "ep1.e2", "ep2.e1", "ep2.e2"]
 
     # Modules and entry points (entry points loaded before modules)
     found = []
     _loader(
         app,
         lambda x: found.append(x),
-        entry_points=['entrypoint1', 'entrypoint2'],
-        modules=['a', 'b']
+        entry_points=["entrypoint1", "entrypoint2"],
+        modules=["a", "b"],
     )
-    assert sorted(found) == ['a', 'b', 'ep1.e1', 'ep1.e2', 'ep2.e1', 'ep2.e2']
+    assert sorted(found) == ["a", "b", "ep1.e1", "ep1.e2", "ep2.e1", "ep2.e2"]
 
 
-@patch('invenio_base.app.iter_entry_points', _mock_entry_points)
+@patch("invenio_base.app.iter_entry_points", _mock_entry_points)
 def test_loader_exceptions():
     """Test exceptions during loading."""
     app = Flask(__name__)
     handler = MockLoggingHandler()
     app.logger.addHandler(handler)
 
     def _raise_func():
         raise Exception()
 
-    assert len(handler.messages['error']) == 0
+    assert len(handler.messages["error"]) == 0
     pytest.raises(
-        Exception, _loader, app, lambda x: x(),
-        entry_points=None, modules=[_raise_func])
-    assert len(handler.messages['error']) == 1
+        Exception, _loader, app, lambda x: x(), entry_points=None, modules=[_raise_func]
+    )
+    assert len(handler.messages["error"]) == 1
 
     pytest.raises(
-        Exception, _loader, app, lambda x: x(),
-        entry_points=['entrypoint3'], modules=None)
-    assert len(handler.messages['error']) == 2
+        Exception,
+        _loader,
+        app,
+        lambda x: x(),
+        entry_points=["entrypoint3"],
+        modules=None,
+    )
+    assert len(handler.messages["error"]) == 2
 
 
 def test_app_loader():
     """Test app loader."""
+
     class FlaskExt(object):
         def __init__(self, app):
             self.app = app
-            app.extensions['ext'] = self
+            app.extensions["ext"] = self
 
-    app = Flask('testapp')
+    app = Flask("testapp")
 
-    assert 'ext' not in app.extensions
+    assert "ext" not in app.extensions
     app_loader(app, modules=[FlaskExt])
-    assert 'ext' in app.extensions
-    assert app.extensions['ext'].app is app
+    assert "ext" in app.extensions
+    assert app.extensions["ext"].app is app
 
 
 def test_blueprint_loader():
     """Test app loader."""
-    bp = Blueprint('test', 'test')
+    bp = Blueprint("test", "test")
 
     def create_blueprint_func(app):
-        return Blueprint('test2', 'test2')
+        return Blueprint("test2", "test2")
 
-    app = Flask('testapp')
+    app = Flask("testapp")
 
     assert len(app.blueprints) == 0
     blueprint_loader(app, modules=[bp, create_blueprint_func])
     assert len(app.blueprints) == 2
-    assert 'test' in app.blueprints
-    assert 'test2' in app.blueprints
+    assert "test" in app.blueprints
+    assert "test2" in app.blueprints
 
 
 def test_coverter_loader():
     """Test converter loader."""
-    app = Flask('testapp')
+    app = Flask("testapp")
 
-    assert 'mylist' not in app.url_map.converters
-    converter_loader(app, modules={'mylist': ListConverter})
-    assert 'mylist' in app.url_map.converters
+    assert "mylist" not in app.url_map.converters
+    converter_loader(app, modules={"mylist": ListConverter})
+    assert "mylist" in app.url_map.converters
 
 
-@patch('invenio_base.app.iter_entry_points', _mock_entry_points)
+@patch("invenio_base.app.iter_entry_points", _mock_entry_points)
 def test_coverter_loader_from_entry_points():
     """Test converter loader."""
-    app = Flask('testapp')
+    app = Flask("testapp")
 
-    assert 'mylist' not in app.url_map.converters
-    converter_loader(app, entry_points=['entrypoint4'])
-    assert 'mylist' in app.url_map.converters
+    assert "mylist" not in app.url_map.converters
+    converter_loader(app, entry_points=["entrypoint4"])
+    assert "mylist" in app.url_map.converters
 
 
-@patch('invenio_base.app.iter_entry_points', _mock_entry_points)
+@patch("invenio_base.app.iter_entry_points", _mock_entry_points)
 def test_coverter_loader_fail():
     """Test converter loader."""
-    app = Flask('testapp')
+    app = Flask("testapp")
 
     with pytest.raises(Exception):
-        converter_loader(app, entry_points=['entrypoint3'])
+        converter_loader(app, entry_points=["entrypoint3"])
 
 
 def test_base_app(tmp_path):
     """Test base app creation."""
     # Test default static_url_path and CLI initialization
-    app = base_app('test')
-    assert app.name == 'test'
+    app = base_app("test")
+    assert app.name == "test"
     assert app.cli
-    assert app.static_url_path == '/static'
+    assert app.static_url_path == "/static"
     assert app.instance_path != tmp_path
 
     # Test specifying instance path
-    app = base_app('test', instance_path=tmp_path)
+    app = base_app("test", instance_path=tmp_path)
     assert app.instance_path == tmp_path
     assert exists(app.instance_path)
     assert app.static_folder is None
 
     # Test automatic instance path creation
-    newpath = join(tmp_path, 'test')
+    newpath = join(tmp_path, "test")
     assert not exists(newpath)
-    app = base_app('test', instance_path=newpath)
+    app = base_app("test", instance_path=newpath)
     assert exists(newpath)
     assert app.static_folder is None
 
     # Test static folder
-    staticpath = join(tmp_path, 'teststatic')
-    app = base_app('test', static_folder=staticpath)
+    staticpath = join(tmp_path, "teststatic")
+    app = base_app("test", static_folder=staticpath)
     assert app.static_folder == staticpath
     assert app.instance_path is not None
 
     # Test static + instance folder
-    staticpath = join(tmp_path, 'teststatic')
-    app = base_app('test', instance_path=tmp_path,
-                   static_folder=staticpath)
+    staticpath = join(tmp_path, "teststatic")
+    app = base_app("test", instance_path=tmp_path, static_folder=staticpath)
     assert app.static_folder == staticpath
     assert app.instance_path == tmp_path
 
     # Test choice loader
     searchpath = join(tmp_path, "tpls")
-    app = base_app('test', template_folder=searchpath)
+    app = base_app("test", template_folder=searchpath)
     assert app.jinja_loader.searchpath == [searchpath]
 
-    app = base_app('test')
-    assert app.jinja_loader.searchpath == [join(app.root_path, 'templates')]
+    app = base_app("test")
+    assert app.jinja_loader.searchpath == [join(app.root_path, "templates")]
 
 
 def test_base_app_class(tmp_path):
     """Test using custom Flask application class."""
+
     class CustomFlask(Flask):
         pass
 
-    app = base_app('test', app_class=CustomFlask)
+    app = base_app("test", app_class=CustomFlask)
     assert isinstance(app, CustomFlask)
 
 
 def test_create_app_factory():
     """Test app factory factory."""
+
     class FlaskExt(object):
         def __init__(self, app):
             self.app = app
-            app.extensions['ext'] = self
+            app.extensions["ext"] = self
 
-    bp = Blueprint('test', 'test')
+    bp = Blueprint("test", "test")
 
     # Create app
-    create_app = create_app_factory(
-        'test', blueprints=[bp], extensions=[FlaskExt])
+    create_app = create_app_factory("test", blueprints=[bp], extensions=[FlaskExt])
     assert callable(create_app)
 
     app = create_app()
-    assert app.name == 'test'
+    assert app.name == "test"
     assert len(app.blueprints) == 1
-    assert 'ext' in app.extensions
+    assert "ext" in app.extensions
 
 
 def test_create_app_debug_flag():
     """Test debug flag propagation (needed by CLI)."""
-    create_app = create_app_factory('test')
+    create_app = create_app_factory("test")
 
     assert create_app().debug is False
     assert create_app(debug=True).debug is True
 
 
 def test_callable_instance_path(tmp_path):
     """Test instance path evaluation."""
 
     def instance_path():
         return tmp_path
 
-    app = create_app_factory('test', instance_path=instance_path)()
+    app = create_app_factory("test", instance_path=instance_path)()
     assert app.instance_path == tmp_path
     assert app.static_folder is None
 
 
 def test_callable_static_path(tmp_path):
     """Test static path evaluation."""
 
     def static_folder():
-        return join(tmp_path, 'teststatic')
+        return join(tmp_path, "teststatic")
 
-    app = create_app_factory('test', static_folder=static_folder)()
-    assert app.static_folder == join(tmp_path, 'teststatic')
+    app = create_app_factory("test", static_folder=static_folder)()
+    assert app.static_folder == join(tmp_path, "teststatic")
     assert app.instance_path is not None
 
 
 def test_create_app_factory_config_loader():
     """Test app factory conf loader."""
+
     def _config_loader(app, **kwargs):
-        app.config['CONFIG_LOADER'] = True
+        app.config["CONFIG_LOADER"] = True
         app.config.update(kwargs)
 
-    create_app = create_app_factory('test', config_loader=_config_loader)
+    create_app = create_app_factory("test", config_loader=_config_loader)
     app = create_app(KWARGS_TEST=True)
-    assert app.config['CONFIG_LOADER']
-    assert app.config['KWARGS_TEST']
+    assert app.config["CONFIG_LOADER"]
+    assert app.config["KWARGS_TEST"]
 
 
 def test_create_app_factory_wsgi_factory():
     """Test app factory wsgi factory."""
+
     def _wsgi_factory(app):
-        return DispatcherMiddleware(app.wsgi_app, {'/test': Flask('dispatch')})
+        return DispatcherMiddleware(app.wsgi_app, {"/test": Flask("dispatch")})
 
-    create_app = create_app_factory('test', wsgi_factory=_wsgi_factory)
+    create_app = create_app_factory("test", wsgi_factory=_wsgi_factory)
     app = create_app()
     assert isinstance(app.wsgi_app, DispatcherMiddleware)
 
 
 def test_create_cli_with_app():
     """Test create cli."""
-    app_name = 'mycmdtest'
+    app_name = "mycmdtest"
     create_app = create_app_factory(app_name)
     cli = create_cli(create_app=create_app)
 
     @cli.command()
     def test_cmd():
-        click.echo('{0} {1}'.format(current_app.name, current_app.debug))
+        click.echo(f"{current_app.name} {current_app.debug}")
 
     runner = CliRunner()
     result = runner.invoke(cli)
     assert result.exit_code == 0
 
-    result = runner.invoke(cli, ['test-cmd'])
+    result = runner.invoke(cli, ["test-cmd"])
     assert result.exit_code == 0
-    assert u'{0} False\n'.format(app_name) in result.output
+    assert f"{app_name} False\n" in result.output
 
 
 def test_create_cli_without_app():
     """Test create cli."""
     from invenio_base.__main__ import cli
 
     @cli.command()
     def test_cmd():
         click.echo(current_app.name)
 
     runner = CliRunner()
     result = runner.invoke(cli)
     assert result.exit_code == 0
 
-    result = runner.invoke(cli, ['test-cmd'])
-    assert result.exit_code != 0
-    assert 'FLASK_APP' in result.output
-
 
 def test_generate_secret_key():
     """Test generation of a secret key."""
     v1 = generate_secret_key()
     v2 = generate_secret_key()
     assert len(v1) == len(v2) == 256
     assert v1 != v2
```

### Comparing `invenio-base-1.2.9/tests/test_cmd.py` & `invenio-base-1.3.0/tests/test_cmd.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 import logging
 from unittest.mock import MagicMock, Mock, patch
 
 import pkg_resources
 import pytest
 from click.testing import CliRunner
-from flask.cli import ScriptInfo
 
 from invenio_base.app import create_app_factory
 from invenio_base.cli import instance
 
 
 @pytest.fixture(autouse=True)
 def force_logging():
@@ -27,116 +26,112 @@
     handler in case a handler is already installed. pytest
     automatically adds a handler to the root logger, causing
     Flask not to add a handler. This is an issue when testing
     Click output which uses the logger to output to the console.
     """
     try:
         from flask.logging import default_handler
-        logger = logging.getLogger('flask.app')
+
+        logger = logging.getLogger("flask.app")
         if default_handler not in logger.handlers:
             logger.handlers.append(default_handler)
     except Exception:
         pass
 
 
 def test_list_entry_points():
     """Test listing of entry points."""
     mock_working_set = pkg_resources.WorkingSet(entries=[])
-    dist = pkg_resources.get_distribution('invenio-base')
+    dist = pkg_resources.get_distribution("invenio-base")
     mock_working_set.add(dist)
 
-    with patch('invenio_base.cli.working_set', new=mock_working_set):
+    with patch("invenio_base.cli.working_set", new=mock_working_set):
         runner = CliRunner()
 
         # Test select an existing entry point
-        result = runner.invoke(
-            instance, ['entrypoints', '-e', 'console_scripts'])
+        result = runner.invoke(instance, ["entrypoints", "-e", "console_scripts"])
         assert result.exit_code == 0
         lines = result.output.splitlines()
-        assert lines[0] == 'console_scripts'
-        assert lines[1] == '  inveniomanage = invenio_base.__main__:cli'
+        assert lines[0] == "console_scripts"
+        assert lines[1] == "  inveniomanage = invenio_base.__main__:cli"
 
         # Test no entry point matching
-        result = runner.invoke(instance, ['entrypoints', '-e', 'nothing_here'])
+        result = runner.invoke(instance, ["entrypoints", "-e", "nothing_here"])
         assert result.exit_code == 0
         assert result.output == ""
 
         # By default we only show entry points groups starting with "invenio"
         dist.get_entry_map = Mock(
             return_value={
-                'invenio_base.apps': {
-                    'myapp': 'myapp = myapp:MyApp',
-                    'app1': 'app1 = app1:MyApp'
-                },
-                'invenio_base.api_apps': {
-                    'myapi': 'myapi = myapi:MyApp'
+                "invenio_base.apps": {
+                    "myapp": "myapp = myapp:MyApp",
+                    "app1": "app1 = app1:MyApp",
                 },
-                'console_scripts': {
-                    'mycli': 'mycli = cli:main'
-                },
-            })
-        result = runner.invoke(instance, [
-            'entrypoints',
-        ])
+                "invenio_base.api_apps": {"myapi": "myapi = myapi:MyApp"},
+                "console_scripts": {"mycli": "mycli = cli:main"},
+            }
+        )
+        result = runner.invoke(
+            instance,
+            [
+                "entrypoints",
+            ],
+        )
         assert result.exit_code == 0
         print(result.output.splitlines())
         lines = result.output.splitlines()
-        assert lines[0] == 'invenio_base.api_apps'
-        assert lines[1] == '  myapi = myapi:MyApp'
-        assert lines[2] == 'invenio_base.apps'
-        assert lines[3] == '  app1 = app1:MyApp'
-        assert lines[4] == '  myapp = myapp:MyApp'
+        assert lines[0] == "invenio_base.api_apps"
+        assert lines[1] == "  myapi = myapi:MyApp"
+        assert lines[2] == "invenio_base.apps"
+        assert lines[3] == "  app1 = app1:MyApp"
+        assert lines[4] == "  myapp = myapp:MyApp"
 
 
 def test_migrate_secret_key():
     """Test cli command for SECRET_KEY change."""
+
     def _config_loader(app, **kwargs):
-        app.config['CONFIG_LOADER'] = True
+        app.config["CONFIG_LOADER"] = True
         app.config.update(kwargs)
 
-    create_app = create_app_factory('test', config_loader=_config_loader)
+    create_app = create_app_factory("test", config_loader=_config_loader)
     app = create_app(KWARGS_TEST=True)
 
-    script_info = ScriptInfo(create_app=lambda info: app)
-
     # Check that CLI command fails when the SECRET_KEY is not set.
-    with app.app_context():
-        runner = CliRunner()
-        result = runner.invoke(
-            instance, ['migrate-secret-key', '--old-key', 'OLD_SECRET_KEY'],
-            obj=script_info)
-        assert result.exit_code == 1
-        assert 'Error: SECRET_KEY is not set in the configuration.' in \
-            result.output
+    runner = app.test_cli_runner()
+    result = runner.invoke(
+        instance, ["migrate-secret-key", "--old-key", "OLD_SECRET_KEY"]
+    )
+    assert result.exit_code == 1
+    assert "Error: SECRET_KEY is not set in the configuration." in result.output
 
     app.secret_key = "SECRET"
-    with patch('importlib_metadata.entry_points') as MockEP:
+    with patch("importlib_metadata.entry_points") as MockEP:
         # Test that the CLI command succeeds when the entrypoint does
         # return a function.
-        entrypoint = MockEP('ep1', 'ep1', 'ep1')
+        entrypoint = MockEP("ep1", "ep1", "ep1")
         entrypoint.load.return_value = MagicMock()
-        with patch('importlib_metadata.entry_points',
-                   return_value={'invenio_base.secret_key': [entrypoint]}):
+        with patch(
+            "importlib_metadata.entry_points",
+            return_value={"invenio_base.secret_key": [entrypoint]},
+        ):
             result = runner.invoke(
-                instance, ['migrate-secret-key', '--old-key',
-                           'OLD_SECRET_KEY'],
-                obj=script_info)
+                instance, ["migrate-secret-key", "--old-key", "OLD_SECRET_KEY"]
+            )
             assert result.exit_code == 0
             assert entrypoint.load.called
-            entrypoint.load.return_value.assert_called_with(
-                old_key='OLD_SECRET_KEY'
-            )
-            assert 'Successfully changed secret key.' in result.output
+            entrypoint.load.return_value.assert_called_with(old_key="OLD_SECRET_KEY")
+            assert "Successfully changed secret key." in result.output
 
         # Test that the CLI command fails correctly when the entrypoint does
         # not return a function.
-        entrypoint = MockEP('ep2', 'ep2', 'ep2')
-        entrypoint.load.return_value = 'ep2'
-        with patch('importlib_metadata.entry_points',
-                   return_value={'ep2': [entrypoint]}):
+        entrypoint = MockEP("ep2", "ep2", "ep2")
+        entrypoint.load.return_value = "ep2"
+        with patch(
+            "importlib_metadata.entry_points", return_value={"ep2": [entrypoint]}
+        ):
             result = runner.invoke(
-                instance, ['migrate-secret-key', '--old-key',
-                           'OLD_SECRET_KEY'],
-                obj=script_info)
+                instance, ["migrate-secret-key", "--old-key", "OLD_SECRET_KEY"]
+            )
             assert result.exit_code == 1
             assert entrypoint.load.called
-            assert 'Failed to perform migration of secret key' in result.output
+            assert "Failed to perform migration of secret key" in result.output
```

### Comparing `invenio-base-1.2.9/tests/test_signals.py` & `invenio-base-1.3.0/tests/test_signals.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 
 from invenio_base.app import create_app_factory
 from invenio_base.signals import app_created, app_loaded
 
 
 def test_create_app_factory():
     """Test signals sending."""
-    calls = {'created': 0, 'loaded': 0}
-    create_app = create_app_factory('test')
+    calls = {"created": 0, "loaded": 0}
+    create_app = create_app_factory("test")
 
     def _receiver(name):
         def _inner(sender, app=None):
             calls[name] += 1
-            calls[f'{name}_app'] = app
+            calls[f"{name}_app"] = app
+
         return _inner
 
-    app_created.connect(_receiver('created'), sender=create_app, weak=False)
-    app_loaded.connect(_receiver('loaded'), sender=create_app, weak=False)
+    app_created.connect(_receiver("created"), sender=create_app, weak=False)
+    app_loaded.connect(_receiver("loaded"), sender=create_app, weak=False)
 
     assert callable(create_app)
 
     app = create_app()
-    assert calls['created'] == 1
-    assert calls['loaded'] == 1
-    assert calls['created_app'] is app
-    assert calls['loaded_app'] is app
+    assert calls["created"] == 1
+    assert calls["loaded"] == 1
+    assert calls["created_app"] is app
+    assert calls["loaded_app"] is app
```

### Comparing `invenio-base-1.2.9/tests/test_utils.py` & `invenio-base-1.3.0/tests/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,22 +14,23 @@
 from invenio_base.wsgi import wsgi_proxyfix
 
 
 def test_obj_or_import_string():
     """Test object or string import utility function."""
     assert obj_or_import_string(wsgi_proxyfix) == wsgi_proxyfix
     assert obj_or_import_string(None, default=wsgi_proxyfix) == wsgi_proxyfix
-    assert obj_or_import_string(
-        'invenio_base.wsgi.wsgi_proxyfix') == wsgi_proxyfix
+    assert obj_or_import_string("invenio_base.wsgi.wsgi_proxyfix") == wsgi_proxyfix
 
 
 def test_load_or_import_from_config():
     """Test load or import from config utility function."""
-    app = Flask('testapp')
-    app.config['OBJ_KEY'] = wsgi_proxyfix
-    app.config['PATH_KEY'] = 'invenio_base.wsgi.wsgi_proxyfix'
+    app = Flask("testapp")
+    app.config["OBJ_KEY"] = wsgi_proxyfix
+    app.config["PATH_KEY"] = "invenio_base.wsgi.wsgi_proxyfix"
 
     with app.app_context():
-        assert load_or_import_from_config('OBJ_KEY') == wsgi_proxyfix
-        assert load_or_import_from_config('PATH_KEY') == wsgi_proxyfix
-        assert load_or_import_from_config(
-            'MISSING_KEY', default=wsgi_proxyfix) == wsgi_proxyfix
+        assert load_or_import_from_config("OBJ_KEY") == wsgi_proxyfix
+        assert load_or_import_from_config("PATH_KEY") == wsgi_proxyfix
+        assert (
+            load_or_import_from_config("MISSING_KEY", default=wsgi_proxyfix)
+            == wsgi_proxyfix
+        )
```

### Comparing `invenio-base-1.2.9/tests/test_wsgi.py` & `invenio-base-1.3.0/tests/test_wsgi.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,113 +16,114 @@
 from werkzeug import __version__ as werkzeug_version
 
 from invenio_base.wsgi import create_wsgi_factory, wsgi_proxyfix
 
 
 def test_create_wsgi_factory():
     """Test wsgi factory creation."""
-    api = Flask('api')
+    api = Flask("api")
 
-    @api.route('/')
+    @api.route("/")
     def apiview():
-        return 'api'
+        return "api"
 
-    app = Flask('app')
+    app = Flask("app")
 
-    @app.route('/')
+    @app.route("/")
     def appview():
-        return 'app'
+        return "app"
 
     # Test factory creation
-    factory = create_wsgi_factory({'/api': lambda **kwargs: api})
+    factory = create_wsgi_factory({"/api": lambda **kwargs: api})
     app.wsgi_app = factory(app)
 
     with app.test_client() as client:
-        assert client.get('/').status_code == 200
-        assert b'app' in client.get('/').data
-        assert client.get('/api/').status_code == 200
-        assert b'api' in client.get('/api/').data
+        assert client.get("/").status_code == 200
+        assert b"app" in client.get("/").data
+        assert client.get("/api/").status_code == 200
+        assert b"api" in client.get("/api/").data
 
 
-@pytest.mark.parametrize('proxies,data', [
-    (2, b'4.3.2.1'), (None, b'1.2.3.4')
-])
+@pytest.mark.parametrize("proxies,data", [(2, b"4.3.2.1"), (None, b"1.2.3.4")])
 def test_proxyfix_wsgi_proxies(proxies, data):
     """Test wsgi factory creation."""
-    app = Flask('app')
-    app.config['WSGI_PROXIES'] = proxies
+    app = Flask("app")
+    app.config["WSGI_PROXIES"] = proxies
 
-    @app.route('/')
+    @app.route("/")
     def appview():
         return str(request.remote_addr)
 
     # Test factory creation
     app.wsgi_app = wsgi_proxyfix()(app)
-    e = {'REMOTE_ADDR': '1.2.3.4'}
+    e = {"REMOTE_ADDR": "1.2.3.4"}
 
     with app.test_client() as client:
-        h = {'X-Forwarded-For': '5.6.7.8, 4.3.2.1, 8.7.6.5'}
-        assert client.get('/', headers=h, environ_base=e).data == data
+        h = {"X-Forwarded-For": "5.6.7.8, 4.3.2.1, 8.7.6.5"}
+        assert client.get("/", headers=h, environ_base=e).data == data
 
 
 @pytest.mark.parametrize(
-    'num_proxies,proxy_config', [
-        (n, {'x_for': n, 'x_proto': n, 'x_host': n, 'x_port': n,
-             'x_prefix': n}) for n in range(2)])
+    "num_proxies,proxy_config",
+    [
+        (n, {"x_for": n, "x_proto": n, "x_host": n, "x_port": n, "x_prefix": n})
+        for n in range(2)
+    ],
+)
 def test_proxyfix_wsgi_config(num_proxies, proxy_config):
     """Test wsgi factory creation with APP_WSGI_CONFIG set."""
-    if version.parse(werkzeug_version) < version.parse('0.15.0'):
+    if version.parse(werkzeug_version) < version.parse("0.15.0"):
         pytest.skip("Unsupported configuration for Werkzeug<0.15.0")
 
-    app = Flask('app')
-    app.config['PROXYFIX_CONFIG'] = proxy_config
+    app = Flask("app")
+    app.config["PROXYFIX_CONFIG"] = proxy_config
 
     data = [
         # application instance
         {
-            'x_for': '1.2.3.4',
-            'x_proto': 'http',
-            'x_host': 'localhost',
-            'x_port': '80',
-            'x_prefix': '',
+            "x_for": "1.2.3.4",
+            "x_proto": "http",
+            "x_host": "localhost",
+            "x_port": "80",
+            "x_prefix": "",
         },
         # proxy number 1
         {
-            'x_for': '5.6.7.8',
-            'x_proto': 'https',
-            'x_host': 'host.external',
-            'x_port': '443',
-            'x_prefix': 'prefix.external',
-        }
+            "x_for": "5.6.7.8",
+            "x_proto": "https",
+            "x_host": "host.external",
+            "x_port": "443",
+            "x_prefix": "prefix.external",
+        },
     ]
 
-    @app.route('/')
+    @app.route("/")
     def appview():
         data = {
-            'x_for': request.environ.get('REMOTE_ADDR'),
-            'x_proto': request.environ.get('wsgi.url_scheme'),
-            'x_host': request.environ.get('SERVER_NAME'),
-            'x_port': request.environ.get('SERVER_PORT'),
-            'x_prefix': request.environ.get('SCRIPT_NAME')
+            "x_for": request.environ.get("REMOTE_ADDR"),
+            "x_proto": request.environ.get("wsgi.url_scheme"),
+            "x_host": request.environ.get("SERVER_NAME"),
+            "x_port": request.environ.get("SERVER_PORT"),
+            "x_prefix": request.environ.get("SCRIPT_NAME"),
         }
         return jsonify(data)
 
     # Test factory creation
     app.wsgi_app = wsgi_proxyfix()(app)
     e = {
-        'REMOTE_ADDR': data[0].get('x_for'),
-        'wsgi.url_scheme': data[0].get('x_proto'),
-        'HTTP_HOST': data[0].get('x_host'),
-        'SERVER_PORT': data[0].get('x_port'),
-        'SCRIPT_NAME': data[0].get('x_prefix'),
+        "REMOTE_ADDR": data[0].get("x_for"),
+        "wsgi.url_scheme": data[0].get("x_proto"),
+        "HTTP_HOST": data[0].get("x_host"),
+        "SERVER_PORT": data[0].get("x_port"),
+        "SCRIPT_NAME": data[0].get("x_prefix"),
     }
 
     with app.test_client() as client:
         h = {
-            'X-Forwarded-For': data[1].get('x_for'),
-            'X-Forwarded-Proto': data[1].get('x_proto'),
-            'X-Forwarded-Host': data[1].get('x_host'),
-            'X-Forwarded-Port': data[1].get('x_port'),
-            'X-Forwarded-Prefix': data[1].get('x_prefix'),
+            "X-Forwarded-For": data[1].get("x_for"),
+            "X-Forwarded-Proto": data[1].get("x_proto"),
+            "X-Forwarded-Host": data[1].get("x_host"),
+            "X-Forwarded-Port": data[1].get("x_port"),
+            "X-Forwarded-Prefix": data[1].get("x_prefix"),
         }
-        res = client.get('/', headers=h, environ_base=e)
+        res = client.get("/", headers=h, environ_base=e)
         assert json.loads(res.get_data(as_text=True)) == data[num_proxies]
```

