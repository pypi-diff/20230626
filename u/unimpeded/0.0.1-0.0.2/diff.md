# Comparing `tmp/unimpeded-0.0.1.tar.gz` & `tmp/unimpeded-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unimpeded-0.0.1.tar", last modified: Mon Jun 26 14:41:46 2023, max compression
+gzip compressed data, was "unimpeded-0.0.2.tar", last modified: Mon Jun 26 15:15:44 2023, max compression
```

## Comparing `unimpeded-0.0.1.tar` & `unimpeded-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:41:46.771002 unimpeded-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-26 14:41:38.000000 unimpeded-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-26 14:41:46.771002 unimpeded-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-26 14:41:38.000000 unimpeded-0.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-26 14:41:38.000000 unimpeded-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 14:41:46.771002 unimpeded-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:41:46.771002 unimpeded-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 14:41:38.000000 unimpeded-0.0.1/tests/test_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:41:46.771002 unimpeded-0.0.1/unimpeded/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 14:41:38.000000 unimpeded-0.0.1/unimpeded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 14:41:38.000000 unimpeded-0.0.1/unimpeded/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:41:46.771002 unimpeded-0.0.1/unimpeded.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-26 14:41:46.000000 unimpeded-0.0.1/unimpeded.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-26 14:41:46.000000 unimpeded-0.0.1/unimpeded.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:41:46.000000 unimpeded-0.0.1/unimpeded.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 14:41:46.000000 unimpeded-0.0.1/unimpeded.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 14:41:46.000000 unimpeded-0.0.1/unimpeded.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:44.044063 unimpeded-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-26 15:15:35.000000 unimpeded-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-26 15:15:44.044063 unimpeded-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-26 15:15:35.000000 unimpeded-0.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-26 15:15:35.000000 unimpeded-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 15:15:44.044063 unimpeded-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:44.044063 unimpeded-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 15:15:35.000000 unimpeded-0.0.2/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:44.044063 unimpeded-0.0.2/unimpeded/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 15:15:35.000000 unimpeded-0.0.2/unimpeded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 15:15:35.000000 unimpeded-0.0.2/unimpeded/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:44.044063 unimpeded-0.0.2/unimpeded.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-26 15:15:44.000000 unimpeded-0.0.2/unimpeded.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-26 15:15:44.000000 unimpeded-0.0.2/unimpeded.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:15:44.000000 unimpeded-0.0.2/unimpeded.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 15:15:44.000000 unimpeded-0.0.2/unimpeded.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 15:15:44.000000 unimpeded-0.0.2/unimpeded.egg-info/top_level.txt
```

### Comparing `unimpeded-0.0.1/LICENSE` & `unimpeded-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unimpeded-0.0.1/PKG-INFO` & `unimpeded-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unimpeded
-Version: 0.0.1
+Version: 0.0.2
 Summary: Universal model comparison & parameter estimation over diverse datasets
 Author-email: Will Handley <williamjameshandley@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Will Handley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,15 +48,15 @@
 License-File: LICENSE
 
 ===========================================================================================
 unimpeded: Universal model comparison & parameter estimation distributed over every dataset
 ===========================================================================================
 :unimpeded: Universal model comparison & parameter estimation distributed over every dataset 
 :Author: Will Handley
-:Version: 0.0.1
+:Version: 0.0.2
 :Homepage: https://github.com/handley-lab/unimpeded
 :Documentation: http://unimpeded.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/unimpeded/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/unimpeded/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/unimpeded/branch/master/graph/badge.svg
```

### Comparing `unimpeded-0.0.1/README.rst` & `unimpeded-0.0.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ===========================================================================================
 unimpeded: Universal model comparison & parameter estimation distributed over every dataset
 ===========================================================================================
 :unimpeded: Universal model comparison & parameter estimation distributed over every dataset 
 :Author: Will Handley
-:Version: 0.0.1
+:Version: 0.0.2
 :Homepage: https://github.com/handley-lab/unimpeded
 :Documentation: http://unimpeded.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/unimpeded/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/unimpeded/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/unimpeded/branch/master/graph/badge.svg
```

### Comparing `unimpeded-0.0.1/pyproject.toml` & `unimpeded-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unimpeded-0.0.1/unimpeded.egg-info/PKG-INFO` & `unimpeded-0.0.2/unimpeded.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unimpeded
-Version: 0.0.1
+Version: 0.0.2
 Summary: Universal model comparison & parameter estimation over diverse datasets
 Author-email: Will Handley <williamjameshandley@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Will Handley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,15 +48,15 @@
 License-File: LICENSE
 
 ===========================================================================================
 unimpeded: Universal model comparison & parameter estimation distributed over every dataset
 ===========================================================================================
 :unimpeded: Universal model comparison & parameter estimation distributed over every dataset 
 :Author: Will Handley
-:Version: 0.0.1
+:Version: 0.0.2
 :Homepage: https://github.com/handley-lab/unimpeded
 :Documentation: http://unimpeded.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/unimpeded/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/unimpeded/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/unimpeded/branch/master/graph/badge.svg
```

