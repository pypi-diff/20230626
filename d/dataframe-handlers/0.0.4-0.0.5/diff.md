# Comparing `tmp/dataframe_handlers-0.0.4.tar.gz` & `tmp/dataframe_handlers-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataframe_handlers-0.0.4.tar", last modified: Mon Jun 26 17:56:31 2023, max compression
+gzip compressed data, was "dataframe_handlers-0.0.5.tar", last modified: Mon Jun 26 19:01:55 2023, max compression
```

## Comparing `dataframe_handlers-0.0.4.tar` & `dataframe_handlers-0.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 17:56:31.919446 dataframe_handlers-0.0.4/
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     5355 2023-06-26 17:22:31.000000 dataframe_handlers-0.0.4/CODE_OF_CONDUCT.md
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     7286 2023-06-26 16:37:04.000000 dataframe_handlers-0.0.4/CONTRIBUTING.md
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     1812 2023-06-26 17:55:14.000000 dataframe_handlers-0.0.4/COVERAGE.md
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     1100 2023-06-25 20:49:06.000000 dataframe_handlers-0.0.4/LICENSE
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)       46 2023-06-26 17:50:45.000000 dataframe_handlers-0.0.4/MANIFEST.in
--rw-r--r--   0 appuser   (1000) appuser   (1000)     5523 2023-06-26 17:56:31.914085 dataframe_handlers-0.0.4/PKG-INFO
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     4990 2023-06-26 16:37:04.000000 dataframe_handlers-0.0.4/README.md
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)      816 2023-06-26 17:08:56.000000 dataframe_handlers-0.0.4/SECURITY.md
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)      904 2023-06-26 17:55:15.000000 dataframe_handlers-0.0.4/coverage.svg
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 17:56:31.643952 dataframe_handlers-0.0.4/dataframe_handlers/
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     2261 2023-06-26 17:50:45.000000 dataframe_handlers-0.0.4/dataframe_handlers/__init__.py
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 17:56:31.732192 dataframe_handlers-0.0.4/dataframe_handlers/base/
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)       78 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.4/dataframe_handlers/base/__init__.py
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     2946 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.4/dataframe_handlers/base/base.py
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 17:56:31.760647 dataframe_handlers-0.0.4/dataframe_handlers/dask_handler/
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)       86 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.4/dataframe_handlers/dask_handler/__init__.py
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     1529 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.4/dataframe_handlers/dask_handler/dask_handler.py
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 17:56:31.788712 dataframe_handlers-0.0.4/dataframe_handlers/pandas_handler/
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)       92 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.4/dataframe_handlers/pandas_handler/__init__.py
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     2029 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.4/dataframe_handlers/pandas_handler/pandas_handler.py
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 17:56:31.819717 dataframe_handlers-0.0.4/dataframe_handlers/vaex_handler/
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)       90 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.4/dataframe_handlers/vaex_handler/__init__.py
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     2219 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.4/dataframe_handlers/vaex_handler/vaex_handler.py
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 17:56:31.852140 dataframe_handlers-0.0.4/dataframe_handlers/xarray_handler/
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)       92 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.4/dataframe_handlers/xarray_handler/__init__.py
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     2549 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.4/dataframe_handlers/xarray_handler/xarray_handler.py
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 17:56:31.704047 dataframe_handlers-0.0.4/dataframe_handlers.egg-info/
--rw-r--r--   0 appuser   (1000) appuser   (1000)     5523 2023-06-26 17:56:31.000000 dataframe_handlers-0.0.4/dataframe_handlers.egg-info/PKG-INFO
--rw-r--r--   0 appuser   (1000) appuser   (1000)      916 2023-06-26 17:56:31.000000 dataframe_handlers-0.0.4/dataframe_handlers.egg-info/SOURCES.txt
--rw-r--r--   0 appuser   (1000) appuser   (1000)        1 2023-06-26 17:56:31.000000 dataframe_handlers-0.0.4/dataframe_handlers.egg-info/dependency_links.txt
--rw-r--r--   0 appuser   (1000) appuser   (1000)       65 2023-06-26 17:56:31.000000 dataframe_handlers-0.0.4/dataframe_handlers.egg-info/requires.txt
--rw-r--r--   0 appuser   (1000) appuser   (1000)       19 2023-06-26 17:56:31.000000 dataframe_handlers-0.0.4/dataframe_handlers.egg-info/top_level.txt
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)     1132 2023-06-26 17:50:45.000000 dataframe_handlers-0.0.4/pyproject.toml
--rw-r--r--   0 appuser   (1000) appuser   (1000)       38 2023-06-26 17:56:31.920496 dataframe_handlers-0.0.4/setup.cfg
-drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 17:56:31.904373 dataframe_handlers-0.0.4/tests/
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)      269 2023-06-26 01:15:00.000000 dataframe_handlers-0.0.4/tests/test_dask_handler.py
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)      211 2023-06-26 01:15:00.000000 dataframe_handlers-0.0.4/tests/test_pandas_handler.py
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)      257 2023-06-26 01:15:00.000000 dataframe_handlers-0.0.4/tests/test_vaex_handler.py
--rwxrwxrwx   0 appuser   (1000) appuser   (1000)      259 2023-06-26 01:15:00.000000 dataframe_handlers-0.0.4/tests/test_xarray_handler.py
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 19:01:55.066791 dataframe_handlers-0.0.5/
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     5355 2023-06-26 17:22:31.000000 dataframe_handlers-0.0.5/CODE_OF_CONDUCT.md
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     7286 2023-06-26 16:37:04.000000 dataframe_handlers-0.0.5/CONTRIBUTING.md
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     1810 2023-06-26 19:01:35.000000 dataframe_handlers-0.0.5/COVERAGE.md
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     1100 2023-06-25 20:49:06.000000 dataframe_handlers-0.0.5/LICENSE
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)       46 2023-06-26 18:02:29.000000 dataframe_handlers-0.0.5/MANIFEST.in
+-rw-r--r--   0 appuser   (1000) appuser   (1000)     5523 2023-06-26 19:01:55.064879 dataframe_handlers-0.0.5/PKG-INFO
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     4990 2023-06-26 16:37:04.000000 dataframe_handlers-0.0.5/README.md
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)      850 2023-06-26 18:05:53.000000 dataframe_handlers-0.0.5/SECURITY.md
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)      924 2023-06-26 19:01:35.000000 dataframe_handlers-0.0.5/coverage.svg
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 19:01:54.808904 dataframe_handlers-0.0.5/dataframe_handlers/
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     2344 2023-06-26 19:01:35.000000 dataframe_handlers-0.0.5/dataframe_handlers/__init__.py
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 19:01:54.893429 dataframe_handlers-0.0.5/dataframe_handlers/base/
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)       78 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.5/dataframe_handlers/base/__init__.py
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     3156 2023-06-26 19:01:35.000000 dataframe_handlers-0.0.5/dataframe_handlers/base/base.py
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 19:01:54.921550 dataframe_handlers-0.0.5/dataframe_handlers/dask_handler/
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)       86 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.5/dataframe_handlers/dask_handler/__init__.py
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     1529 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.5/dataframe_handlers/dask_handler/dask_handler.py
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 19:01:54.949978 dataframe_handlers-0.0.5/dataframe_handlers/pandas_handler/
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)       92 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.5/dataframe_handlers/pandas_handler/__init__.py
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     2029 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.5/dataframe_handlers/pandas_handler/pandas_handler.py
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 19:01:54.977941 dataframe_handlers-0.0.5/dataframe_handlers/vaex_handler/
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)       90 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.5/dataframe_handlers/vaex_handler/__init__.py
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     2219 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.5/dataframe_handlers/vaex_handler/vaex_handler.py
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 19:01:55.006591 dataframe_handlers-0.0.5/dataframe_handlers/xarray_handler/
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)       92 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.5/dataframe_handlers/xarray_handler/__init__.py
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     2549 2023-06-25 23:17:33.000000 dataframe_handlers-0.0.5/dataframe_handlers/xarray_handler/xarray_handler.py
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 19:01:54.865727 dataframe_handlers-0.0.5/dataframe_handlers.egg-info/
+-rw-r--r--   0 appuser   (1000) appuser   (1000)     5523 2023-06-26 19:01:54.000000 dataframe_handlers-0.0.5/dataframe_handlers.egg-info/PKG-INFO
+-rw-r--r--   0 appuser   (1000) appuser   (1000)      916 2023-06-26 19:01:54.000000 dataframe_handlers-0.0.5/dataframe_handlers.egg-info/SOURCES.txt
+-rw-r--r--   0 appuser   (1000) appuser   (1000)        1 2023-06-26 19:01:54.000000 dataframe_handlers-0.0.5/dataframe_handlers.egg-info/dependency_links.txt
+-rw-r--r--   0 appuser   (1000) appuser   (1000)       65 2023-06-26 19:01:54.000000 dataframe_handlers-0.0.5/dataframe_handlers.egg-info/requires.txt
+-rw-r--r--   0 appuser   (1000) appuser   (1000)       19 2023-06-26 19:01:54.000000 dataframe_handlers-0.0.5/dataframe_handlers.egg-info/top_level.txt
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)     1132 2023-06-26 19:01:35.000000 dataframe_handlers-0.0.5/pyproject.toml
+-rw-r--r--   0 appuser   (1000) appuser   (1000)       38 2023-06-26 19:01:55.067855 dataframe_handlers-0.0.5/setup.cfg
+drwxr-xr-x   0 appuser   (1000) appuser   (1000)        0 2023-06-26 19:01:55.052910 dataframe_handlers-0.0.5/tests/
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)      269 2023-06-26 01:15:00.000000 dataframe_handlers-0.0.5/tests/test_dask_handler.py
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)      211 2023-06-26 01:15:00.000000 dataframe_handlers-0.0.5/tests/test_pandas_handler.py
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)      257 2023-06-26 01:15:00.000000 dataframe_handlers-0.0.5/tests/test_vaex_handler.py
+-rwxrwxrwx   0 appuser   (1000) appuser   (1000)      259 2023-06-26 01:15:00.000000 dataframe_handlers-0.0.5/tests/test_xarray_handler.py
```

### Comparing `dataframe_handlers-0.0.4/CODE_OF_CONDUCT.md` & `dataframe_handlers-0.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dataframe_handlers-0.0.4/CONTRIBUTING.md` & `dataframe_handlers-0.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dataframe_handlers-0.0.4/COVERAGE.md` & `dataframe_handlers-0.0.5/COVERAGE.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-| Name                                                   |    Stmts |     Miss |   Cover |   Missing |
-|------------------------------------------------------- | -------: | -------: | ------: | --------: |
-| dataframe\_handlers/\_\_init\_\_.py                    |       35 |        8 |     77% |17-18, 26-27, 35-36, 67, 72 |
-| dataframe\_handlers/base/\_\_init\_\_.py               |        2 |        0 |    100% |           |
-| dataframe\_handlers/base/base.py                       |       29 |        8 |     72% |27, 45, 58, 71, 91, 95, 99, 115 |
-| dataframe\_handlers/dask\_handler/\_\_init\_\_.py      |        2 |        0 |    100% |           |
-| dataframe\_handlers/dask\_handler/dask\_handler.py     |       20 |        0 |    100% |           |
-| dataframe\_handlers/pandas\_handler/\_\_init\_\_.py    |        2 |        0 |    100% |           |
-| dataframe\_handlers/pandas\_handler/pandas\_handler.py |       26 |        0 |    100% |           |
-| dataframe\_handlers/xarray\_handler/\_\_init\_\_.py    |        2 |        0 |    100% |           |
-| dataframe\_handlers/xarray\_handler/xarray\_handler.py |       36 |        0 |    100% |           |
-| tests/\_\_init\_\_.py                                  |        2 |        0 |    100% |           |
-| tests/base.py                                          |       55 |        1 |     98% |        25 |
-| tests/test\_dask\_handler.py                           |        7 |        0 |    100% |           |
-| tests/test\_pandas\_handler.py                         |        6 |        0 |    100% |           |
-| tests/test\_xarray\_handler.py                         |        7 |        0 |    100% |           |
-|                                              **TOTAL** |  **231** |   **17** | **93%** |           |
-
-1 empty file skipped.
+| Name                                                   |    Stmts |     Miss |    Cover |   Missing |
+|------------------------------------------------------- | -------: | -------: | -------: | --------: |
+| dataframe\_handlers/\_\_init\_\_.py                    |       29 |        0 |     100% |           |
+| dataframe\_handlers/base/\_\_init\_\_.py               |        2 |        0 |     100% |           |
+| dataframe\_handlers/base/base.py                       |       21 |        0 |     100% |           |
+| dataframe\_handlers/dask\_handler/\_\_init\_\_.py      |        2 |        0 |     100% |           |
+| dataframe\_handlers/dask\_handler/dask\_handler.py     |       20 |        0 |     100% |           |
+| dataframe\_handlers/pandas\_handler/\_\_init\_\_.py    |        2 |        0 |     100% |           |
+| dataframe\_handlers/pandas\_handler/pandas\_handler.py |       26 |        0 |     100% |           |
+| dataframe\_handlers/xarray\_handler/\_\_init\_\_.py    |        2 |        0 |     100% |           |
+| dataframe\_handlers/xarray\_handler/xarray\_handler.py |       36 |        0 |     100% |           |
+| tests/\_\_init\_\_.py                                  |        2 |        0 |     100% |           |
+| tests/base.py                                          |       61 |        0 |     100% |           |
+| tests/test\_dask\_handler.py                           |        7 |        0 |     100% |           |
+| tests/test\_pandas\_handler.py                         |        6 |        0 |     100% |           |
+| tests/test\_xarray\_handler.py                         |        7 |        0 |     100% |           |
+|                                              **TOTAL** |  **223** |    **0** | **100%** |           |
+
+1 empty file skipped.
```

### Comparing `dataframe_handlers-0.0.4/LICENSE` & `dataframe_handlers-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dataframe_handlers-0.0.4/PKG-INFO` & `dataframe_handlers-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataframe_handlers
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for handling dataframes with optional backends.
 Author: Joshua Sundance Bailey
 Maintainer: Joshua Sundance Bailey
 License: MIT
 Project-URL: Repository, https://github.com/joshuasundance-swca/dataframe_handlers.git
 Keywords: dataframe,interoperability
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dataframe_handlers-0.0.4/README.md` & `dataframe_handlers-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dataframe_handlers-0.0.4/SECURITY.md` & `dataframe_handlers-0.0.5/SECURITY.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 3. [CodeQL code scanning](https://docs.github.com/en/code-security/code-scanning/automatically-scanning-your-code-for-vulnerabilities-and-errors/about-code-scanning-with-codeql)
 4. [secret scanning](https://docs.github.com/en/code-security/secret-scanning/about-secret-scanning)
 
 ## Supported Versions
 
 | Version | Supported          |
 | ------- | ------------------ |
+| 0.0.4   | :white_check_mark: |
 | 0.0.3   | :white_check_mark: |
 | 0.0.2   | :white_check_mark: |
 | 0.0.1   | :white_check_mark: |
 
 ## Reporting a Vulnerability
 
 Please report security issues by raising an Issue in the GitHub repository.
```

### Comparing `dataframe_handlers-0.0.4/coverage.svg` & `dataframe_handlers-0.0.5/coverage.svg`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
-00000020: 462d 3822 3f3e 0a3c 7376 6720 786d 6c6e  F-8"?>.<svg xmln
-00000030: 733d 2268 7474 703a 2f2f 7777 772e 7733  s="http://www.w3
-00000040: 2e6f 7267 2f32 3030 302f 7376 6722 2077  .org/2000/svg" w
-00000050: 6964 7468 3d22 3939 2220 6865 6967 6874  idth="99" height
-00000060: 3d22 3230 223e 0a20 2020 203c 6c69 6e65  ="20">.    <line
-00000070: 6172 4772 6164 6965 6e74 2069 643d 2262  arGradient id="b
-00000080: 2220 7832 3d22 3022 2079 323d 2231 3030  " x2="0" y2="100
-00000090: 2522 3e0a 2020 2020 2020 2020 3c73 746f  %">.        <sto
-000000a0: 7020 6f66 6673 6574 3d22 3022 2073 746f  p offset="0" sto
-000000b0: 702d 636f 6c6f 723d 2223 6262 6222 2073  p-color="#bbb" s
-000000c0: 746f 702d 6f70 6163 6974 793d 222e 3122  top-opacity=".1"
-000000d0: 2f3e 0a20 2020 2020 2020 203c 7374 6f70  />.        <stop
-000000e0: 206f 6666 7365 743d 2231 2220 7374 6f70   offset="1" stop
-000000f0: 2d6f 7061 6369 7479 3d22 2e31 222f 3e0a  -opacity=".1"/>.
-00000100: 2020 2020 3c2f 6c69 6e65 6172 4772 6164      </linearGrad
-00000110: 6965 6e74 3e0a 2020 2020 3c6d 6173 6b20  ient>.    <mask 
-00000120: 6964 3d22 6122 3e0a 2020 2020 2020 2020  id="a">.        
-00000130: 3c72 6563 7420 7769 6474 683d 2239 3922  <rect width="99"
-00000140: 2068 6569 6768 743d 2232 3022 2072 783d   height="20" rx=
-00000150: 2233 2220 6669 6c6c 3d22 2366 6666 222f  "3" fill="#fff"/
-00000160: 3e0a 2020 2020 3c2f 6d61 736b 3e0a 2020  >.    </mask>.  
-00000170: 2020 3c67 206d 6173 6b3d 2275 726c 2823    <g mask="url(#
-00000180: 6129 223e 0a20 2020 2020 2020 203c 7061  a)">.        <pa
-00000190: 7468 2066 696c 6c3d 2223 3535 3522 2064  th fill="#555" d
-000001a0: 3d22 4d30 2030 6836 3376 3230 4830 7a22  ="M0 0h63v20H0z"
-000001b0: 2f3e 0a20 2020 2020 2020 203c 7061 7468  />.        <path
-000001c0: 2066 696c 6c3d 2223 3937 4341 3030 2220   fill="#97CA00" 
-000001d0: 643d 224d 3633 2030 6833 3676 3230 4836  d="M63 0h36v20H6
-000001e0: 337a 222f 3e0a 2020 2020 2020 2020 3c70  3z"/>.        <p
-000001f0: 6174 6820 6669 6c6c 3d22 7572 6c28 2362  ath fill="url(#b
-00000200: 2922 2064 3d22 4d30 2030 6839 3976 3230  )" d="M0 0h99v20
-00000210: 4830 7a22 2f3e 0a20 2020 203c 2f67 3e0a  H0z"/>.    </g>.
-00000220: 2020 2020 3c67 2066 696c 6c3d 2223 6666      <g fill="#ff
-00000230: 6622 2074 6578 742d 616e 6368 6f72 3d22  f" text-anchor="
-00000240: 6d69 6464 6c65 2220 666f 6e74 2d66 616d  middle" font-fam
-00000250: 696c 793d 2244 656a 6156 7520 5361 6e73  ily="DejaVu Sans
-00000260: 2c56 6572 6461 6e61 2c47 656e 6576 612c  ,Verdana,Geneva,
-00000270: 7361 6e73 2d73 6572 6966 2220 666f 6e74  sans-serif" font
-00000280: 2d73 697a 653d 2231 3122 3e0a 2020 2020  -size="11">.    
-00000290: 2020 2020 3c74 6578 7420 783d 2233 312e      <text x="31.
-000002a0: 3522 2079 3d22 3135 2220 6669 6c6c 3d22  5" y="15" fill="
-000002b0: 2330 3130 3130 3122 2066 696c 6c2d 6f70  #010101" fill-op
-000002c0: 6163 6974 793d 222e 3322 3e63 6f76 6572  acity=".3">cover
-000002d0: 6167 653c 2f74 6578 743e 0a20 2020 2020  age</text>.     
-000002e0: 2020 203c 7465 7874 2078 3d22 3331 2e35     <text x="31.5
-000002f0: 2220 793d 2231 3422 3e63 6f76 6572 6167  " y="14">coverag
-00000300: 653c 2f74 6578 743e 0a20 2020 2020 2020  e</text>.       
-00000310: 203c 7465 7874 2078 3d22 3830 2220 793d   <text x="80" y=
-00000320: 2231 3522 2066 696c 6c3d 2223 3031 3031  "15" fill="#0101
-00000330: 3031 2220 6669 6c6c 2d6f 7061 6369 7479  01" fill-opacity
-00000340: 3d22 2e33 223e 3933 253c 2f74 6578 743e  =".3">93%</text>
-00000350: 0a20 2020 2020 2020 203c 7465 7874 2078  .        <text x
-00000360: 3d22 3830 2220 793d 2231 3422 3e39 3325  ="80" y="14">93%
-00000370: 3c2f 7465 7874 3e0a 2020 2020 3c2f 673e  </text>.    </g>
-00000380: 0a3c 2f73 7667 3e0a                      .</svg>.
+00000020: 462d 3822 3f3e 0d0a 3c73 7667 2078 6d6c  F-8"?>..<svg xml
+00000030: 6e73 3d22 6874 7470 3a2f 2f77 7777 2e77  ns="http://www.w
+00000040: 332e 6f72 672f 3230 3030 2f73 7667 2220  3.org/2000/svg" 
+00000050: 7769 6474 683d 2239 3922 2068 6569 6768  width="99" heigh
+00000060: 743d 2232 3022 3e0d 0a20 2020 203c 6c69  t="20">..    <li
+00000070: 6e65 6172 4772 6164 6965 6e74 2069 643d  nearGradient id=
+00000080: 2262 2220 7832 3d22 3022 2079 323d 2231  "b" x2="0" y2="1
+00000090: 3030 2522 3e0d 0a20 2020 2020 2020 203c  00%">..        <
+000000a0: 7374 6f70 206f 6666 7365 743d 2230 2220  stop offset="0" 
+000000b0: 7374 6f70 2d63 6f6c 6f72 3d22 2362 6262  stop-color="#bbb
+000000c0: 2220 7374 6f70 2d6f 7061 6369 7479 3d22  " stop-opacity="
+000000d0: 2e31 222f 3e0d 0a20 2020 2020 2020 203c  .1"/>..        <
+000000e0: 7374 6f70 206f 6666 7365 743d 2231 2220  stop offset="1" 
+000000f0: 7374 6f70 2d6f 7061 6369 7479 3d22 2e31  stop-opacity=".1
+00000100: 222f 3e0d 0a20 2020 203c 2f6c 696e 6561  "/>..    </linea
+00000110: 7247 7261 6469 656e 743e 0d0a 2020 2020  rGradient>..    
+00000120: 3c6d 6173 6b20 6964 3d22 6122 3e0d 0a20  <mask id="a">.. 
+00000130: 2020 2020 2020 203c 7265 6374 2077 6964         <rect wid
+00000140: 7468 3d22 3939 2220 6865 6967 6874 3d22  th="99" height="
+00000150: 3230 2220 7278 3d22 3322 2066 696c 6c3d  20" rx="3" fill=
+00000160: 2223 6666 6622 2f3e 0d0a 2020 2020 3c2f  "#fff"/>..    </
+00000170: 6d61 736b 3e0d 0a20 2020 203c 6720 6d61  mask>..    <g ma
+00000180: 736b 3d22 7572 6c28 2361 2922 3e0d 0a20  sk="url(#a)">.. 
+00000190: 2020 2020 2020 203c 7061 7468 2066 696c         <path fil
+000001a0: 6c3d 2223 3535 3522 2064 3d22 4d30 2030  l="#555" d="M0 0
+000001b0: 6836 3376 3230 4830 7a22 2f3e 0d0a 2020  h63v20H0z"/>..  
+000001c0: 2020 2020 2020 3c70 6174 6820 6669 6c6c        <path fill
+000001d0: 3d22 2334 6331 2220 643d 224d 3633 2030  ="#4c1" d="M63 0
+000001e0: 6833 3676 3230 4836 337a 222f 3e0d 0a20  h36v20H63z"/>.. 
+000001f0: 2020 2020 2020 203c 7061 7468 2066 696c         <path fil
+00000200: 6c3d 2275 726c 2823 6229 2220 643d 224d  l="url(#b)" d="M
+00000210: 3020 3068 3939 7632 3048 307a 222f 3e0d  0 0h99v20H0z"/>.
+00000220: 0a20 2020 203c 2f67 3e0d 0a20 2020 203c  .    </g>..    <
+00000230: 6720 6669 6c6c 3d22 2366 6666 2220 7465  g fill="#fff" te
+00000240: 7874 2d61 6e63 686f 723d 226d 6964 646c  xt-anchor="middl
+00000250: 6522 2066 6f6e 742d 6661 6d69 6c79 3d22  e" font-family="
+00000260: 4465 6a61 5675 2053 616e 732c 5665 7264  DejaVu Sans,Verd
+00000270: 616e 612c 4765 6e65 7661 2c73 616e 732d  ana,Geneva,sans-
+00000280: 7365 7269 6622 2066 6f6e 742d 7369 7a65  serif" font-size
+00000290: 3d22 3131 223e 0d0a 2020 2020 2020 2020  ="11">..        
+000002a0: 3c74 6578 7420 783d 2233 312e 3522 2079  <text x="31.5" y
+000002b0: 3d22 3135 2220 6669 6c6c 3d22 2330 3130  ="15" fill="#010
+000002c0: 3130 3122 2066 696c 6c2d 6f70 6163 6974  101" fill-opacit
+000002d0: 793d 222e 3322 3e63 6f76 6572 6167 653c  y=".3">coverage<
+000002e0: 2f74 6578 743e 0d0a 2020 2020 2020 2020  /text>..        
+000002f0: 3c74 6578 7420 783d 2233 312e 3522 2079  <text x="31.5" y
+00000300: 3d22 3134 223e 636f 7665 7261 6765 3c2f  ="14">coverage</
+00000310: 7465 7874 3e0d 0a20 2020 2020 2020 203c  text>..        <
+00000320: 7465 7874 2078 3d22 3830 2220 793d 2231  text x="80" y="1
+00000330: 3522 2066 696c 6c3d 2223 3031 3031 3031  5" fill="#010101
+00000340: 2220 6669 6c6c 2d6f 7061 6369 7479 3d22  " fill-opacity="
+00000350: 2e33 223e 3130 3025 3c2f 7465 7874 3e0d  .3">100%</text>.
+00000360: 0a20 2020 2020 2020 203c 7465 7874 2078  .        <text x
+00000370: 3d22 3830 2220 793d 2231 3422 3e31 3030  ="80" y="14">100
+00000380: 253c 2f74 6578 743e 0d0a 2020 2020 3c2f  %</text>..    </
+00000390: 673e 0d0a 3c2f 7376 673e 0d0a            g>..</svg>..
```

### Comparing `dataframe_handlers-0.0.4/dataframe_handlers/__init__.py` & `dataframe_handlers-0.0.5/dataframe_handlers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 from typing import Any, Optional, Type
 
 from .base import BaseDataFrameHandler
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 __all__ = ["BaseDataFrameHandler"]
 
 dispatch_dict = {}
 
 try:
     import pandas as pd
     from .pandas_handler import PandasDataFrameHandler
 
     __all__.append("PandasDataFrameHandler")
     dispatch_dict[pd.DataFrame] = PandasDataFrameHandler
-
-except ImportError:
+except ImportError:  # pragma: no cover
     pass
 
+
 try:
     import dask.dataframe as dd
     from .dask_handler import DaskDataFrameHandler
 
     __all__.append("DaskDataFrameHandler")
     dispatch_dict[dd.DataFrame] = DaskDataFrameHandler
-except ImportError:
+except ImportError:  # pragma: no cover
     pass
 
+
 try:
     import xarray as xr
     from .xarray_handler import XarrayDataFrameHandler
 
     __all__.append("XarrayDataFrameHandler")
     dispatch_dict[xr.Dataset] = XarrayDataFrameHandler
-except ImportError:
+except ImportError:  # pragma: no cover
     pass
 
+
 # try:
 #     import vaex
 #     from .vaex_handler import VaexDataFrameHandler
 #
 #     __all__.append("VaexDataFrameHandler")
 #     dispatch_dict[vaex.dataframe.DataFrame] = VaexDataFrameHandler
-# except ImportError:
+# except ImportError: # pragma: no cover
 #     pass
 
 
 def get_handler(df: Any, handler_type: Optional[Type] = None) -> BaseDataFrameHandler:
     """
     Function to get the appropriate handler based on the dataframe type.
```

### Comparing `dataframe_handlers-0.0.4/dataframe_handlers/base/base.py` & `dataframe_handlers-0.0.5/dataframe_handlers/base/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         Args:
             column: Name of the column.
             limit: Maximum number of unique values to return.
 
         Returns:
             Collection of unique values.
         """
-        pass
 
     @abc.abstractmethod
     def get_value_counts(
         self,
         column: str,
         limit: Optional[int] = None,
     ) -> Mapping[str, int]:
@@ -38,41 +37,38 @@
         Args:
             column: Name of the column.
             limit: Maximum number of value counts to return.
 
         Returns:
             (value, count) Mapping
         """
-        pass
 
     @abc.abstractmethod
     def get_data_range(self, column: str) -> Sequence:
         """
         Get the minimum and maximum values in a column of the DataFrame.
 
         Args:
             column: Name of the column.
 
         Returns:
             Sequence containing the minimum and maximum values.
         """
-        pass
 
     @abc.abstractmethod
     def get_missing_filter(self, column: str) -> Sequence[bool]:
         """
         Filter the DataFrame based on missing values in a column.
 
         Args:
             column: Name of the column.
 
         Returns:
             Boolean Series indicating missing values.
         """
-        pass
 
     @abc.abstractmethod
     def get_value_filter(
         self,
         column: str,
         values: list,
         invert: bool = False,
@@ -84,23 +80,32 @@
             column: Name of the column.
             values: List of values to filter on.
             invert: Flag indicating whether to invert the filter.
 
         Returns:
             Boolean Series indicating the filtered rows.
         """
-        pass
 
     @abc.abstractmethod
     def get_columns(self) -> Collection[str]:
-        pass
+        """
+        Return Collection of column names as strings.
+
+        Returns:
+            Collection of column names as strings.
+        """
 
     @abc.abstractmethod
     def get_numeric_columns(self) -> Collection[str]:
-        pass
+        """
+        Return Collection of numeric column names as strings.
+
+        Returns:
+            Collection of numeric column names as strings.
+        """
 
     @abc.abstractmethod
     def get_column_types(
         self,
         default_str: bool = True,
     ) -> Mapping[str, Union[object, type, str]]:
         """
@@ -108,8 +113,7 @@
 
         Args:
             default_str: If not numeric or bool, default to str.
 
         Returns:
             Dictionary mapping column names to their types.
         """
-        pass
```

### Comparing `dataframe_handlers-0.0.4/dataframe_handlers/dask_handler/dask_handler.py` & `dataframe_handlers-0.0.5/dataframe_handlers/dask_handler/dask_handler.py`

 * *Files identical despite different names*

### Comparing `dataframe_handlers-0.0.4/dataframe_handlers/pandas_handler/pandas_handler.py` & `dataframe_handlers-0.0.5/dataframe_handlers/pandas_handler/pandas_handler.py`

 * *Files identical despite different names*

### Comparing `dataframe_handlers-0.0.4/dataframe_handlers/vaex_handler/vaex_handler.py` & `dataframe_handlers-0.0.5/dataframe_handlers/vaex_handler/vaex_handler.py`

 * *Files identical despite different names*

### Comparing `dataframe_handlers-0.0.4/dataframe_handlers/xarray_handler/xarray_handler.py` & `dataframe_handlers-0.0.5/dataframe_handlers/xarray_handler/xarray_handler.py`

 * *Files identical despite different names*

### Comparing `dataframe_handlers-0.0.4/dataframe_handlers.egg-info/PKG-INFO` & `dataframe_handlers-0.0.5/dataframe_handlers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataframe-handlers
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for handling dataframes with optional backends.
 Author: Joshua Sundance Bailey
 Maintainer: Joshua Sundance Bailey
 License: MIT
 Project-URL: Repository, https://github.com/joshuasundance-swca/dataframe_handlers.git
 Keywords: dataframe,interoperability
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dataframe_handlers-0.0.4/dataframe_handlers.egg-info/SOURCES.txt` & `dataframe_handlers-0.0.5/dataframe_handlers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataframe_handlers-0.0.4/pyproject.toml` & `dataframe_handlers-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "dataframe_handlers"
-version = "0.0.4"
+version = "0.0.5"
 description = "A package for handling dataframes with optional backends."
 authors = [{name="Joshua Sundance Bailey"}]
 maintainers = [{name="Joshua Sundance Bailey"}]
 license = {text="MIT"}
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -24,15 +24,15 @@
 pandas = ["pandas"]
 dask = ["dask[dataframe]", "pandas"]
 #vaex = ["vaex"]
 xarray = ["xarray"]
 
 
 [tool.bumpver]
-current_version = "0.0.4"
+current_version = "0.0.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

