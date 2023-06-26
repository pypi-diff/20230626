# Comparing `tmp/gwlandscape-python-0.3.2.tar.gz` & `tmp/gwlandscape_python-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwlandscape-python-0.3.2.tar", max compression
+gzip compressed data, was "gwlandscape_python-0.3.3.tar", max compression
```

## Comparing `gwlandscape-python-0.3.2.tar` & `gwlandscape_python-0.3.3.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1076 2022-08-25 03:57:12.620934 gwlandscape-python-0.3.2/LICENSE
--rw-r--r--   0        0        0      524 2023-03-27 03:08:09.587795 gwlandscape-python-0.3.2/README.rst
--rw-r--r--   0        0        0      342 2022-08-31 08:22:19.506487 gwlandscape-python-0.3.2/gwlandscape_python/__init__.py
--rw-r--r--   0        0        0     2170 2023-04-26 23:39:52.338808 gwlandscape-python-0.3.2/gwlandscape_python/dataset_type.py
--rw-r--r--   0        0        0    17552 2023-04-21 06:22:03.415309 gwlandscape-python-0.3.2/gwlandscape_python/gwlandscape.py
--rw-r--r--   0        0        0     1608 2023-04-26 23:39:52.338808 gwlandscape-python-0.3.2/gwlandscape_python/keyword_type.py
--rw-r--r--   0        0        0     1920 2023-04-26 23:39:52.338808 gwlandscape-python-0.3.2/gwlandscape_python/model_type.py
--rw-r--r--   0        0        0     3801 2023-04-26 23:39:52.338808 gwlandscape-python-0.3.2/gwlandscape_python/publication_type.py
--rw-r--r--   0        0        0      227 2022-08-31 07:40:02.705327 gwlandscape-python-0.3.2/gwlandscape_python/settings.py
--rw-r--r--   0        0        0        0 2022-08-25 03:57:12.624934 gwlandscape-python-0.3.2/gwlandscape_python/tests/__init__.py
--rw-r--r--   0        0        0     5874 2023-04-26 23:39:52.338808 gwlandscape-python-0.3.2/gwlandscape_python/tests/conftest.py
--rw-r--r--   0        0        0     2657 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.2/gwlandscape_python/tests/test_dataset_type.py
--rw-r--r--   0        0        0    16979 2023-04-26 23:39:52.338808 gwlandscape-python-0.3.2/gwlandscape_python/tests/test_gwlandscape_python.py
--rw-r--r--   0        0        0     2234 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.2/gwlandscape_python/tests/test_keyword_type.py
--rw-r--r--   0        0        0     2290 2023-04-20 04:41:39.756269 gwlandscape-python-0.3.2/gwlandscape_python/tests/test_model_type.py
--rw-r--r--   0        0        0     3938 2023-04-26 23:39:52.338808 gwlandscape-python-0.3.2/gwlandscape_python/tests/test_publication_type.py
--rw-r--r--   0        0        0      152 2022-08-25 03:57:12.624934 gwlandscape-python-0.3.2/gwlandscape_python/tests/utils.py
--rw-r--r--   0        0        0       54 2022-08-31 07:40:02.709327 gwlandscape-python-0.3.2/gwlandscape_python/utils/__init__.py
--rw-r--r--   0        0        0     4075 2022-08-31 07:40:02.709327 gwlandscape-python-0.3.2/gwlandscape_python/utils/tests/test_utils.py
--rw-r--r--   0        0        0     1357 2022-08-31 07:40:02.713327 gwlandscape-python-0.3.2/gwlandscape_python/utils/utils.py
--rw-r--r--   0        0        0     1074 2023-04-26 23:39:52.338808 gwlandscape-python-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1661 2023-04-27 00:55:40.483421 gwlandscape-python-0.3.2/setup.py
--rw-r--r--   0        0        0     1618 2023-04-27 00:55:40.483638 gwlandscape-python-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-08-25 03:57:12.620934 gwlandscape_python-0.3.3/LICENSE
+-rw-r--r--   0        0        0      524 2023-03-27 03:08:09.587795 gwlandscape_python-0.3.3/README.rst
+-rw-r--r--   0        0        0      342 2022-08-31 08:22:19.506487 gwlandscape_python-0.3.3/gwlandscape_python/__init__.py
+-rw-r--r--   0        0        0     2170 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.3/gwlandscape_python/dataset_type.py
+-rw-r--r--   0        0        0    17552 2023-04-21 06:22:03.415309 gwlandscape_python-0.3.3/gwlandscape_python/gwlandscape.py
+-rw-r--r--   0        0        0     1608 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.3/gwlandscape_python/keyword_type.py
+-rw-r--r--   0        0        0     1920 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.3/gwlandscape_python/model_type.py
+-rw-r--r--   0        0        0     3801 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.3/gwlandscape_python/publication_type.py
+-rw-r--r--   0        0        0      227 2022-08-31 07:40:02.705327 gwlandscape_python-0.3.3/gwlandscape_python/settings.py
+-rw-r--r--   0        0        0        0 2022-08-25 03:57:12.624934 gwlandscape_python-0.3.3/gwlandscape_python/tests/__init__.py
+-rw-r--r--   0        0        0     5874 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.3/gwlandscape_python/tests/conftest.py
+-rw-r--r--   0        0        0     2657 2023-04-20 04:41:39.756269 gwlandscape_python-0.3.3/gwlandscape_python/tests/test_dataset_type.py
+-rw-r--r--   0        0        0    16979 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.3/gwlandscape_python/tests/test_gwlandscape_python.py
+-rw-r--r--   0        0        0     2234 2023-04-20 04:41:39.756269 gwlandscape_python-0.3.3/gwlandscape_python/tests/test_keyword_type.py
+-rw-r--r--   0        0        0     2290 2023-04-20 04:41:39.756269 gwlandscape_python-0.3.3/gwlandscape_python/tests/test_model_type.py
+-rw-r--r--   0        0        0     3938 2023-04-26 23:39:52.338808 gwlandscape_python-0.3.3/gwlandscape_python/tests/test_publication_type.py
+-rw-r--r--   0        0        0      152 2022-08-25 03:57:12.624934 gwlandscape_python-0.3.3/gwlandscape_python/tests/utils.py
+-rw-r--r--   0        0        0       54 2022-08-31 07:40:02.709327 gwlandscape_python-0.3.3/gwlandscape_python/utils/__init__.py
+-rw-r--r--   0        0        0     4075 2022-08-31 07:40:02.709327 gwlandscape_python-0.3.3/gwlandscape_python/utils/tests/test_utils.py
+-rw-r--r--   0        0        0     1357 2022-08-31 07:40:02.713327 gwlandscape_python-0.3.3/gwlandscape_python/utils/utils.py
+-rw-r--r--   0        0        0     1074 2023-06-26 02:45:08.714202 gwlandscape_python-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1722 1970-01-01 00:00:00.000000 gwlandscape_python-0.3.3/PKG-INFO
```

### Comparing `gwlandscape-python-0.3.2/LICENSE` & `gwlandscape_python-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.2/README.rst` & `gwlandscape_python-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.2/gwlandscape_python/dataset_type.py` & `gwlandscape_python-0.3.3/gwlandscape_python/dataset_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.2/gwlandscape_python/gwlandscape.py` & `gwlandscape_python-0.3.3/gwlandscape_python/gwlandscape.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.2/gwlandscape_python/keyword_type.py` & `gwlandscape_python-0.3.3/gwlandscape_python/keyword_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.2/gwlandscape_python/model_type.py` & `gwlandscape_python-0.3.3/gwlandscape_python/model_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.2/gwlandscape_python/publication_type.py` & `gwlandscape_python-0.3.3/gwlandscape_python/publication_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.2/gwlandscape_python/tests/conftest.py` & `gwlandscape_python-0.3.3/gwlandscape_python/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.2/gwlandscape_python/tests/test_dataset_type.py` & `gwlandscape_python-0.3.3/gwlandscape_python/tests/test_dataset_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.2/gwlandscape_python/tests/test_gwlandscape_python.py` & `gwlandscape_python-0.3.3/gwlandscape_python/tests/test_gwlandscape_python.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.2/gwlandscape_python/tests/test_keyword_type.py` & `gwlandscape_python-0.3.3/gwlandscape_python/tests/test_keyword_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.2/gwlandscape_python/tests/test_model_type.py` & `gwlandscape_python-0.3.3/gwlandscape_python/tests/test_model_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.2/gwlandscape_python/tests/test_publication_type.py` & `gwlandscape_python-0.3.3/gwlandscape_python/tests/test_publication_type.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.2/gwlandscape_python/utils/tests/test_utils.py` & `gwlandscape_python-0.3.3/gwlandscape_python/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.2/gwlandscape_python/utils/utils.py` & `gwlandscape_python-0.3.3/gwlandscape_python/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gwlandscape-python-0.3.2/pyproject.toml` & `gwlandscape_python-0.3.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "gwlandscape-python"
-version = "0.3.2"
+version = "0.3.3"
 description = "Wrapper of GWDC API, used for interacting with the GWLandscape endpoints"
 authors = ["Thomas Reichardt <treichardt@swin.edu.au>", "Lewis Lakerink <llakerink@swin.edu.au"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/gravitationalwavedc/gwlandscape_python"
 include = ["LICENSE",]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-gwdc-python = "^0.4.1"
+gwdc-python = "^0.6.0"
 requests = "^2.25.1"
 jwt = "^1.2.0"
 graphene-file-upload = "^1.3.0"
 importlib-metadata = "^4.5.0"
 Sphinx = {version = "^4.0.2", optional = true}
 sphinx-rtd-theme = {version = "^0.5.2", optional = true}
 tqdm = "^4.61.2"
```

### Comparing `gwlandscape-python-0.3.2/setup.py` & `gwlandscape_python-0.3.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,54 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: gwlandscape-python
+Version: 0.3.3
+Summary: Wrapper of GWDC API, used for interacting with the GWLandscape endpoints
+Home-page: https://github.com/gravitationalwavedc/gwlandscape_python
+License: MIT
+Author: Thomas Reichardt
+Author-email: treichardt@swin.edu.au
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: docs
+Requires-Dist: Sphinx (>=4.0.2,<5.0.0) ; extra == "docs"
+Requires-Dist: graphene-file-upload (>=1.3.0,<2.0.0)
+Requires-Dist: gwdc-python (>=0.6.0,<0.7.0)
+Requires-Dist: importlib-metadata (>=4.5.0,<5.0.0)
+Requires-Dist: jwt (>=1.2.0,<2.0.0)
+Requires-Dist: requests (>=2.25.1,<3.0.0)
+Requires-Dist: sphinx-rtd-theme (>=0.5.2,<0.6.0) ; extra == "docs"
+Requires-Dist: tqdm (>=4.61.2,<5.0.0)
+Project-URL: Repository, https://github.com/gravitationalwavedc/gwlandscape_python
+Description-Content-Type: text/x-rst
+
+GWLandscape Python API
+======================
+
+`GWLandscape <https://gwlandscape.org.au/>`_ is a service used to handle both the submission of COMPAS jobs (todo)
+
+Check out the `documentation <https://gwlandscape-python.readthedocs.io/en/latest/>`_ for more information.
+
+Installation
+------------
+
+The gwlandscape-python package can be installed with
+
+::
+
+    pip install gwlandscape-python
 
-packages = \
-['gwlandscape_python',
- 'gwlandscape_python.tests',
- 'gwlandscape_python.utils',
- 'gwlandscape_python.utils.tests']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['graphene-file-upload>=1.3.0,<2.0.0',
- 'gwdc-python>=0.4.1,<0.5.0',
- 'importlib-metadata>=4.5.0,<5.0.0',
- 'jwt>=1.2.0,<2.0.0',
- 'requests>=2.25.1,<3.0.0',
- 'tqdm>=4.61.2,<5.0.0']
-
-extras_require = \
-{'docs': ['Sphinx>=4.0.2,<5.0.0', 'sphinx-rtd-theme>=0.5.2,<0.6.0']}
-
-setup_kwargs = {
-    'name': 'gwlandscape-python',
-    'version': '0.3.2',
-    'description': 'Wrapper of GWDC API, used for interacting with the GWLandscape endpoints',
-    'long_description': "GWLandscape Python API\n======================\n\n`GWLandscape <https://gwlandscape.org.au/>`_ is a service used to handle both the submission of COMPAS jobs (todo)\n\nCheck out the `documentation <https://gwlandscape-python.readthedocs.io/en/latest/>`_ for more information.\n\nInstallation\n------------\n\nThe gwlandscape-python package can be installed with\n\n::\n\n    pip install gwlandscape-python\n\n\nExample\n-------\n\n::\n\n    >>> from gwlandscape_python import GWLandscape\n    >>> gwl = GWLandscape(token='<user_api_token_here>')\n\n",
-    'author': 'Thomas Reichardt',
-    'author_email': 'treichardt@swin.edu.au',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/gravitationalwavedc/gwlandscape_python',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
+
+Example
+-------
+
+::
+
+    >>> from gwlandscape_python import GWLandscape
+    >>> gwl = GWLandscape(token='<user_api_token_here>')
 
 
-setup(**setup_kwargs)
```

