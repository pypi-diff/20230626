# Comparing `tmp/pyintelx-0.0.6.tar.gz` & `tmp/pyintelx-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyintelx-0.0.6.tar", last modified: Mon Jun 26 19:28:26 2023, max compression
+gzip compressed data, was "pyintelx-0.0.8.tar", last modified: Mon Jun 26 19:32:48 2023, max compression
```

## Comparing `pyintelx-0.0.6.tar` & `pyintelx-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:28:26.946318 pyintelx-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-26 19:28:26.946318 pyintelx-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-26 19:28:17.000000 pyintelx-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:28:26.946318 pyintelx-0.0.6/pyintelx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:28:17.000000 pyintelx-0.0.6/pyintelx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:28:26.946318 pyintelx-0.0.6/pyintelx/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-06-26 19:28:17.000000 pyintelx-0.0.6/pyintelx/cli/pyintelx
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-26 19:28:17.000000 pyintelx-0.0.6/pyintelx/intelx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:28:26.946318 pyintelx-0.0.6/pyintelx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-26 19:28:26.000000 pyintelx-0.0.6/pyintelx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-26 19:28:26.000000 pyintelx-0.0.6/pyintelx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:28:26.000000 pyintelx-0.0.6/pyintelx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 19:28:26.000000 pyintelx-0.0.6/pyintelx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 19:28:26.000000 pyintelx-0.0.6/pyintelx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 19:28:26.946318 pyintelx-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-26 19:28:17.000000 pyintelx-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:32:48.082282 pyintelx-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-26 19:32:48.078282 pyintelx-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-26 19:32:38.000000 pyintelx-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:32:48.078282 pyintelx-0.0.8/pyintelx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:32:38.000000 pyintelx-0.0.8/pyintelx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:32:48.078282 pyintelx-0.0.8/pyintelx/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-06-26 19:32:38.000000 pyintelx-0.0.8/pyintelx/cli/pyintelx
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-26 19:32:38.000000 pyintelx-0.0.8/pyintelx/intelx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:32:48.078282 pyintelx-0.0.8/pyintelx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-26 19:32:48.000000 pyintelx-0.0.8/pyintelx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-26 19:32:48.000000 pyintelx-0.0.8/pyintelx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:32:48.000000 pyintelx-0.0.8/pyintelx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 19:32:48.000000 pyintelx-0.0.8/pyintelx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 19:32:48.000000 pyintelx-0.0.8/pyintelx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 19:32:48.082282 pyintelx-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-26 19:32:38.000000 pyintelx-0.0.8/setup.py
```

### Comparing `pyintelx-0.0.6/PKG-INFO` & `pyintelx-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyintelx
-Version: 0.0.6
+Version: 0.0.8
 Summary: This lib add support to use the Identity API from Intelx.io
 Home-page: https://github.com/csirtamericas/pyintelxio
 Author: Fermin Baudino, Einar Lanfranco
 License: MIT
 Keywords: python, package, distribution
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -21,64 +21,64 @@
 
 Original source could be find here: *https://github.com/IntelligenceX/SDK/tree/master/Python*
 
 Installation
 ------------
 
 ```bash
-pip3 install pyintelxio
+pip3 install pyintelx
 ```
 
 Usage as command
 ================
 
 ```bash 
 
-pyintelxio -apikey {API_KEY} -search {search_term} -limit 10 
+pyintelx -apikey {API_KEY} -search {search_term} -limit 10 
 
-pyintelxio -apikey {API_KEY} -search {search_term} -limit 10 --identityenabled
+pyintelx -apikey {API_KEY} -search {search_term} -limit 10 --identityenabled
 
 ```
 
 SEARCH EXAMPLES
 ---------------
 
 * Query for 10 leaks containing pepe@example.com in intelx.io API
 
 ```bash
-pyintelxio -apikey {API_KEY} search -search pepe@example.com -limit 10
+pyintelx -apikey {API_KEY} search -search pepe@example.com -limit 10
 ```
 
 * Query for 10 leaks of accounts and passwords for domain example.com in identity.intelx.io API
 
 ```bash
-pyintelxio -apikey {API_KEY} -search example.com -limit 10 --identityenabled
+pyintelx -apikey {API_KEY} -search example.com -limit 10 --identityenabled
 ```
 * Download some leak file identied by SYSTEM_ID from some previous search
 
 ```bash
-pyintelxio -apikey {API_KEY} -download {SYSTEM_ID} -name {FILE_NAME} -bucket {BUCKET_NAME}
+pyintelx -apikey {API_KEY} -download {SYSTEM_ID} -name {FILE_NAME} -bucket {BUCKET_NAME}
 ```
 
 
 Usage as library
 ================
 
 * Print account information
 
 ```python
-import pyintelxio
+import pyintelx
 api = 
 
 ```
 
 * Search for 
 
 ```python
-import pyintelxio
+import pyintelx
 ```
 
 ## Buckets list
 - darknet.tor
 - darknet.i2p
 - documents.public.scihub
 - dumpster
