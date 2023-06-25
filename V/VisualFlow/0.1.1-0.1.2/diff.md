# Comparing `tmp/VisualFlow-0.1.1.tar.gz` & `tmp/VisualFlow-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisualFlow-0.1.1.tar", last modified: Sun Jun 25 22:41:49 2023, max compression
+gzip compressed data, was "VisualFlow-0.1.2.tar", last modified: Sun Jun 25 22:53:46 2023, max compression
```

## Comparing `VisualFlow-0.1.1.tar` & `VisualFlow-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 22:41:49.297432 VisualFlow-0.1.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4134 2023-06-25 22:41:49.297432 VisualFlow-0.1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2651 2023-06-25 22:23:46.000000 VisualFlow-0.1.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 22:41:49.297432 VisualFlow-0.1.1/VisualFlow.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4134 2023-06-25 22:41:49.000000 VisualFlow-0.1.1/VisualFlow.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      221 2023-06-25 22:41:49.000000 VisualFlow-0.1.1/VisualFlow.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-25 22:41:49.000000 VisualFlow-0.1.1/VisualFlow.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-06-25 22:41:49.000000 VisualFlow-0.1.1/VisualFlow.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        4 2023-06-25 22:41:49.000000 VisualFlow-0.1.1/VisualFlow.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-25 22:41:49.297432 VisualFlow-0.1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1011 2023-06-25 22:41:21.000000 VisualFlow-0.1.1/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 22:41:49.297432 VisualFlow-0.1.1/src/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 22:23:46.000000 VisualFlow-0.1.1/src/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18981 2023-06-25 22:23:46.000000 VisualFlow-0.1.1/src/visualflow.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 22:53:46.601877 VisualFlow-0.1.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4134 2023-06-25 22:53:46.597877 VisualFlow-0.1.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2651 2023-06-25 22:23:46.000000 VisualFlow-0.1.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 22:53:46.597877 VisualFlow-0.1.2/VisualFlow.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4134 2023-06-25 22:53:46.000000 VisualFlow-0.1.2/VisualFlow.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      221 2023-06-25 22:53:46.000000 VisualFlow-0.1.2/VisualFlow.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-25 22:53:46.000000 VisualFlow-0.1.2/VisualFlow.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-06-25 22:53:46.000000 VisualFlow-0.1.2/VisualFlow.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        4 2023-06-25 22:53:46.000000 VisualFlow-0.1.2/VisualFlow.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-25 22:53:46.601877 VisualFlow-0.1.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1011 2023-06-25 22:52:49.000000 VisualFlow-0.1.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 22:53:46.597877 VisualFlow-0.1.2/src/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-25 22:23:46.000000 VisualFlow-0.1.2/src/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18981 2023-06-25 22:23:46.000000 VisualFlow-0.1.2/src/visualflow.py
```

### Comparing `VisualFlow-0.1.1/PKG-INFO` & `VisualFlow-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisualFlow
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library for object detection format conversion
 Home-page: https://github.com/Ojas-Sharma/VisualFlow
 Author: Ojas Sharma
 Author-email: ojassharma1607@gmail.com
 License: UNKNOWN
 Description: # VisualFlow
```

### Comparing `VisualFlow-0.1.1/README.md` & `VisualFlow-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `VisualFlow-0.1.1/VisualFlow.egg-info/PKG-INFO` & `VisualFlow-0.1.2/VisualFlow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisualFlow
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library for object detection format conversion
 Home-page: https://github.com/Ojas-Sharma/VisualFlow
 Author: Ojas Sharma
 Author-email: ojassharma1607@gmail.com
 License: UNKNOWN
 Description: # VisualFlow
```

### Comparing `VisualFlow-0.1.1/setup.py` & `VisualFlow-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='VisualFlow',
-    version='0.1.1',
+    version='0.1.2',
     author='Ojas Sharma',
     author_email='ojassharma1607@gmail.com',
     description='A Python library for object detection format conversion',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Ojas-Sharma/VisualFlow',
     packages=find_packages(),
```

### Comparing `VisualFlow-0.1.1/src/visualflow.py` & `VisualFlow-0.1.2/src/visualflow.py`

 * *Files identical despite different names*
