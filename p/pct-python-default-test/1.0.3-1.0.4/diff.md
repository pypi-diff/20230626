# Comparing `tmp/pct_python_default_test-1.0.3.tar.gz` & `tmp/pct_python_default_test-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pct_python_default_test-1.0.3.tar", last modified: Fri Jan 13 00:29:53 2023, max compression
+gzip compressed data, was "pct_python_default_test-1.0.4.tar", last modified: Mon Jun 26 21:27:53 2023, max compression
```

## Comparing `pct_python_default_test-1.0.3.tar` & `pct_python_default_test-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:29:53.825313 pct_python_default_test-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-01-13 00:29:14.000000 pct_python_default_test-1.0.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-01-13 00:29:14.000000 pct_python_default_test-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-13 00:29:14.000000 pct_python_default_test-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-01-13 00:29:53.825313 pct_python_default_test-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-01-13 00:29:14.000000 pct_python_default_test-1.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:29:53.825313 pct_python_default_test-1.0.3/pct_python_default_test/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-01-13 00:29:14.000000 pct_python_default_test-1.0.3/pct_python_default_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-01-13 00:29:14.000000 pct_python_default_test-1.0.3/pct_python_default_test/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-01-13 00:29:14.000000 pct_python_default_test-1.0.3/pct_python_default_test/pct_python_default_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-01-13 00:29:14.000000 pct_python_default_test-1.0.3/pct_python_default_test/pct_python_default_test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 00:29:14.000000 pct_python_default_test-1.0.3/pct_python_default_test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:29:53.825313 pct_python_default_test-1.0.3/pct_python_default_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-01-13 00:29:53.000000 pct_python_default_test-1.0.3/pct_python_default_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-01-13 00:29:53.000000 pct_python_default_test-1.0.3/pct_python_default_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 00:29:53.000000 pct_python_default_test-1.0.3/pct_python_default_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-13 00:29:53.000000 pct_python_default_test-1.0.3/pct_python_default_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 00:29:53.000000 pct_python_default_test-1.0.3/pct_python_default_test.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-13 00:29:53.000000 pct_python_default_test-1.0.3/pct_python_default_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-13 00:29:53.000000 pct_python_default_test-1.0.3/pct_python_default_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-01-13 00:29:14.000000 pct_python_default_test-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-01-13 00:29:53.829313 pct_python_default_test-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-01-13 00:29:14.000000 pct_python_default_test-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:27:53.761475 pct_python_default_test-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-26 21:27:53.761475 pct_python_default_test-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:27:53.761475 pct_python_default_test-1.0.4/pct_python_default_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/pct_python_default_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/pct_python_default_test/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/pct_python_default_test/pct_python_default_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/pct_python_default_test/pct_python_default_test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/pct_python_default_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:27:53.761475 pct_python_default_test-1.0.4/pct_python_default_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-26 21:27:53.000000 pct_python_default_test-1.0.4/pct_python_default_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-26 21:27:53.000000 pct_python_default_test-1.0.4/pct_python_default_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:27:53.000000 pct_python_default_test-1.0.4/pct_python_default_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-26 21:27:53.000000 pct_python_default_test-1.0.4/pct_python_default_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 21:27:53.000000 pct_python_default_test-1.0.4/pct_python_default_test.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 21:27:53.000000 pct_python_default_test-1.0.4/pct_python_default_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 21:27:53.000000 pct_python_default_test-1.0.4/pct_python_default_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-26 21:27:53.761475 pct_python_default_test-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 21:27:53.761475 pct_python_default_test-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-26 21:27:16.000000 pct_python_default_test-1.0.4/tests/test_cli.py
```

### Comparing `pct_python_default_test-1.0.3/CHANGES.rst` & `pct_python_default_test-1.0.4/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 Changelog
 ---------
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.0.4
+---------
+2023-06-26:
+    - correct black settings
+    - get rid of travis
+    - do not upload .egg files to pypi.org
+
 v1.0.3
 ---------
 2023-01-13:
     - update github actions : checkout@v3 and setup-python@v4
     - remove "better code" badges
     - remove python 3.6 tests
     - add python 3.11 tests
