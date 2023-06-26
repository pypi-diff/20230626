# Comparing `tmp/qurix-data-catalog-0.1.1.tar.gz` & `tmp/qurix-data-catalog-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qurix-data-catalog-0.1.1.tar", last modified: Thu Jun 15 10:42:45 2023, max compression
+gzip compressed data, was "qurix-data-catalog-1.0.0.tar", last modified: Mon Jun 26 16:14:54 2023, max compression
```

## Comparing `qurix-data-catalog-0.1.1.tar` & `qurix-data-catalog-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:42:45.530789 qurix-data-catalog-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-06-15 10:42:18.000000 qurix-data-catalog-0.1.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-15 10:42:45.530789 qurix-data-catalog-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-15 10:42:18.000000 qurix-data-catalog-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:42:45.526789 qurix-data-catalog-0.1.1/qurix/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:42:45.526789 qurix-data-catalog-0.1.1/qurix/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:42:45.530789 qurix-data-catalog-0.1.1/qurix/data/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-15 10:42:18.000000 qurix-data-catalog-0.1.1/qurix/data/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-15 10:42:18.000000 qurix-data-catalog-0.1.1/qurix/data/catalog/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-15 10:42:18.000000 qurix-data-catalog-0.1.1/qurix/data/catalog/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:42:45.530789 qurix-data-catalog-0.1.1/qurix_data_catalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-15 10:42:45.000000 qurix-data-catalog-0.1.1/qurix_data_catalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-15 10:42:45.000000 qurix-data-catalog-0.1.1/qurix_data_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:42:45.000000 qurix-data-catalog-0.1.1/qurix_data_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-15 10:42:45.000000 qurix-data-catalog-0.1.1/qurix_data_catalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 10:42:45.000000 qurix-data-catalog-0.1.1/qurix_data_catalog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 10:42:45.530789 qurix-data-catalog-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-15 10:42:18.000000 qurix-data-catalog-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:42:45.530789 qurix-data-catalog-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:42:18.000000 qurix-data-catalog-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-15 10:42:18.000000 qurix-data-catalog-0.1.1/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:14:54.236944 qurix-data-catalog-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-26 16:14:54.236944 qurix-data-catalog-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-26 16:14:36.000000 qurix-data-catalog-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:14:54.232944 qurix-data-catalog-1.0.0/qurix/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:14:54.232944 qurix-data-catalog-1.0.0/qurix/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:14:54.232944 qurix-data-catalog-1.0.0/qurix/data/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 16:14:36.000000 qurix-data-catalog-1.0.0/qurix/data/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 16:14:36.000000 qurix-data-catalog-1.0.0/qurix/data/catalog/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-26 16:14:36.000000 qurix-data-catalog-1.0.0/qurix/data/catalog/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:14:54.236944 qurix-data-catalog-1.0.0/qurix_data_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-26 16:14:54.000000 qurix-data-catalog-1.0.0/qurix_data_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-26 16:14:54.000000 qurix-data-catalog-1.0.0/qurix_data_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:14:54.000000 qurix-data-catalog-1.0.0/qurix_data_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-26 16:14:54.000000 qurix-data-catalog-1.0.0/qurix_data_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 16:14:54.000000 qurix-data-catalog-1.0.0/qurix_data_catalog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 16:14:54.236944 qurix-data-catalog-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-26 16:14:36.000000 qurix-data-catalog-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:14:54.236944 qurix-data-catalog-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:14:36.000000 qurix-data-catalog-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-26 16:14:36.000000 qurix-data-catalog-1.0.0/tests/test_client.py
```

### Comparing `qurix-data-catalog-0.1.1/PKG-INFO` & `qurix-data-catalog-1.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: qurix-data-catalog
-Version: 0.1.1
-Summary: qurix Data Catalog Client for Python
-Home-page: https://github.com/qurixtechnology/python-package-template
-Author: qurix Technology
-Keywords: python
-Requires-Python: >=3.10, <4
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENCE
-
 # Python package template
 
 Template for Python packages for qurix Technology.
 
 ## Structure
 
 A normal Python package will start with the namespace `qurix` as in this sample package. A sample structure is as follows:
@@ -32,14 +20,35 @@
 ├── requirements.txt
 ├── setup.py
 └── tests
     ├── __init__.py
     └── test_client.py
 ```
 
-## Versioning
+## Versioning and release
+
+Package versions will be identified according to [semantic versioning](https://semver.org/lang/en). The release process will deploy in both [Test PyPI](https://test.pypi.org/) and [PyPI](https://pypi.org/).
 
-According to [semantic versioning](https://semver.org/lang/en).
+```mermaid
+gitGraph
+    commit
+    branch staging
+    branch feature/some-feature
+    checkout feature/some-feature
+    commit
+    commit
+    checkout staging
+    merge feature/some-feature id: "Test PyPI"
+    checkout main
+    merge staging id: "Release in PyPI" tag: "v0.1.0"
+    branch fix/some-fix
+    checkout fix/some-fix
+    commit
+    checkout staging
+    merge fix/some-fix id: "Test PyPI again"
+    checkout main
+    merge staging id: "New fix release in PyPI" tag: "v0.1.1"
+```
 
 ## Deployment
 
-Using Github Actions. See `.github/worfklows/`
+Using Github Actions. See `.github/worfklows/`
```

### Comparing `qurix-data-catalog-0.1.1/setup.py` & `qurix-data-catalog-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 with open("qurix/data/catalog/__version__.py", "r") as file_handler:
     exec(file_handler.read(), main_ns)
 
 setup(
     name="qurix-data-catalog",
     version=main_ns["VERSION"],
     author="qurix Technology",
+    license_files=("LICENSE"),
     description="qurix Data Catalog Client for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/qurixtechnology/python-package-template",
     packages=find_namespace_packages(),
     install_requires=[
     ],
```

