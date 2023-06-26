# Comparing `tmp/invokelint-0.8.0.tar.gz` & `tmp/invokelint-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invokelint-0.8.0.tar", last modified: Sun Apr 30 12:39:16 2023, max compression
+gzip compressed data, was "invokelint-0.8.1.tar", last modified: Mon Jun 26 05:52:45 2023, max compression
```

## Comparing `invokelint-0.8.0.tar` & `invokelint-0.8.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:39:16.731866 invokelint-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-30 12:38:15.000000 invokelint-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-30 12:38:15.000000 invokelint-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12388 2023-04-30 12:39:16.731866 invokelint-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-04-30 12:38:15.000000 invokelint-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:39:16.727865 invokelint-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-30 12:38:15.000000 invokelint-0.8.0/docs/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:39:16.731866 invokelint-0.8.0/invokelint/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:39:16.731866 invokelint-0.8.0/invokelint/path/
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/path/filter_duplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/path/setuptools.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/ruff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-30 12:38:15.000000 invokelint-0.8.0/invokelint/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:39:16.731866 invokelint-0.8.0/invokelint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12388 2023-04-30 12:39:16.000000 invokelint-0.8.0/invokelint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-30 12:39:16.000000 invokelint-0.8.0/invokelint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:39:16.000000 invokelint-0.8.0/invokelint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 12:39:16.000000 invokelint-0.8.0/invokelint.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-30 12:39:16.000000 invokelint-0.8.0/invokelint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-30 12:39:16.000000 invokelint-0.8.0/invokelint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-04-30 12:38:15.000000 invokelint-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-30 12:39:16.735865 invokelint-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-30 12:38:15.000000 invokelint-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 12:39:16.731866 invokelint-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-30 12:38:15.000000 invokelint-0.8.0/tests/test__clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-30 12:38:15.000000 invokelint-0.8.0/tests/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-30 12:38:15.000000 invokelint-0.8.0/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-30 12:38:15.000000 invokelint-0.8.0/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-30 12:38:15.000000 invokelint-0.8.0/tests/test_style.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-30 12:38:15.000000 invokelint-0.8.0/tests/test_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:52:45.203769 invokelint-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-26 05:51:52.000000 invokelint-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 05:51:52.000000 invokelint-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12388 2023-06-26 05:52:45.203769 invokelint-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-06-26 05:51:52.000000 invokelint-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:52:45.199769 invokelint-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-06-26 05:51:52.000000 invokelint-0.8.1/docs/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:52:45.203769 invokelint-0.8.1/invokelint/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-26 05:51:52.000000 invokelint-0.8.1/invokelint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-26 05:51:52.000000 invokelint-0.8.1/invokelint/_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-26 05:51:52.000000 invokelint-0.8.1/invokelint/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-06-26 05:51:52.000000 invokelint-0.8.1/invokelint/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:52:45.203769 invokelint-0.8.1/invokelint/path/
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-26 05:51:52.000000 invokelint-0.8.1/invokelint/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-26 05:51:52.000000 invokelint-0.8.1/invokelint/path/filter_duplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-26 05:51:52.000000 invokelint-0.8.1/invokelint/path/setuptools.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 05:51:52.000000 invokelint-0.8.1/invokelint/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-26 05:51:52.000000 invokelint-0.8.1/invokelint/ruff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-26 05:51:52.000000 invokelint-0.8.1/invokelint/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-26 05:51:52.000000 invokelint-0.8.1/invokelint/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-26 05:51:52.000000 invokelint-0.8.1/invokelint/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:52:45.203769 invokelint-0.8.1/invokelint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12388 2023-06-26 05:52:45.000000 invokelint-0.8.1/invokelint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-26 05:52:45.000000 invokelint-0.8.1/invokelint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 05:52:45.000000 invokelint-0.8.1/invokelint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 05:52:44.000000 invokelint-0.8.1/invokelint.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 05:52:45.000000 invokelint-0.8.1/invokelint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 05:52:45.000000 invokelint-0.8.1/invokelint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-06-26 05:51:52.000000 invokelint-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-26 05:52:45.203769 invokelint-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-26 05:51:52.000000 invokelint-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 05:52:45.203769 invokelint-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-26 05:51:52.000000 invokelint-0.8.1/tests/test__clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-26 05:51:52.000000 invokelint-0.8.1/tests/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-26 05:51:52.000000 invokelint-0.8.1/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-26 05:51:52.000000 invokelint-0.8.1/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-26 05:51:52.000000 invokelint-0.8.1/tests/test_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-06-26 05:51:52.000000 invokelint-0.8.1/tests/test_test.py
```

### Comparing `invokelint-0.8.0/LICENSE` & `invokelint-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invokelint-0.8.0/PKG-INFO` & `invokelint-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invokelint
-Version: 0.8.0
+Version: 0.8.1
 Summary: Invokes Python dev tools at once.
 Author-email: Yukihiko Shinoda <yuk.hik.future@gmail.com>
 Maintainer-email: Yukihiko Shinoda <yuk.hik.future@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yukihiko Shinoda
