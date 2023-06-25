# Comparing `tmp/stormlibpp-0.2.0.tar.gz` & `tmp/stormlibpp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stormlibpp-0.2.0.tar", last modified: Sun Jun 25 18:52:44 2023, max compression
+gzip compressed data, was "stormlibpp-0.3.0.tar", last modified: Sun Jun 25 23:08:19 2023, max compression
```

## Comparing `stormlibpp-0.2.0.tar` & `stormlibpp-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 18:52:44.916409 stormlibpp-0.2.0/
--rw-r--r--   0 gormo      (501) staff       (20)     1067 2023-06-24 17:20:21.000000 stormlibpp-0.2.0/LICENSE
--rw-r--r--   0 gormo      (501) staff       (20)     1665 2023-06-25 18:52:44.916290 stormlibpp-0.2.0/PKG-INFO
--rw-r--r--   0 gormo      (501) staff       (20)      108 2023-06-24 18:31:15.000000 stormlibpp-0.2.0/README.md
--rw-r--r--   0 gormo      (501) staff       (20)      557 2023-06-25 18:52:40.000000 stormlibpp-0.2.0/pyproject.toml
--rw-r--r--   0 gormo      (501) staff       (20)       38 2023-06-25 18:52:44.916448 stormlibpp-0.2.0/setup.cfg
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 18:52:44.913888 stormlibpp-0.2.0/src/
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 18:52:44.915045 stormlibpp-0.2.0/src/stormlibpp/
--rw-r--r--   0 gormo      (501) staff       (20)     1419 2023-06-25 18:52:40.000000 stormlibpp-0.2.0/src/stormlibpp/__init__.py
--rw-r--r--   0 gormo      (501) staff       (20)      663 2023-06-25 16:40:51.000000 stormlibpp-0.2.0/src/stormlibpp/errors.py
--rw-r--r--   0 gormo      (501) staff       (20)      507 2023-06-25 18:48:29.000000 stormlibpp-0.2.0/src/stormlibpp/node.py
--rw-r--r--   0 gormo      (501) staff       (20)     9151 2023-06-25 18:31:41.000000 stormlibpp-0.2.0/src/stormlibpp/stormpkg.py
--rw-r--r--   0 gormo      (501) staff       (20)     1396 2023-06-25 16:42:23.000000 stormlibpp-0.2.0/src/stormlibpp/telepath.py
--rw-r--r--   0 gormo      (501) staff       (20)     1507 2023-06-25 18:15:47.000000 stormlibpp-0.2.0/src/stormlibpp/utils.py
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 18:52:44.915749 stormlibpp-0.2.0/src/stormlibpp.egg-info/
--rw-r--r--   0 gormo      (501) staff       (20)     1665 2023-06-25 18:52:44.000000 stormlibpp-0.2.0/src/stormlibpp.egg-info/PKG-INFO
--rw-r--r--   0 gormo      (501) staff       (20)      440 2023-06-25 18:52:44.000000 stormlibpp-0.2.0/src/stormlibpp.egg-info/SOURCES.txt
--rw-r--r--   0 gormo      (501) staff       (20)        1 2023-06-25 18:52:44.000000 stormlibpp-0.2.0/src/stormlibpp.egg-info/dependency_links.txt
--rw-r--r--   0 gormo      (501) staff       (20)       17 2023-06-25 18:52:44.000000 stormlibpp-0.2.0/src/stormlibpp.egg-info/requires.txt
--rw-r--r--   0 gormo      (501) staff       (20)       11 2023-06-25 18:52:44.000000 stormlibpp-0.2.0/src/stormlibpp.egg-info/top_level.txt
-drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 18:52:44.916118 stormlibpp-0.2.0/tests/
--rw-r--r--   0 gormo      (501) staff       (20)     1699 2023-06-25 18:37:46.000000 stormlibpp-0.2.0/tests/test_stormpkg.py
--rw-r--r--   0 gormo      (501) staff       (20)      720 2023-06-25 16:42:23.000000 stormlibpp-0.2.0/tests/test_telepath.py
--rw-r--r--   0 gormo      (501) staff       (20)      419 2023-06-24 18:31:15.000000 stormlibpp-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 23:08:19.813611 stormlibpp-0.3.0/
+-rw-r--r--   0 gormo      (501) staff       (20)     1067 2023-06-24 17:20:21.000000 stormlibpp-0.3.0/LICENSE
+-rw-r--r--   0 gormo      (501) staff       (20)     1665 2023-06-25 23:08:19.813482 stormlibpp-0.3.0/PKG-INFO
+-rw-r--r--   0 gormo      (501) staff       (20)      108 2023-06-24 18:31:15.000000 stormlibpp-0.3.0/README.md
+-rw-r--r--   0 gormo      (501) staff       (20)      557 2023-06-25 23:08:15.000000 stormlibpp-0.3.0/pyproject.toml
+-rw-r--r--   0 gormo      (501) staff       (20)       38 2023-06-25 23:08:19.813652 stormlibpp-0.3.0/setup.cfg
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 23:08:19.810546 stormlibpp-0.3.0/src/
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 23:08:19.811705 stormlibpp-0.3.0/src/stormlibpp/
+-rw-r--r--   0 gormo      (501) staff       (20)     1447 2023-06-25 23:08:15.000000 stormlibpp-0.3.0/src/stormlibpp/__init__.py
+-rw-r--r--   0 gormo      (501) staff       (20)      663 2023-06-25 16:40:51.000000 stormlibpp-0.3.0/src/stormlibpp/errors.py
+-rw-r--r--   0 gormo      (501) staff       (20)     5371 2023-06-25 22:22:23.000000 stormlibpp-0.3.0/src/stormlibpp/node.py
+-rw-r--r--   0 gormo      (501) staff       (20)     9151 2023-06-25 18:55:59.000000 stormlibpp-0.3.0/src/stormlibpp/stormpkg.py
+-rw-r--r--   0 gormo      (501) staff       (20)     1396 2023-06-25 16:42:23.000000 stormlibpp-0.3.0/src/stormlibpp/telepath.py
+-rw-r--r--   0 gormo      (501) staff       (20)     1507 2023-06-25 18:55:59.000000 stormlibpp-0.3.0/src/stormlibpp/utils.py
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 23:08:19.812645 stormlibpp-0.3.0/src/stormlibpp.egg-info/
+-rw-r--r--   0 gormo      (501) staff       (20)     1665 2023-06-25 23:08:19.000000 stormlibpp-0.3.0/src/stormlibpp.egg-info/PKG-INFO
+-rw-r--r--   0 gormo      (501) staff       (20)      459 2023-06-25 23:08:19.000000 stormlibpp-0.3.0/src/stormlibpp.egg-info/SOURCES.txt
+-rw-r--r--   0 gormo      (501) staff       (20)        1 2023-06-25 23:08:19.000000 stormlibpp-0.3.0/src/stormlibpp.egg-info/dependency_links.txt
+-rw-r--r--   0 gormo      (501) staff       (20)       17 2023-06-25 23:08:19.000000 stormlibpp-0.3.0/src/stormlibpp.egg-info/requires.txt
+-rw-r--r--   0 gormo      (501) staff       (20)       11 2023-06-25 23:08:19.000000 stormlibpp-0.3.0/src/stormlibpp.egg-info/top_level.txt
+drwxr-xr-x   0 gormo      (501) staff       (20)        0 2023-06-25 23:08:19.813294 stormlibpp-0.3.0/tests/
+-rw-r--r--   0 gormo      (501) staff       (20)     1438 2023-06-25 22:24:01.000000 stormlibpp-0.3.0/tests/test_node.py
+-rw-r--r--   0 gormo      (501) staff       (20)     1699 2023-06-25 18:55:59.000000 stormlibpp-0.3.0/tests/test_stormpkg.py
+-rw-r--r--   0 gormo      (501) staff       (20)      720 2023-06-25 16:42:23.000000 stormlibpp-0.3.0/tests/test_telepath.py
+-rw-r--r--   0 gormo      (501) staff       (20)      419 2023-06-24 18:31:15.000000 stormlibpp-0.3.0/tests/test_utils.py
```

### Comparing `stormlibpp-0.2.0/LICENSE` & `stormlibpp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stormlibpp-0.2.0/PKG-INFO` & `stormlibpp-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stormlibpp
-Version: 0.2.0
+Version: 0.3.0
 Summary: The stormlibpp Python package
 Author: John Gorman
 License: MIT License
         
         Copyright (c) 2023 John Gorman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `stormlibpp-0.2.0/pyproject.toml` & `stormlibpp-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "stormlibpp"
-version = "0.2.0"
+version = "0.3.0"
 description = "The stormlibpp Python package"
 readme = "README.md"
 requires-python = ">=3.11"
 
 # Fill in dependencies here.
 dependencies = [
     "synapse==2.139.0"
```

