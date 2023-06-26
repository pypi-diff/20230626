# Comparing `tmp/pytest-enabler-2.1.1.tar.gz` & `tmp/pytest-enabler-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-enabler-2.1.1.tar", last modified: Fri May 12 21:28:15 2023, max compression
+gzip compressed data, was "pytest-enabler-2.2.0.tar", last modified: Mon Jun 26 02:26:47 2023, max compression
```

## Comparing `pytest-enabler-2.1.1.tar` & `pytest-enabler-2.2.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:28:15.444024 pytest-enabler-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:28:15.444024 pytest-enabler-2.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:28:15.444024 pytest-enabler-2.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-12 21:28:15.444024 pytest-enabler-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:28:15.444024 pytest-enabler-2.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:28:15.444024 pytest-enabler-2.1.1/pytest_enabler/
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/pytest_enabler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:28:15.444024 pytest-enabler-2.1.1/pytest_enabler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-12 21:28:15.000000 pytest-enabler-2.1.1/pytest_enabler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-12 21:28:15.000000 pytest-enabler-2.1.1/pytest_enabler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 21:28:15.000000 pytest-enabler-2.1.1/pytest_enabler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-12 21:28:15.000000 pytest-enabler-2.1.1/pytest_enabler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-12 21:28:15.000000 pytest-enabler-2.1.1/pytest_enabler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-12 21:28:15.000000 pytest-enabler-2.1.1/pytest_enabler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-12 21:28:15.444024 pytest-enabler-2.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:28:15.444024 pytest-enabler-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/tests/test_enabler.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-12 21:27:55.000000 pytest-enabler-2.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:26:47.850073 pytest-enabler-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:26:47.846073 pytest-enabler-2.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:26:47.846073 pytest-enabler-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-26 02:26:47.850073 pytest-enabler-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:26:47.846073 pytest-enabler-2.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:26:47.846073 pytest-enabler-2.2.0/pytest_enabler/
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/pytest_enabler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/pytest_enabler/default.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:26:47.850073 pytest-enabler-2.2.0/pytest_enabler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-26 02:26:47.000000 pytest-enabler-2.2.0/pytest_enabler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-26 02:26:47.000000 pytest-enabler-2.2.0/pytest_enabler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 02:26:47.000000 pytest-enabler-2.2.0/pytest_enabler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 02:26:47.000000 pytest-enabler-2.2.0/pytest_enabler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-26 02:26:47.000000 pytest-enabler-2.2.0/pytest_enabler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 02:26:47.000000 pytest-enabler-2.2.0/pytest_enabler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-26 02:26:47.850073 pytest-enabler-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 02:26:47.850073 pytest-enabler-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/tests/test_enabler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-26 02:26:25.000000 pytest-enabler-2.2.0/tox.ini
```

### Comparing `pytest-enabler-2.1.1/.github/workflows/main.yml` & `pytest-enabler-2.2.0/.github/workflows/main.yml`

 * *Files 8% similar despite different names*

```diff
@@ -38,27 +38,22 @@
 
 
 jobs:
   test:
     strategy:
       matrix:
         python:
-        - "3.7"
+        - "3.8"
         - "3.11"
         - "3.12"
-        # Workaround for actions/setup-python#508
-        dev:
-        - -dev
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
-        - python: "3.8"
-          platform: ubuntu-latest
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
         - python: pypy3.9
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
@@ -68,31 +63,30 @@
         with:
           # fetch all branches and tags (to get tags for versioning)
           # ref actions/checkout#448
           fetch-depth: 0
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
+          python-version: ${{ matrix.python }}
+          allow-prereleases: true
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Run tests
         run: tox
 
   docs:
     runs-on: ubuntu-latest
     env:
       TOXENV: docs
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
-        with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Run tests
         run: tox
 
   check:  # This job does nothing and is only used for the branch protection
