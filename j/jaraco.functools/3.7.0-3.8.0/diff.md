# Comparing `tmp/jaraco.functools-3.7.0.tar.gz` & `tmp/jaraco.functools-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.functools-3.7.0.tar", last modified: Mon May 29 08:12:10 2023, max compression
+gzip compressed data, was "jaraco.functools-3.8.0.tar", last modified: Mon Jun 26 01:20:44 2023, max compression
```

## Comparing `jaraco.functools-3.7.0.tar` & `jaraco.functools-3.8.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:12:10.598692 jaraco.functools-3.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:12:10.590692 jaraco.functools-3.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:12:10.590692 jaraco.functools-3.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-29 08:12:10.598692 jaraco.functools-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:12:10.590692 jaraco.functools-3.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:12:10.594692 jaraco.functools-3.7.0/jaraco/
--rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/jaraco/functools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:12:10.598692 jaraco.functools-3.7.0/jaraco.functools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-29 08:12:10.000000 jaraco.functools-3.7.0/jaraco.functools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-29 08:12:10.000000 jaraco.functools-3.7.0/jaraco.functools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:12:10.000000 jaraco.functools-3.7.0/jaraco.functools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-29 08:12:10.000000 jaraco.functools-3.7.0/jaraco.functools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 08:12:10.000000 jaraco.functools-3.7.0/jaraco.functools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 08:12:10.598692 jaraco.functools-3.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/test_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:20:44.024293 jaraco.functools-3.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:20:44.024293 jaraco.functools-3.8.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:20:44.024293 jaraco.functools-3.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-26 01:20:44.024293 jaraco.functools-3.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:20:44.024293 jaraco.functools-3.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:20:44.024293 jaraco.functools-3.8.0/jaraco/
+-rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/jaraco/functools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 01:20:44.024293 jaraco.functools-3.8.0/jaraco.functools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-26 01:20:43.000000 jaraco.functools-3.8.0/jaraco.functools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-26 01:20:44.000000 jaraco.functools-3.8.0/jaraco.functools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 01:20:43.000000 jaraco.functools-3.8.0/jaraco.functools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-26 01:20:43.000000 jaraco.functools-3.8.0/jaraco.functools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 01:20:43.000000 jaraco.functools-3.8.0/jaraco.functools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-26 01:20:44.024293 jaraco.functools-3.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/test_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-26 01:20:18.000000 jaraco.functools-3.8.0/tox.ini
```

### Comparing `jaraco.functools-3.7.0/.github/workflows/main.yml` & `jaraco.functools-3.8.0/.github/workflows/main.yml`

 * *Files 4% similar despite different names*

```diff
@@ -38,57 +38,51 @@
 
 
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
     continue-on-error: ${{ matrix.python == '3.12' }}
     steps:
       - uses: actions/checkout@v3
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

### Comparing `jaraco.functools-3.7.0/CHANGES.rst` & `jaraco.functools-3.8.0/NEWS.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v3.8.0
+======
+
+Features
+--------
+
+- Require Python 3.8 or later.
+
+
 v3.7.0
 ======
 
 Added ``bypass_unless`` and ``bypass_when`` and ``identity``.
 
 v3.6.0
 ======
```

### Comparing `jaraco.functools-3.7.0/LICENSE` & `jaraco.functools-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.functools-3.7.0/PKG-INFO` & `jaraco.functools-3.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: jaraco.functools
-Version: 3.7.0
+Version: 3.8.0
 Summary: Functools like those found in stdlib
 Home-page: https://github.com/jaraco/jaraco.functools
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/jaraco.functools.svg
    :target: https://pypi.org/project/jaraco.functools
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.functools.svg
 
 .. image:: https://github.com/jaraco/jaraco.functools/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.functools/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracofunctools/badge/?version=latest
    :target: https://jaracofunctools.readthedocs.io/en/latest/?badge=latest
```

### Comparing `jaraco.functools-3.7.0/README.rst` & `jaraco.functools-3.8.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.functools.svg
 
 .. image:: https://github.com/jaraco/jaraco.functools/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.functools/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracofunctools/badge/?version=latest
    :target: https://jaracofunctools.readthedocs.io/en/latest/?badge=latest
```

### Comparing `jaraco.functools-3.7.0/conftest.py` & `jaraco.functools-3.8.0/conftest.py`

 * *Files identical despite different names*

### Comparing `jaraco.functools-3.7.0/docs/conf.py` & `jaraco.functools-3.8.0/docs/conf.py`

 * *Files 2% similar despite different names*

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

### Comparing `jaraco.functools-3.7.0/jaraco/functools.py` & `jaraco.functools-3.8.0/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `jaraco.functools-3.7.0/jaraco.functools.egg-info/PKG-INFO` & `jaraco.functools-3.8.0/jaraco.functools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: jaraco.functools
-Version: 3.7.0
+Version: 3.8.0
 Summary: Functools like those found in stdlib
 Home-page: https://github.com/jaraco/jaraco.functools
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/jaraco.functools.svg
    :target: https://pypi.org/project/jaraco.functools
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.functools.svg
 
 .. image:: https://github.com/jaraco/jaraco.functools/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.functools/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracofunctools/badge/?version=latest
    :target: https://jaracofunctools.readthedocs.io/en/latest/?badge=latest
```

### Comparing `jaraco.functools-3.7.0/pytest.ini` & `jaraco.functools-3.8.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco.functools-3.7.0/setup.cfg` & `jaraco.functools-3.8.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	more_itertools
 
 [options.packages.find]
 exclude = 
 	build*
 	dist*
```

### Comparing `jaraco.functools-3.7.0/test_functools.py` & `jaraco.functools-3.8.0/test_functools.py`

 * *Files identical despite different names*

