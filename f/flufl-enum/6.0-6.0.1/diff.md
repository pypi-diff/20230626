# Comparing `tmp/flufl_enum-6.0.tar.gz` & `tmp/flufl_enum-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flufl_enum-6.0.tar", last modified: Tue Jun  6 16:17:58 2023, max compression
+gzip compressed data, was "flufl_enum-6.0.1.tar", last modified: Mon Jun 26 16:46:16 2023, max compression
```

## Comparing `flufl_enum-6.0.tar` & `flufl_enum-6.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      558 2023-06-06 16:17:30.671521 flufl_enum-6.0/LICENSE
--rw-r--r--   0        0        0     1165 2023-06-06 16:17:30.672521 flufl_enum-6.0/README.rst
--rw-r--r--   0        0        0     1377 2023-06-06 16:17:30.672521 flufl_enum-6.0/conftest.py
--rw-r--r--   0        0        0     6516 2023-06-06 16:17:30.672521 flufl_enum-6.0/docs/NEWS.rst
--rw-r--r--   0        0        0        0 2023-06-06 16:17:30.696521 flufl_enum-6.0/docs/__init__.py
--rw-r--r--   0        0        0      221 2023-06-06 16:17:30.672521 flufl_enum-6.0/docs/apiref.rst
--rw-r--r--   0        0        0     7176 2023-06-06 16:17:30.672521 flufl_enum-6.0/docs/conf.py
--rw-r--r--   0        0        0     2456 2023-06-06 16:17:30.672521 flufl_enum-6.0/docs/index.rst
--rw-r--r--   0        0        0    14725 2023-06-06 16:17:30.672521 flufl_enum-6.0/docs/using.rst
--rw-r--r--   0        0        0     3007 2023-06-06 16:17:58.452742 flufl_enum-6.0/pyproject.toml
--rw-r--r--   0        0        0      221 2023-06-06 16:17:30.673521 flufl_enum-6.0/src/flufl/enum/__init__.py
--rw-r--r--   0        0        0     9048 2023-06-06 16:17:30.673521 flufl_enum-6.0/src/flufl/enum/_enum.py
--rw-r--r--   0        0        0        0 2023-06-06 16:17:30.696521 flufl_enum-6.0/test/__init__.py
--rw-r--r--   0        0        0       92 2023-06-06 16:17:30.673521 flufl_enum-6.0/test/fruit.py
--rw-r--r--   0        0        0    10088 2023-06-06 16:17:30.673521 flufl_enum-6.0/test/test_enum.py
--rw-r--r--   0        0        0      772 2023-06-06 16:17:30.673521 flufl_enum-6.0/tox.ini
--rw-r--r--   0        0        0     2243 1970-01-01 00:00:00.000000 flufl_enum-6.0/PKG-INFO
+-rw-r--r--   0        0        0      558 2023-06-26 16:45:49.345758 flufl_enum-6.0.1/LICENSE
+-rw-r--r--   0        0        0     1165 2023-06-26 16:45:49.345758 flufl_enum-6.0.1/README.rst
+-rw-r--r--   0        0        0     1377 2023-06-26 16:45:49.345758 flufl_enum-6.0.1/conftest.py
+-rw-r--r--   0        0        0     6667 2023-06-26 16:45:49.345758 flufl_enum-6.0.1/docs/NEWS.rst
+-rw-r--r--   0        0        0        0 2023-06-26 16:45:49.369758 flufl_enum-6.0.1/docs/__init__.py
+-rw-r--r--   0        0        0      221 2023-06-26 16:45:49.345758 flufl_enum-6.0.1/docs/apiref.rst
+-rw-r--r--   0        0        0     7203 2023-06-26 16:45:49.345758 flufl_enum-6.0.1/docs/conf.py
+-rw-r--r--   0        0        0     2456 2023-06-26 16:45:49.345758 flufl_enum-6.0.1/docs/index.rst
+-rw-r--r--   0        0        0    14725 2023-06-26 16:45:49.345758 flufl_enum-6.0.1/docs/using.rst
+-rw-r--r--   0        0        0     3013 2023-06-26 16:46:16.595063 flufl_enum-6.0.1/pyproject.toml
+-rw-r--r--   0        0        0      223 2023-06-26 16:45:49.346758 flufl_enum-6.0.1/src/flufl/enum/__init__.py
+-rw-r--r--   0        0        0     9048 2023-06-26 16:45:49.346758 flufl_enum-6.0.1/src/flufl/enum/_enum.py
+-rw-r--r--   0        0        0        0 2023-06-26 16:45:49.369758 flufl_enum-6.0.1/test/__init__.py
+-rw-r--r--   0        0        0       92 2023-06-26 16:45:49.346758 flufl_enum-6.0.1/test/fruit.py
+-rw-r--r--   0        0        0    10088 2023-06-26 16:45:49.346758 flufl_enum-6.0.1/test/test_enum.py
+-rw-r--r--   0        0        0      772 2023-06-26 16:45:49.346758 flufl_enum-6.0.1/tox.ini
+-rw-r--r--   0        0        0     2245 1970-01-01 00:00:00.000000 flufl_enum-6.0.1/PKG-INFO
```

### Comparing `flufl_enum-6.0/LICENSE` & `flufl_enum-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flufl_enum-6.0/README.rst` & `flufl_enum-6.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `flufl_enum-6.0/conftest.py` & `flufl_enum-6.0.1/conftest.py`

 * *Files identical despite different names*

