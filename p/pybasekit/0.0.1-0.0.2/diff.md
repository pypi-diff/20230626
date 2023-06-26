# Comparing `tmp/pybasekit-0.0.1.tar.gz` & `tmp/pybasekit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybasekit-0.0.1.tar", last modified: Fri Jun 16 19:11:40 2023, max compression
+gzip compressed data, was "pybasekit-0.0.2.tar", last modified: Mon Jun 26 19:00:40 2023, max compression
```

## Comparing `pybasekit-0.0.1.tar` & `pybasekit-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 19:11:40.401638 pybasekit-0.0.1/
--rw-rw-rw-   0        0        0     1083 2023-06-16 18:40:25.000000 pybasekit-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1673 2023-06-16 19:11:40.401638 pybasekit-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1216 2023-06-16 19:11:35.000000 pybasekit-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 19:11:40.401638 pybasekit-0.0.1/pybasekit.egg-info/
--rw-rw-rw-   0        0        0     1673 2023-06-16 19:11:40.000000 pybasekit-0.0.1/pybasekit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      158 2023-06-16 19:11:40.000000 pybasekit-0.0.1/pybasekit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 19:11:40.000000 pybasekit-0.0.1/pybasekit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 19:11:40.000000 pybasekit-0.0.1/pybasekit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 19:11:40.401638 pybasekit-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      943 2023-06-16 19:11:37.000000 pybasekit-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 19:00:40.681315 pybasekit-0.0.2/
+-rw-rw-rw-   0        0        0     1083 2023-06-16 18:40:25.000000 pybasekit-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1673 2023-06-26 19:00:40.680314 pybasekit-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1216 2023-06-16 19:11:35.000000 pybasekit-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 19:00:40.670803 pybasekit-0.0.2/pybasekit/
+-rw-rw-rw-   0        0        0    12289 2023-06-26 18:56:36.000000 pybasekit-0.0.2/pybasekit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 19:00:40.679313 pybasekit-0.0.2/pybasekit.egg-info/
+-rw-rw-rw-   0        0        0     1673 2023-06-26 19:00:40.000000 pybasekit-0.0.2/pybasekit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-06-26 19:00:40.000000 pybasekit-0.0.2/pybasekit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 19:00:40.000000 pybasekit-0.0.2/pybasekit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-26 19:00:40.000000 pybasekit-0.0.2/pybasekit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 19:00:40.681315 pybasekit-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      943 2023-06-26 18:56:45.000000 pybasekit-0.0.2/setup.py
```

### Comparing `pybasekit-0.0.1/LICENSE` & `pybasekit-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pybasekit-0.0.1/PKG-INFO` & `pybasekit-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybasekit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Basic local database system
 Author: Because
 Author-email: 
 Keywords: python,db,database,storage
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pybasekit-0.0.1/README.md` & `pybasekit-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pybasekit-0.0.1/pybasekit.egg-info/PKG-INFO` & `pybasekit-0.0.2/pybasekit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybasekit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Basic local database system
 Author: Because
 Author-email: 
 Keywords: python,db,database,storage
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pybasekit-0.0.1/setup.py` & `pybasekit-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Basic local database system'
 LONG_DESCRIPTION = 'A very basic database system for python and personal small projects.'
 
 # Setting up
 setup(
     name="pybasekit",
     version=VERSION,
```

