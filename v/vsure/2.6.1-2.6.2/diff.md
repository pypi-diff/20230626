# Comparing `tmp/vsure-2.6.1.tar.gz` & `tmp/vsure-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsure-2.6.1.tar", last modified: Sun Mar  5 19:59:59 2023, max compression
+gzip compressed data, was "vsure-2.6.2.tar", last modified: Mon Jun 26 08:15:38 2023, max compression
```

## Comparing `vsure-2.6.1.tar` & `vsure-2.6.2.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxr-x   0 per       (1000) per       (1000)        0 2023-03-05 19:59:59.742977 vsure-2.6.1/
--rw-rw-r--   0 per       (1000) per       (1000)     1082 2020-06-25 19:31:35.000000 vsure-2.6.1/LICENSE
--rw-rw-r--   0 per       (1000) per       (1000)       16 2020-10-28 18:46:19.000000 vsure-2.6.1/MANIFEST.in
--rw-rw-r--   0 per       (1000) per       (1000)      728 2023-03-05 19:59:59.738977 vsure-2.6.1/PKG-INFO
--rw-rw-r--   0 per       (1000) per       (1000)     7410 2023-03-05 19:52:47.000000 vsure-2.6.1/README.md
--rw-rw-r--   0 per       (1000) per       (1000)       38 2023-03-05 19:59:59.742977 vsure-2.6.1/setup.cfg
--rw-rw-r--   0 per       (1000) per       (1000)     1095 2023-03-05 19:44:35.000000 vsure-2.6.1/setup.py
-drwxrwxr-x   0 per       (1000) per       (1000)        0 2023-03-05 19:59:59.734977 vsure-2.6.1/test/
--rw-rw-r--   0 per       (1000) per       (1000)     1672 2022-09-10 14:24:33.000000 vsure-2.6.1/test/test_base_url_func.py
-drwxrwxr-x   0 per       (1000) per       (1000)        0 2023-03-05 19:59:59.738977 vsure-2.6.1/verisure/
--rw-rw-r--   0 per       (1000) per       (1000)      480 2023-03-05 19:53:49.000000 vsure-2.6.1/verisure/__init__.py
--rw-rw-r--   0 per       (1000) per       (1000)     4639 2023-03-05 19:53:57.000000 vsure-2.6.1/verisure/__main__.py
--rw-rw-r--   0 per       (1000) per       (1000)    34493 2023-03-05 19:43:01.000000 vsure-2.6.1/verisure/session.py
--rw-rw-r--   0 per       (1000) per       (1000)      699 2022-11-22 21:55:31.000000 vsure-2.6.1/verisure/verisure.py
-drwxrwxr-x   0 per       (1000) per       (1000)        0 2023-03-05 19:59:59.738977 vsure-2.6.1/vsure.egg-info/
--rw-r--r--   0 per       (1000) per       (1000)      728 2023-03-05 19:59:59.000000 vsure-2.6.1/vsure.egg-info/PKG-INFO
--rw-r--r--   0 per       (1000) per       (1000)      348 2023-03-05 19:59:59.000000 vsure-2.6.1/vsure.egg-info/SOURCES.txt
--rw-r--r--   0 per       (1000) per       (1000)        1 2023-03-05 19:59:59.000000 vsure-2.6.1/vsure.egg-info/dependency_links.txt
--rw-r--r--   0 per       (1000) per       (1000)       67 2023-03-05 19:59:59.000000 vsure-2.6.1/vsure.egg-info/entry_points.txt
--rw-r--r--   0 per       (1000) per       (1000)       32 2023-03-05 19:59:59.000000 vsure-2.6.1/vsure.egg-info/requires.txt
--rw-r--r--   0 per       (1000) per       (1000)        9 2023-03-05 19:59:59.000000 vsure-2.6.1/vsure.egg-info/top_level.txt
--rw-r--r--   0 per       (1000) per       (1000)        1 2020-06-25 19:36:24.000000 vsure-2.6.1/vsure.egg-info/zip-safe
+drwxrwxr-x   0 per       (1000) per       (1000)        0 2023-06-26 08:15:38.866215 vsure-2.6.2/
+-rw-rw-r--   0 per       (1000) per       (1000)     1082 2020-06-25 19:31:35.000000 vsure-2.6.2/LICENSE
+-rw-rw-r--   0 per       (1000) per       (1000)       16 2020-10-28 18:46:19.000000 vsure-2.6.2/MANIFEST.in
+-rw-rw-r--   0 per       (1000) per       (1000)      739 2023-06-26 08:15:38.866215 vsure-2.6.2/PKG-INFO
+-rw-rw-r--   0 per       (1000) per       (1000)     7436 2023-06-26 08:14:50.000000 vsure-2.6.2/README.md
+-rw-rw-r--   0 per       (1000) per       (1000)       38 2023-06-26 08:15:38.866215 vsure-2.6.2/setup.cfg
+-rw-rw-r--   0 per       (1000) per       (1000)     1095 2023-06-26 08:14:50.000000 vsure-2.6.2/setup.py
+drwxrwxr-x   0 per       (1000) per       (1000)        0 2023-06-26 08:15:38.866215 vsure-2.6.2/test/
+-rw-rw-r--   0 per       (1000) per       (1000)     1672 2022-09-10 14:24:33.000000 vsure-2.6.2/test/test_base_url_func.py
+drwxrwxr-x   0 per       (1000) per       (1000)        0 2023-06-26 08:15:38.866215 vsure-2.6.2/verisure/
+-rw-rw-r--   0 per       (1000) per       (1000)      480 2023-06-26 08:14:45.000000 vsure-2.6.2/verisure/__init__.py
+-rw-rw-r--   0 per       (1000) per       (1000)     4639 2023-06-26 08:14:45.000000 vsure-2.6.2/verisure/__main__.py
+-rw-rw-r--   0 per       (1000) per       (1000)    34464 2023-06-26 08:14:50.000000 vsure-2.6.2/verisure/session.py
+drwxrwxr-x   0 per       (1000) per       (1000)        0 2023-06-26 08:15:38.866215 vsure-2.6.2/vsure.egg-info/
+-rw-r--r--   0 per       (1000) per       (1000)      739 2023-06-26 08:15:38.000000 vsure-2.6.2/vsure.egg-info/PKG-INFO
+-rw-r--r--   0 per       (1000) per       (1000)      327 2023-06-26 08:15:38.000000 vsure-2.6.2/vsure.egg-info/SOURCES.txt
+-rw-r--r--   0 per       (1000) per       (1000)        1 2023-06-26 08:15:38.000000 vsure-2.6.2/vsure.egg-info/dependency_links.txt
+-rw-r--r--   0 per       (1000) per       (1000)       67 2023-06-26 08:15:38.000000 vsure-2.6.2/vsure.egg-info/entry_points.txt
+-rw-r--r--   0 per       (1000) per       (1000)       32 2023-06-26 08:15:38.000000 vsure-2.6.2/vsure.egg-info/requires.txt
+-rw-r--r--   0 per       (1000) per       (1000)        9 2023-06-26 08:15:38.000000 vsure-2.6.2/vsure.egg-info/top_level.txt
+-rw-r--r--   0 per       (1000) per       (1000)        1 2020-06-25 19:36:24.000000 vsure-2.6.2/vsure.egg-info/zip-safe
```

### Comparing `vsure-2.6.1/LICENSE` & `vsure-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vsure-2.6.1/PKG-INFO` & `vsure-2.6.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: vsure
-Version: 2.6.1
+Version: 2.6.2
 Summary: Read and change status of verisure devices through mypages.
 Home-page: http://github.com/persandstrom/python-verisure
 Author: Per Sandstrom
 Author-email: per.j.sandstrom@gmail.com
 License: MIT
