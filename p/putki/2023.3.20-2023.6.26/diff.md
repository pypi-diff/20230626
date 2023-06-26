# Comparing `tmp/putki-2023.3.20.tar.gz` & `tmp/putki-2023.6.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "putki-2023.3.20.tar", last modified: Sun Mar 19 22:33:07 2023, max compression
+gzip compressed data, was "putki-2023.6.26.tar", last modified: Mon Jun 26 21:42:22 2023, max compression
```

## Comparing `putki-2023.3.20.tar` & `putki-2023.6.26.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-03-19 22:33:07.092537 putki-2023.3.20/
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 putki-2023.3.20/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)     3080 2023-03-19 22:33:07.092391 putki-2023.3.20/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     2091 2023-03-14 22:39:13.000000 putki-2023.3.20/README.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-03-19 22:33:07.090560 putki-2023.3.20/putki/
--rw-r--r--   0 ruth       (501) staff       (20)     2293 2023-03-19 22:31:28.000000 putki-2023.3.20/putki/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      123 2022-12-30 17:54:14.000000 putki-2023.3.20/putki/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)     1021 2023-03-19 22:28:46.000000 putki-2023.3.20/putki/api.py
--rw-r--r--   0 ruth       (501) staff       (20)     3621 2023-01-01 20:46:13.000000 putki-2023.3.20/putki/cli.py
--rw-r--r--   0 ruth       (501) staff       (20)     1918 2023-03-19 16:35:37.000000 putki-2023.3.20/putki/discover.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-03-19 22:33:07.091968 putki-2023.3.20/putki.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     3080 2023-03-19 22:33:07.000000 putki-2023.3.20/putki.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)      310 2023-03-19 22:33:07.000000 putki-2023.3.20/putki.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2023-03-19 22:33:07.000000 putki-2023.3.20/putki.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       40 2023-03-19 22:33:07.000000 putki-2023.3.20/putki.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)      118 2023-03-19 22:33:07.000000 putki-2023.3.20/putki.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)        6 2023-03-19 22:33:07.000000 putki-2023.3.20/putki.egg-info/top_level.txt
--rw-r--r--   0 ruth       (501) staff       (20)     2586 2023-03-19 22:27:04.000000 putki-2023.3.20/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       38 2023-03-19 22:33:07.092573 putki-2023.3.20/setup.cfg
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-03-19 22:33:07.092227 putki-2023.3.20/test/
--rw-r--r--   0 ruth       (501) staff       (20)      377 2023-03-19 21:17:56.000000 putki-2023.3.20/test/test_discover.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-26 21:42:22.042358 putki-2023.6.26/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 putki-2023.6.26/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)     3130 2023-06-26 21:42:22.042218 putki-2023.6.26/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2091 2023-03-14 22:39:13.000000 putki-2023.6.26/README.md
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-26 21:42:22.038987 putki-2023.6.26/putki/
+-rw-r--r--   0 ruth       (501) staff       (20)     2293 2023-06-26 21:41:05.000000 putki-2023.6.26/putki/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      123 2022-12-30 17:54:14.000000 putki-2023.6.26/putki/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1021 2023-03-19 22:28:46.000000 putki-2023.6.26/putki/api.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3621 2023-01-01 20:46:13.000000 putki-2023.6.26/putki/cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3238 2023-06-26 20:53:53.000000 putki-2023.6.26/putki/discover.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-26 21:42:22.041613 putki-2023.6.26/putki.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3130 2023-06-26 21:42:22.000000 putki-2023.6.26/putki.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)      310 2023-06-26 21:42:22.000000 putki-2023.6.26/putki.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-26 21:42:22.000000 putki-2023.6.26/putki.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       40 2023-06-26 21:42:22.000000 putki-2023.6.26/putki.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)      118 2023-06-26 21:42:22.000000 putki-2023.6.26/putki.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        6 2023-06-26 21:42:22.000000 putki-2023.6.26/putki.egg-info/top_level.txt
+-rw-r--r--   0 ruth       (501) staff       (20)     2648 2023-06-26 21:40:43.000000 putki-2023.6.26/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-26 21:42:22.042394 putki-2023.6.26/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-26 21:42:22.042032 putki-2023.6.26/test/
+-rw-r--r--   0 ruth       (501) staff       (20)      377 2023-03-19 21:17:56.000000 putki-2023.6.26/test/test_discover.py
```

### Comparing `putki-2023.3.20/LICENSE` & `putki-2023.6.26/LICENSE`

 * *Files identical despite different names*

### Comparing `putki-2023.3.20/PKG-INFO` & `putki-2023.6.26/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: putki
-Version: 2023.3.20
+Version: 2023.6.26
 Summary: Pipeline (Finnish: putki) - discovering and executing a specific task description.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/putki
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/putki
 Project-URL: Documentation, https://codes.dilettant.life/docs/putki
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/putki
 Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/putki
 Keywords: developer-tools,devops
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Putki
 
 Pipeline (Finnish: putki) - discovering and executing a specific task description.
