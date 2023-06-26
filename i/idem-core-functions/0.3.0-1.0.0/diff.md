# Comparing `tmp/idem-core-functions-0.3.0.tar.gz` & `tmp/idem-core-functions-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-core-functions-0.3.0.tar", last modified: Mon May 22 15:13:45 2023, max compression
+gzip compressed data, was "idem-core-functions-1.0.0.tar", last modified: Mon Jun 26 15:44:03 2023, max compression
```

## Comparing `idem-core-functions-0.3.0.tar` & `idem-core-functions-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:13:45.054485 idem-core-functions-0.3.0/
--rw-r--r--   0 root         (0) root         (0)    11345 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6551 2023-05-22 15:13:45.054485 idem-core-functions-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5737 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:13:45.054485 idem-core-functions-0.3.0/idem_core_functions/
--rw-r--r--   0 root         (0) root         (0)     1271 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/idem_core_functions/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:13:45.054485 idem-core-functions-0.3.0/idem_core_functions/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:13:45.054485 idem-core-functions-0.3.0/idem_core_functions/exec/core/
--rw-r--r--   0 root         (0) root         (0)     5094 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/idem_core_functions/exec/core/collection.py
--rw-r--r--   0 root         (0) root         (0)     7624 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/idem_core_functions/exec/core/conversion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:13:45.054485 idem-core-functions-0.3.0/idem_core_functions/exec/core/encoder/
--rw-r--r--   0 root         (0) root         (0)     2774 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/idem_core_functions/exec/core/encoder/base64.py
--rw-r--r--   0 root         (0) root         (0)     1877 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/idem_core_functions/exec/core/encoding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:13:45.054485 idem-core-functions-0.3.0/idem_core_functions/exec/core/encryption/
--rw-r--r--   0 root         (0) root         (0)     7334 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/idem_core_functions/exec/core/encryption/gpg.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/idem_core_functions/exec/core/string.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-22 15:13:44.000000 idem-core-functions-0.3.0/idem_core_functions/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:13:45.054485 idem-core-functions-0.3.0/idem_core_functions.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6551 2023-05-22 15:13:45.000000 idem-core-functions-0.3.0/idem_core_functions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      622 2023-05-22 15:13:45.000000 idem-core-functions-0.3.0/idem_core_functions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 15:13:45.000000 idem-core-functions-0.3.0/idem_core_functions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-22 15:13:45.000000 idem-core-functions-0.3.0/idem_core_functions.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-22 15:13:45.000000 idem-core-functions-0.3.0/idem_core_functions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-22 15:13:45.000000 idem-core-functions-0.3.0/idem_core_functions.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-22 15:13:45.054485 idem-core-functions-0.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2749 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:44:03.840370 idem-core-functions-1.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11345 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6551 2023-06-26 15:44:03.840370 idem-core-functions-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5737 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:44:03.836370 idem-core-functions-1.0.0/idem_core_functions/
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/idem_core_functions/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:44:03.836370 idem-core-functions-1.0.0/idem_core_functions/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:44:03.840370 idem-core-functions-1.0.0/idem_core_functions/exec/core/
+-rw-r--r--   0 root         (0) root         (0)     5094 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/idem_core_functions/exec/core/collection.py
+-rw-r--r--   0 root         (0) root         (0)     7624 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/idem_core_functions/exec/core/conversion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:44:03.840370 idem-core-functions-1.0.0/idem_core_functions/exec/core/encoder/
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/idem_core_functions/exec/core/encoder/base64.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/idem_core_functions/exec/core/encoding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:44:03.840370 idem-core-functions-1.0.0/idem_core_functions/exec/core/encryption/
+-rw-r--r--   0 root         (0) root         (0)     7334 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/idem_core_functions/exec/core/encryption/gpg.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/idem_core_functions/exec/core/string.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-26 15:44:03.000000 idem-core-functions-1.0.0/idem_core_functions/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 15:44:03.840370 idem-core-functions-1.0.0/idem_core_functions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6551 2023-06-26 15:44:03.000000 idem-core-functions-1.0.0/idem_core_functions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      622 2023-06-26 15:44:03.000000 idem-core-functions-1.0.0/idem_core_functions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 15:44:03.000000 idem-core-functions-1.0.0/idem_core_functions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-26 15:44:03.000000 idem-core-functions-1.0.0/idem_core_functions.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-06-26 15:44:03.000000 idem-core-functions-1.0.0/idem_core_functions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-26 15:44:03.000000 idem-core-functions-1.0.0/idem_core_functions.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-26 15:44:03.840370 idem-core-functions-1.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-06-26 15:43:49.000000 idem-core-functions-1.0.0/setup.py
```

### Comparing `idem-core-functions-0.3.0/LICENSE` & `idem-core-functions-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-core-functions-0.3.0/PKG-INFO` & `idem-core-functions-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-core-functions
-Version: 0.3.0
+Version: 1.0.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Barnali Rakshit
 Author-email: brakshit@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-core-functions-0.3.0/README.rst` & `idem-core-functions-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `idem-core-functions-0.3.0/idem_core_functions/conf.py` & `idem-core-functions-1.0.0/idem_core_functions/conf.py`

 * *Files identical despite different names*

### Comparing `idem-core-functions-0.3.0/idem_core_functions/exec/core/collection.py` & `idem-core-functions-1.0.0/idem_core_functions/exec/core/collection.py`

 * *Files identical despite different names*

### Comparing `idem-core-functions-0.3.0/idem_core_functions/exec/core/conversion.py` & `idem-core-functions-1.0.0/idem_core_functions/exec/core/conversion.py`

 * *Files identical despite different names*

### Comparing `idem-core-functions-0.3.0/idem_core_functions/exec/core/encoder/base64.py` & `idem-core-functions-1.0.0/idem_core_functions/exec/core/encoder/base64.py`

 * *Files identical despite different names*

### Comparing `idem-core-functions-0.3.0/idem_core_functions/exec/core/encoding.py` & `idem-core-functions-1.0.0/idem_core_functions/exec/core/encoding.py`

 * *Files identical despite different names*

### Comparing `idem-core-functions-0.3.0/idem_core_functions/exec/core/encryption/gpg.py` & `idem-core-functions-1.0.0/idem_core_functions/exec/core/encryption/gpg.py`

 * *Files identical despite different names*

### Comparing `idem-core-functions-0.3.0/idem_core_functions/exec/core/string.py` & `idem-core-functions-1.0.0/idem_core_functions/exec/core/string.py`

 * *Files identical despite different names*

### Comparing `idem-core-functions-0.3.0/idem_core_functions.egg-info/PKG-INFO` & `idem-core-functions-1.0.0/idem_core_functions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-core-functions
-Version: 0.3.0
+Version: 1.0.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Barnali Rakshit
 Author-email: brakshit@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-core-functions-0.3.0/idem_core_functions.egg-info/SOURCES.txt` & `idem-core-functions-1.0.0/idem_core_functions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-core-functions-0.3.0/setup.py` & `idem-core-functions-1.0.0/setup.py`

 * *Files identical despite different names*

