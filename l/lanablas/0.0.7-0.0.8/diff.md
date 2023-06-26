# Comparing `tmp/lanablas-0.0.7.tar.gz` & `tmp/lanablas-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanablas-0.0.7.tar", last modified: Sun Jun 25 09:32:20 2023, max compression
+gzip compressed data, was "lanablas-0.0.8.tar", last modified: Mon Jun 26 09:34:04 2023, max compression
```

## Comparing `lanablas-0.0.7.tar` & `lanablas-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-25 09:32:20.522398 lanablas-0.0.7/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-06-20 12:16:48.000000 lanablas-0.0.7/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1959 2023-06-25 09:32:20.522155 lanablas-0.0.7/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1547 2023-06-25 09:11:41.000000 lanablas-0.0.7/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-25 09:32:20.520703 lanablas-0.0.7/lanablas/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1113 2023-06-25 09:18:54.000000 lanablas-0.0.7/lanablas/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    13273 2023-06-25 09:32:14.000000 lanablas-0.0.7/lanablas/matrix.c
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-25 09:32:20.521792 lanablas-0.0.7/lanablas.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1959 2023-06-25 09:32:19.000000 lanablas-0.0.7/lanablas.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      193 2023-06-25 09:32:20.000000 lanablas-0.0.7/lanablas.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-25 09:32:19.000000 lanablas-0.0.7/lanablas.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       16 2023-06-25 09:32:20.000000 lanablas-0.0.7/lanablas.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-06-25 09:32:20.522481 lanablas-0.0.7/setup.cfg
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1116 2023-06-25 09:11:36.000000 lanablas-0.0.7/setup.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-26 09:34:04.384001 lanablas-0.0.8/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-06-20 12:16:48.000000 lanablas-0.0.8/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2158 2023-06-26 09:34:04.383725 lanablas-0.0.8/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1746 2023-06-26 09:29:17.000000 lanablas-0.0.8/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-26 09:34:04.381161 lanablas-0.0.8/lanablas/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1113 2023-06-26 09:29:12.000000 lanablas-0.0.8/lanablas/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    13248 2023-06-25 09:35:50.000000 lanablas-0.0.8/lanablas/matrix.c
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-26 09:34:04.383203 lanablas-0.0.8/lanablas.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2158 2023-06-26 09:34:03.000000 lanablas-0.0.8/lanablas.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      193 2023-06-26 09:34:04.000000 lanablas-0.0.8/lanablas.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-26 09:34:03.000000 lanablas-0.0.8/lanablas.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       16 2023-06-26 09:34:03.000000 lanablas-0.0.8/lanablas.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-06-26 09:34:04.384096 lanablas-0.0.8/setup.cfg
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1097 2023-06-26 09:33:55.000000 lanablas-0.0.8/setup.py
```

### Comparing `lanablas-0.0.7/LICENSE` & `lanablas-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lanablas-0.0.7/PKG-INFO` & `lanablas-0.0.8/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,26 @@
-Metadata-Version: 2.1
-Name: lanablas
-Version: 0.0.7
-Summary: Extension module for matrix multiplication
-Author: Marco Salvalaggio
-Author-email: mar.salvalaggio@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## LanaBLAS 🐑
 