```

### Comparing `putki-2023.3.20/README.md` & `putki-2023.6.26/README.md`

 * *Files identical despite different names*

### Comparing `putki-2023.3.20/putki/__init__.py` & `putki-2023.6.26/putki/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import datetime as dti
 import logging
 import os
 import pathlib
 from typing import List, no_type_check
 
 # [[[fill git_describe()]]]
-__version__ = '2023.3.20+parent.94c09fdc'
-# [[[end]]] (checksum: dfbe5da5072cf0e8feea97ad1bb8622d)
+__version__ = '2023.6.26+parent.c8205dfc'
+# [[[end]]] (checksum: 83560d0a74d2d1a11491c5a537894bde)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 
 APP_NAME = 'Pipeline (Finnish: putki) - discovering and executing a specific task description.'
 APP_ALIAS = 'putki'
 APP_ENV = 'PUTKI'
```

### Comparing `putki-2023.3.20/putki/api.py` & `putki-2023.6.26/putki/api.py`

 * *Files identical despite different names*

### Comparing `putki-2023.3.20/putki/cli.py` & `putki-2023.6.26/putki/cli.py`

 * *Files identical despite different names*

### Comparing `putki-2023.3.20/putki.egg-info/PKG-INFO` & `putki-2023.6.26/putki.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: putki
-Version: 2023.3.20
+Version: 2023.6.26
 Summary: Pipeline (Finnish: putki) - discovering and executing a specific task description.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/putki
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/putki
 Project-URL: Documentation, https://codes.dilettant.life/docs/putki
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/putki
 Project-URL: Test-Coverage, https://codes.dilettant.life/coverage/putki
 Keywords: developer-tools,devops
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Putki
 
 Pipeline (Finnish: putki) - discovering and executing a specific task description.
```

### Comparing `putki-2023.3.20/pyproject.toml` & `putki-2023.6.26/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "putki"
-version = "2023.3.20"
+version = "2023.6.26"
 description = "Pipeline (Finnish: putki) - discovering and executing a specific task description."
 readme = "README.md"
 authors = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 maintainers = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.9",
 ]
 keywords = ["developer-tools", "devops"]
 dependencies = [
-    "GitPython >= 3.1.30",
+    "GitPython >= 3.1.31",
     "PyYAML >= 6.0",
-    "typer >= 0.7.0",
+    "typer >= 0.9.0",
 ]
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "coverage", "hypothesis", "mypy", "pytest", "pytest-cov", "pytest-flake8", "ruff"]
 
 [project.urls]
 Homepage = "https://git.sr.ht/~sthagen/putki"
 Bug-Tracker = "https://todo.sr.ht/~sthagen/putki"
@@ -41,15 +42,15 @@
 [tool.setuptools.packages.find]
 include = ["putki"]
 exclude = ["test*"]
 
 [tool.black]
 line-length = 120
 skip-string-normalization = true
-target-version = ["py310", "py311"]
+target-version = ["py39", "py310", "py311", "py312"]
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 precision = 2
 exclude_lines = [
```

