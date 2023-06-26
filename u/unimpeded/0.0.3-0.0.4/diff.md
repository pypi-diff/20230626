# Comparing `tmp/unimpeded-0.0.3.tar.gz` & `tmp/unimpeded-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unimpeded-0.0.3.tar", last modified: Mon Jun 26 15:28:31 2023, max compression
+gzip compressed data, was "unimpeded-0.0.4.tar", last modified: Mon Jun 26 15:52:58 2023, max compression
```

## Comparing `unimpeded-0.0.3.tar` & `unimpeded-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:28:31.167843 unimpeded-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-26 15:28:20.000000 unimpeded-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-26 15:28:31.167843 unimpeded-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-26 15:28:20.000000 unimpeded-0.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-26 15:28:20.000000 unimpeded-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 15:28:31.171843 unimpeded-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:28:31.167843 unimpeded-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 15:28:20.000000 unimpeded-0.0.3/tests/test_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:28:31.167843 unimpeded-0.0.3/unimpeded/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 15:28:20.000000 unimpeded-0.0.3/unimpeded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 15:28:20.000000 unimpeded-0.0.3/unimpeded/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:28:31.167843 unimpeded-0.0.3/unimpeded.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-26 15:28:31.000000 unimpeded-0.0.3/unimpeded.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-26 15:28:31.000000 unimpeded-0.0.3/unimpeded.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:28:31.000000 unimpeded-0.0.3/unimpeded.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 15:28:31.000000 unimpeded-0.0.3/unimpeded.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 15:28:31.000000 unimpeded-0.0.3/unimpeded.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:52:58.664056 unimpeded-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-26 15:52:49.000000 unimpeded-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-26 15:52:58.664056 unimpeded-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-26 15:52:49.000000 unimpeded-0.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-26 15:52:49.000000 unimpeded-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 15:52:58.664056 unimpeded-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:52:58.660056 unimpeded-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 15:52:49.000000 unimpeded-0.0.4/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:52:58.660056 unimpeded-0.0.4/unimpeded/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 15:52:49.000000 unimpeded-0.0.4/unimpeded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 15:52:49.000000 unimpeded-0.0.4/unimpeded/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:52:58.664056 unimpeded-0.0.4/unimpeded.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-26 15:52:58.000000 unimpeded-0.0.4/unimpeded.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-26 15:52:58.000000 unimpeded-0.0.4/unimpeded.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:52:58.000000 unimpeded-0.0.4/unimpeded.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 15:52:58.000000 unimpeded-0.0.4/unimpeded.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 15:52:58.000000 unimpeded-0.0.4/unimpeded.egg-info/top_level.txt
```

### Comparing `unimpeded-0.0.3/LICENSE` & `unimpeded-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unimpeded-0.0.3/PKG-INFO` & `unimpeded-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unimpeded
-Version: 0.0.3
+Version: 0.0.4
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
-:Version: 0.0.3
+:Version: 0.0.4
 :Homepage: https://github.com/handley-lab/unimpeded
 :Documentation: http://unimpeded.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/unimpeded/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/unimpeded/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/unimpeded/branch/master/graph/badge.svg
```

### Comparing `unimpeded-0.0.3/README.rst` & `unimpeded-0.0.4/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ===========================================================================================
 unimpeded: Universal model comparison & parameter estimation distributed over every dataset
 ===========================================================================================
 :unimpeded: Universal model comparison & parameter estimation distributed over every dataset 
 :Author: Will Handley
-:Version: 0.0.3
+:Version: 0.0.4
 :Homepage: https://github.com/handley-lab/unimpeded
 :Documentation: http://unimpeded.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/unimpeded/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/unimpeded/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/unimpeded/branch/master/graph/badge.svg
```

### Comparing `unimpeded-0.0.3/pyproject.toml` & `unimpeded-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unimpeded-0.0.3/unimpeded.egg-info/PKG-INFO` & `unimpeded-0.0.4/unimpeded.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unimpeded
-Version: 0.0.3
+Version: 0.0.4
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
-:Version: 0.0.3
+:Version: 0.0.4
 :Homepage: https://github.com/handley-lab/unimpeded
 :Documentation: http://unimpeded.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/unimpeded/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/unimpeded/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/unimpeded/branch/master/graph/badge.svg
```

