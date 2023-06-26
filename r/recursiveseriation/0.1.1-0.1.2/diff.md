# Comparing `tmp/recursiveseriation-0.1.1.tar.gz` & `tmp/recursiveseriation-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recursiveseriation-0.1.1.tar", max compression
+gzip compressed data, was "recursiveseriation-0.1.2.tar", max compression
```

## Comparing `recursiveseriation-0.1.1.tar` & `recursiveseriation-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1076 2023-06-23 21:55:08.312130 recursiveseriation-0.1.1/LICENSE
--rw-r--r--   0        0        0      737 2023-06-23 21:55:08.320130 recursiveseriation-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      343 2023-06-23 21:55:08.320130 recursiveseriation-0.1.1/recursiveseriation/__init__.py
--rw-r--r--   0        0        0     1706 2023-06-23 21:55:08.320130 recursiveseriation-0.1.1/recursiveseriation/exc.py
--rw-r--r--   0        0        0     4765 2023-06-23 21:55:08.320130 recursiveseriation-0.1.1/recursiveseriation/logger.py
--rw-r--r--   0        0        0     2107 2023-06-23 21:55:08.320130 recursiveseriation-0.1.1/recursiveseriation/settings.py
--rw-r--r--   0        0        0        0 2023-06-23 21:55:08.320130 recursiveseriation-0.1.1/recursiveseriation/solver/__init__.py
--rw-r--r--   0        0        0     7056 2023-06-23 21:55:08.320130 recursiveseriation-0.1.1/recursiveseriation/solver/neighbours_graph.py
--rw-r--r--   0        0        0     5421 2023-06-23 21:55:08.320130 recursiveseriation-0.1.1/recursiveseriation/solver/qtree.py
--rw-r--r--   0        0        0    14001 2023-06-23 21:55:08.320130 recursiveseriation-0.1.1/recursiveseriation/solver/seriation.py
--rw-r--r--   0        0        0     2597 2023-06-23 21:55:08.320130 recursiveseriation-0.1.1/recursiveseriation/utils.py
--rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 recursiveseriation-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-26 15:11:03.101563 recursiveseriation-0.1.2/LICENSE
+-rw-r--r--   0        0        0      743 2023-06-26 15:11:03.105563 recursiveseriation-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      343 2023-06-26 15:11:03.105563 recursiveseriation-0.1.2/recursiveseriation/__init__.py
+-rw-r--r--   0        0        0     1706 2023-06-26 15:11:03.105563 recursiveseriation-0.1.2/recursiveseriation/exc.py
+-rw-r--r--   0        0        0     4765 2023-06-26 15:11:03.105563 recursiveseriation-0.1.2/recursiveseriation/logger.py
+-rw-r--r--   0        0        0     2107 2023-06-26 15:11:03.105563 recursiveseriation-0.1.2/recursiveseriation/settings.py
+-rw-r--r--   0        0        0        0 2023-06-26 15:11:03.105563 recursiveseriation-0.1.2/recursiveseriation/solver/__init__.py
+-rw-r--r--   0        0        0     7056 2023-06-26 15:11:03.105563 recursiveseriation-0.1.2/recursiveseriation/solver/neighbours_graph.py
+-rw-r--r--   0        0        0     5421 2023-06-26 15:11:03.105563 recursiveseriation-0.1.2/recursiveseriation/solver/qtree.py
+-rw-r--r--   0        0        0    14001 2023-06-26 15:11:03.105563 recursiveseriation-0.1.2/recursiveseriation/solver/seriation.py
+-rw-r--r--   0        0        0     2597 2023-06-26 15:11:03.105563 recursiveseriation-0.1.2/recursiveseriation/utils.py
+-rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 recursiveseriation-0.1.2/PKG-INFO
```

### Comparing `recursiveseriation-0.1.1/LICENSE` & `recursiveseriation-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `recursiveseriation-0.1.1/pyproject.toml` & `recursiveseriation-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name ="recursiveseriation"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python implementation of the 'Recursive Seriation' algorithm for reordering strict circular Robisonian matrices"
 authors = ["Santiago Armstrong <santiagoarmstrong@gmail.com>"]
 
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.8, <4.0"
 structlog = "^20.2.0"
 python-dotenv = "^0.15.0"
 pydantic = "^1.7.3"
 numpy = "^1.24.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.2"
```

### Comparing `recursiveseriation-0.1.1/recursiveseriation/exc.py` & `recursiveseriation-0.1.2/recursiveseriation/exc.py`

 * *Files identical despite different names*

### Comparing `recursiveseriation-0.1.1/recursiveseriation/logger.py` & `recursiveseriation-0.1.2/recursiveseriation/logger.py`

 * *Files identical despite different names*

### Comparing `recursiveseriation-0.1.1/recursiveseriation/settings.py` & `recursiveseriation-0.1.2/recursiveseriation/settings.py`

 * *Files identical despite different names*

### Comparing `recursiveseriation-0.1.1/recursiveseriation/solver/neighbours_graph.py` & `recursiveseriation-0.1.2/recursiveseriation/solver/neighbours_graph.py`

 * *Files identical despite different names*

### Comparing `recursiveseriation-0.1.1/recursiveseriation/solver/qtree.py` & `recursiveseriation-0.1.2/recursiveseriation/solver/qtree.py`

 * *Files identical despite different names*

### Comparing `recursiveseriation-0.1.1/recursiveseriation/solver/seriation.py` & `recursiveseriation-0.1.2/recursiveseriation/solver/seriation.py`

 * *Files identical despite different names*

### Comparing `recursiveseriation-0.1.1/recursiveseriation/utils.py` & `recursiveseriation-0.1.2/recursiveseriation/utils.py`

 * *Files identical despite different names*

### Comparing `recursiveseriation-0.1.1/PKG-INFO` & `recursiveseriation-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: recursiveseriation
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python implementation of the 'Recursive Seriation' algorithm for reordering strict circular Robisonian matrices
 Author: Santiago Armstrong
 Author-email: santiagoarmstrong@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pydantic (>=1.7.3,<2.0.0)
 Requires-Dist: python-dotenv (>=0.15.0,<0.16.0)
 Requires-Dist: structlog (>=20.2.0,<21.0.0)
```

