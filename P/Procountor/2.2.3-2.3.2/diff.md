# Comparing `tmp/Procountor-2.2.3.tar.gz` & `tmp/Procountor-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Procountor-2.2.3.tar", last modified: Wed Nov 17 09:18:48 2021, max compression
+gzip compressed data, was "/home/runner/work/Procountor/Procountor/dist/.tmp-y2vdb40j/Procountor-2.3.2.tar", last modified: Mon Jun 26 11:23:59 2023, max compression
```

## Comparing `Procountor-2.2.3.tar` & `Procountor-2.3.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-17 09:18:48.154369 Procountor-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2021-11-17 09:18:36.000000 Procountor-2.2.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3787 2021-11-17 09:18:36.000000 Procountor-2.2.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      891 2021-11-17 09:18:36.000000 Procountor-2.2.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-17 09:18:36.000000 Procountor-2.2.3/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)      262 2021-11-17 09:18:36.000000 Procountor-2.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2762 2021-11-17 09:18:48.154369 Procountor-2.2.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-17 09:18:48.150369 Procountor-2.2.3/Procountor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2762 2021-11-17 09:18:48.000000 Procountor-2.2.3/Procountor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2021-11-17 09:18:48.000000 Procountor-2.2.3/Procountor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-17 09:18:48.000000 Procountor-2.2.3/Procountor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-17 09:18:47.000000 Procountor-2.2.3/Procountor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-11-17 09:18:48.000000 Procountor-2.2.3/Procountor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-11-17 09:18:48.000000 Procountor-2.2.3/Procountor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-11-17 09:18:36.000000 Procountor-2.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-17 09:18:48.150369 Procountor-2.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      611 2021-11-17 09:18:36.000000 Procountor-2.2.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-17 09:18:48.150369 Procountor-2.2.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-11-17 09:18:36.000000 Procountor-2.2.3/docs/source/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5179 2021-11-17 09:18:36.000000 Procountor-2.2.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       36 2021-11-17 09:18:36.000000 Procountor-2.2.3/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-11-17 09:18:36.000000 Procountor-2.2.3/docs/source/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      507 2021-11-17 09:18:36.000000 Procountor-2.2.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2021-11-17 09:18:36.000000 Procountor-2.2.3/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-11-17 09:18:36.000000 Procountor-2.2.3/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)      339 2021-11-17 09:18:36.000000 Procountor-2.2.3/docs/source/procountor.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-11-17 09:18:36.000000 Procountor-2.2.3/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-11-17 09:18:36.000000 Procountor-2.2.3/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-17 09:18:48.150369 Procountor-2.2.3/procountor/
--rw-r--r--   0 runner    (1001) docker     (121)      183 2021-11-17 09:18:36.000000 Procountor-2.2.3/procountor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31299 2021-11-17 09:18:36.000000 Procountor-2.2.3/procountor/api_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)     7587 2021-11-17 09:18:36.000000 Procountor-2.2.3/procountor/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2021-11-17 09:18:48.154369 Procountor-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1429 2021-11-17 09:18:36.000000 Procountor-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-17 09:18:48.154369 Procountor-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/test_000_client_core.py
--rw-r--r--   0 runner    (1001) docker     (121)     1975 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/test_001_attachment.py
--rw-r--r--   0 runner    (1001) docker     (121)      725 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/test_002_bank_accounts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1775 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/test_003_bank_statements.py
--rw-r--r--   0 runner    (1001) docker     (121)     1306 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/test_004_business_partners.py
--rw-r--r--   0 runner    (1001) docker     (121)      490 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/test_005_coa.py
--rw-r--r--   0 runner    (1001) docker     (121)      656 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/test_006_company.py
--rw-r--r--   0 runner    (1001) docker     (121)     1389 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/test_007_currencies.py
--rw-r--r--   0 runner    (1001) docker     (121)     1207 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/test_008_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/test_009_fiscal_years.py
--rw-r--r--   0 runner    (1001) docker     (121)     3738 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/test_010_invoices.py
--rw-r--r--   0 runner    (1001) docker     (121)      934 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/test_011_ledger_receipts.py
--rw-r--r--   0 runner    (1001) docker     (121)      273 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/test_012_payments.py
--rw-r--r--   0 runner    (1001) docker     (121)     1357 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/test_013_product.py
--rw-r--r--   0 runner    (1001) docker     (121)      549 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/test_014_reference_payments.py
--rw-r--r--   0 runner    (1001) docker     (121)      505 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/test_015_session_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/test_016_users.py
--rw-r--r--   0 runner    (1001) docker     (121)      796 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/test_017_vats.py
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2021-11-17 09:18:36.000000 Procountor-2.2.3/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:23:59.000000 Procountor-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-26 11:23:48.000000 Procountor-2.3.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-26 11:23:48.000000 Procountor-2.3.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-26 11:23:48.000000 Procountor-2.3.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 11:23:48.000000 Procountor-2.3.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-26 11:23:48.000000 Procountor-2.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-26 11:23:59.000000 Procountor-2.3.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:23:59.000000 Procountor-2.3.2/Procountor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-26 11:23:59.000000 Procountor-2.3.2/Procountor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-26 11:23:59.000000 Procountor-2.3.2/Procountor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 11:23:59.000000 Procountor-2.3.2/Procountor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 11:23:58.000000 Procountor-2.3.2/Procountor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-26 11:23:59.000000 Procountor-2.3.2/Procountor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 11:23:59.000000 Procountor-2.3.2/Procountor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-26 11:23:48.000000 Procountor-2.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:23:59.000000 Procountor-2.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-26 11:23:48.000000 Procountor-2.3.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:23:59.000000 Procountor-2.3.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 11:23:48.000000 Procountor-2.3.2/docs/source/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-06-26 11:23:48.000000 Procountor-2.3.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 11:23:48.000000 Procountor-2.3.2/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 11:23:48.000000 Procountor-2.3.2/docs/source/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-26 11:23:48.000000 Procountor-2.3.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-26 11:23:48.000000 Procountor-2.3.2/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-26 11:23:48.000000 Procountor-2.3.2/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-26 11:23:48.000000 Procountor-2.3.2/docs/source/procountor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-26 11:23:48.000000 Procountor-2.3.2/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-26 11:23:48.000000 Procountor-2.3.2/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:23:59.000000 Procountor-2.3.2/procountor/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-26 11:23:48.000000 Procountor-2.3.2/procountor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31299 2023-06-26 11:23:48.000000 Procountor-2.3.2/procountor/api_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-06-26 11:23:48.000000 Procountor-2.3.2/procountor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-26 11:23:59.000000 Procountor-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-26 11:23:48.000000 Procountor-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:23:59.000000 Procountor-2.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/test_000_client_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/test_001_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/test_002_bank_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/test_003_bank_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/test_004_business_partners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/test_005_coa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/test_006_company.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/test_007_currencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/test_008_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/test_009_fiscal_years.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/test_010_invoices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/test_011_ledger_receipts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/test_012_payments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/test_013_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/test_014_reference_payments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/test_015_session_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/test_016_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/test_017_vats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-26 11:23:48.000000 Procountor-2.3.2/tests/test_client.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `Procountor-2.2.3/CONTRIBUTING.rst` & `Procountor-2.3.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/HISTORY.rst` & `Procountor-2.3.2/HISTORY.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 =======
 History
 =======
 
+2.3.2 (2022-06-26)
+------------------
+
+* up version number to test new release process
+
+2.3.1 (2022-06-26)
+------------------
+
+* Don't send empty json body in get requests
+  * fixes problem with azure api gateway rejecting messages
+* remove travis
+
 2.2.1 (2021-11-15)
 ------------------
 
 * Better API Token error message if getting token fails
 
 1.2.0 (2020-04-08)
 ------------------
```

