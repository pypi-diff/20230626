# Comparing `tmp/traffsimpy-0.1.7.tar.gz` & `tmp/traffsimpy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traffsimpy-0.1.7.tar", last modified: Mon Jun 26 10:07:30 2023, max compression
+gzip compressed data, was "traffsimpy-0.1.8.tar", last modified: Mon Jun 26 10:41:20 2023, max compression
```

## Comparing `traffsimpy-0.1.7.tar` & `traffsimpy-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-26 10:07:30.800238 traffsimpy-0.1.7/
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     1075 2023-06-09 14:22:54.000000 traffsimpy-0.1.7/LICENSE
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)       35 2023-06-26 10:06:48.000000 traffsimpy-0.1.7/MANIFEST.in
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     3180 2023-06-26 10:07:30.800037 traffsimpy-0.1.7/PKG-INFO
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     1443 2023-06-25 23:06:42.000000 traffsimpy-0.1.7/README.md
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)      844 2023-06-26 10:07:22.000000 traffsimpy-0.1.7/pyproject.toml
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)       38 2023-06-26 10:07:30.800304 traffsimpy-0.1.7/setup.cfg
-drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-26 10:07:30.791181 traffsimpy-0.1.7/src/
-drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-26 10:07:30.795316 traffsimpy-0.1.7/src/traffsimpy/
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)      433 2023-06-26 10:07:22.000000 traffsimpy-0.1.7/src/traffsimpy/__init__.py
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)    48602 2023-06-08 11:28:29.000000 traffsimpy-0.1.7/src/traffsimpy/components.py
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     2460 2023-06-26 09:28:57.000000 traffsimpy-0.1.7/src/traffsimpy/constants.py
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     4210 2023-06-06 12:17:56.000000 traffsimpy-0.1.7/src/traffsimpy/drawing.py
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     9649 2023-06-05 18:36:17.000000 traffsimpy-0.1.7/src/traffsimpy/math_and_util.py
-drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-26 10:07:30.798865 traffsimpy-0.1.7/src/traffsimpy/resources/
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     6148 2023-02-14 10:32:23.000000 traffsimpy-0.1.7/src/traffsimpy/resources/.DS_Store
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)      436 2023-03-16 21:46:18.000000 traffsimpy-0.1.7/src/traffsimpy/resources/chevron.svg
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)   203952 2022-11-19 17:31:29.000000 traffsimpy-0.1.7/src/traffsimpy/resources/jbmono.ttf
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     8334 2023-06-07 11:47:16.000000 traffsimpy-0.1.7/src/traffsimpy/settings.py
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)    38015 2023-06-06 14:10:20.000000 traffsimpy-0.1.7/src/traffsimpy/simulation.py
-drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-26 10:07:30.797361 traffsimpy-0.1.7/src/traffsimpy.egg-info/
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     3180 2023-06-26 10:07:30.000000 traffsimpy-0.1.7/src/traffsimpy.egg-info/PKG-INFO
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)      539 2023-06-26 10:07:30.000000 traffsimpy-0.1.7/src/traffsimpy.egg-info/SOURCES.txt
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)        1 2023-06-26 10:07:30.000000 traffsimpy-0.1.7/src/traffsimpy.egg-info/dependency_links.txt
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)      104 2023-06-26 10:07:30.000000 traffsimpy-0.1.7/src/traffsimpy.egg-info/requires.txt
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)       11 2023-06-26 10:07:30.000000 traffsimpy-0.1.7/src/traffsimpy.egg-info/top_level.txt
+drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-26 10:41:20.302471 traffsimpy-0.1.8/
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     1075 2023-06-09 14:22:54.000000 traffsimpy-0.1.8/LICENSE
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)       35 2023-06-26 10:06:48.000000 traffsimpy-0.1.8/MANIFEST.in
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     3181 2023-06-26 10:41:20.302261 traffsimpy-0.1.8/PKG-INFO
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     1443 2023-06-25 23:06:42.000000 traffsimpy-0.1.8/README.md
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)      845 2023-06-26 10:41:13.000000 traffsimpy-0.1.8/pyproject.toml
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)       38 2023-06-26 10:41:20.302534 traffsimpy-0.1.8/setup.cfg
+drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-26 10:41:20.294326 traffsimpy-0.1.8/src/
+drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-26 10:41:20.298122 traffsimpy-0.1.8/src/traffsimpy/
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)      433 2023-06-26 10:41:13.000000 traffsimpy-0.1.8/src/traffsimpy/__init__.py
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)    48602 2023-06-08 11:28:29.000000 traffsimpy-0.1.8/src/traffsimpy/components.py
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     2460 2023-06-26 09:28:57.000000 traffsimpy-0.1.8/src/traffsimpy/constants.py
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     4210 2023-06-06 12:17:56.000000 traffsimpy-0.1.8/src/traffsimpy/drawing.py
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     9649 2023-06-05 18:36:17.000000 traffsimpy-0.1.8/src/traffsimpy/math_and_util.py
+drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-26 10:41:20.301130 traffsimpy-0.1.8/src/traffsimpy/resources/
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     6148 2023-02-14 10:32:23.000000 traffsimpy-0.1.8/src/traffsimpy/resources/.DS_Store
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)      436 2023-03-16 21:46:18.000000 traffsimpy-0.1.8/src/traffsimpy/resources/chevron.svg
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)   203952 2022-11-19 17:31:29.000000 traffsimpy-0.1.8/src/traffsimpy/resources/jbmono.ttf
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     8334 2023-06-07 11:47:16.000000 traffsimpy-0.1.8/src/traffsimpy/settings.py
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)    38015 2023-06-06 14:10:20.000000 traffsimpy-0.1.8/src/traffsimpy/simulation.py
+drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-26 10:41:20.300126 traffsimpy-0.1.8/src/traffsimpy.egg-info/
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     3181 2023-06-26 10:41:20.000000 traffsimpy-0.1.8/src/traffsimpy.egg-info/PKG-INFO
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)      539 2023-06-26 10:41:20.000000 traffsimpy-0.1.8/src/traffsimpy.egg-info/SOURCES.txt
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)        1 2023-06-26 10:41:20.000000 traffsimpy-0.1.8/src/traffsimpy.egg-info/dependency_links.txt
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)      104 2023-06-26 10:41:20.000000 traffsimpy-0.1.8/src/traffsimpy.egg-info/requires.txt
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)       11 2023-06-26 10:41:20.000000 traffsimpy-0.1.8/src/traffsimpy.egg-info/top_level.txt
```

### Comparing `traffsimpy-0.1.7/LICENSE` & `traffsimpy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.7/PKG-INFO` & `traffsimpy-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traffsimpy
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simulate traffic flow
 Author-email: Hippolyte Cosserat <hippolytecosserat@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hippolyte Cosserat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/hcosserat/traffsimpy
 Keywords: simulation,traffic,vehicules,roads
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TraffSimPy
 
 Module Python permettant de modéliser le trafic routier de n'importe quel réseau.
