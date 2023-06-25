# Comparing `tmp/traffsimpy-0.1.2.tar.gz` & `tmp/traffsimpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traffsimpy-0.1.2.tar", last modified: Sun Jun 25 23:13:54 2023, max compression
+gzip compressed data, was "traffsimpy-0.1.3.tar", last modified: Sun Jun 25 23:40:54 2023, max compression
```

## Comparing `traffsimpy-0.1.2.tar` & `traffsimpy-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-25 23:13:54.697947 traffsimpy-0.1.2/
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     1075 2023-06-09 14:22:54.000000 traffsimpy-0.1.2/LICENSE
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     3180 2023-06-25 23:13:54.697764 traffsimpy-0.1.2/PKG-INFO
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     1443 2023-06-25 23:06:42.000000 traffsimpy-0.1.2/README.md
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)      795 2023-06-25 23:09:32.000000 traffsimpy-0.1.2/pyproject.toml
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)       38 2023-06-25 23:13:54.698000 traffsimpy-0.1.2/setup.cfg
-drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-25 23:13:54.691434 traffsimpy-0.1.2/src/
-drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-25 23:13:54.691510 traffsimpy-0.1.2/src/traffsimpy/
-drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-25 23:13:54.696579 traffsimpy-0.1.2/src/traffsimpy/traffsimpy/
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)      433 2023-06-25 23:13:44.000000 traffsimpy-0.1.2/src/traffsimpy/traffsimpy/__init__.py
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)    48602 2023-06-08 11:28:29.000000 traffsimpy-0.1.2/src/traffsimpy/traffsimpy/components.py
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     2480 2023-06-25 22:40:59.000000 traffsimpy-0.1.2/src/traffsimpy/traffsimpy/constants.py
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     4210 2023-06-06 12:17:56.000000 traffsimpy-0.1.2/src/traffsimpy/traffsimpy/drawing.py
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     9649 2023-06-05 18:36:17.000000 traffsimpy-0.1.2/src/traffsimpy/traffsimpy/math_and_util.py
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     8334 2023-06-07 11:47:16.000000 traffsimpy-0.1.2/src/traffsimpy/traffsimpy/settings.py
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)    38015 2023-06-06 14:10:20.000000 traffsimpy-0.1.2/src/traffsimpy/traffsimpy/simulation.py
-drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-25 23:13:54.693074 traffsimpy-0.1.2/src/traffsimpy.egg-info/
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     3180 2023-06-25 23:13:54.000000 traffsimpy-0.1.2/src/traffsimpy.egg-info/PKG-INFO
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)      496 2023-06-25 23:13:54.000000 traffsimpy-0.1.2/src/traffsimpy.egg-info/SOURCES.txt
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)        1 2023-06-25 23:13:54.000000 traffsimpy-0.1.2/src/traffsimpy.egg-info/dependency_links.txt
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)      104 2023-06-25 23:13:54.000000 traffsimpy-0.1.2/src/traffsimpy.egg-info/requires.txt
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)       11 2023-06-25 23:13:54.000000 traffsimpy-0.1.2/src/traffsimpy.egg-info/top_level.txt
+drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-25 23:40:54.766632 traffsimpy-0.1.3/
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     1075 2023-06-09 14:22:54.000000 traffsimpy-0.1.3/LICENSE
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     3180 2023-06-25 23:40:54.766386 traffsimpy-0.1.3/PKG-INFO
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     1443 2023-06-25 23:06:42.000000 traffsimpy-0.1.3/README.md
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)      795 2023-06-25 23:40:48.000000 traffsimpy-0.1.3/pyproject.toml
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)       38 2023-06-25 23:40:54.766778 traffsimpy-0.1.3/setup.cfg
+drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-25 23:40:54.760480 traffsimpy-0.1.3/src/
+drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-25 23:40:54.763923 traffsimpy-0.1.3/src/traffsimpy/
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)      433 2023-06-25 23:40:48.000000 traffsimpy-0.1.3/src/traffsimpy/__init__.py
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)    48602 2023-06-08 11:28:29.000000 traffsimpy-0.1.3/src/traffsimpy/components.py
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     2478 2023-06-25 23:40:18.000000 traffsimpy-0.1.3/src/traffsimpy/constants.py
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     4210 2023-06-06 12:17:56.000000 traffsimpy-0.1.3/src/traffsimpy/drawing.py
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     9649 2023-06-05 18:36:17.000000 traffsimpy-0.1.3/src/traffsimpy/math_and_util.py
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     8334 2023-06-07 11:47:16.000000 traffsimpy-0.1.3/src/traffsimpy/settings.py
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)    38015 2023-06-06 14:10:20.000000 traffsimpy-0.1.3/src/traffsimpy/simulation.py
+drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-25 23:40:54.766034 traffsimpy-0.1.3/src/traffsimpy.egg-info/
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     3180 2023-06-25 23:40:54.000000 traffsimpy-0.1.3/src/traffsimpy.egg-info/PKG-INFO
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)      419 2023-06-25 23:40:54.000000 traffsimpy-0.1.3/src/traffsimpy.egg-info/SOURCES.txt
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)        1 2023-06-25 23:40:54.000000 traffsimpy-0.1.3/src/traffsimpy.egg-info/dependency_links.txt
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)      104 2023-06-25 23:40:54.000000 traffsimpy-0.1.3/src/traffsimpy.egg-info/requires.txt
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)       11 2023-06-25 23:40:54.000000 traffsimpy-0.1.3/src/traffsimpy.egg-info/top_level.txt
```

### Comparing `traffsimpy-0.1.2/LICENSE` & `traffsimpy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.2/PKG-INFO` & `traffsimpy-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traffsimpy
-Version: 0.1.2
+Version: 0.1.3
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
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TraffSimPy
 
 Module Python permettant de modéliser le trafic routier de n'importe quel réseau.
