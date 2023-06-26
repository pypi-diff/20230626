# Comparing `tmp/mse_cli_core-0.1a7.tar.gz` & `tmp/mse_cli_core-0.1a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mse_cli_core-0.1a7.tar", last modified: Fri Jun 23 07:12:22 2023, max compression
+gzip compressed data, was "mse_cli_core-0.1a8.tar", last modified: Mon Jun 26 07:06:00 2023, max compression
```

## Comparing `mse_cli_core-0.1a7.tar` & `mse_cli_core-0.1a8.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:12:22.305821 mse_cli_core-0.1a7/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-23 07:12:22.305821 mse_cli_core-0.1a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-23 07:12:22.305821 mse_cli_core-0.1a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:12:22.293821 mse_cli_core-0.1a7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:12:22.301821 mse_cli_core-0.1a7/src/mse_cli_core/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/clock_tick.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/enclave.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/ignore_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/no_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/spinner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/src/mse_cli_core/test_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:12:22.301821 mse_cli_core-0.1a7/src/mse_cli_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-23 07:12:22.000000 mse_cli_core-0.1a7/src/mse_cli_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-23 07:12:22.000000 mse_cli_core-0.1a7/src/mse_cli_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:12:22.000000 mse_cli_core-0.1a7/src/mse_cli_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-23 07:12:22.000000 mse_cli_core-0.1a7/src/mse_cli_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 07:12:22.000000 mse_cli_core-0.1a7/src/mse_cli_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:12:22.000000 mse_cli_core-0.1a7/src/mse_cli_core.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:12:22.301821 mse_cli_core-0.1a7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/tests/test_base64.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/tests/test_boostrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/tests/test_ignore_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/tests/test_no_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/tests/test_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-23 07:11:53.000000 mse_cli_core-0.1a7/tests/test_test_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:06:00.401110 mse_cli_core-0.1a8/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-26 07:06:00.401110 mse_cli_core-0.1a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-26 07:06:00.405110 mse_cli_core-0.1a8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:06:00.393110 mse_cli_core-0.1a8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:06:00.397110 mse_cli_core-0.1a8/src/mse_cli_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/clock_tick.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10184 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/enclave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/ignore_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/no_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/src/mse_cli_core/test_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:06:00.401110 mse_cli_core-0.1a8/src/mse_cli_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-26 07:06:00.000000 mse_cli_core-0.1a8/src/mse_cli_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-26 07:06:00.000000 mse_cli_core-0.1a8/src/mse_cli_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 07:06:00.000000 mse_cli_core-0.1a8/src/mse_cli_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-26 07:06:00.000000 mse_cli_core-0.1a8/src/mse_cli_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 07:06:00.000000 mse_cli_core-0.1a8/src/mse_cli_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 07:06:00.000000 mse_cli_core-0.1a8/src/mse_cli_core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 07:06:00.401110 mse_cli_core-0.1a8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/tests/test_base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/tests/test_boostrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12210 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/tests/test_ignore_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/tests/test_no_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/tests/test_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-26 07:05:30.000000 mse_cli_core-0.1a8/tests/test_test_docker.py
```

### Comparing `mse_cli_core-0.1a7/PKG-INFO` & `mse_cli_core-0.1a8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse_cli_core
-Version: 0.1a7
+Version: 0.1a8
 Summary: Utils for MicroService Encryption Python CLIs
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Project-URL: Documentation, https://docs.cosmian.com
 Project-URL: Source, https://github.com/Cosmian/mse-cli-core
```

### Comparing `mse_cli_core-0.1a7/setup.cfg` & `mse_cli_core-0.1a8/setup.cfg`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a7/setup.py` & `mse_cli_core-0.1a8/setup.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a7/src/mse_cli_core/base64.py` & `mse_cli_core-0.1a8/src/mse_cli_core/base64.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a7/src/mse_cli_core/bootstrap.py` & `mse_cli_core-0.1a8/src/mse_cli_core/bootstrap.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a7/src/mse_cli_core/clock_tick.py` & `mse_cli_core-0.1a8/src/mse_cli_core/clock_tick.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a7/src/mse_cli_core/enclave.py` & `mse_cli_core-0.1a8/src/mse_cli_core/enclave.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a7/src/mse_cli_core/fs.py` & `mse_cli_core-0.1a8/src/mse_cli_core/fs.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a7/src/mse_cli_core/ignore_file.py` & `mse_cli_core-0.1a8/src/mse_cli_core/ignore_file.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a7/src/mse_cli_core/no_sgx_docker.py` & `mse_cli_core-0.1a8/src/mse_cli_core/no_sgx_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a7/src/mse_cli_core/sgx_docker.py` & `mse_cli_core-0.1a8/src/mse_cli_core/sgx_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a7/src/mse_cli_core/spinner.py` & `mse_cli_core-0.1a8/src/mse_cli_core/spinner.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a7/src/mse_cli_core/test_docker.py` & `mse_cli_core-0.1a8/src/mse_cli_core/test_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a7/src/mse_cli_core.egg-info/PKG-INFO` & `mse_cli_core-0.1a8/src/mse_cli_core.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse-cli-core
-Version: 0.1a7
+Version: 0.1a8
 Summary: Utils for MicroService Encryption Python CLIs
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Project-URL: Documentation, https://docs.cosmian.com
 Project-URL: Source, https://github.com/Cosmian/mse-cli-core
```

### Comparing `mse_cli_core-0.1a7/src/mse_cli_core.egg-info/SOURCES.txt` & `mse_cli_core-0.1a8/src/mse_cli_core.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.md
 setup.cfg
 setup.py
 src/mse_cli_core/__init__.py
 src/mse_cli_core/base64.py
 src/mse_cli_core/bootstrap.py
 src/mse_cli_core/clock_tick.py
+src/mse_cli_core/conf.py
 src/mse_cli_core/enclave.py
 src/mse_cli_core/fs.py
 src/mse_cli_core/ignore_file.py
 src/mse_cli_core/no_sgx_docker.py
 src/mse_cli_core/sgx_docker.py
 src/mse_cli_core/spinner.py
 src/mse_cli_core/test_docker.py
@@ -16,11 +17,12 @@
 src/mse_cli_core.egg-info/SOURCES.txt
 src/mse_cli_core.egg-info/dependency_links.txt
 src/mse_cli_core.egg-info/requires.txt
 src/mse_cli_core.egg-info/top_level.txt
 src/mse_cli_core.egg-info/zip-safe
 tests/test_base64.py
 tests/test_boostrap.py
+tests/test_conf.py
 tests/test_ignore_file.py
 tests/test_no_sgx_docker.py
 tests/test_sgx_docker.py
 tests/test_test_docker.py
```

### Comparing `mse_cli_core-0.1a7/tests/test_base64.py` & `mse_cli_core-0.1a8/tests/test_base64.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a7/tests/test_boostrap.py` & `mse_cli_core-0.1a8/tests/test_boostrap.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a7/tests/test_ignore_file.py` & `mse_cli_core-0.1a8/tests/test_ignore_file.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a7/tests/test_no_sgx_docker.py` & `mse_cli_core-0.1a8/tests/test_no_sgx_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a7/tests/test_sgx_docker.py` & `mse_cli_core-0.1a8/tests/test_sgx_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a7/tests/test_test_docker.py` & `mse_cli_core-0.1a8/tests/test_test_docker.py`

 * *Files identical despite different names*

