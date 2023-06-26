# Comparing `tmp/testflows-1.9.8.tar.gz` & `tmp/testflows-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows-1.9.8.tar", last modified: Tue May 31 16:57:09 2022, max compression
+gzip compressed data, was "testflows-1.9.9.tar", last modified: Tue May 31 22:34:12 2022, max compression
```

## Comparing `testflows-1.9.8.tar` & `testflows-1.9.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-05-31 16:57:09.655045 testflows-1.9.8/
--rw-rw-r--   0 user      (1000) user      (1000)     3660 2022-05-31 16:57:09.654044 testflows-1.9.8/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2383 2021-08-30 01:39:14.000000 testflows-1.9.8/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       38 2022-05-31 16:57:09.655045 testflows-1.9.8/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1840 2022-05-31 16:56:45.000000 testflows-1.9.8/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-05-31 16:57:09.653045 testflows-1.9.8/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-05-31 16:57:09.654044 testflows-1.9.8/testflows/version/
--rw-rw-r--   0 user      (1000) user      (1000)      739 2021-07-20 00:22:38.000000 testflows-1.9.8/testflows/version/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-05-31 16:57:09.654044 testflows-1.9.8/testflows.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3660 2022-05-31 16:57:09.000000 testflows-1.9.8/testflows.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      244 2022-05-31 16:57:09.000000 testflows-1.9.8/testflows.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-05-31 16:57:09.000000 testflows-1.9.8/testflows.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2021-08-30 01:58:25.000000 testflows-1.9.8/testflows.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)      231 2022-05-31 16:57:09.000000 testflows-1.9.8/testflows.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2022-05-31 16:57:09.000000 testflows-1.9.8/testflows.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-05-31 22:34:12.731317 testflows-1.9.9/
+-rw-rw-r--   0 user      (1000) user      (1000)     3660 2022-05-31 22:34:12.731317 testflows-1.9.9/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2383 2021-08-30 01:39:14.000000 testflows-1.9.9/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2022-05-31 22:34:12.731317 testflows-1.9.9/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1840 2022-05-31 22:33:45.000000 testflows-1.9.9/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-05-31 22:34:12.731317 testflows-1.9.9/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-05-31 22:34:12.731317 testflows-1.9.9/testflows/version/
+-rw-rw-r--   0 user      (1000) user      (1000)      739 2021-07-20 00:22:38.000000 testflows-1.9.9/testflows/version/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-05-31 22:34:12.731317 testflows-1.9.9/testflows.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3660 2022-05-31 22:34:12.000000 testflows-1.9.9/testflows.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      244 2022-05-31 22:34:12.000000 testflows-1.9.9/testflows.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2022-05-31 22:34:12.000000 testflows-1.9.9/testflows.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2021-08-30 01:58:25.000000 testflows-1.9.9/testflows.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)      231 2022-05-31 22:34:12.000000 testflows-1.9.9/testflows.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2022-05-31 22:34:12.000000 testflows-1.9.9/testflows.egg-info/top_level.txt
```

### Comparing `testflows-1.9.8/PKG-INFO` & `testflows-1.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows
-Version: 1.9.8
+Version: 1.9.9
 Summary: TestFlows.com Open-Source Software Testing Framework
 Home-page: https://github.com/testflows/testflows
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Description: # TestFlows.com Open-Source Software Testing Framework
```

### Comparing `testflows-1.9.8/README.md` & `testflows-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `testflows-1.9.8/setup.py` & `testflows-1.9.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 setup(
     name="testflows",
-    version="1.9.8",
+    version="1.9.9",
     description="TestFlows.com Open-Source Software Testing Framework",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/testflows/testflows",
     classifiers=[
@@ -35,15 +35,15 @@
     python_requires='>=3.8',
     license="Apache-2.0",
     packages=[
         "testflows.version"
     ],
     zip_safe=False,
     install_requires=[
-        "testflows.core==1.9.220531.1165602",
+        "testflows.core==1.9.220531.1223249",
         "testflows.asserts==6.4.211221.1165422",
         "testflows.stash==1.1.220510.1154615",
         "testflows.uexpect==1.6.210811.1002209",
         "testflows.connect==1.7.210811.1000931",
         "testflows.database==1.6.200713.1142213"
     ],
     extras_require={
```

### Comparing `testflows-1.9.8/testflows/version/__init__.py` & `testflows-1.9.9/testflows/version/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows-1.9.8/testflows.egg-info/PKG-INFO` & `testflows-1.9.9/testflows.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows
-Version: 1.9.8
+Version: 1.9.9
 Summary: TestFlows.com Open-Source Software Testing Framework
 Home-page: https://github.com/testflows/testflows
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Description: # TestFlows.com Open-Source Software Testing Framework
```