### Comparing `flufl_enum-6.0/docs/NEWS.rst` & `flufl_enum-6.0.1/docs/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =====================
 flufl.enum change log
 =====================
 
+6.0.1 (2023-06-26)
+==================
+* Update dependencies.
+* This release also utilizes a newer ``pdm-backend`` which fixes the project
+  metadata.
+
 6.0 (2023-06-05)
 ================
 * Drop Python 3.7 support. (GL#4)
 * Switch from ``flake8`` and ``isort`` to ``ruff`` for code quality. (GL#5)
 * More GitLab CI integration improvements.
 * Bump dependencies.
```

### Comparing `flufl_enum-6.0/docs/conf.py` & `flufl_enum-6.0.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     ]
 
 intersphinx_mapping = {
     'python': ('https://docs.python.org/', None),
     }
 
 #autodoc_typehints = 'both'
+autoclass_content = 'both'
 
 # We don't want to document the EnumValue.__init__() arguments because user
 # code will never call it directly.
 def skip_init(app, what, name, obj, skip, options):
     if getattr(obj, '__qualname__', None) == 'EnumValue.__init__':
         return True
     return skip
```

### Comparing `flufl_enum-6.0/docs/index.rst` & `flufl_enum-6.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `flufl_enum-6.0/docs/using.rst` & `flufl_enum-6.0.1/docs/using.rst`

 * *Files identical despite different names*

### Comparing `flufl_enum-6.0/pyproject.toml` & `flufl_enum-6.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "atpublic",
 ]
 dynamic = []
-version = "6.0"
+version = "6.0.1"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 "Home Page" = "https://fluflenum.readthedocs.io"
 Documentation = "https://fluflenum.readthedocs.io"
@@ -60,17 +60,17 @@
     "coverage[toml]",
     "diff-cover",
     "pytest",
     "pytest-cov",
     "sybil",
 ]
 qa = [
-    "ruff",
-    "mypy",
     "blue",
+    "mypy",
+    "ruff",
 ]
 docs = [
     "sphinx",
     "furo",
 ]
 
 [tool.pytest.ini_options]
@@ -111,15 +111,15 @@
 ]
 
 [tool.ruff.pydocstyle]
 convention = "pep257"
 
 [tool.ruff.isort]
 known-first-party = [
-    "public",
+    "flufl.enum",
 ]
 lines-after-imports = 2
 lines-between-types = 1
 order-by-type = true
 
 [tool.mypy]
 mypy_path = "src"
```

### Comparing `flufl_enum-6.0/src/flufl/enum/_enum.py` & `flufl_enum-6.0.1/src/flufl/enum/_enum.py`

 * *Files identical despite different names*

### Comparing `flufl_enum-6.0/test/test_enum.py` & `flufl_enum-6.0.1/test/test_enum.py`

 * *Files identical despite different names*

### Comparing `flufl_enum-6.0/tox.ini` & `flufl_enum-6.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `flufl_enum-6.0/PKG-INFO` & `flufl_enum-6.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flufl-enum
-Version: 6.0
+Name: flufl.enum
+Version: 6.0.1
 Summary: A Python enumeration package
 Keywords: enum
 Author-Email: Barry Warsaw <barry@python.org>
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
```

