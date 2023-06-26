# Comparing `tmp/prepper-1.2.0.tar.gz` & `tmp/prepper-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prepper-1.2.0.tar", last modified: Sun Jun 11 21:48:10 2023, max compression
+gzip compressed data, was "prepper-1.2.2.tar", last modified: Mon Jun 26 16:05:30 2023, max compression
```

## Comparing `prepper-1.2.0.tar` & `prepper-1.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:48:10.460364 prepper-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:48:10.456364 prepper-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:48:10.460364 prepper-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-11 21:48:00.000000 prepper-1.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-11 21:48:00.000000 prepper-1.2.0/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-11 21:48:00.000000 prepper-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-11 21:48:00.000000 prepper-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-11 21:48:00.000000 prepper-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-11 21:48:10.460364 prepper-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-11 21:48:00.000000 prepper-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:48:10.460364 prepper-1.2.0/prepper/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-11 21:48:00.000000 prepper-1.2.0/prepper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-11 21:48:10.000000 prepper-1.2.0/prepper/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-11 21:48:00.000000 prepper-1.2.0/prepper/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-11 21:48:00.000000 prepper-1.2.0/prepper/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    19362 2023-06-11 21:48:00.000000 prepper-1.2.0/prepper/exportable.py
--rw-r--r--   0 runner    (1001) docker     (123)    26985 2023-06-11 21:48:00.000000 prepper-1.2.0/prepper/io_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:48:10.460364 prepper-1.2.0/prepper/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:48:00.000000 prepper-1.2.0/prepper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-11 21:48:00.000000 prepper-1.2.0/prepper/tests/test_IO.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-11 21:48:00.000000 prepper-1.2.0/prepper/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-11 21:48:00.000000 prepper-1.2.0/prepper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:48:10.460364 prepper-1.2.0/prepper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-11 21:48:10.000000 prepper-1.2.0/prepper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-11 21:48:10.000000 prepper-1.2.0/prepper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 21:48:10.000000 prepper-1.2.0/prepper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-11 21:48:10.000000 prepper-1.2.0/prepper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-11 21:48:10.000000 prepper-1.2.0/prepper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-11 21:48:00.000000 prepper-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 21:48:10.460364 prepper-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.302766 prepper-1.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.298766 prepper-1.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.302766 prepper-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-26 16:05:18.000000 prepper-1.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-26 16:05:18.000000 prepper-1.2.2/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-26 16:05:18.000000 prepper-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-26 16:05:18.000000 prepper-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-26 16:05:18.000000 prepper-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-26 16:05:30.302766 prepper-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 16:05:18.000000 prepper-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.302766 prepper-1.2.2/prepper/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-26 16:05:18.000000 prepper-1.2.2/prepper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 16:05:30.000000 prepper-1.2.2/prepper/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-26 16:05:18.000000 prepper-1.2.2/prepper/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 16:05:18.000000 prepper-1.2.2/prepper/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19362 2023-06-26 16:05:18.000000 prepper-1.2.2/prepper/exportable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26985 2023-06-26 16:05:18.000000 prepper-1.2.2/prepper/io_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.302766 prepper-1.2.2/prepper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:18.000000 prepper-1.2.2/prepper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-26 16:05:18.000000 prepper-1.2.2/prepper/tests/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-26 16:05:18.000000 prepper-1.2.2/prepper/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-26 16:05:18.000000 prepper-1.2.2/prepper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.302766 prepper-1.2.2/prepper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-26 16:05:30.000000 prepper-1.2.2/prepper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-26 16:05:30.000000 prepper-1.2.2/prepper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:05:30.000000 prepper-1.2.2/prepper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-26 16:05:30.000000 prepper-1.2.2/prepper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 16:05:30.000000 prepper-1.2.2/prepper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-26 16:05:18.000000 prepper-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 16:05:30.302766 prepper-1.2.2/setup.cfg
```

### Comparing `prepper-1.2.0/.github/workflows/python-publish.yml` & `prepper-1.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `prepper-1.2.0/.github/workflows/python-test.yml` & `prepper-1.2.2/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `prepper-1.2.0/.gitignore` & `prepper-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `prepper-1.2.0/.pre-commit-config.yaml` & `prepper-1.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `prepper-1.2.0/LICENSE` & `prepper-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prepper-1.2.0/prepper/caching.py` & `prepper-1.2.2/prepper/caching.py`

 * *Files identical despite different names*

### Comparing `prepper-1.2.0/prepper/enums.py` & `prepper-1.2.2/prepper/enums.py`

 * *Files identical despite different names*

### Comparing `prepper-1.2.0/prepper/exportable.py` & `prepper-1.2.2/prepper/exportable.py`

 * *Files identical despite different names*

### Comparing `prepper-1.2.0/prepper/io_handlers.py` & `prepper-1.2.2/prepper/io_handlers.py`

 * *Files identical despite different names*

### Comparing `prepper-1.2.0/prepper/tests/test_IO.py` & `prepper-1.2.2/prepper/tests/test_IO.py`

 * *Files identical despite different names*

### Comparing `prepper-1.2.0/prepper/tests/test_decorators.py` & `prepper-1.2.2/prepper/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `prepper-1.2.0/prepper/utils.py` & `prepper-1.2.2/prepper/utils.py`

 * *Files identical despite different names*

### Comparing `prepper-1.2.0/prepper.egg-info/SOURCES.txt` & `prepper-1.2.2/prepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prepper-1.2.0/pyproject.toml` & `prepper-1.2.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "h5py ~= 3.8.0",
+    "h5py >= 3.8.0",
     "loguru >= 0.6.0",
-    "aenum ~= 3.1.11",
-    "numpy ~= 1.23.5",
-    "pandas ~= 1.5.1",
-    "joblib ~= 1.2.0",
+    "aenum >= 3.1.11",
+    "numpy >= 1.23.5",
+    "pandas >= 1.5.1",
+    "joblib >= 1.2.0",
     "typing_extensions >= 4.6.3",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 CI = ["pytest", "pytest-cov","hypothesis","pylint"]
```

