# Comparing `tmp/pranerpacker-0.0.1.tar.gz` & `tmp/pranerpacker-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pranerpacker-0.0.1.tar", last modified: Mon Jun 26 18:51:22 2023, max compression
+gzip compressed data, was "dist\pranerpacker-0.0.2.tar", last modified: Mon Jun 26 18:58:10 2023, max compression
```

## Comparing `pranerpacker-0.0.1.tar` & `pranerpacker-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 18:51:22.491872 pranerpacker-0.0.1/
--rw-rw-rw-   0        0        0      566 2023-06-26 18:51:22.489877 pranerpacker-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-26 18:51:22.440092 pranerpacker-0.0.1/pranerpacker/
--rw-rw-rw-   0        0        0       43 2023-06-26 18:50:28.000000 pranerpacker-0.0.1/pranerpacker/__init__.py
--rw-rw-rw-   0        0        0       40 2023-06-26 18:03:36.000000 pranerpacker-0.0.1/pranerpacker/basepranee.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:51:22.487886 pranerpacker-0.0.1/pranerpacker.egg-info/
--rw-rw-rw-   0        0        0      566 2023-06-26 18:51:22.000000 pranerpacker-0.0.1/pranerpacker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-06-26 18:51:22.000000 pranerpacker-0.0.1/pranerpacker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 18:51:22.000000 pranerpacker-0.0.1/pranerpacker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-26 18:51:22.000000 pranerpacker-0.0.1/pranerpacker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 18:51:22.491872 pranerpacker-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      906 2023-06-26 18:50:46.000000 pranerpacker-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:10.970137 pranerpacker-0.0.2/
+-rw-rw-rw-   0        0        0      566 2023-06-26 18:58:10.968143 pranerpacker-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:10.930771 pranerpacker-0.0.2/pranerpacker/
+-rw-rw-rw-   0        0        0       43 2023-06-26 18:50:28.000000 pranerpacker-0.0.2/pranerpacker/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-06-26 18:53:45.000000 pranerpacker-0.0.2/pranerpacker/basepranee.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:58:10.964724 pranerpacker-0.0.2/pranerpacker.egg-info/
+-rw-rw-rw-   0        0        0      566 2023-06-26 18:58:10.000000 pranerpacker-0.0.2/pranerpacker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-06-26 18:58:10.000000 pranerpacker-0.0.2/pranerpacker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 18:58:10.000000 pranerpacker-0.0.2/pranerpacker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-26 18:58:10.000000 pranerpacker-0.0.2/pranerpacker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 18:58:10.970137 pranerpacker-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      906 2023-06-26 18:53:53.000000 pranerpacker-0.0.2/setup.py
```

### Comparing `pranerpacker-0.0.1/PKG-INFO` & `pranerpacker-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pranerpacker
-Version: 0.0.1
+Version: 0.0.2
 Summary: Praneeths first Python package
 Author: Sai Praneeth Renduchinthala
 Author-email: praneeth.renduchinthala210@gmail.com
 Keywords: pranerpacker
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pranerpacker-0.0.1/pranerpacker.egg-info/PKG-INFO` & `pranerpacker-0.0.2/pranerpacker.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pranerpacker
-Version: 0.0.1
+Version: 0.0.2
 Summary: Praneeths first Python package
 Author: Sai Praneeth Renduchinthala
 Author-email: praneeth.renduchinthala210@gmail.com
 Keywords: pranerpacker
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `pranerpacker-0.0.1/setup.py` & `pranerpacker-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.2' 
 DESCRIPTION = 'Praneeths first Python package'
 LONG_DESCRIPTION = 'praneeths first package with a slightly longer description'
 
 
 setup(
      
         name="pranerpacker",
```

