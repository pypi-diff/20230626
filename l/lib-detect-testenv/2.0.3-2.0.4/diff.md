# Comparing `tmp/lib_detect_testenv-2.0.3.tar.gz` & `tmp/lib_detect_testenv-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_detect_testenv-2.0.3.tar", last modified: Thu Jan 12 23:45:50 2023, max compression
+gzip compressed data, was "lib_detect_testenv-2.0.4.tar", last modified: Mon Jun 26 20:04:01 2023, max compression
```

## Comparing `lib_detect_testenv-2.0.3.tar` & `lib_detect_testenv-2.0.4.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:45:50.702648 lib_detect_testenv-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-01-12 23:45:14.000000 lib_detect_testenv-2.0.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-01-12 23:45:14.000000 lib_detect_testenv-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-12 23:45:14.000000 lib_detect_testenv-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-01-12 23:45:50.702648 lib_detect_testenv-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-01-12 23:45:14.000000 lib_detect_testenv-2.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:45:50.698648 lib_detect_testenv-2.0.3/lib_detect_testenv/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-01-12 23:45:14.000000 lib_detect_testenv-2.0.3/lib_detect_testenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-01-12 23:45:14.000000 lib_detect_testenv-2.0.3/lib_detect_testenv/__init__conf__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-01-12 23:45:14.000000 lib_detect_testenv-2.0.3/lib_detect_testenv/lib_detect_testenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-01-12 23:45:14.000000 lib_detect_testenv-2.0.3/lib_detect_testenv/lib_detect_testenv_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 23:45:14.000000 lib_detect_testenv-2.0.3/lib_detect_testenv/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 23:45:50.698648 lib_detect_testenv-2.0.3/lib_detect_testenv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-01-12 23:45:50.000000 lib_detect_testenv-2.0.3/lib_detect_testenv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-01-12 23:45:50.000000 lib_detect_testenv-2.0.3/lib_detect_testenv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 23:45:50.000000 lib_detect_testenv-2.0.3/lib_detect_testenv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-12 23:45:50.000000 lib_detect_testenv-2.0.3/lib_detect_testenv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 23:45:50.000000 lib_detect_testenv-2.0.3/lib_detect_testenv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-12 23:45:50.000000 lib_detect_testenv-2.0.3/lib_detect_testenv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-12 23:45:50.000000 lib_detect_testenv-2.0.3/lib_detect_testenv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-01-12 23:45:14.000000 lib_detect_testenv-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-01-12 23:45:50.702648 lib_detect_testenv-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-01-12 23:45:14.000000 lib_detect_testenv-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:04:01.439535 lib_detect_testenv-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-06-26 20:04:01.439535 lib_detect_testenv-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10892 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:04:01.435535 lib_detect_testenv-2.0.4/lib_detect_testenv/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/lib_detect_testenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/lib_detect_testenv/__init__conf__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/lib_detect_testenv/lib_detect_testenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/lib_detect_testenv/lib_detect_testenv_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/lib_detect_testenv/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:04:01.435535 lib_detect_testenv-2.0.4/lib_detect_testenv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-06-26 20:04:01.000000 lib_detect_testenv-2.0.4/lib_detect_testenv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-26 20:04:01.000000 lib_detect_testenv-2.0.4/lib_detect_testenv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:04:01.000000 lib_detect_testenv-2.0.4/lib_detect_testenv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 20:04:01.000000 lib_detect_testenv-2.0.4/lib_detect_testenv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 20:04:01.000000 lib_detect_testenv-2.0.4/lib_detect_testenv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 20:04:01.000000 lib_detect_testenv-2.0.4/lib_detect_testenv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 20:04:01.000000 lib_detect_testenv-2.0.4/lib_detect_testenv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-26 20:04:01.439535 lib_detect_testenv-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 20:04:01.435535 lib_detect_testenv-2.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-26 20:03:23.000000 lib_detect_testenv-2.0.4/tests/test_cli.py
```

### Comparing `lib_detect_testenv-2.0.3/CHANGES.rst` & `lib_detect_testenv-2.0.4/CHANGES.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.4
+---------
+2023-06-26: suppress upload of .egg files to pypi.org
+
 v2.0.3
 ---------
 2023-01-13:
     - update github actions : checkout@v3 and setup-python@v4
     - remove "better code" badges
     - remove python 3.6 tests
     - add python 3.11 tests