```

### Comparing `pytest-enabler-2.1.1/LICENSE` & `pytest-enabler-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-enabler-2.1.1/PKG-INFO` & `pytest-enabler-2.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 Metadata-Version: 2.1
 Name: pytest-enabler
-Version: 2.1.1
+Version: 2.2.0
 Summary: Enable installed pytest plugins
 Home-page: https://github.com/jaraco/pytest-enabler
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Pytest
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/pytest-enabler.svg
    :target: https://pypi.org/project/pytest-enabler
 
 .. image:: https://img.shields.io/pypi/pyversions/pytest-enabler.svg
 
 .. image:: https://github.com/jaraco/pytest-enabler/workflows/tests/badge.svg
    :target: https://github.com/jaraco/pytest-enabler/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
-The 'enabler' plugin allows configuration of plugins if present, but omits the settings if the plugin is not present. For example, to configure black to be enabled if the plugin is present, but not when it is not, add the following to your pyproject.toml::
+The ``enabler`` plugin allows configuration of plugins if present, but omits the settings if the plugin is not present. For example, the following config enables black to be enabled when present::
 
     [tool.pytest-enabler.black]
     addopts = "--black"
 
 Then, to temporarily disable a plugin, use pytest's built-in support for disabling a plugin::
 
     pytest -p no:black
 
+``enabler`` includes a `default config <https://github.com/jaraco/pytest-enabler/blob/main/pytest_enabler/default.toml>`_.
+
 Known to work with the following plugins:
 
 - pytest-black
 - pytest-cov
 - pytest-flake8
 - pytest-mypy
 - pytest-ruff
```

### Comparing `pytest-enabler-2.1.1/docs/conf.py` & `pytest-enabler-2.2.0/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 master_doc = "index"
 html_theme = "furo"
 
 # Link dates and other references in the changelog
 extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
```

### Comparing `pytest-enabler-2.1.1/pytest.ini` & `pytest-enabler-2.2.0/pytest.ini`

 * *Files 9% similar despite different names*

```diff
@@ -17,8 +17,11 @@
 
 	# realpython/pytest-mypy#152
 	ignore:'encoding' argument not specified::pytest_mypy
 
 	# python/cpython#100750
 	ignore:'encoding' argument not specified::platform
 
+	# pypa/build#615
+	ignore:'encoding' argument not specified::build.env
+
 	## end upstream
```

### Comparing `pytest-enabler-2.1.1/pytest_enabler/__init__.py` & `pytest-enabler-2.2.0/pytest_enabler/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import contextlib
+import pathlib
 import shlex
 import sys
 
+import importlib_resources as resources
+
 import toml
 from jaraco.context import suppress
 from jaraco.functools import apply
 
 
 def none_as_empty(ob):
     """
@@ -15,24 +18,31 @@
     {}
     >>> none_as_empty({'a': 1})
     {'a': 1}
     """
     return ob or {}
 
 
+def read_plugins_stream(stream):
+    defn = toml.load(stream)
+    return defn["tool"]["pytest-enabler"]
+
+
 @apply(none_as_empty)
 @suppress(Exception)
-def read_plugins(filename):
-    with open(filename, encoding='utf-8') as strm:
-        defn = toml.load(strm)
-    return defn["tool"]["pytest-enabler"]
+def read_plugins(path):
+    with path.open(encoding='utf-8') as stream:
+        return read_plugins_stream(stream)
 
 
 def pytest_load_initial_conftests(early_config, parser, args):
-    plugins = read_plugins('pyproject.toml')
+    plugins = {
+        **read_plugins(resources.files().joinpath('default.toml')),
+        **read_plugins(pathlib.Path('pyproject.toml')),
+    }
 
     def _has_plugin(name):
         pm = early_config.pluginmanager
         return pm.has_plugin(name) or pm.has_plugin('pytest_' + name)
 
     enabled = {key: plugins[key] for key in plugins if _has_plugin(key)}
     for plugin in enabled.values():