### Comparing `stormlibpp-0.2.0/src/stormlibpp/__init__.py` & `stormlibpp-0.3.0/src/stormlibpp/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,13 +25,14 @@
   It currently contains mostly classes for describing standard Telepath API
   return values.
 
 - ``stormpkg`` defines the ``StormPkg`` class.
 
 """
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 from . import errors
 from . import utils
+from .node import StormNode
 from .stormpkg import StormPkg
 from .telepath import (genDefaultTelepathRetn, TelepathRetn)
```

### Comparing `stormlibpp-0.2.0/src/stormlibpp/errors.py` & `stormlibpp-0.3.0/src/stormlibpp/errors.py`

 * *Files identical despite different names*

### Comparing `stormlibpp-0.2.0/src/stormlibpp/stormpkg.py` & `stormlibpp-0.3.0/src/stormlibpp/stormpkg.py`

 * *Files identical despite different names*

### Comparing `stormlibpp-0.2.0/src/stormlibpp/telepath.py` & `stormlibpp-0.3.0/src/stormlibpp/telepath.py`

 * *Files identical despite different names*

### Comparing `stormlibpp-0.2.0/src/stormlibpp/utils.py` & `stormlibpp-0.3.0/src/stormlibpp/utils.py`

 * *Files identical despite different names*

### Comparing `stormlibpp-0.2.0/src/stormlibpp.egg-info/PKG-INFO` & `stormlibpp-0.3.0/src/stormlibpp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stormlibpp
-Version: 0.2.0
+Version: 0.3.0
 Summary: The stormlibpp Python package
 Author: John Gorman
 License: MIT License
         
         Copyright (c) 2023 John Gorman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `stormlibpp-0.2.0/tests/test_stormpkg.py` & `stormlibpp-0.3.0/tests/test_stormpkg.py`

 * *Files identical despite different names*

### Comparing `stormlibpp-0.2.0/tests/test_telepath.py` & `stormlibpp-0.3.0/tests/test_telepath.py`

 * *Files identical despite different names*

