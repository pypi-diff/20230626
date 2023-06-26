# Comparing `tmp/galaxy-test-driver-23.0.2.tar.gz` & `tmp/galaxy-test-driver-23.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/test_driver/dist/.tmp-7_e31_r8/galaxy-test-driver-23.0.2.tar", last modified: Tue Jun 13 17:14:48 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/test_driver/dist/.tmp-e8zys88p/galaxy-test-driver-23.0.3.tar", last modified: Mon Jun 26 09:58:03 2023, max compression
```

## Comparing `galaxy-test-driver-23.0.2.tar` & `galaxy-test-driver-23.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-13 17:04:36.000000 galaxy-test-driver-23.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/galaxy_test/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/galaxy_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/galaxy_test/driver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/galaxy_test/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43296 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/galaxy_test/driver/driver_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/galaxy_test/driver/integration_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/galaxy_test/driver/integration_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/galaxy_test/driver/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/galaxy_test/driver/testcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/galaxy_test/driver/uses_shed.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/galaxy_test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/galaxy_test_driver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/galaxy_test_driver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/galaxy_test_driver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/galaxy_test_driver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/galaxy_test_driver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/galaxy_test_driver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:58:03.000000 galaxy-test-driver-23.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-26 09:48:33.000000 galaxy-test-driver-23.0.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-26 09:48:32.000000 galaxy-test-driver-23.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 09:48:33.000000 galaxy-test-driver-23.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-26 09:58:03.000000 galaxy-test-driver-23.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-26 09:48:33.000000 galaxy-test-driver-23.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 09:48:33.000000 galaxy-test-driver-23.0.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:58:03.000000 galaxy-test-driver-23.0.3/galaxy_test/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-26 09:48:33.000000 galaxy-test-driver-23.0.3/galaxy_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:58:03.000000 galaxy-test-driver-23.0.3/galaxy_test/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:48:33.000000 galaxy-test-driver-23.0.3/galaxy_test/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43296 2023-06-26 09:48:33.000000 galaxy-test-driver-23.0.3/galaxy_test/driver/driver_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-26 09:48:33.000000 galaxy-test-driver-23.0.3/galaxy_test/driver/integration_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-26 09:48:33.000000 galaxy-test-driver-23.0.3/galaxy_test/driver/integration_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-26 09:48:33.000000 galaxy-test-driver-23.0.3/galaxy_test/driver/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-26 09:48:33.000000 galaxy-test-driver-23.0.3/galaxy_test/driver/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-26 09:48:33.000000 galaxy-test-driver-23.0.3/galaxy_test/driver/uses_shed.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:48:33.000000 galaxy-test-driver-23.0.3/galaxy_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:58:03.000000 galaxy-test-driver-23.0.3/galaxy_test_driver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-26 09:58:03.000000 galaxy-test-driver-23.0.3/galaxy_test_driver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-26 09:58:03.000000 galaxy-test-driver-23.0.3/galaxy_test_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:58:03.000000 galaxy-test-driver-23.0.3/galaxy_test_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-26 09:58:03.000000 galaxy-test-driver-23.0.3/galaxy_test_driver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 09:58:03.000000 galaxy-test-driver-23.0.3/galaxy_test_driver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 09:48:33.000000 galaxy-test-driver-23.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-26 09:58:03.000000 galaxy-test-driver-23.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 09:48:33.000000 galaxy-test-driver-23.0.3/test-requirements.txt
```

### Comparing `galaxy-test-driver-23.0.2/LICENSE` & `galaxy-test-driver-23.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-test-driver-23.0.2/PKG-INFO` & `galaxy-test-driver-23.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-test-driver
-Version: 23.0.2
+Version: 23.0.3
 Summary: Galaxy test driver
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,14 +43,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.3 (2023-06-26)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.2 (2023-06-13)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.1 (2023-06-08)
```

### Comparing `galaxy-test-driver-23.0.2/galaxy_test/driver/driver_util.py` & `galaxy-test-driver-23.0.3/galaxy_test/driver/driver_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-driver-23.0.2/galaxy_test/driver/integration_setup.py` & `galaxy-test-driver-23.0.3/galaxy_test/driver/integration_setup.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-driver-23.0.2/galaxy_test/driver/integration_util.py` & `galaxy-test-driver-23.0.3/galaxy_test/driver/integration_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-driver-23.0.2/galaxy_test/driver/uses_shed.py` & `galaxy-test-driver-23.0.3/galaxy_test/driver/uses_shed.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-driver-23.0.2/galaxy_test_driver.egg-info/PKG-INFO` & `galaxy-test-driver-23.0.3/galaxy_test_driver.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-test-driver
-Version: 23.0.2
+Version: 23.0.3
 Summary: Galaxy test driver
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -43,14 +43,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.3 (2023-06-26)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.2 (2023-06-13)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.1 (2023-06-08)
```

### Comparing `galaxy-test-driver-23.0.2/galaxy_test_driver.egg-info/SOURCES.txt` & `galaxy-test-driver-23.0.3/galaxy_test_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-test-driver-23.0.2/setup.cfg` & `galaxy-test-driver-23.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-test-driver
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.2
+version = 23.0.3
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-app
 	galaxy-config
 	galaxy-data
```

