# Comparing `tmp/VisualFlow-0.1.3.tar.gz` & `tmp/VisualFlow-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisualFlow-0.1.3.tar", last modified: Mon Jun 26 02:30:25 2023, max compression
+gzip compressed data, was "VisualFlow-0.1.4.tar", last modified: Mon Jun 26 02:46:50 2023, max compression
```

## Comparing `VisualFlow-0.1.3.tar` & `VisualFlow-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 02:30:25.433817 VisualFlow-0.1.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4134 2023-06-26 02:30:25.433817 VisualFlow-0.1.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2651 2023-06-25 22:23:46.000000 VisualFlow-0.1.3/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 02:30:25.433817 VisualFlow-0.1.3/VisualFlow/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       24 2023-06-26 02:25:04.000000 VisualFlow-0.1.3/VisualFlow/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18981 2023-06-25 22:23:46.000000 VisualFlow-0.1.3/VisualFlow/visualflow.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 02:30:25.433817 VisualFlow-0.1.3/VisualFlow.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4134 2023-06-26 02:30:25.000000 VisualFlow-0.1.3/VisualFlow.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      235 2023-06-26 02:30:25.000000 VisualFlow-0.1.3/VisualFlow.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-26 02:30:25.000000 VisualFlow-0.1.3/VisualFlow.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-06-26 02:30:25.000000 VisualFlow-0.1.3/VisualFlow.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-06-26 02:30:25.000000 VisualFlow-0.1.3/VisualFlow.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-26 02:30:25.433817 VisualFlow-0.1.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1011 2023-06-26 02:30:00.000000 VisualFlow-0.1.3/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 02:46:50.195799 VisualFlow-0.1.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4134 2023-06-26 02:46:50.195799 VisualFlow-0.1.4/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2651 2023-06-25 22:23:46.000000 VisualFlow-0.1.4/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 02:46:50.195799 VisualFlow-0.1.4/VisualFlow/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       35 2023-06-26 02:45:48.000000 VisualFlow-0.1.4/VisualFlow/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18981 2023-06-25 22:23:46.000000 VisualFlow-0.1.4/VisualFlow/visualflow.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-26 02:46:50.195799 VisualFlow-0.1.4/VisualFlow.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4134 2023-06-26 02:46:50.000000 VisualFlow-0.1.4/VisualFlow.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      235 2023-06-26 02:46:50.000000 VisualFlow-0.1.4/VisualFlow.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-26 02:46:50.000000 VisualFlow-0.1.4/VisualFlow.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2023-06-26 02:46:50.000000 VisualFlow-0.1.4/VisualFlow.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-06-26 02:46:50.000000 VisualFlow-0.1.4/VisualFlow.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-26 02:46:50.195799 VisualFlow-0.1.4/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1011 2023-06-26 02:46:12.000000 VisualFlow-0.1.4/setup.py
```

### Comparing `VisualFlow-0.1.3/PKG-INFO` & `VisualFlow-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisualFlow
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python library for object detection format conversion
 Home-page: https://github.com/Ojas-Sharma/VisualFlow
 Author: Ojas Sharma
 Author-email: ojassharma1607@gmail.com
 License: UNKNOWN
 Description: # VisualFlow
```

### Comparing `VisualFlow-0.1.3/README.md` & `VisualFlow-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `VisualFlow-0.1.3/VisualFlow/visualflow.py` & `VisualFlow-0.1.4/VisualFlow/visualflow.py`

 * *Files identical despite different names*

### Comparing `VisualFlow-0.1.3/VisualFlow.egg-info/PKG-INFO` & `VisualFlow-0.1.4/VisualFlow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisualFlow
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python library for object detection format conversion
 Home-page: https://github.com/Ojas-Sharma/VisualFlow
 Author: Ojas Sharma
 Author-email: ojassharma1607@gmail.com
 License: UNKNOWN
 Description: # VisualFlow
```

### Comparing `VisualFlow-0.1.3/setup.py` & `VisualFlow-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='VisualFlow',
-    version='0.1.3',
+    version='0.1.4',
     author='Ojas Sharma',
     author_email='ojassharma1607@gmail.com',
     description='A Python library for object detection format conversion',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Ojas-Sharma/VisualFlow',
     packages=find_packages(),
```