```

### Comparing `pytest-enabler-2.1.1/pytest_enabler.egg-info/PKG-INFO` & `pytest-enabler-2.2.0/pytest_enabler.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 Metadata-Version: 2.1
 Name: pytest-enabler
-Version: 2.1.1
+Version: 2.2.0
 Summary: Enable installed pytest plugins
 Home-page: https://github.com/jaraco/pytest-enabler
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Pytest
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/pytest-enabler.svg
    :target: https://pypi.org/project/pytest-enabler
 
 .. image:: https://img.shields.io/pypi/pyversions/pytest-enabler.svg
 
 .. image:: https://github.com/jaraco/pytest-enabler/workflows/tests/badge.svg
    :target: https://github.com/jaraco/pytest-enabler/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
-.. .. image:: https://readthedocs.org/projects/skeleton/badge/?version=latest
-..    :target: https://skeleton.readthedocs.io/en/latest/?badge=latest
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/skeleton-2023-informational
    :target: https://blog.jaraco.com/skeleton
 
-The 'enabler' plugin allows configuration of plugins if present, but omits the settings if the plugin is not present. For example, to configure black to be enabled if the plugin is present, but not when it is not, add the following to your pyproject.toml::
+The ``enabler`` plugin allows configuration of plugins if present, but omits the settings if the plugin is not present. For example, the following config enables black to be enabled when present::
 
     [tool.pytest-enabler.black]
     addopts = "--black"
 
 Then, to temporarily disable a plugin, use pytest's built-in support for disabling a plugin::
 
     pytest -p no:black
 
+``enabler`` includes a `default config <https://github.com/jaraco/pytest-enabler/blob/main/pytest_enabler/default.toml>`_.
+
 Known to work with the following plugins:
 
 - pytest-black
 - pytest-cov
 - pytest-flake8
 - pytest-mypy
 - pytest-ruff
```

### Comparing `pytest-enabler-2.1.1/pytest_enabler.egg-info/SOURCES.txt` & `pytest-enabler-2.2.0/pytest_enabler.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 .coveragerc
 .editorconfig
 .pre-commit-config.yaml
 .readthedocs.yaml
-CHANGES.rst
 LICENSE
+NEWS.rst
 README.rst
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
+towncrier.toml
 tox.ini
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
 pytest_enabler/__init__.py
+pytest_enabler/default.toml
 pytest_enabler.egg-info/PKG-INFO
 pytest_enabler.egg-info/SOURCES.txt
 pytest_enabler.egg-info/dependency_links.txt
 pytest_enabler.egg-info/entry_points.txt
 pytest_enabler.egg-info/requires.txt
 pytest_enabler.egg-info/top_level.txt
 tests/test_enabler.py
```

### Comparing `pytest-enabler-2.1.1/setup.cfg` & `pytest-enabler-2.2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Framework :: Pytest
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	toml
 	jaraco.functools
 	jaraco.context
+	importlib_resources >= 5.10
 
 [options.packages.find]
 exclude = 
 	build*
 	dist*
 	docs*
 	tests*
```

### Comparing `pytest-enabler-2.1.1/tox.ini` & `pytest-enabler-2.2.0/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 [tox]
-envlist = python
-minversion = 3.2
-# https://github.com/jaraco/skeleton/issues/6
-tox_pip_extensions_ext_venv_update = true
 toxworkdir={env:TOX_WORK_DIR:.tox}
 
 
 [testenv]
 deps =
 setenv =
 	PYTHONWARNDEFAULTENCODING = 1
@@ -21,14 +17,24 @@
 	docs
 	testing
 changedir = docs
 commands =
 	python -m sphinx -W --keep-going . {toxinidir}/build/html
 	python -m sphinxlint
 
+[testenv:finalize]
+skip_install = True
+deps =
+	towncrier
+	jaraco.develop >= 7.23
+passenv = *
+commands =
+	python -m jaraco.develop.finalize
+
+
 [testenv:release]
 skip_install = True
 deps =
 	build
 	twine>=3
 	jaraco.develop>=7.1
 passenv =
```

