# Comparing `tmp/dataframe_handlers-0.0.2.tar.gz` & `tmp/dataframe_handlers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataframe_handlers-0.0.2.tar", last modified: Mon Jun 26 01:37:42 2023, max compression
+gzip compressed data, was "dataframe_handlers-0.0.3.tar", last modified: Mon Jun 26 01:48:13 2023, max compression
```

## Comparing `dataframe_handlers-0.0.2.tar` & `dataframe_handlers-0.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 01:37:42.992350 dataframe_handlers-0.0.2/
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     1100 2023-06-25 20:49:06.000000 dataframe_handlers-0.0.2/LICENSE
--rw-r--r--   0 appuser   (1000) appuser   (1000)     5463 2023-06-26 01:37:42.983594 dataframe_handlers-0.0.2/PKG-INFO
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     4918 2023-06-26 01:15:00.000000 dataframe_handlers-0.0.2/README.md
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 01:37:42.601733 dataframe_handlers-0.0.2/dataframe_handlers/
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     2261 2023-06-26 01:29:01.000000 dataframe_handlers-0.0.2/dataframe_handlers/__init__.py
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 01:37:42.741966 dataframe_handlers-0.0.2/dataframe_handlers/base/
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)       78 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.2/dataframe_handlers/base/__init__.py
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     2946 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.2/dataframe_handlers/base/base.py
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 01:37:42.790020 dataframe_handlers-0.0.2/dataframe_handlers/dask_handler/
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)       86 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.2/dataframe_handlers/dask_handler/__init__.py
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     1529 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.2/dataframe_handlers/dask_handler/dask_handler.py
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 01:37:42.828628 dataframe_handlers-0.0.2/dataframe_handlers/pandas_handler/
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)       92 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.2/dataframe_handlers/pandas_handler/__init__.py
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     2029 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.2/dataframe_handlers/pandas_handler/pandas_handler.py
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 01:37:42.866239 dataframe_handlers-0.0.2/dataframe_handlers/vaex_handler/
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)       90 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.2/dataframe_handlers/vaex_handler/__init__.py
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     2219 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.2/dataframe_handlers/vaex_handler/vaex_handler.py
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 01:37:42.904794 dataframe_handlers-0.0.2/dataframe_handlers/xarray_handler/
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)       92 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.2/dataframe_handlers/xarray_handler/__init__.py
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     2549 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.2/dataframe_handlers/xarray_handler/xarray_handler.py
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 01:37:42.695063 dataframe_handlers-0.0.2/dataframe_handlers.egg-info/
--rw-r--r--   0 appuser   (1000) appuser   (1000)     5463 2023-06-26 01:37:42.000000 dataframe_handlers-0.0.2/dataframe_handlers.egg-info/PKG-INFO
--rw-r--r--   0 appuser   (1000) appuser   (1000)      832 2023-06-26 01:37:42.000000 dataframe_handlers-0.0.2/dataframe_handlers.egg-info/SOURCES.txt
--rw-r--r--   0 appuser   (1000) appuser   (1000)        1 2023-06-26 01:37:42.000000 dataframe_handlers-0.0.2/dataframe_handlers.egg-info/dependency_links.txt
--rw-r--r--   0 appuser   (1000) appuser   (1000)      151 2023-06-26 01:37:42.000000 dataframe_handlers-0.0.2/dataframe_handlers.egg-info/requires.txt
--rw-r--r--   0 appuser   (1000) appuser   (1000)       19 2023-06-26 01:37:42.000000 dataframe_handlers-0.0.2/dataframe_handlers.egg-info/top_level.txt
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     1331 2023-06-26 01:37:25.000000 dataframe_handlers-0.0.2/pyproject.toml
--rw-r--r--   0 appuser   (1000) appuser   (1000)       38 2023-06-26 01:37:42.993488 dataframe_handlers-0.0.2/setup.cfg
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 01:37:42.975139 dataframe_handlers-0.0.2/tests/
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)      269 2023-06-26 01:15:00.000000 dataframe_handlers-0.0.2/tests/test_dask_handler.py
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)      211 2023-06-26 01:15:00.000000 dataframe_handlers-0.0.2/tests/test_pandas_handler.py
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)      257 2023-06-26 01:15:00.000000 dataframe_handlers-0.0.2/tests/test_vaex_handler.py
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)      259 2023-06-26 01:15:00.000000 dataframe_handlers-0.0.2/tests/test_xarray_handler.py
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 01:48:13.178441 dataframe_handlers-0.0.3/
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     1100 2023-06-25 20:49:06.000000 dataframe_handlers-0.0.3/LICENSE
+-rw-r--r--   0 appuser   (1000) appuser   (1000)     5627 2023-06-26 01:48:13.167799 dataframe_handlers-0.0.3/PKG-INFO
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     5084 2023-06-26 01:46:16.000000 dataframe_handlers-0.0.3/README.md
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 01:48:12.768004 dataframe_handlers-0.0.3/dataframe_handlers/
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     2185 2023-06-26 01:47:20.000000 dataframe_handlers-0.0.3/dataframe_handlers/__init__.py
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 01:48:12.903049 dataframe_handlers-0.0.3/dataframe_handlers/base/
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)       78 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.3/dataframe_handlers/base/__init__.py
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     2946 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.3/dataframe_handlers/base/base.py
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 01:48:12.948753 dataframe_handlers-0.0.3/dataframe_handlers/dask_handler/
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)       86 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.3/dataframe_handlers/dask_handler/__init__.py
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     1529 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.3/dataframe_handlers/dask_handler/dask_handler.py
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 01:48:12.996859 dataframe_handlers-0.0.3/dataframe_handlers/pandas_handler/
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)       92 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.3/dataframe_handlers/pandas_handler/__init__.py
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     2029 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.3/dataframe_handlers/pandas_handler/pandas_handler.py
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 01:48:13.034253 dataframe_handlers-0.0.3/dataframe_handlers/vaex_handler/
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)       90 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.3/dataframe_handlers/vaex_handler/__init__.py
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     2219 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.3/dataframe_handlers/vaex_handler/vaex_handler.py
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 01:48:13.085727 dataframe_handlers-0.0.3/dataframe_handlers/xarray_handler/
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)       92 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.3/dataframe_handlers/xarray_handler/__init__.py
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     2549 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.3/dataframe_handlers/xarray_handler/xarray_handler.py
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 01:48:12.864188 dataframe_handlers-0.0.3/dataframe_handlers.egg-info/
+-rw-r--r--   0 appuser   (1000) appuser   (1000)     5627 2023-06-26 01:48:12.000000 dataframe_handlers-0.0.3/dataframe_handlers.egg-info/PKG-INFO
+-rw-r--r--   0 appuser   (1000) appuser   (1000)      832 2023-06-26 01:48:12.000000 dataframe_handlers-0.0.3/dataframe_handlers.egg-info/SOURCES.txt
+-rw-r--r--   0 appuser   (1000) appuser   (1000)        1 2023-06-26 01:48:12.000000 dataframe_handlers-0.0.3/dataframe_handlers.egg-info/dependency_links.txt
+-rw-r--r--   0 appuser   (1000) appuser   (1000)      151 2023-06-26 01:48:12.000000 dataframe_handlers-0.0.3/dataframe_handlers.egg-info/requires.txt
+-rw-r--r--   0 appuser   (1000) appuser   (1000)       19 2023-06-26 01:48:12.000000 dataframe_handlers-0.0.3/dataframe_handlers.egg-info/top_level.txt
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     1280 2023-06-26 01:47:20.000000 dataframe_handlers-0.0.3/pyproject.toml
+-rw-r--r--   0 appuser   (1000) appuser   (1000)       38 2023-06-26 01:48:13.180041 dataframe_handlers-0.0.3/setup.cfg
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 01:48:13.159706 dataframe_handlers-0.0.3/tests/
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)      269 2023-06-26 01:15:00.000000 dataframe_handlers-0.0.3/tests/test_dask_handler.py
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)      211 2023-06-26 01:15:00.000000 dataframe_handlers-0.0.3/tests/test_pandas_handler.py
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)      257 2023-06-26 01:15:00.000000 dataframe_handlers-0.0.3/tests/test_vaex_handler.py
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)      259 2023-06-26 01:15:00.000000 dataframe_handlers-0.0.3/tests/test_xarray_handler.py
```

### Comparing `dataframe_handlers-0.0.2/LICENSE` & `dataframe_handlers-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dataframe_handlers-0.0.2/PKG-INFO` & `dataframe_handlers-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataframe_handlers
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for handling dataframes with optional backends.
 Author: Joshua Sundance Bailey
 Maintainer: Joshua Sundance Bailey
 License: MIT
 Project-URL: Repository, https://github.com/joshuasundance-swca/dataframe_handlers.git
 Keywords: dataframe,interoperability
 Classifier: License :: OSI Approved :: MIT License
