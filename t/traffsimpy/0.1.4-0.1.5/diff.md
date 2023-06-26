# Comparing `tmp/traffsimpy-0.1.4.tar.gz` & `tmp/traffsimpy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traffsimpy-0.1.4.tar", last modified: Sun Jun 25 23:48:14 2023, max compression
+gzip compressed data, was "traffsimpy-0.1.5.tar", last modified: Mon Jun 26 09:26:17 2023, max compression
```

## Comparing `traffsimpy-0.1.4.tar` & `traffsimpy-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-25 23:48:14.172613 traffsimpy-0.1.4/
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     1075 2023-06-09 14:22:54.000000 traffsimpy-0.1.4/LICENSE
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     3180 2023-06-25 23:48:14.172419 traffsimpy-0.1.4/PKG-INFO
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     1443 2023-06-25 23:06:42.000000 traffsimpy-0.1.4/README.md
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)      795 2023-06-25 23:48:07.000000 traffsimpy-0.1.4/pyproject.toml
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)       38 2023-06-25 23:48:14.172675 traffsimpy-0.1.4/setup.cfg
-drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-25 23:48:14.166533 traffsimpy-0.1.4/src/
-drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-25 23:48:14.170089 traffsimpy-0.1.4/src/traffsimpy/
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)      433 2023-06-25 23:48:07.000000 traffsimpy-0.1.4/src/traffsimpy/__init__.py
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)    48602 2023-06-08 11:28:29.000000 traffsimpy-0.1.4/src/traffsimpy/components.py
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     2480 2023-06-25 23:47:20.000000 traffsimpy-0.1.4/src/traffsimpy/constants.py
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     4210 2023-06-06 12:17:56.000000 traffsimpy-0.1.4/src/traffsimpy/drawing.py
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     9649 2023-06-05 18:36:17.000000 traffsimpy-0.1.4/src/traffsimpy/math_and_util.py
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     8334 2023-06-07 11:47:16.000000 traffsimpy-0.1.4/src/traffsimpy/settings.py
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)    38015 2023-06-06 14:10:20.000000 traffsimpy-0.1.4/src/traffsimpy/simulation.py
-drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-25 23:48:14.172117 traffsimpy-0.1.4/src/traffsimpy.egg-info/
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)     3180 2023-06-25 23:48:14.000000 traffsimpy-0.1.4/src/traffsimpy.egg-info/PKG-INFO
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)      419 2023-06-25 23:48:14.000000 traffsimpy-0.1.4/src/traffsimpy.egg-info/SOURCES.txt
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)        1 2023-06-25 23:48:14.000000 traffsimpy-0.1.4/src/traffsimpy.egg-info/dependency_links.txt
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)      104 2023-06-25 23:48:14.000000 traffsimpy-0.1.4/src/traffsimpy.egg-info/requires.txt
--rw-r--r--   0 hippolytecosserat   (501) staff       (20)       11 2023-06-25 23:48:14.000000 traffsimpy-0.1.4/src/traffsimpy.egg-info/top_level.txt
+drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-26 09:26:17.250253 traffsimpy-0.1.5/
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     1075 2023-06-09 14:22:54.000000 traffsimpy-0.1.5/LICENSE
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     3180 2023-06-26 09:26:17.250075 traffsimpy-0.1.5/PKG-INFO
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     1443 2023-06-25 23:06:42.000000 traffsimpy-0.1.5/README.md
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)      795 2023-06-26 09:25:29.000000 traffsimpy-0.1.5/pyproject.toml
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)       38 2023-06-26 09:26:17.250315 traffsimpy-0.1.5/setup.cfg
+drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-26 09:26:17.244109 traffsimpy-0.1.5/src/
+drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-26 09:26:17.247887 traffsimpy-0.1.5/src/traffsimpy/
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)      433 2023-06-26 09:25:29.000000 traffsimpy-0.1.5/src/traffsimpy/__init__.py
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)    48602 2023-06-08 11:28:29.000000 traffsimpy-0.1.5/src/traffsimpy/components.py
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     2468 2023-06-26 09:23:22.000000 traffsimpy-0.1.5/src/traffsimpy/constants.py
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     4210 2023-06-06 12:17:56.000000 traffsimpy-0.1.5/src/traffsimpy/drawing.py
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     9649 2023-06-05 18:36:17.000000 traffsimpy-0.1.5/src/traffsimpy/math_and_util.py
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     8334 2023-06-07 11:47:16.000000 traffsimpy-0.1.5/src/traffsimpy/settings.py
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)    38015 2023-06-06 14:10:20.000000 traffsimpy-0.1.5/src/traffsimpy/simulation.py
+drwxr-xr-x   0 hippolytecosserat   (501) staff       (20)        0 2023-06-26 09:26:17.249788 traffsimpy-0.1.5/src/traffsimpy.egg-info/
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)     3180 2023-06-26 09:26:17.000000 traffsimpy-0.1.5/src/traffsimpy.egg-info/PKG-INFO
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)      419 2023-06-26 09:26:17.000000 traffsimpy-0.1.5/src/traffsimpy.egg-info/SOURCES.txt
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)        1 2023-06-26 09:26:17.000000 traffsimpy-0.1.5/src/traffsimpy.egg-info/dependency_links.txt
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)      104 2023-06-26 09:26:17.000000 traffsimpy-0.1.5/src/traffsimpy.egg-info/requires.txt
+-rw-r--r--   0 hippolytecosserat   (501) staff       (20)       11 2023-06-26 09:26:17.000000 traffsimpy-0.1.5/src/traffsimpy.egg-info/top_level.txt
```

### Comparing `traffsimpy-0.1.4/LICENSE` & `traffsimpy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.4/PKG-INFO` & `traffsimpy-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traffsimpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simulate traffic flow
 Author-email: Hippolyte Cosserat <hippolytecosserat@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hippolyte Cosserat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `traffsimpy-0.1.4/README.md` & `traffsimpy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.4/pyproject.toml` & `traffsimpy-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "traffsimpy"
-version = "0.1.4"
+version = "0.1.5"
 description = "Simulate traffic flow"
 readme = "README.md"
 authors = [{ name = "Hippolyte Cosserat", email = "hippolytecosserat@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `traffsimpy-0.1.4/src/traffsimpy/components.py` & `traffsimpy-0.1.5/src/traffsimpy/components.py`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.4/src/traffsimpy/constants.py` & `traffsimpy-0.1.5/src/traffsimpy/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from colorama import Fore, Style
 from importlib.resources import files
 
 INF = float("+inf")
 
-DEF_FONT_PATH = files("traffsimpy.resources").joinpath("resources/jbmono.ttf")
-DEF_ARROW_PATH = files("traffsimpy.resources").joinpath("resources/chevron.svg")
+DEF_FONT_PATH = files("src.traffsimpy").joinpath("resources/jbmono.ttf")
+DEF_ARROW_PATH = files("src.traffsimpy").joinpath("resources/chevron.svg")
 
 TXT_RED = Fore.RED
 TXT_BOLD = Style.BRIGHT
 TXT_RESET = Style.RESET_ALL
 
 BLACK = (0, 0, 0)
 WHITE = (255, 255, 255)
```

### Comparing `traffsimpy-0.1.4/src/traffsimpy/drawing.py` & `traffsimpy-0.1.5/src/traffsimpy/drawing.py`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.4/src/traffsimpy/math_and_util.py` & `traffsimpy-0.1.5/src/traffsimpy/math_and_util.py`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.4/src/traffsimpy/settings.py` & `traffsimpy-0.1.5/src/traffsimpy/settings.py`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.4/src/traffsimpy/simulation.py` & `traffsimpy-0.1.5/src/traffsimpy/simulation.py`

 * *Files identical despite different names*

### Comparing `traffsimpy-0.1.4/src/traffsimpy.egg-info/PKG-INFO` & `traffsimpy-0.1.5/src/traffsimpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traffsimpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simulate traffic flow
 Author-email: Hippolyte Cosserat <hippolytecosserat@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hippolyte Cosserat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