```

### Comparing `lib_detect_testenv-2.0.3/LICENSE` & `lib_detect_testenv-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.3/PKG-INFO` & `lib_detect_testenv-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: lib_detect_testenv
-Version: 2.0.3
+Version: 2.0.4
 Summary: detects if pytest or doctest or pyrunner on pycharm is running
 Home-page: https://github.com/bitranox/lib_detect_testenv
 Author: Robert Nowotny
 Author-email: bitranox@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 lib_detect_testenv
 ==================
 
 
-Version v2.0.3 as of 2023-01-13 see `Changelog`_
+Version v2.0.4 as of 2023-06-26 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -70,17 +70,17 @@
 detects test environments: pytest, doctest and pycharm docrunner
 
 ----
 
 automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.7.0 or newer
 
-tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
 `100% code coverage <https://codecov.io/gh/bitranox/lib_detect_testenv>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -401,14 +401,18 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.4
+---------
+2023-06-26: suppress upload of .egg files to pypi.org
+
 v2.0.3
 ---------
 2023-01-13:
     - update github actions : checkout@v3 and setup-python@v4
     - remove "better code" badges
     - remove python 3.6 tests
     - add python 3.11 tests
```

### Comparing `lib_detect_testenv-2.0.3/README.rst` & `lib_detect_testenv-2.0.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 lib_detect_testenv
 ==================
 
 
-Version v2.0.3 as of 2023-01-13 see `Changelog`_
+Version v2.0.4 as of 2023-06-26 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -52,17 +52,17 @@
 detects test environments: pytest, doctest and pycharm docrunner
 
 ----
 
 automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.7.0 or newer
 
-tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
 `100% code coverage <https://codecov.io/gh/bitranox/lib_detect_testenv>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -383,14 +383,18 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.4
+---------
+2023-06-26: suppress upload of .egg files to pypi.org
+
 v2.0.3
 ---------
 2023-01-13:
     - update github actions : checkout@v3 and setup-python@v4
     - remove "better code" badges
     - remove python 3.6 tests
     - add python 3.11 tests
```

### Comparing `lib_detect_testenv-2.0.3/lib_detect_testenv/__init__.py` & `lib_detect_testenv-2.0.4/lib_detect_testenv/__init__.py`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.3/lib_detect_testenv/lib_detect_testenv.py` & `lib_detect_testenv-2.0.4/lib_detect_testenv/lib_detect_testenv.py`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.3/lib_detect_testenv/lib_detect_testenv_cli.py` & `lib_detect_testenv-2.0.4/lib_detect_testenv/lib_detect_testenv_cli.py`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.3/lib_detect_testenv.egg-info/PKG-INFO` & `lib_detect_testenv-2.0.4/lib_detect_testenv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: lib-detect-testenv
-Version: 2.0.3
+Version: 2.0.4
 Summary: detects if pytest or doctest or pyrunner on pycharm is running
 Home-page: https://github.com/bitranox/lib_detect_testenv
 Author: Robert Nowotny
 Author-email: bitranox@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 lib_detect_testenv
 ==================
 
 
-Version v2.0.3 as of 2023-01-13 see `Changelog`_
+Version v2.0.4 as of 2023-06-26 see `Changelog`_
 
 |build_badge| |license| |jupyter| |pypi| |pypi-downloads| |black|
 
 |codecov| |cc_maintain| |cc_issues| |cc_coverage| |snyk|
 
 
 
@@ -70,17 +70,17 @@
 detects test environments: pytest, doctest and pycharm docrunner
 
 ----
 
 automated tests, Travis Matrix, Documentation, Badges, etc. are managed with `PizzaCutter <https://github
 .com/bitranox/PizzaCutter>`_ (cookiecutter on steroids)
 