```

### Comparing `invokelint-0.8.0/README.md` & `invokelint-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `invokelint-0.8.0/docs/CONTRIBUTING.md` & `invokelint-0.8.1/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `invokelint-0.8.0/invokelint/_clean.py` & `invokelint-0.8.1/invokelint/_clean.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.8.0/invokelint/dist.py` & `invokelint-0.8.1/invokelint/dist.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.8.0/invokelint/lint.py` & `invokelint-0.8.1/invokelint/lint.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.8.0/invokelint/path/__init__.py` & `invokelint-0.8.1/invokelint/path/__init__.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.8.0/invokelint/path/filter_duplication.py` & `invokelint-0.8.1/invokelint/path/filter_duplication.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.8.0/invokelint/path/setuptools.py` & `invokelint-0.8.1/invokelint/path/setuptools.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.8.0/invokelint/ruff.py` & `invokelint-0.8.1/invokelint/ruff.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.8.0/invokelint/run.py` & `invokelint-0.8.1/invokelint/run.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.8.0/invokelint/test.py` & `invokelint-0.8.1/invokelint/test.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.8.0/invokelint.egg-info/PKG-INFO` & `invokelint-0.8.1/invokelint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invokelint
-Version: 0.8.0
+Version: 0.8.1
 Summary: Invokes Python dev tools at once.
 Author-email: Yukihiko Shinoda <yuk.hik.future@gmail.com>
 Maintainer-email: Yukihiko Shinoda <yuk.hik.future@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Yukihiko Shinoda
```

### Comparing `invokelint-0.8.0/invokelint.egg-info/SOURCES.txt` & `invokelint-0.8.1/invokelint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invokelint-0.8.0/pyproject.toml` & `invokelint-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "invokelint"
-version = "0.8.0"
+version = "0.8.1"
 description = "Invokes Python dev tools at once."
 readme = "README.md"
 # Dependency: setuptools>=61.0.0 requires Python 3.7
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = [
     "autoflake",
@@ -58,14 +58,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
     "Topic :: Software Development :: Testing",
     "Topic :: Software Development :: Testing :: Unit",
     "Typing :: Typed",
 ]
 dependencies = [
+    "click",
     "invoke",
     # To import setuptools.discovery
     "setuptools>=61.0.0",
 ]
 
 [project.optional-dependencies]
 test = []
```

### Comparing `invokelint-0.8.0/tests/test__clean.py` & `invokelint-0.8.1/tests/test__clean.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.8.0/tests/test_dist.py` & `invokelint-0.8.1/tests/test_dist.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.8.0/tests/test_lint.py` & `invokelint-0.8.1/tests/test_lint.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.8.0/tests/test_run.py` & `invokelint-0.8.1/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `invokelint-0.8.0/tests/test_style.py` & `invokelint-0.8.1/tests/test_style.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 
 if TYPE_CHECKING:
     from invoke import Context
 
 PYTHON_DIR = "invokelint setup.py tasks.py tests"
 
 LIST_COMMAND_EXPECTED_STYLE_WITHOUT_RUFF = [
-    f"docformatter --recursive --wrap-summaries 119 --wrap-descriptions 119 --in-place {PYTHON_DIR}",
+    f"docformatter --recursive --in-place {PYTHON_DIR}",
     f"isort {PYTHON_DIR}",
     f"autoflake --recursive --in-place {PYTHON_DIR}",
     f"black {PYTHON_DIR}",
 ]
 LIST_COMMAND_EXPECTED_STYLE = [
     *LIST_COMMAND_EXPECTED_STYLE_WITHOUT_RUFF,
     "ruff --fix --show-fixes --ignore S101 tests",
 ]
 LIST_COMMAND_EXPECTED_STYLE_CHECK = [
-    f"docformatter --recursive --wrap-summaries 119 --wrap-descriptions 119 --check {PYTHON_DIR}",
+    f"docformatter --recursive --check {PYTHON_DIR}",
     f"isort --check-only --diff {PYTHON_DIR}",
     f"autoflake --recursive --check {PYTHON_DIR}",
     f"black --check --diff {PYTHON_DIR}",
     "ruff --show-fixes --ignore S101 tests",
 ]
```

### Comparing `invokelint-0.8.0/tests/test_test.py` & `invokelint-0.8.1/tests/test_test.py`

 * *Files identical despite different names*

