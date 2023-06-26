# Comparing `tmp/ocrd_utils-2.8.3.tar.gz` & `tmp/ocrd_utils-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ocrd_utils-2.8.3.tar", last modified: Mon Jun  8 16:56:33 2020, max compression
+gzip compressed data, was "dist/ocrd_utils-2.9.0.tar", last modified: Tue Jun  9 17:33:29 2020, max compression
```

## Comparing `ocrd_utils-2.8.3.tar` & `ocrd_utils-2.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-08 16:56:33.000000 ocrd_utils-2.8.3/
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-08 16:56:33.000000 ocrd_utils-2.8.3/ocrd_utils/
--rw-rw-r--   0 kba       (1000) kba       (1000)     3604 2020-06-07 13:19:20.000000 ocrd_utils-2.8.3/ocrd_utils/logging.py
--rw-rw-r--   0 kba       (1000) kba       (1000)    30283 2020-06-06 19:26:51.000000 ocrd_utils-2.8.3/ocrd_utils/__init__.py
--rw-rw-r--   0 kba       (1000) kba       (1000)      911 2020-05-12 11:01:01.000000 ocrd_utils-2.8.3/ocrd_utils/deprecate.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     2069 2020-06-07 19:05:48.000000 ocrd_utils-2.8.3/ocrd_utils/constants.py
--rw-rw-r--   0 kba       (1000) kba       (1000)       38 2020-06-08 16:56:33.000000 ocrd_utils-2.8.3/setup.cfg
--rw-rw-r--   0 kba       (1000) kba       (1000)      636 2020-06-08 16:54:29.000000 ocrd_utils-2.8.3/setup.py
--rw-rw-r--   0 kba       (1000) kba       (1000)     2696 2020-06-08 16:56:33.000000 ocrd_utils-2.8.3/PKG-INFO
-drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-08 16:56:33.000000 ocrd_utils-2.8.3/ocrd_utils.egg-info/
--rw-rw-r--   0 kba       (1000) kba       (1000)      280 2020-06-08 16:56:32.000000 ocrd_utils-2.8.3/ocrd_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)       28 2020-06-08 16:56:32.000000 ocrd_utils-2.8.3/ocrd_utils.egg-info/requires.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)       11 2020-06-08 16:56:32.000000 ocrd_utils-2.8.3/ocrd_utils.egg-info/top_level.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)     2696 2020-06-08 16:56:32.000000 ocrd_utils-2.8.3/ocrd_utils.egg-info/PKG-INFO
--rw-rw-r--   0 kba       (1000) kba       (1000)        1 2020-06-08 16:56:32.000000 ocrd_utils-2.8.3/ocrd_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 kba       (1000) kba       (1000)     2114 2020-06-06 19:26:51.000000 ocrd_utils-2.8.3/README.md
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-09 17:33:29.000000 ocrd_utils-2.9.0/
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-09 17:33:29.000000 ocrd_utils-2.9.0/ocrd_utils/
+-rw-rw-r--   0 kba       (1000) kba       (1000)     3601 2020-06-09 17:08:17.000000 ocrd_utils-2.9.0/ocrd_utils/logging.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)    30283 2020-06-06 19:26:51.000000 ocrd_utils-2.9.0/ocrd_utils/__init__.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)      911 2020-05-12 11:01:01.000000 ocrd_utils-2.9.0/ocrd_utils/deprecate.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     2069 2020-06-09 13:50:15.000000 ocrd_utils-2.9.0/ocrd_utils/constants.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)       38 2020-06-09 17:33:29.000000 ocrd_utils-2.9.0/setup.cfg
+-rw-rw-r--   0 kba       (1000) kba       (1000)      636 2020-06-09 17:30:26.000000 ocrd_utils-2.9.0/setup.py
+-rw-rw-r--   0 kba       (1000) kba       (1000)     2696 2020-06-09 17:33:29.000000 ocrd_utils-2.9.0/PKG-INFO
+drwxrwxr-x   0 kba       (1000) kba       (1000)        0 2020-06-09 17:33:29.000000 ocrd_utils-2.9.0/ocrd_utils.egg-info/
+-rw-rw-r--   0 kba       (1000) kba       (1000)      280 2020-06-09 17:33:29.000000 ocrd_utils-2.9.0/ocrd_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       28 2020-06-09 17:33:29.000000 ocrd_utils-2.9.0/ocrd_utils.egg-info/requires.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)       11 2020-06-09 17:33:29.000000 ocrd_utils-2.9.0/ocrd_utils.egg-info/top_level.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)     2696 2020-06-09 17:33:29.000000 ocrd_utils-2.9.0/ocrd_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 kba       (1000) kba       (1000)        1 2020-06-09 17:33:29.000000 ocrd_utils-2.9.0/ocrd_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 kba       (1000) kba       (1000)     2114 2020-06-06 19:26:51.000000 ocrd_utils-2.9.0/README.md
```

### Comparing `ocrd_utils-2.8.3/ocrd_utils/logging.py` & `ocrd_utils-2.9.0/ocrd_utils/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         self.propagate = not self.handlers
 
 logging.setLoggerClass(PropagationShyLogger)
 logging.getLogger().propagate = False
 
 def getLevelName(lvl):
     """
-    Get (numerical) python logging level for (string) spec-defined log level name.
+    Get (string) python logging level for (string) spec-defined log level name.
     """
     lvl = _ocrdLevel2pythonLevel.get(lvl, lvl)
     return logging.getLevelName(lvl)
 
 def setOverrideLogLevel(lvl):
     """
     Override all logger filter levels to include lvl and above.
```

### Comparing `ocrd_utils-2.8.3/ocrd_utils/__init__.py` & `ocrd_utils-2.9.0/ocrd_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ocrd_utils-2.8.3/ocrd_utils/deprecate.py` & `ocrd_utils-2.9.0/ocrd_utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `ocrd_utils-2.8.3/ocrd_utils/constants.py` & `ocrd_utils-2.9.0/ocrd_utils/constants.py`

 * *Files identical despite different names*

### Comparing `ocrd_utils-2.8.3/setup.py` & `ocrd_utils-2.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 install_requires = open('requirements.txt').read().split('\n')
 
 setup(
     name='ocrd_utils',
-    version='2.8.3',
+    version='2.9.0',
     description='OCR-D framework - shared code, helpers, constants',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Konstantin Baierer',
     author_email='unixprog@gmail.com',
     url='https://github.com/OCR-D/core',
     license='Apache License 2.0',
```

### Comparing `ocrd_utils-2.8.3/PKG-INFO` & `ocrd_utils-2.9.0/ocrd_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ocrd_utils
-Version: 2.8.3
+Name: ocrd-utils
+Version: 2.9.0
 Summary: OCR-D framework - shared code, helpers, constants
 Home-page: https://github.com/OCR-D/core
 Author: Konstantin Baierer
 Author-email: unixprog@gmail.com
 License: Apache License 2.0
 Description: # ocrd_utils
```

### Comparing `ocrd_utils-2.8.3/ocrd_utils.egg-info/PKG-INFO` & `ocrd_utils-2.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ocrd-utils
-Version: 2.8.3
+Name: ocrd_utils
+Version: 2.9.0
 Summary: OCR-D framework - shared code, helpers, constants
 Home-page: https://github.com/OCR-D/core
 Author: Konstantin Baierer
 Author-email: unixprog@gmail.com
 License: Apache License 2.0
 Description: # ocrd_utils
```

### Comparing `ocrd_utils-2.8.3/README.md` & `ocrd_utils-2.9.0/README.md`

 * *Files identical despite different names*