### Comparing `Procountor-2.2.3/PKG-INFO` & `Procountor-2.3.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: Procountor
-Version: 2.2.3
+Version: 2.3.2
 Summary: Python library for calling Procountor REST API
 Home-page: https://github.com/vilkasgroup/Procountor
 Author: Joonas Maliniemi
 Author-email: joonas@vilkas.fi
 License: MIT license
 Keywords: procountor
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
@@ -55,18 +54,56 @@
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
+Releasing new version to pypi
+---------
+
+Install dev tools
+
+```
+pipenv install --dev
+```
+
+Update `HISTORY.rst` and commit the changes.
+
+Bump version. (patch | minor | major depending on the scale of changes)
+
+```
+bumpversion patch
+```
+
+Push changes and tags.
+
+```
+git push
+git push --tags
+```
+
+Double check that the github action runs successfully.
+
 =======
 History
 =======
 
+2.3.2 (2022-06-26)
+------------------
+
+* up version number to test new release process
+
+2.3.1 (2022-06-26)
+------------------
+
+* Don't send empty json body in get requests
+  * fixes problem with azure api gateway rejecting messages
+* remove travis
+
 2.2.1 (2021-11-15)
 ------------------
 
 * Better API Token error message if getting token fails
 
 1.2.0 (2020-04-08)
 ------------------