```

### Comparing `traffsimpy-0.1.7/README.md` & `traffsimpy-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.7/pyproject.toml` & `traffsimpy-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "traffsimpy"
-version = "0.1.7"
+version = "0.1.8"
 description = "Simulate traffic flow"
 readme = "README.md"
 authors = [{ name = "Hippolyte Cosserat", email = "hippolytecosserat@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -23,11 +23,11 @@
     "matplotlib>=3.7.0",
     "numpy>=1.24.2",
     "pandas>=1.5.3",
     "pygame>=2.1.3",
     "PyYAML>=6.0",
     "webcolors>=1.12"]
 
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 
 [project.urls]
 Homepage = "https://github.com/hcosserat/traffsimpy"
```

### Comparing `traffsimpy-0.1.7/src/traffsimpy/components.py` & `traffsimpy-0.1.8/src/traffsimpy/components.py`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.7/src/traffsimpy/constants.py` & `traffsimpy-0.1.8/src/traffsimpy/constants.py`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.7/src/traffsimpy/drawing.py` & `traffsimpy-0.1.8/src/traffsimpy/drawing.py`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.7/src/traffsimpy/math_and_util.py` & `traffsimpy-0.1.8/src/traffsimpy/math_and_util.py`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.7/src/traffsimpy/resources/.DS_Store` & `traffsimpy-0.1.8/src/traffsimpy/resources/.DS_Store`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.7/src/traffsimpy/resources/jbmono.ttf` & `traffsimpy-0.1.8/src/traffsimpy/resources/jbmono.ttf`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.7/src/traffsimpy/settings.py` & `traffsimpy-0.1.8/src/traffsimpy/settings.py`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.7/src/traffsimpy/simulation.py` & `traffsimpy-0.1.8/src/traffsimpy/simulation.py`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.7/src/traffsimpy.egg-info/PKG-INFO` & `traffsimpy-0.1.8/src/traffsimpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traffsimpy
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simulate traffic flow
 Author-email: Hippolyte Cosserat <hippolytecosserat@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hippolyte Cosserat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/hcosserat/traffsimpy
 Keywords: simulation,traffic,vehicules,roads
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TraffSimPy
 
 Module Python permettant de modéliser le trafic routier de n'importe quel réseau.
```

### Comparing `traffsimpy-0.1.7/src/traffsimpy.egg-info/SOURCES.txt` & `traffsimpy-0.1.8/src/traffsimpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