```

### Comparing `traffsimpy-0.1.2/README.md` & `traffsimpy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.2/pyproject.toml` & `traffsimpy-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "traffsimpy"
-version = "0.1.2"
+version = "0.1.3"
 description = "Simulate traffic flow"
 readme = "README.md"
 authors = [{ name = "Hippolyte Cosserat", email = "hippolytecosserat@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -20,11 +20,11 @@
     "matplotlib>=3.7.0",
     "numpy>=1.24.2",
     "pandas>=1.5.3",
     "pygame>=2.1.3",
     "PyYAML>=6.0",
     "webcolors>=1.12"]
 
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 
 [project.urls]
 Homepage = "https://github.com/hcosserat/traffsimpy"
```

### Comparing `traffsimpy-0.1.2/src/traffsimpy/traffsimpy/components.py` & `traffsimpy-0.1.3/src/traffsimpy/components.py`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.2/src/traffsimpy/traffsimpy/constants.py` & `traffsimpy-0.1.3/src/traffsimpy/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from colorama import Fore, Style
 from importlib.resources import files
 
 INF = float("+inf")
 
-DEF_FONT_PATH = files("traffsimpy.resources").joinpath("resources/jbmono.ttf")
-DEF_ARROW_PATH = files("traffsimpy.resources").joinpath("resources/chevron.svg")
+DEF_FONT_PATH = files("traffsimp.resources").joinpath("resources/jbmono.ttf")
+DEF_ARROW_PATH = files("traffsimp.resources").joinpath("resources/chevron.svg")
 
 TXT_RED = Fore.RED
 TXT_BOLD = Style.BRIGHT
 TXT_RESET = Style.RESET_ALL
 
 BLACK = (0, 0, 0)
 WHITE = (255, 255, 255)
```

### Comparing `traffsimpy-0.1.2/src/traffsimpy/traffsimpy/drawing.py` & `traffsimpy-0.1.3/src/traffsimpy/drawing.py`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.2/src/traffsimpy/traffsimpy/math_and_util.py` & `traffsimpy-0.1.3/src/traffsimpy/math_and_util.py`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.2/src/traffsimpy/traffsimpy/settings.py` & `traffsimpy-0.1.3/src/traffsimpy/settings.py`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.2/src/traffsimpy/traffsimpy/simulation.py` & `traffsimpy-0.1.3/src/traffsimpy/simulation.py`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.2/src/traffsimpy.egg-info/PKG-INFO` & `traffsimpy-0.1.3/src/traffsimpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traffsimpy
-Version: 0.1.2
+Version: 0.1.3
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
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TraffSimPy
 
 Module Python permettant de modéliser le trafic routier de n'importe quel réseau.
```