@@ -106,9 +143,7 @@
 * Bump version: 0.0.1 -> 0.1.0
 
 
 0.0.1 (2018-03-15)
 ------------------
 
 * First release for PyPi
-
-
```

### Comparing `Procountor-2.2.3/Procountor.egg-info/PKG-INFO` & `Procountor-2.3.2/Procountor.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: Procountor
-Version: 2.2.3
+Version: 2.3.2
 Summary: Python library for calling Procountor REST API
 Home-page: https://github.com/vilkasgroup/Procountor
 Author: Joonas Maliniemi
 Author-email: joonas@vilkas.fi
 License: MIT license
 Keywords: procountor
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
@@ -55,18 +54,56 @@
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
+Releasing new version to pypi
+---------
+
+Install dev tools
+
+```
+pipenv install --dev
+```
+
+Update `HISTORY.rst` and commit the changes.
+
+Bump version. (patch | minor | major depending on the scale of changes)
+
+```
+bumpversion patch
+```
+
+Push changes and tags.
+
+```
+git push
+git push --tags
+```
+
+Double check that the github action runs successfully.
+
 =======
 History
 =======
 
+2.3.2 (2022-06-26)
+------------------
+
+* up version number to test new release process
+
+2.3.1 (2022-06-26)
+------------------
+
+* Don't send empty json body in get requests
+  * fixes problem with azure api gateway rejecting messages
+* remove travis
+
 2.2.1 (2021-11-15)
 ------------------
 
 * Better API Token error message if getting token fails
 
 1.2.0 (2020-04-08)
 ------------------
@@ -106,9 +143,7 @@
 * Bump version: 0.0.1 -> 0.1.0
 
 
 0.0.1 (2018-03-15)
 ------------------
 
 * First release for PyPi
-
-
```

### Comparing `Procountor-2.2.3/Procountor.egg-info/SOURCES.txt` & `Procountor-2.3.2/Procountor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/README.rst` & `Procountor-2.3.2/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -33,7 +33,34 @@
 Credits
 ---------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
