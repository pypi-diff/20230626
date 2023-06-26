# Comparing `tmp/cardsort-0.2.4.tar.gz` & `tmp/cardsort-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardsort-0.2.4.tar", max compression
+gzip compressed data, was "cardsort-0.2.6.tar", max compression
```

## Comparing `cardsort-0.2.4.tar` & `cardsort-0.2.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1077 2023-04-26 16:20:46.065297 cardsort-0.2.4/LICENSE
--rw-r--r--   0        0        0     2320 2023-04-26 16:20:46.065297 cardsort-0.2.4/README.md
--rw-r--r--   0        0        0     1344 2023-04-26 16:21:26.441783 cardsort-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      260 2023-04-26 16:20:46.069296 cardsort-0.2.4/src/cardsort/__init__.py
--rw-r--r--   0        0        0     9780 2023-04-26 16:20:46.069296 cardsort-0.2.4/src/cardsort/analysis.py
--rw-r--r--   0        0        0     2992 1970-01-01 00:00:00.000000 cardsort-0.2.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1077 2023-04-26 17:02:38.939947 cardsort-0.2.6/LICENSE
+-rw-r--r--   0        0        0     2320 2023-04-26 17:02:38.939947 cardsort-0.2.6/README.md
+-rw-r--r--   0        0        0     1356 2023-04-26 17:03:18.355560 cardsort-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      260 2023-04-26 17:02:38.943946 cardsort-0.2.6/src/cardsort/__init__.py
+-rw-r--r--   0        0        0     9780 2023-04-26 17:02:38.943946 cardsort-0.2.6/src/cardsort/analysis.py
+-rw-r--r--   0        0        0     2992 1970-01-01 00:00:00.000000 cardsort-0.2.6/PKG-INFO
```

### Comparing `cardsort-0.2.4/LICENSE` & `cardsort-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cardsort-0.2.4/README.md` & `cardsort-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `cardsort-0.2.4/pyproject.toml` & `cardsort-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cardsort"
-version = "0.2.4"
+version = "0.2.6"
 description = "Analyse data from open card sorting"
 authors = ["Katharina Kloppenborg"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
@@ -25,15 +25,15 @@
 myst-nb = "^0.17.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
-version_variable = "pyproject.toml:version" # version location
+version_variable = "pyproject.toml:tool.poetry.version" # version location
 version_source = "tag"                      # getting release version from GitHub tag
 branch = "main"                             # branch to make releases of
 changelog_file = "CHANGELOG.md"             # changelog file
 build_command = "poetry build"              # build dists
 dist_path = "dist/"                         # where to put dists
 upload_to_release = true                    # auto-create GitHub release
 upload_to_pypi = false                      # don't auto-upload to PyPI
```

### Comparing `cardsort-0.2.4/src/cardsort/analysis.py` & `cardsort-0.2.6/src/cardsort/analysis.py`

 * *Files identical despite different names*

### Comparing `cardsort-0.2.4/PKG-INFO` & `cardsort-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardsort
-Version: 0.2.4
+Version: 0.2.6
 Summary: Analyse data from open card sorting
 License: MIT
 Author: Katharina Kloppenborg
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