-Description: A python3 module for reading and changing status of verisure devices through mypages.
 Keywords: home automation verisure
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+License-File: LICENSE
+
+A python3 module for reading and changing status of verisure devices through mypages.
+
```

### Comparing `vsure-2.6.1/README.md` & `vsure-2.6.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 This software is not affiliated with Verisure Holding AB and the developers take no
 legal responsibility for the functionality or security of your Verisure Alarms and
 devices.
 
 ## Version History
 
 ```txt
+2.6.2 Fix request wrapper
 2.6.1 Move to automation subdomain
 2.6.0 Add Get Firmware Version
 2.5.6 Fix docstring, cookie lasts 15 minutes
 2.5.5 Solved bug during response error except using CLI
 2.5.4 Add possibility to set giid to all queries, refactoring and resolve lint warnings
 2.5.3 Refactor login
 2.5.2 Fix XBN Database is not activated
```

### Comparing `vsure-2.6.1/setup.py` & `vsure-2.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Setup for python-verisure """
 
 from setuptools import setup
 
 setup(
     name='vsure',
-    version='2.6.1',
+    version='2.6.2',
     description='Read and change status of verisure devices through mypages.',
     long_description='A python3 module for reading and changing status of '
     + 'verisure devices through mypages.',
     url='http://github.com/persandstrom/python-verisure',
     author='Per Sandstrom',
     author_email='per.j.sandstrom@gmail.com',
     license='MIT',
```

### Comparing `vsure-2.6.1/test/test_base_url_func.py` & `vsure-2.6.2/test/test_base_url_func.py`

 * *Files identical despite different names*

### Comparing `vsure-2.6.1/verisure/__main__.py` & `vsure-2.6.2/verisure/__main__.py`

 * *Files identical despite different names*

### Comparing `vsure-2.6.1/verisure/session.py` & `vsure-2.6.2/verisure/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                 try:
                     response = function(base_url+url, *args, **kwargs)
                     if response.status_code == 200:
                         if "SYS_00004" in response.text:
                             self._base_urls.reverse()
                             continue
                         return response
-                    raise ResponseError(response.status_code, response.text)
+                    response.raise_for_status()
                 except requests.exceptions.RequestException as ex:
                     last_exception = ex
                 self._base_urls.reverse()
             raise Error from last_exception
         return wrapper
```

### Comparing `vsure-2.6.1/vsure.egg-info/PKG-INFO` & `vsure-2.6.2/vsure.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: vsure
-Version: 2.6.1
+Version: 2.6.2
 Summary: Read and change status of verisure devices through mypages.
 Home-page: http://github.com/persandstrom/python-verisure
 Author: Per Sandstrom
 Author-email: per.j.sandstrom@gmail.com
 License: MIT
-Description: A python3 module for reading and changing status of verisure devices through mypages.
 Keywords: home automation verisure
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+License-File: LICENSE
+
+A python3 module for reading and changing status of verisure devices through mypages.
+
```