-[![stability-wip](https://img.shields.io/badge/stability-wip-lightgrey.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#work-in-progress) [![macOS](https://img.shields.io/badge/macos-compatible-brightgreen.svg)](https://github.com/your-repo) [![Windows](https://img.shields.io/badge/windows-not%20compatible-red.svg)](https://github.com/your-repo) [![Linux](https://img.shields.io/badge/linux-not%20compatible-red.svg)](https://github.com/your-repo) [![Tests Passing](https://img.shields.io/badge/tests-passing-brightgreen.svg)](https://github.com/your-repo)
+[![stability-wip](https://img.shields.io/badge/stability-wip-lightgrey.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#work-in-progress) [![macOS](https://img.shields.io/badge/macos-compatible-brightgreen.svg)](https://github.com/your-repo) [![Windows](https://img.shields.io/badge/windows-not%20compatible-red.svg)](https://github.com/your-repo) [![Linux](https://img.shields.io/badge/linux-not%20compatible-red.svg)](https://github.com/your-repo) [![Tests Passing](https://img.shields.io/badge/tests-passing-brightgreen.svg)](https://github.com/your-repo) [![PyPI - Status](https://img.shields.io/pypi/v/lanablas.svg)](https://pypi.org/project/lanablas/) [![Project Status](https://img.shields.io/badge/status-broken-red)](https://github.com/USER/REPO)
+
+
 
 
 **L***inear* **A**lgebra for **n***octurnal* *and* **a**dventurous *data scientists exploring **BLAS***
 
 
 **LanaBLAS** is a repository primarily used for testing the development of CPython extension modules with external dependencies, such as ([OpenBLAS](https://github.com/xianyi/OpenBLAS)). It's a work-in-progress memetic project aimed at having fun and learning new things.
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas==0.0.7
+pip install lanablas==0.0.8
 ```
 
 ## Example 
 
 ```python
 from lanablas import Matrix
 
@@ -47,9 +35,7 @@
 c = a + b
 print(c)
 print(type(c), b.shape)
 ```
 
 For more comprehensive examples, please visit the [examples](https://github.com/marcosalvalaggio/lana-blas/tree/main/examples) folder
 
-
-
```

### Comparing `lanablas-0.0.7/lanablas/__init__.py` & `lanablas-0.0.8/lanablas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Union, List
 from matrix import Matrix
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 
 def inject(data: Union[float, int, List, List[List]]) -> List[List[float]]:
     """
     Injects the input data into a matrix.
 
     Args:
```

### Comparing `lanablas-0.0.7/lanablas/matrix.c` & `lanablas-0.0.8/lanablas/matrix.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-//TODO - Matrix_negative
 //TODO - Matrix_pow
 //TODO - Matrix_matmul
 //TODO - Matrix_truediv
 #include <Python.h>
 #include <cblas.h>
```

### Comparing `lanablas-0.0.7/lanablas.egg-info/PKG-INFO` & `lanablas-0.0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: lanablas
-Version: 0.0.7
+Version: 0.0.8
 Summary: Extension module for matrix multiplication
 Author: Marco Salvalaggio
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## LanaBLAS 🐑
 
-[![stability-wip](https://img.shields.io/badge/stability-wip-lightgrey.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#work-in-progress) [![macOS](https://img.shields.io/badge/macos-compatible-brightgreen.svg)](https://github.com/your-repo) [![Windows](https://img.shields.io/badge/windows-not%20compatible-red.svg)](https://github.com/your-repo) [![Linux](https://img.shields.io/badge/linux-not%20compatible-red.svg)](https://github.com/your-repo) [![Tests Passing](https://img.shields.io/badge/tests-passing-brightgreen.svg)](https://github.com/your-repo)
+[![stability-wip](https://img.shields.io/badge/stability-wip-lightgrey.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#work-in-progress) [![macOS](https://img.shields.io/badge/macos-compatible-brightgreen.svg)](https://github.com/your-repo) [![Windows](https://img.shields.io/badge/windows-not%20compatible-red.svg)](https://github.com/your-repo) [![Linux](https://img.shields.io/badge/linux-not%20compatible-red.svg)](https://github.com/your-repo) [![Tests Passing](https://img.shields.io/badge/tests-passing-brightgreen.svg)](https://github.com/your-repo) [![PyPI - Status](https://img.shields.io/pypi/v/lanablas.svg)](https://pypi.org/project/lanablas/) [![Project Status](https://img.shields.io/badge/status-broken-red)](https://github.com/USER/REPO)
+
+
 
 
 **L***inear* **A**lgebra for **n***octurnal* *and* **a**dventurous *data scientists exploring **BLAS***
 
 
 **LanaBLAS** is a repository primarily used for testing the development of CPython extension modules with external dependencies, such as ([OpenBLAS](https://github.com/xianyi/OpenBLAS)). It's a work-in-progress memetic project aimed at having fun and learning new things.
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas==0.0.7
+pip install lanablas==0.0.8
 ```
 
 ## Example 
 
 ```python
 from lanablas import Matrix
```

### Comparing `lanablas-0.0.7/setup.py` & `lanablas-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,22 +7,22 @@
     long_description = f.read()
 
 
 module_extension = Extension(
     'matrix',
     sources=['lanablas/matrix.c'],
     libraries=['openblas'],  # Link against the BLAS library
-    extra_compile_args=['-std=c11'],  # Set the C standard to C11
-    include_dirs=['/usr/local/opt/openblas/include'],  # BLAS include directory
-    library_dirs=['/usr/local/opt/openblas/lib'],  # BLAS library directory
+    extra_compile_args=['-std=c11'],
+    include_dirs=['openblas/include'],  # BLAS include directory within your package
+    library_dirs=['openblas/lib'],  # BLAS library directory within your package
 )
 
 setup(
 name='lanablas',
-    version='0.0.7',
+    version='0.0.8',
     description='Extension module for matrix multiplication',
     author='Marco Salvalaggio',
     author_email='mar.salvalaggio@gmail.com',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['lanablas'],
```