+
+
+Releasing new version to pypi
+---------
+
+Install dev tools
+
+```
+pipenv install --dev
+```
+
+Update `HISTORY.rst` and commit the changes.
+
+Bump version. (patch | minor | major depending on the scale of changes)
+
+```
+bumpversion patch
+```
+
+Push changes and tags.
+
+```
+git push
+git push --tags
+```
+
+Double check that the github action runs successfully.
```

### Comparing `Procountor-2.2.3/docs/Makefile` & `Procountor-2.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/docs/source/conf.py` & `Procountor-2.3.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/docs/source/installation.rst` & `Procountor-2.3.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/procountor/api_methods.py` & `Procountor-2.3.2/procountor/api_methods.py`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/procountor/client.py` & `Procountor-2.3.2/procountor/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import re
 import requests
 from requests_toolbelt.multipart import decoder
+
 try:
     from urllib.parse import urlparse, parse_qs, urlencode
 except ImportError:
     from urlparse import urlparse, parse_qs
     from urllib import urlencode
 
 from .api_methods import ApiMethods
@@ -22,197 +23,228 @@
     :param client_secret: Procountor REST API client secret, string
     :param redirect_uri: URI where redirected after authentication, string
     :param test_mode: Wether to use test api or real api, bool
     :param api_version: Cen be latest, supported or >= 20.01, string
     """
 
     _endpoints = {
-        'hosts' : {
-            'production': "https://api.procountor.com",
-            'test': "https://api-test.procountor.com",
+        "hosts": {
+            "production": "https://api.procountor.com",
+            "test": "https://pts-procountor.pubdev.azure.procountor.com",
+        },
+        "version": {
+            "latest": "latest/api",
+            "supported": "supported/api",
+            "specified": "v{}/api",
         },
-        'version' : {
-            'latest': "latest/api",
-            'supported': "supported/api",
-            'specified': "v{}/api",
-        }
     }
 
-    def __init__(self, api_key, client_id, client_secret, redirect_uri, test_mode=True, api_version='supported'):
-        self.api_key = api_key,
+    def __init__(
+        self,
+        api_key,
+        client_id,
+        client_secret,
+        redirect_uri,
+        test_mode=True,
+        api_version="supported",
+    ):
+        self.api_key = (api_key,)
         self.client_id = client_id
         self.client_secret = client_secret
         self.redirect_uri = redirect_uri
         self.test_mode = test_mode
         self.api_version = api_version
         self._get_token()
 
     @property
     def api_url(self):
-
-        if self.api_version in ['latest', 'supported']:
-            version = Client._endpoints['version'][self.api_version]
+        if self.api_version in ["latest", "supported"]:
+            version = Client._endpoints["version"][self.api_version]
         elif re.match("^2[0-9]\.[0-9]{2}$", self.api_version):
             version_number = "{}{}".format(self.api_version[0:2], self.api_version[3:5])
-            version = Client._endpoints['version']['specified'].format(version_number)
+            version = Client._endpoints["version"]["specified"].format(version_number)
         else:
-            raise ValueError("Given value for api version {} is not valid. Valid values are latest, supported or Api version >= 20.01".format(self.api_version)) 
+            raise ValueError(
+                "Given value for api version {} is not valid. Valid values are latest, supported or Api version >= 20.01".format(
+                    self.api_version
+                )
+            )
 
         return "{}/{}/".format(self.api_host, version)
 
     @property
     def api_host(self):
-        host = Client._endpoints['hosts']['test' if self.test_mode else 'production']
+        host = Client._endpoints["hosts"]["test" if self.test_mode else "production"]
         return host
 
     def _create_endpoint(self, endpoint, queries={}):
         """
 
         :return: url, string
         """
         return "{}{}".format(endpoint, self._dict_to_url_query(queries))
 
     def _dict_to_url_query(self, url_dict):
         """
         :return: url s
         """
-        
+
         if isinstance(url_dict, dict):
-            if (len(url_dict) > 0):
+            if len(url_dict) > 0:
                 return "?{}".format(urlencode(url_dict))
             else:
                 return ""
         else:
-            raise Exception("Given params are not dict. The type was {}".format(type(url_dict)))
+            raise Exception(
+                "Given params are not dict. The type was {}".format(type(url_dict))
+            )
 
     def invalidate_token(self):
         """Method invalidates the access token"""
 
         method = "POST"
         endpoint = "logout"
-        headers = {
-            'authorization': 'Bearer ' + self.access_token
-        }
+        headers = {"authorization": "Bearer " + self.access_token}
         url = "{}/{}".format(self.api_host, endpoint)
 
         return self.request(method, endpoint, headers, url)
 
     def _get_token(self):
         """Makes a request and returns an access token. Access token is valid for
         3600 seconds.
 
         :return: granted tokens, str
         """
 
         params = {
-            'grant_type': 'client_credentials',
-            'client_id': self.client_id,
-            'client_secret': self.client_secret,
-            'redirect_uri': self.redirect_uri,
-            'api_key': self.api_key
+            "grant_type": "client_credentials",
+            "client_id": self.client_id,
+            "client_secret": self.client_secret,
+            "redirect_uri": self.redirect_uri,
+            "api_key": self.api_key,
         }
 
-        headers = {
-            'content-type': 'application/x-www-form-urlencoded'
-        }
+        headers = {"content-type": "application/x-www-form-urlencoded"}
 
-        url = self.api_url + 'oauth/token/'
+        url = self.api_url + "oauth/token/"
         response = requests.post(url, params=params, headers=headers)
         status_code = response.status_code
 
         if status_code != 200:
-
             if status_code == 404:
-                raise RuntimeError("Not found api endpoint. Please, check your API version.")
+                raise RuntimeError(
+                    "Not found api endpoint. Please, check your API version."
+                )
 
             if status_code == 401:
-                raise RuntimeError("Authentication failed. Please, check your credentials.")
-
-            raise RuntimeError("Authentication got an unexpected HTTP Status code: " + status_code + ".")
+                raise RuntimeError(
+                    "Authentication failed. Please, check your credentials."
+                )
+
+            raise RuntimeError(
+                "Authentication got an unexpected HTTP Status code: "
+                + status_code
+                + "."
+            )
 
         json_content = response.json()
 
-        access_token = json_content.get('access_token', None)
+        access_token = json_content.get("access_token", None)
 
         if access_token is None:
-            raise RuntimeError("Cannot read the access_token from the response. Response was: " + json_content)
+            raise RuntimeError(
+                "Cannot read the access_token from the response. Response was: "
+                + json_content
+            )
 
         self.access_token = access_token
         return access_token
 
     def _handleResponse(self, response):
         """
         TODO: This text
 
         :return: response as dict. Dict has a key named status for HTTP-status code. In error case there is string
         """
 
-        answer = {'status': response.status_code}
+        answer = {"status": response.status_code}
 
         if response.status_code in (200, 202):
             try:
-                if response.headers['Content-Type'].startswith("multipart/"):
-                    meta, filebytes = decoder.MultipartDecoder.from_response(response).parts
-                    answer['content'] = filebytes.content
-                    answer['metadata'] = json.loads(meta.content.decode('utf-8'))
+                if response.headers["Content-Type"].startswith("multipart/"):
+                    meta, filebytes = decoder.MultipartDecoder.from_response(
+                        response
+                    ).parts
+                    answer["content"] = filebytes.content
+                    answer["metadata"] = json.loads(meta.content.decode("utf-8"))
                 else:
-                    answer['content'] = response.json()
+                    answer["content"] = response.json()
             except:
-                answer['message'] = response.text
+                answer["message"] = response.text
         else:
-            answer['message'] = response.text
+            answer["message"] = response.text
 
         return answer
 
-    def request(self, method, endpoint, headers=None, url=None, files=None, *args, **kwargs):
+    def request(
+        self, method, endpoint, headers=None, url=None, files=None, *args, **kwargs
+    ):
         """Method to make HTTP requests over Procountor REST API
 
         :param method: wanted request method, uppercase string
         :param endpoint: wanted REST API endpoint, string
         :param headers: Overwrite HTTP-headers, dict
         :param kwargs: query parameters to pass to Procountor, dict
         :return: response from rest server, dict
         """
         headers = headers or self._headers(method, endpoint)
         url = url or self.api_url + endpoint
 
-        response = requests.request(method, url, headers=headers, files=files, json=kwargs)
+        # Test environment (Microsoft-Azure-Application-Gateway)
+        # doesn't like if there is a json body in (for ex.) GET method.
+        json = None if len(kwargs) == 0 else kwargs
+
+        response = requests.request(
+            method, url, headers=headers, files=files, json=json
+        )
 
         # refresh token if out of date
         if response.status_code == 401:
             self.access_token = self._get_token()
-            response = requests.request(method, url, headers=headers, files=files, json=kwargs)
+            response = requests.request(
+                method, url, headers=headers, files=files, json=json
+            )
 
         return self._handleResponse(response)
 
     def _headers(self, method, endpoint):
         """Method returns correct headers for request
 
         :param method: request method, string
         :param endpoint: request endpoint, string
         :return: headers for request, dict
         """
 
         if "attachments" in endpoint:
             if method == "GET":
                 headers = {
-                    'content-type': 'multipart/mixed',
-                    'authorization': 'Bearer {}'.format(self.access_token),
+                    "content-type": "multipart/mixed",
+                    "authorization": "Bearer {}".format(self.access_token),
                 }
             elif method == "POST":
                 headers = {
                     # can't put 'content-type': 'multipart/form-data' here as documentation says. Requests generates it
                     # automatically.
-                    'authorization': 'Bearer {}'.format(self.access_token),
+                    "authorization": "Bearer {}".format(self.access_token),
                 }
             else:
                 headers = {
-                    'content-type': 'application/json',
-                    'authorization': 'Bearer {}'.format(self.access_token),
+                    "content-type": "application/json",
+                    "authorization": "Bearer {}".format(self.access_token),
                 }
         else:
             headers = {
-                'content-type': 'application/json',
-                'authorization': 'Bearer {}'.format(self.access_token),
+                "content-type": "application/json",
+                "authorization": "Bearer {}".format(self.access_token),
             }
 
         return headers
```

