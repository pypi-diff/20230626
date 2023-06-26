# Comparing `tmp/pyhandytools-0.0.1.tar.gz` & `tmp/pyhandytools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhandytools-0.0.1.tar", last modified: Sat Jun 24 16:05:40 2023, max compression
+gzip compressed data, was "pyhandytools-0.0.2.tar", last modified: Mon Jun 26 16:24:46 2023, max compression
```

## Comparing `pyhandytools-0.0.1.tar` & `pyhandytools-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jmchen     (501) staff       (20)        0 2023-06-24 16:05:40.600697 pyhandytools-0.0.1/
--rw-r--r--   0 jmchen     (501) staff       (20)    11354 2023-06-24 15:27:46.000000 pyhandytools-0.0.1/LICENSE
--rw-r--r--   0 jmchen     (501) staff       (20)      386 2023-06-24 16:05:40.600549 pyhandytools-0.0.1/PKG-INFO
--rw-r--r--   0 jmchen     (501) staff       (20)      102 2023-06-24 15:50:46.000000 pyhandytools-0.0.1/README.md
-drwxr-xr-x   0 jmchen     (501) staff       (20)        0 2023-06-24 16:05:40.599636 pyhandytools-0.0.1/pyhandytools/
--rw-r--r--   0 jmchen     (501) staff       (20)       48 2023-06-24 15:16:23.000000 pyhandytools-0.0.1/pyhandytools/__init__.py
--rw-r--r--   0 jmchen     (501) staff       (20)      712 2023-06-24 15:50:46.000000 pyhandytools-0.0.1/pyhandytools/file.py
-drwxr-xr-x   0 jmchen     (501) staff       (20)        0 2023-06-24 16:05:40.600381 pyhandytools-0.0.1/pyhandytools.egg-info/
--rw-r--r--   0 jmchen     (501) staff       (20)      386 2023-06-24 16:05:40.000000 pyhandytools-0.0.1/pyhandytools.egg-info/PKG-INFO
--rw-r--r--   0 jmchen     (501) staff       (20)      251 2023-06-24 16:05:40.000000 pyhandytools-0.0.1/pyhandytools.egg-info/SOURCES.txt
--rw-r--r--   0 jmchen     (501) staff       (20)        1 2023-06-24 16:05:40.000000 pyhandytools-0.0.1/pyhandytools.egg-info/dependency_links.txt
--rw-r--r--   0 jmchen     (501) staff       (20)        7 2023-06-24 16:05:40.000000 pyhandytools-0.0.1/pyhandytools.egg-info/requires.txt
--rw-r--r--   0 jmchen     (501) staff       (20)       13 2023-06-24 16:05:40.000000 pyhandytools-0.0.1/pyhandytools.egg-info/top_level.txt
--rw-r--r--   0 jmchen     (501) staff       (20)       38 2023-06-24 16:05:40.600755 pyhandytools-0.0.1/setup.cfg
--rw-r--r--   0 jmchen     (501) staff       (20)      698 2023-06-24 16:05:33.000000 pyhandytools-0.0.1/setup.py
+drwxr-xr-x   0 jmchen     (501) staff       (20)        0 2023-06-26 16:24:46.100101 pyhandytools-0.0.2/
+-rw-r--r--   0 jmchen     (501) staff       (20)    11354 2023-06-24 15:27:46.000000 pyhandytools-0.0.2/LICENSE
+-rw-r--r--   0 jmchen     (501) staff       (20)      386 2023-06-26 16:24:46.099861 pyhandytools-0.0.2/PKG-INFO
+-rw-r--r--   0 jmchen     (501) staff       (20)      102 2023-06-24 15:50:46.000000 pyhandytools-0.0.2/README.md
+drwxr-xr-x   0 jmchen     (501) staff       (20)        0 2023-06-26 16:24:46.098883 pyhandytools-0.0.2/pyhandytools/
+-rw-r--r--   0 jmchen     (501) staff       (20)       48 2023-06-24 15:16:23.000000 pyhandytools-0.0.2/pyhandytools/__init__.py
+-rw-r--r--   0 jmchen     (501) staff       (20)      924 2023-06-26 16:18:30.000000 pyhandytools-0.0.2/pyhandytools/file.py
+drwxr-xr-x   0 jmchen     (501) staff       (20)        0 2023-06-26 16:24:46.099605 pyhandytools-0.0.2/pyhandytools.egg-info/
+-rw-r--r--   0 jmchen     (501) staff       (20)      386 2023-06-26 16:24:46.000000 pyhandytools-0.0.2/pyhandytools.egg-info/PKG-INFO
+-rw-r--r--   0 jmchen     (501) staff       (20)      251 2023-06-26 16:24:46.000000 pyhandytools-0.0.2/pyhandytools.egg-info/SOURCES.txt
+-rw-r--r--   0 jmchen     (501) staff       (20)        1 2023-06-26 16:24:46.000000 pyhandytools-0.0.2/pyhandytools.egg-info/dependency_links.txt
+-rw-r--r--   0 jmchen     (501) staff       (20)        7 2023-06-26 16:24:46.000000 pyhandytools-0.0.2/pyhandytools.egg-info/requires.txt
+-rw-r--r--   0 jmchen     (501) staff       (20)       13 2023-06-26 16:24:46.000000 pyhandytools-0.0.2/pyhandytools.egg-info/top_level.txt
+-rw-r--r--   0 jmchen     (501) staff       (20)       38 2023-06-26 16:24:46.100167 pyhandytools-0.0.2/setup.cfg
+-rw-r--r--   0 jmchen     (501) staff       (20)      698 2023-06-26 16:20:23.000000 pyhandytools-0.0.2/setup.py
```

### Comparing `pyhandytools-0.0.1/LICENSE` & `pyhandytools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhandytools-0.0.1/pyhandytools/file.py` & `pyhandytools-0.0.2/pyhandytools/file.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # !/usr/bin/env python3
 # _*_ coding: utf-8 _*_
 import json
+import os
 from typing import Union
 
 from loguru import logger
 
 
 class FileUtils:
     @staticmethod
@@ -18,7 +19,13 @@
         with open(json_path, 'r', encoding='utf-8') as f:
             _ = f.read()
             if _ == '':
                 logger.warning(f'Your json file in {json_path} is empty!!!')
                 return {}
             data = json.loads(_)
         return data
+
+    @staticmethod
+    def check_dir_path(dir_path: str):
+        if not os.path.exists(dir_path):
+            os.makedirs(dir_path, exist_ok=True)
+            logger.warning(f'mkdir path: {dir_path}')
```

### Comparing `pyhandytools-0.0.1/setup.py` & `pyhandytools-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup, find_packages
 
 with open(path.join(path.abspath(path.dirname(__file__)), 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pyhandytools',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     include_package_data=True,
     url='https://github.com/JimouChen/py-handy',
     author='Jimou Chen',
     author_email='neaya1024@gmail.com',
     description='Python handy tools',
     long_description=long_description,
```

