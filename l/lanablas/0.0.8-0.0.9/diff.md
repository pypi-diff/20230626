# Comparing `tmp/lanablas-0.0.8.tar.gz` & `tmp/lanablas-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanablas-0.0.8.tar", last modified: Mon Jun 26 09:34:04 2023, max compression
+gzip compressed data, was "lanablas-0.0.9.tar", last modified: Mon Jun 26 09:57:26 2023, max compression
```

## Comparing `lanablas-0.0.8.tar` & `lanablas-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-26 09:34:04.384001 lanablas-0.0.8/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-06-20 12:16:48.000000 lanablas-0.0.8/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2158 2023-06-26 09:34:04.383725 lanablas-0.0.8/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1746 2023-06-26 09:29:17.000000 lanablas-0.0.8/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-26 09:34:04.381161 lanablas-0.0.8/lanablas/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1113 2023-06-26 09:29:12.000000 lanablas-0.0.8/lanablas/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    13248 2023-06-25 09:35:50.000000 lanablas-0.0.8/lanablas/matrix.c
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-26 09:34:04.383203 lanablas-0.0.8/lanablas.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2158 2023-06-26 09:34:03.000000 lanablas-0.0.8/lanablas.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      193 2023-06-26 09:34:04.000000 lanablas-0.0.8/lanablas.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-26 09:34:03.000000 lanablas-0.0.8/lanablas.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       16 2023-06-26 09:34:03.000000 lanablas-0.0.8/lanablas.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-06-26 09:34:04.384096 lanablas-0.0.8/setup.cfg
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1097 2023-06-26 09:33:55.000000 lanablas-0.0.8/setup.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-26 09:57:26.002445 lanablas-0.0.9/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-06-20 12:16:48.000000 lanablas-0.0.9/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2158 2023-06-26 09:57:26.002102 lanablas-0.0.9/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1746 2023-06-26 09:56:38.000000 lanablas-0.0.9/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-26 09:57:25.999034 lanablas-0.0.9/lanablas/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1113 2023-06-26 09:56:33.000000 lanablas-0.0.9/lanablas/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    13248 2023-06-25 09:35:50.000000 lanablas-0.0.9/lanablas/matrix.c
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-26 09:57:26.001465 lanablas-0.0.9/lanablas.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2158 2023-06-26 09:57:25.000000 lanablas-0.0.9/lanablas.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      193 2023-06-26 09:57:25.000000 lanablas-0.0.9/lanablas.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-26 09:57:25.000000 lanablas-0.0.9/lanablas.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       16 2023-06-26 09:57:25.000000 lanablas-0.0.9/lanablas.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-06-26 09:57:26.002575 lanablas-0.0.9/setup.cfg
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1617 2023-06-26 09:57:18.000000 lanablas-0.0.9/setup.py
```

### Comparing `lanablas-0.0.8/LICENSE` & `lanablas-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lanablas-0.0.8/PKG-INFO` & `lanablas-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanablas
-Version: 0.0.8
+Version: 0.0.9
 Summary: Extension module for matrix multiplication
 Author: Marco Salvalaggio
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas==0.0.8
+pip install lanablas==0.0.9
 ```
 
 ## Example 
 
 ```python
 from lanablas import Matrix
```

### Comparing `lanablas-0.0.8/README.md` & `lanablas-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas==0.0.8
+pip install lanablas==0.0.9
 ```
 
 ## Example 
 
 ```python
 from lanablas import Matrix
```

### Comparing `lanablas-0.0.8/lanablas/__init__.py` & `lanablas-0.0.9/lanablas/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Union, List
 from matrix import Matrix
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 
 def inject(data: Union[float, int, List, List[List]]) -> List[List[float]]:
     """
     Injects the input data into a matrix.
 
     Args:
```

### Comparing `lanablas-0.0.8/lanablas/matrix.c` & `lanablas-0.0.9/lanablas/matrix.c`

 * *Files identical despite different names*

### Comparing `lanablas-0.0.8/lanablas.egg-info/PKG-INFO` & `lanablas-0.0.9/lanablas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanablas
-Version: 0.0.8
+Version: 0.0.9
 Summary: Extension module for matrix multiplication
 Author: Marco Salvalaggio
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -26,15 +26,15 @@
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas==0.0.8
+pip install lanablas==0.0.9
 ```
 
 ## Example 
 
 ```python
 from lanablas import Matrix
```