```

### Comparing `pct_python_default_test-1.0.3/LICENSE` & `pct_python_default_test-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.3/PKG-INFO` & `pct_python_default_test-1.0.4/pct_python_default_test.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pct_python_default_test
-Version: 1.0.3
+Name: pct-python-default-test
+Version: 1.0.4
 Summary: a pizzacutter default test project, crated with PizzaCutter and the PizzaCutter default python template
 Home-page: https://github.com/bitranox/pct_python_default_test
 Author: Robert Nowotny
 Author-email: bitranox@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 pct_python_default_test
 =======================
 
 
-Version v1.0.3 as of 2023-01-13 see `Changelog`_
+Version v1.0.4 as of 2023-06-26 see `Changelog`_
 
 |build_badge| |license| |jupyter| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -77,22 +77,22 @@
 More Information can be found here :
     - `PizzaCutter <https://github.com/bitranox/PizzaCutter>`_
     - `PizzaCutter python default template <https://github.com/bitranox/pct_python_default>`_
     - more templates to come
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.7.0 or newer
 
 tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/pct_python_default_test>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/pct_python_default_test/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/pct_python_default_test/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/pct_python_default_test/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -263,14 +263,21 @@
 Changelog
 ---------
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.0.4
+---------
+2023-06-26:
+    - correct black settings
+    - get rid of travis
+    - do not upload .egg files to pypi.org
+
 v1.0.3
 ---------
 2023-01-13:
     - update github actions : checkout@v3 and setup-python@v4
     - remove "better code" badges
     - remove python 3.6 tests
     - add python 3.11 tests
```

### Comparing `pct_python_default_test-1.0.3/README.rst` & `pct_python_default_test-1.0.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pct_python_default_test
 =======================
 
 
-Version v1.0.3 as of 2023-01-13 see `Changelog`_
+Version v1.0.4 as of 2023-06-26 see `Changelog`_
 
 |build_badge| |license| |jupyter| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -59,22 +59,22 @@
 More Information can be found here :
     - `PizzaCutter <https://github.com/bitranox/PizzaCutter>`_
     - `PizzaCutter python default template <https://github.com/bitranox/pct_python_default>`_
     - more templates to come
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.7.0 or newer
 
 tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/pct_python_default_test>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/pct_python_default_test/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/pct_python_default_test/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/pct_python_default_test/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -245,14 +245,21 @@
 Changelog
 ---------
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.0.4
+---------
+2023-06-26:
+    - correct black settings
+    - get rid of travis
+    - do not upload .egg files to pypi.org
+
 v1.0.3
 ---------
 2023-01-13:
     - update github actions : checkout@v3 and setup-python@v4
     - remove "better code" badges
     - remove python 3.6 tests
     - add python 3.11 tests
```

### Comparing `pct_python_default_test-1.0.3/pct_python_default_test/__init__conf__.py` & `pct_python_default_test-1.0.4/pct_python_default_test/__init__conf__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # CONF
 
 name = "pct_python_default_test"
 title = "a pizzacutter default test project, crated with PizzaCutter and the PizzaCutter default python template"
-version = "v1.0.3"
+version = "v1.0.4"
 url = "https://github.com/bitranox/pct_python_default_test"
 author = "Robert Nowotny"
 author_email = "bitranox@gmail.com"
 shell_command = "pct_python_default_test"
 
 
 def print_info() -> None:
     print(
         """\
 
 Info for pct_python_default_test:
 
     a pizzacutter default test project, crated with PizzaCutter and the PizzaCutter default python template
 
-    Version : v1.0.3
+    Version : v1.0.4
     Url     : https://github.com/bitranox/pct_python_default_test
     Author  : Robert Nowotny
     Email   : bitranox@gmail.com"""
     )
```

### Comparing `pct_python_default_test-1.0.3/pct_python_default_test/pct_python_default_test.py` & `pct_python_default_test-1.0.4/pct_python_default_test/pct_python_default_test.py`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.3/pct_python_default_test/pct_python_default_test_cli.py` & `pct_python_default_test-1.0.4/pct_python_default_test/pct_python_default_test_cli.py`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.3/pct_python_default_test.egg-info/PKG-INFO` & `pct_python_default_test-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pct-python-default-test
-Version: 1.0.3
+Name: pct_python_default_test
+Version: 1.0.4
 Summary: a pizzacutter default test project, crated with PizzaCutter and the PizzaCutter default python template
 Home-page: https://github.com/bitranox/pct_python_default_test
 Author: Robert Nowotny
 Author-email: bitranox@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 pct_python_default_test
 =======================
 
 