@@ -34,25 +34,27 @@
 
 `dataframe_handlers` aims to provide an abstract base class and concrete implementations for handling and manipulating dataframes of various types in Python.
 While the interface may be applicable to many use cases, the immediate goal is to standardize interaction with dataframe libraries and enable interoperability between them in the context of the [Solara](https://solara.dev) Python library, which can be used to create reactive web apps using pure Python.
 
 
 ## Installation
 
+https://pypi.org/project/dataframe-handlers
+
 ```bash
 # any of the following
 
-pip install .
-pip install .[pandas]
-pip install .[dask]
-pip install .[xarray]
-# pip install .[vaex]
-pip install .[testing]
+pip install dataframe-handlers
+pip install dataframe-handlers[pandas]
+pip install dataframe-handlers[dask]
+pip install dataframe-handlers[xarray]
+# pip install dataframe-handlers[vaex]
+pip install dataframe-handlers[testing]
 
-pip install .[pandas,xarray,testing]
+pip install dataframe-handlers[pandas,xarray,testing]
 ```
 
 ## Usage
 
 The base class, `BaseDataFrameHandler`, defines an abstract interface with the following methods:
 
 - `get_unique(column: str, limit: Optional[int] = None) -> Collection`
```

### Comparing `dataframe_handlers-0.0.2/README.md` & `dataframe_handlers-0.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 
 `dataframe_handlers` aims to provide an abstract base class and concrete implementations for handling and manipulating dataframes of various types in Python.
 While the interface may be applicable to many use cases, the immediate goal is to standardize interaction with dataframe libraries and enable interoperability between them in the context of the [Solara](https://solara.dev) Python library, which can be used to create reactive web apps using pure Python.
 
 
 ## Installation
 
+https://pypi.org/project/dataframe-handlers
+
 ```bash
 # any of the following
 
-pip install .
-pip install .[pandas]
-pip install .[dask]
-pip install .[xarray]
-# pip install .[vaex]
-pip install .[testing]
+pip install dataframe-handlers
+pip install dataframe-handlers[pandas]
+pip install dataframe-handlers[dask]
+pip install dataframe-handlers[xarray]
+# pip install dataframe-handlers[vaex]
+pip install dataframe-handlers[testing]
 
-pip install .[pandas,xarray,testing]
+pip install dataframe-handlers[pandas,xarray,testing]
 ```
 
 ## Usage
 
 The base class, `BaseDataFrameHandler`, defines an abstract interface with the following methods:
 
 - `get_unique(column: str, limit: Optional[int] = None) -> Collection`
```

### Comparing `dataframe_handlers-0.0.2/dataframe_handlers/base/base.py` & `dataframe_handlers-0.0.3/dataframe_handlers/base/base.py`

 * *Files identical despite different names*

### Comparing `dataframe_handlers-0.0.2/dataframe_handlers/dask_handler/dask_handler.py` & `dataframe_handlers-0.0.3/dataframe_handlers/dask_handler/dask_handler.py`

 * *Files identical despite different names*

### Comparing `dataframe_handlers-0.0.2/dataframe_handlers/pandas_handler/pandas_handler.py` & `dataframe_handlers-0.0.3/dataframe_handlers/pandas_handler/pandas_handler.py`

 * *Files identical despite different names*

### Comparing `dataframe_handlers-0.0.2/dataframe_handlers/vaex_handler/vaex_handler.py` & `dataframe_handlers-0.0.3/dataframe_handlers/vaex_handler/vaex_handler.py`

 * *Files identical despite different names*

### Comparing `dataframe_handlers-0.0.2/dataframe_handlers/xarray_handler/xarray_handler.py` & `dataframe_handlers-0.0.3/dataframe_handlers/xarray_handler/xarray_handler.py`

 * *Files identical despite different names*

### Comparing `dataframe_handlers-0.0.2/dataframe_handlers.egg-info/PKG-INFO` & `dataframe_handlers-0.0.3/dataframe_handlers.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataframe-handlers
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for handling dataframes with optional backends.
 Author: Joshua Sundance Bailey
 Maintainer: Joshua Sundance Bailey
 License: MIT
 Project-URL: Repository, https://github.com/joshuasundance-swca/dataframe_handlers.git
 Keywords: dataframe,interoperability
 Classifier: License :: OSI Approved :: MIT License
@@ -34,25 +34,27 @@
 
 `dataframe_handlers` aims to provide an abstract base class and concrete implementations for handling and manipulating dataframes of various types in Python.
 While the interface may be applicable to many use cases, the immediate goal is to standardize interaction with dataframe libraries and enable interoperability between them in the context of the [Solara](https://solara.dev) Python library, which can be used to create reactive web apps using pure Python.
 
 
 ## Installation
 
+https://pypi.org/project/dataframe-handlers
+
 ```bash
 # any of the following
 
-pip install .
-pip install .[pandas]
-pip install .[dask]
-pip install .[xarray]
-# pip install .[vaex]
-pip install .[testing]
+pip install dataframe-handlers
+pip install dataframe-handlers[pandas]
+pip install dataframe-handlers[dask]
+pip install dataframe-handlers[xarray]
+# pip install dataframe-handlers[vaex]
+pip install dataframe-handlers[testing]
 
-pip install .[pandas,xarray,testing]
+pip install dataframe-handlers[pandas,xarray,testing]
 ```
 
 ## Usage
 
 The base class, `BaseDataFrameHandler`, defines an abstract interface with the following methods:
 
 - `get_unique(column: str, limit: Optional[int] = None) -> Collection`
```

### Comparing `dataframe_handlers-0.0.2/dataframe_handlers.egg-info/SOURCES.txt` & `dataframe_handlers-0.0.3/dataframe_handlers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataframe_handlers-0.0.2/pyproject.toml` & `dataframe_handlers-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-[build-system]
-requires = ["setuptools", "wheel"]
-
-[project]
-name = "dataframe_handlers"
-version = "0.0.2"
-description = "A package for handling dataframes with optional backends."
-authors = [{name="Joshua Sundance Bailey"}]
-maintainers = [{name="Joshua Sundance Bailey"}]
-license = {text="MIT"}
-readme = "README.md"
-requires-python = ">=3.9"
-classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-]
-keywords = ["dataframe", "interoperability"]
-
-[project.urls]
-Repository = "https://github.com/joshuasundance-swca/dataframe_handlers.git"
-
-# Define optional dependencies
-[project.optional-dependencies]
-pandas = ["pandas"]
-dask = ["dask[dataframe]", "pandas"]
-#vaex = ["vaex"]
-xarray = ["xarray"]
-testing = [
-    "bumpver",
-    "coverage",
-    "coverage-badge",
-    "dask[dataframe]",
-    "numpy",
-#    "vaex",
-    "pandas",
-    "pytest",
-    "xarray",
-]
-
-[tool.bumpver]
-current_version = "0.0.2"
-version_pattern = "MAJOR.MINOR.PATCH"
-commit_message = "bump version {old_version} -> {new_version}"
-commit = true
-tag = true
-push = false
-
-[tool.bumpver.file_patterns]
-"pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
-"dataframe_handlers/__init__.py" = ["{version}"]
+[build-system]
+requires = ["setuptools", "wheel"]
+
+[project]
+name = "dataframe_handlers"
+version = "0.0.3"
+description = "A package for handling dataframes with optional backends."
+authors = [{name="Joshua Sundance Bailey"}]
+maintainers = [{name="Joshua Sundance Bailey"}]
+license = {text="MIT"}
+readme = "README.md"
+requires-python = ">=3.9"
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+]
+keywords = ["dataframe", "interoperability"]
+
+[project.urls]
+Repository = "https://github.com/joshuasundance-swca/dataframe_handlers.git"
+
+# Define optional dependencies
+[project.optional-dependencies]
+pandas = ["pandas"]
+dask = ["dask[dataframe]", "pandas"]
+#vaex = ["vaex"]
+xarray = ["xarray"]
+testing = [
+    "bumpver",
+    "coverage",
+    "coverage-badge",
+    "dask[dataframe]",
+    "numpy",
+#    "vaex",
+    "pandas",
+    "pytest",
+    "xarray",
+]
+
+[tool.bumpver]
+current_version = "0.0.3"
+version_pattern = "MAJOR.MINOR.PATCH"
+commit_message = "bump version {old_version} -> {new_version}"
+commit = true
+tag = true
+push = false
+
+[tool.bumpver.file_patterns]
+"pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
+"dataframe_handlers/__init__.py" = ["{version}"]
```