### Comparing `Procountor-2.2.3/setup.py` & `Procountor-2.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 test_requirements = [
     # TODO: put package test requirements here
 ]
 
 setup(
     name='Procountor',
-    version='2.2.3',
+    version='2.3.2',
     description="Python library for calling Procountor REST API",
     long_description=readme + '\n\n' + history,
     author="Joonas Maliniemi",
     author_email='joonas@vilkas.fi',
     url='https://github.com/vilkasgroup/Procountor',
     packages=find_packages(include=['procountor']),
     include_package_data=True,
```

### Comparing `Procountor-2.2.3/tests/test_000_client_core.py` & `Procountor-2.3.2/tests/test_000_client_core.py`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/tests/test_001_attachment.py` & `Procountor-2.3.2/tests/test_001_attachment.py`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/tests/test_002_bank_accounts.py` & `Procountor-2.3.2/tests/test_002_bank_accounts.py`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/tests/test_003_bank_statements.py` & `Procountor-2.3.2/tests/test_003_bank_statements.py`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/tests/test_004_business_partners.py` & `Procountor-2.3.2/tests/test_004_business_partners.py`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/tests/test_006_company.py` & `Procountor-2.3.2/tests/test_006_company.py`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/tests/test_007_currencies.py` & `Procountor-2.3.2/tests/test_007_currencies.py`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/tests/test_008_dimensions.py` & `Procountor-2.3.2/tests/test_008_dimensions.py`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/tests/test_010_invoices.py` & `Procountor-2.3.2/tests/test_010_invoices.py`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/tests/test_011_ledger_receipts.py` & `Procountor-2.3.2/tests/test_011_ledger_receipts.py`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/tests/test_013_product.py` & `Procountor-2.3.2/tests/test_013_product.py`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/tests/test_014_reference_payments.py` & `Procountor-2.3.2/tests/test_014_reference_payments.py`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/tests/test_016_users.py` & `Procountor-2.3.2/tests/test_016_users.py`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/tests/test_017_vats.py` & `Procountor-2.3.2/tests/test_017_vats.py`

 * *Files identical despite different names*

### Comparing `Procountor-2.2.3/tests/test_client.py` & `Procountor-2.3.2/tests/test_client.py`

 * *Files identical despite different names*