-Python version required: 3.6.0 or newer
+Python version required: 3.7.0 or newer
 
-tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.8 - architectures: amd64
+tested on recent linux with python 3.7, 3.8, 3.9, 3.10, 3.11, pypy-3.9 - architectures: amd64
 
 `100% code coverage <https://codecov.io/gh/bitranox/lib_detect_testenv>`_, flake8 style checking ,mypy static type checking ,tested under `Linux, macOS, Windows <https://github.com/bitranox/lib_detect_testenv/actions/workflows/python-package.yml>`_, automatic daily builds and monitoring
 
 ----
 
 - `Try it Online`_
 - `Usage`_
@@ -401,14 +401,18 @@
 Changelog
 =========
 
 - new MAJOR version for incompatible API changes,
 - new MINOR version for added functionality in a backwards compatible manner
 - new PATCH version for backwards compatible bug fixes
 
+v2.0.4
+---------
+2023-06-26: suppress upload of .egg files to pypi.org
+
 v2.0.3
 ---------
 2023-01-13:
     - update github actions : checkout@v3 and setup-python@v4
     - remove "better code" badges
     - remove python 3.6 tests
     - add python 3.11 tests
```

### Comparing `lib_detect_testenv-2.0.3/lib_detect_testenv.egg-info/SOURCES.txt` & `lib_detect_testenv-2.0.4/lib_detect_testenv.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 lib_detect_testenv/py.typed
 lib_detect_testenv.egg-info/PKG-INFO
 lib_detect_testenv.egg-info/SOURCES.txt
 lib_detect_testenv.egg-info/dependency_links.txt
 lib_detect_testenv.egg-info/entry_points.txt
 lib_detect_testenv.egg-info/not-zip-safe
 lib_detect_testenv.egg-info/requires.txt
-lib_detect_testenv.egg-info/top_level.txt
+lib_detect_testenv.egg-info/top_level.txt
+tests/test_cli.py
```

### Comparing `lib_detect_testenv-2.0.3/setup.cfg` & `lib_detect_testenv-2.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `lib_detect_testenv-2.0.3/setup.py` & `lib_detect_testenv-2.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 if is_travis_deploy() and is_tagged_commit():
     setup_requires = strip_links_from_required(setup_requires)
     tests_require = strip_links_from_required(tests_require)
     install_requires = strip_links_from_required(install_requires)
 
 setup_kwargs: Dict[str, Any] = dict()
 setup_kwargs["name"] = "lib_detect_testenv"
-setup_kwargs["version"] = "v2.0.3"
+setup_kwargs["version"] = "v2.0.4"
 setup_kwargs["url"] = "https://github.com/bitranox/lib_detect_testenv"
 setup_kwargs["packages"] = find_packages()
 setup_kwargs["package_data"] = {"lib_detect_testenv": ["py.typed", "*.pyi", "__init__.pyi"]}
 setup_kwargs["description"] = "detects if pytest or doctest or pyrunner on pycharm is running"
 setup_kwargs["long_description"] = long_description
 setup_kwargs["long_description_content_type"] = "text/x-rst"
 setup_kwargs["author"] = "Robert Nowotny"
@@ -106,13 +106,13 @@
 # minimally needs to run tests - no project requirements here
 setup_kwargs["tests_require"] = tests_require
 # specify what a project minimally needs to run correctly
 setup_kwargs["install_requires"] = install_requires
 # minimally needs to run the setup script, dependencies needs also to put here for "setup.py install test"
 # dependencies must not be put here for pip install
 setup_kwargs["setup_requires"] = setup_requires
-setup_kwargs["python_requires"] = ">=3.6.0"
+setup_kwargs["python_requires"] = ">=3.7.0"
 setup_kwargs["zip_safe"] = False
 
 
 if __name__ == "__main__":
     setup(**setup_kwargs)
```

