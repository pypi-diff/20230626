# Comparing `tmp/py-avro-schema-2.1.1.tar.gz` & `tmp/py-avro-schema-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-avro-schema-2.1.1.tar", last modified: Fri Jun 23 11:47:37 2023, max compression
+gzip compressed data, was "py-avro-schema-2.1.2.tar", last modified: Mon Jun 26 07:38:11 2023, max compression
```

## Comparing `py-avro-schema-2.1.1.tar` & `py-avro-schema-2.1.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:37.884956 py-avro-schema-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:37.876956 py-avro-schema-2.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:37.880956 py-avro-schema-2.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/.github/workflows/release-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/.github/workflows/test-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/LICENSE_HEADER.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-06-23 11:47:37.884956 py-avro-schema-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:37.880956 py-avro-schema-2.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/docs/py_avro_schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/docs/types.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 11:47:37.884956 py-avro-schema-2.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:37.876956 py-avro-schema-2.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:37.880956 py-avro-schema-2.1.1/src/py_avro_schema/
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/src/py_avro_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34882 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/src/py_avro_schema/_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/src/py_avro_schema/_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/src/py_avro_schema/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/src/py_avro_schema/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:37.880956 py-avro-schema-2.1.1/src/py_avro_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-06-23 11:47:37.000000 py-avro-schema-2.1.1/src/py_avro_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-23 11:47:37.000000 py-avro-schema-2.1.1/src/py_avro_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 11:47:37.000000 py-avro-schema-2.1.1/src/py_avro_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-23 11:47:37.000000 py-avro-schema-2.1.1/src/py_avro_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 11:47:37.000000 py-avro-schema-2.1.1/src/py_avro_schema.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:47:37.884956 py-avro-schema-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/tests/test_avro_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/tests/test_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/tests/test_logicals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/tests/test_plain_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/tests/test_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/tests/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-23 11:47:22.000000 py-avro-schema-2.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:38:11.283255 py-avro-schema-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:38:11.275255 py-avro-schema-2.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:38:11.279255 py-avro-schema-2.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/.github/workflows/release-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/.github/workflows/test-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/LICENSE_HEADER.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-06-26 07:38:11.279255 py-avro-schema-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:38:11.279255 py-avro-schema-2.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/docs/py_avro_schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/docs/types.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 07:38:11.283255 py-avro-schema-2.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:38:11.275255 py-avro-schema-2.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:38:11.279255 py-avro-schema-2.1.2/src/py_avro_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/src/py_avro_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34882 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/src/py_avro_schema/_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/src/py_avro_schema/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/src/py_avro_schema/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/src/py_avro_schema/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:38:11.279255 py-avro-schema-2.1.2/src/py_avro_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14365 2023-06-26 07:38:11.000000 py-avro-schema-2.1.2/src/py_avro_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-26 07:38:11.000000 py-avro-schema-2.1.2/src/py_avro_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 07:38:11.000000 py-avro-schema-2.1.2/src/py_avro_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-26 07:38:11.000000 py-avro-schema-2.1.2/src/py_avro_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 07:38:11.000000 py-avro-schema-2.1.2/src/py_avro_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:38:11.279255 py-avro-schema-2.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/tests/test_avro_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/tests/test_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/tests/test_logicals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/tests/test_plain_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/tests/test_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/tests/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-26 07:38:00.000000 py-avro-schema-2.1.2/tox.ini
```

### Comparing `py-avro-schema-2.1.1/.flake8` & `py-avro-schema-2.1.2/.flake8`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/.github/workflows/release-package.yml` & `py-avro-schema-2.1.2/.github/workflows/release-package.yml`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/.github/workflows/test-package.yml` & `py-avro-schema-2.1.2/.github/workflows/test-package.yml`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/.gitignore` & `py-avro-schema-2.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/.pre-commit-config.yaml` & `py-avro-schema-2.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/LICENSE` & `py-avro-schema-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/LICENSE_HEADER.txt` & `py-avro-schema-2.1.2/LICENSE_HEADER.txt`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/PKG-INFO` & `py-avro-schema-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-avro-schema
-Version: 2.1.1
+Version: 2.1.2
 Summary: Generate Apache Avro schemas for Python types including standard library data-classes and Pydantic data models.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `py-avro-schema-2.1.1/README.md` & `py-avro-schema-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/docs/conf.py` & `py-avro-schema-2.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/docs/index.rst` & `py-avro-schema-2.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/docs/tutorial.rst` & `py-avro-schema-2.1.2/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/docs/types.rst` & `py-avro-schema-2.1.2/docs/types.rst`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/pyproject.toml` & `py-avro-schema-2.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
 # Minimum supported Python version
 requires-python = ">=3.7"
 # All runtime dependencies that must be packaged, pin major version only.
 dependencies = [
     "avro~=1.10",
     "importlib-metadata<4; python_version<'3.8'",
+    "memoization~=0.4",
     "orjson~=3.5",
     "typeguard~=2.12",
 ]
 
 
 [project.urls]
```

### Comparing `py-avro-schema-2.1.1/src/py_avro_schema/__init__.py` & `py-avro-schema-2.1.2/src/py_avro_schema/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
 .. seealso::
 
    Data types supported by **py-avro-schema**: :doc:`types`.
 
 """
 
-import functools
 from typing import Optional, Type
 
+import memoization
 import orjson
 
 from py_avro_schema._schemas import JSON_OPTIONS, Option, schema
 from py_avro_schema._typing import DecimalType
 
 try:
     from importlib import metadata
@@ -43,15 +43,15 @@
 __all__ = [
     "generate",
     "DecimalType",
     "Option",
 ]
 
 
-@functools.lru_cache(maxsize=None)
+@memoization.cached
 def generate(
     py_type: Type,
     *,
     namespace: Optional[str] = None,
     options: Option = Option(0),
 ) -> bytes:
     """
```

### Comparing `py-avro-schema-2.1.1/src/py_avro_schema/_schemas.py` & `py-avro-schema-2.1.2/src/py_avro_schema/_schemas.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/src/py_avro_schema/_testing.py` & `py-avro-schema-2.1.2/src/py_avro_schema/_testing.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/src/py_avro_schema/_typing.py` & `py-avro-schema-2.1.2/src/py_avro_schema/_typing.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/src/py_avro_schema.egg-info/PKG-INFO` & `py-avro-schema-2.1.2/src/py_avro_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-avro-schema
-Version: 2.1.1
+Version: 2.1.2
 Summary: Generate Apache Avro schemas for Python types including standard library data-classes and Pydantic data models.
 Author-email: "J.P. Morgan Chase & Co." <open_source@jpmorgan.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `py-avro-schema-2.1.1/src/py_avro_schema.egg-info/SOURCES.txt` & `py-avro-schema-2.1.2/src/py_avro_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/tests/test_avro_schema.py` & `py-avro-schema-2.1.2/tests/test_avro_schema.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/tests/test_dataclass.py` & `py-avro-schema-2.1.2/tests/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/tests/test_logicals.py` & `py-avro-schema-2.1.2/tests/test_logicals.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/tests/test_plain_class.py` & `py-avro-schema-2.1.2/tests/test_plain_class.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/tests/test_primitives.py` & `py-avro-schema-2.1.2/tests/test_primitives.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/tests/test_pydantic.py` & `py-avro-schema-2.1.2/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/tests/test_typing.py` & `py-avro-schema-2.1.2/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `py-avro-schema-2.1.1/tox.ini` & `py-avro-schema-2.1.2/tox.ini`

 * *Files identical despite different names*