-Version v1.0.3 as of 2023-01-13 see `Changelog`_
+Version v1.0.4 as of 2023-06-26 see `Changelog`_
 
 |build_badge| |license| |jupyter| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -77,22 +77,22 @@
 More Information can be found here :
     - `PizzaCutter <https://github.com/bitranox/PizzaCutter>`_
     - `PizzaCutter python default template <https://github.com/bitranox/pct_python_default>`_
     - more templates to come
 
 ----
 
-automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
+automated tests, Github Actions, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
 Python version required: 3.7.0 or newer
 
 tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
-`100% code coverage <https://codecov.io/gh/bitranox/pct_python_default_test>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/pct_python_default_test/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
+`100% code coverage <https://codeclimate.com/github/bitranox/pct_python_default_test/test_coverage>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/pct_python_default_test/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
 - `Usage from Commandline`_
 - `Installation and Upgrade`_
@@ -263,14 +263,21 @@
 Changelog
 ---------
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v1.0.4
+---------
+2023-06-26:
+    - correct black settings
+    - get rid of travis
+    - do not upload .egg files to pypi.org
+
 v1.0.3
 ---------
 2023-01-13:
     - update github actions : checkout@v3 and setup-python@v4
     - remove "better code" badges
     - remove python 3.6 tests
     - add python 3.11 tests
```

### Comparing `pct_python_default_test-1.0.3/pct_python_default_test.egg-info/SOURCES.txt` & `pct_python_default_test-1.0.4/pct_python_default_test.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 pct_python_default_test/py.typed
 pct_python_default_test.egg-info/PKG-INFO
 pct_python_default_test.egg-info/SOURCES.txt
 pct_python_default_test.egg-info/dependency_links.txt
 pct_python_default_test.egg-info/entry_points.txt
 pct_python_default_test.egg-info/not-zip-safe
 pct_python_default_test.egg-info/requires.txt
-pct_python_default_test.egg-info/top_level.txt
+pct_python_default_test.egg-info/top_level.txt
+tests/test_cli.py
```

### Comparing `pct_python_default_test-1.0.3/setup.cfg` & `pct_python_default_test-1.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pct_python_default_test-1.0.3/setup.py` & `pct_python_default_test-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pathlib
 from typing import Any, List, Dict
 
 from setuptools import setup  # type: ignore
 from setuptools import find_packages
 
 
-def is_travis_deploy() -> bool:
+def is_deploy() -> bool:
     if os.getenv("DEPLOY_SDIST", "") or os.getenv("DEPLOY_WHEEL", ""):
         return is_tagged_commit()
     else:
         return False
 
 
 def is_tagged_commit() -> bool:
@@ -73,22 +73,22 @@
 
 
 tests_require = get_requirements_from_file("requirements_test.txt")
 install_requires = get_requirements_from_file("requirements.txt")
 setup_requires = list(set(tests_require + install_requires))
 
 # for deploy on pypi we must not rely on imports from github
-if is_travis_deploy() and is_tagged_commit():
+if is_deploy() and is_tagged_commit():
     setup_requires = strip_links_from_required(setup_requires)
     tests_require = strip_links_from_required(tests_require)
     install_requires = strip_links_from_required(install_requires)
 
 setup_kwargs: Dict[str, Any] = dict()
 setup_kwargs["name"] = "pct_python_default_test"
-setup_kwargs["version"] = "v1.0.3"
+setup_kwargs["version"] = "v1.0.4"
 setup_kwargs["url"] = "https://github.com/bitranox/pct_python_default_test"
 setup_kwargs["packages"] = find_packages()
 setup_kwargs["package_data"] = {"pct_python_default_test": ["py.typed", "*.pyi", "__init__.pyi"]}
 setup_kwargs["description"] = "a pizzacutter default test project, crated with PizzaCutter and the PizzaCutter default python template"
 setup_kwargs["long_description"] = long_description
 setup_kwargs["long_description_content_type"] = "text/x-rst"
 setup_kwargs["author"] = "Robert Nowotny"
```