```

### Comparing `pyintelx-0.0.6/README.md` & `pyintelx-0.0.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -5,64 +5,64 @@
 
 Original source could be find here: *https://github.com/IntelligenceX/SDK/tree/master/Python*
 
 Installation
 ------------
 
 ```bash
-pip3 install pyintelxio
+pip3 install pyintelx
 ```
 
 Usage as command
 ================
 
 ```bash 
 
-pyintelxio -apikey {API_KEY} -search {search_term} -limit 10 
+pyintelx -apikey {API_KEY} -search {search_term} -limit 10 
 
-pyintelxio -apikey {API_KEY} -search {search_term} -limit 10 --identityenabled
+pyintelx -apikey {API_KEY} -search {search_term} -limit 10 --identityenabled
 
 ```
 
 SEARCH EXAMPLES
 ---------------
 
 * Query for 10 leaks containing pepe@example.com in intelx.io API
 
 ```bash
-pyintelxio -apikey {API_KEY} search -search pepe@example.com -limit 10
+pyintelx -apikey {API_KEY} search -search pepe@example.com -limit 10
 ```
 
 * Query for 10 leaks of accounts and passwords for domain example.com in identity.intelx.io API
 
 ```bash
-pyintelxio -apikey {API_KEY} -search example.com -limit 10 --identityenabled
+pyintelx -apikey {API_KEY} -search example.com -limit 10 --identityenabled
 ```
 * Download some leak file identied by SYSTEM_ID from some previous search
 
 ```bash
-pyintelxio -apikey {API_KEY} -download {SYSTEM_ID} -name {FILE_NAME} -bucket {BUCKET_NAME}
+pyintelx -apikey {API_KEY} -download {SYSTEM_ID} -name {FILE_NAME} -bucket {BUCKET_NAME}
 ```
 
 
 Usage as library
 ================
 
 * Print account information
 
 ```python
-import pyintelxio
+import pyintelx
 api = 
 
 ```
 
 * Search for 
 
 ```python
-import pyintelxio
+import pyintelx
 ```
 
 ## Buckets list
 - darknet.tor
 - darknet.i2p
 - documents.public.scihub
 - dumpster
```

### Comparing `pyintelx-0.0.6/pyintelx/cli/pyintelx` & `pyintelx-0.0.8/pyintelx/cli/pyintelx`

 * *Files identical despite different names*

### Comparing `pyintelx-0.0.6/pyintelx/intelx.py` & `pyintelx-0.0.8/pyintelx/intelx.py`

 * *Files identical despite different names*

### Comparing `pyintelx-0.0.6/pyintelx.egg-info/PKG-INFO` & `pyintelx-0.0.8/pyintelx.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyintelx
-Version: 0.0.6
+Version: 0.0.8
 Summary: This lib add support to use the Identity API from Intelx.io
 Home-page: https://github.com/csirtamericas/pyintelxio
 Author: Fermin Baudino, Einar Lanfranco
 License: MIT
 Keywords: python, package, distribution
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -21,64 +21,64 @@
 
 Original source could be find here: *https://github.com/IntelligenceX/SDK/tree/master/Python*
 
 Installation
 ------------
 
 ```bash
-pip3 install pyintelxio
+pip3 install pyintelx
 ```
 
 Usage as command
 ================
 
 ```bash 
 
-pyintelxio -apikey {API_KEY} -search {search_term} -limit 10 
+pyintelx -apikey {API_KEY} -search {search_term} -limit 10 
 
-pyintelxio -apikey {API_KEY} -search {search_term} -limit 10 --identityenabled
+pyintelx -apikey {API_KEY} -search {search_term} -limit 10 --identityenabled
 
 ```
 
 SEARCH EXAMPLES
 ---------------
 
 * Query for 10 leaks containing pepe@example.com in intelx.io API
 
 ```bash
-pyintelxio -apikey {API_KEY} search -search pepe@example.com -limit 10
+pyintelx -apikey {API_KEY} search -search pepe@example.com -limit 10
 ```
 
 * Query for 10 leaks of accounts and passwords for domain example.com in identity.intelx.io API
 
 ```bash
-pyintelxio -apikey {API_KEY} -search example.com -limit 10 --identityenabled
+pyintelx -apikey {API_KEY} -search example.com -limit 10 --identityenabled
 ```
 * Download some leak file identied by SYSTEM_ID from some previous search
 
 ```bash
-pyintelxio -apikey {API_KEY} -download {SYSTEM_ID} -name {FILE_NAME} -bucket {BUCKET_NAME}
+pyintelx -apikey {API_KEY} -download {SYSTEM_ID} -name {FILE_NAME} -bucket {BUCKET_NAME}
 ```
 
 
 Usage as library
 ================
 
 * Print account information
 
 ```python
-import pyintelxio
+import pyintelx
 api = 
 
 ```
 
 * Search for 
 
 ```python
-import pyintelxio
+import pyintelx
 ```
 
 ## Buckets list
 - darknet.tor
 - darknet.i2p
 - documents.public.scihub
 - dumpster
```

### Comparing `pyintelx-0.0.6/setup.py` & `pyintelx-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='pyintelx',
-    version='0.0.6',
+    version='0.0.8',
     description='This lib add support to use the Identity API from Intelx.io',
     install_requires=['requests'],
     license='MIT',
     keywords=['python, package, distribution'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Fermin Baudino, Einar Lanfranco',
```

