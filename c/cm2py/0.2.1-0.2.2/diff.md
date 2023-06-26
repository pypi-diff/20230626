# Comparing `tmp/cm2py-0.2.1.tar.gz` & `tmp/cm2py-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cm2py-0.2.1.tar", last modified: Sun Jun 25 04:25:36 2023, max compression
+gzip compressed data, was "cm2py-0.2.2.tar", last modified: Mon Jun 26 11:05:01 2023, max compression
```

## Comparing `cm2py-0.2.1.tar` & `cm2py-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 04:25:36.436139 cm2py-0.2.1/
--rw-rw-rw-   0        0        0     1116 2023-05-09 09:46:12.000000 cm2py-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     3012 2023-06-25 04:25:36.435139 cm2py-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1189 2023-06-25 04:24:23.000000 cm2py-0.2.1/README.md
--rw-rw-rw-   0        0        0      687 2023-06-25 04:24:27.000000 cm2py-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-25 04:25:36.437134 cm2py-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-25 04:25:36.356133 cm2py-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-25 04:25:36.380132 cm2py-0.2.1/src/cm2py/
--rw-rw-rw-   0        0        0      213 2023-05-21 06:01:41.000000 cm2py-0.2.1/src/cm2py/__init__.py
--rw-rw-rw-   0        0        0     6198 2023-06-25 04:24:27.000000 cm2py-0.2.1/src/cm2py/cm2py.py
-drwxrwxrwx   0        0        0        0 2023-06-25 04:25:36.426141 cm2py-0.2.1/src/cm2py.egg-info/
--rw-rw-rw-   0        0        0     3012 2023-06-25 04:25:36.000000 cm2py-0.2.1/src/cm2py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-06-25 04:25:36.000000 cm2py-0.2.1/src/cm2py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 04:25:36.000000 cm2py-0.2.1/src/cm2py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-25 04:25:36.000000 cm2py-0.2.1/src/cm2py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-25 04:25:36.000000 cm2py-0.2.1/src/cm2py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-25 04:25:36.431132 cm2py-0.2.1/tests/
--rw-rw-rw-   0        0        0     1671 2023-06-25 04:18:52.000000 cm2py-0.2.1/tests/test_app.py
+drwxrwxrwx   0        0        0        0 2023-06-26 11:05:01.153236 cm2py-0.2.2/
+-rw-rw-rw-   0        0        0     1116 2023-05-09 09:46:12.000000 cm2py-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     3012 2023-06-26 11:05:01.150227 cm2py-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1189 2023-06-25 04:24:23.000000 cm2py-0.2.2/README.md
+-rw-rw-rw-   0        0        0      675 2023-06-26 11:04:20.000000 cm2py-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 11:05:01.153236 cm2py-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 11:05:01.070226 cm2py-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 11:05:01.099225 cm2py-0.2.2/src/cm2py/
+-rw-rw-rw-   0        0        0      213 2023-05-21 06:01:41.000000 cm2py-0.2.2/src/cm2py/__init__.py
+-rw-rw-rw-   0        0        0     6211 2023-06-26 11:04:24.000000 cm2py-0.2.2/src/cm2py/cm2py.py
+drwxrwxrwx   0        0        0        0 2023-06-26 11:05:01.143226 cm2py-0.2.2/src/cm2py.egg-info/
+-rw-rw-rw-   0        0        0     3012 2023-06-26 11:05:01.000000 cm2py-0.2.2/src/cm2py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-06-26 11:05:01.000000 cm2py-0.2.2/src/cm2py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 11:05:01.000000 cm2py-0.2.2/src/cm2py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-26 11:05:01.000000 cm2py-0.2.2/src/cm2py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-26 11:05:01.000000 cm2py-0.2.2/src/cm2py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 11:05:01.147231 cm2py-0.2.2/tests/
+-rw-rw-rw-   0        0        0     1671 2023-06-25 04:18:52.000000 cm2py-0.2.2/tests/test_app.py
```

### Comparing `cm2py-0.2.1/LICENSE` & `cm2py-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cm2py-0.2.1/PKG-INFO` & `cm2py-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm2py
-Version: 0.2.1
+Version: 0.2.2
 Summary: Circuit Maker 2 save generation and manipulation package
 Author-email: SKM GEEK <qestudios17@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cm2py-0.2.1/README.md` & `cm2py-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cm2py-0.2.1/pyproject.toml` & `cm2py-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cm2py"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="SKM GEEK", email="qestudios17@gmail.com" },
 ]
 description = "Circuit Maker 2 save generation and manipulation package"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "uuid",
-  "numpy"
+  "uuid"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/QEStudios/cm2py"
 "Bug Tracker" = "https://github.com/QEStudios/cm2py/issues"
```

### Comparing `cm2py-0.2.1/src/cm2py/cm2py.py` & `cm2py-0.2.2/src/cm2py/cm2py.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 __copyright__ = "Copyright 2023, SKM GEEK"
 __date__ = "2023/05/21"
 __deprecated__ = False
 __email__ = "qestudios17@example.com"
 __license__ = "MIT"
 __maintainer__ = "SKM GEEK"
 __status__ = "Production"
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 import re
 from uuid import UUID, uuid4
-import numpy as np
+import math
 
 
 class Save:
     """A class to represent a save, which can be modified."""
 
     def __init__(self):
         self.blocks = []
         self.connections = {}
 
     def addBlock(self, blockId, pos, state=False, properties=None, snapToGrid=True):
         """Add a block to the save."""
         if snapToGrid:
-            newBlock = Block(blockId, tuple(np.floor(pos)), state=state, properties=properties)
+            newBlock = Block(blockId, tuple([int(math.floor(i)) for i in pos]), state=state, properties=properties)
         else:
             newBlock = Block(blockId, pos, state=state, properties=properties)
         self.blocks.append(newBlock)
         return newBlock
 
     def addConnection(self, source, target):
         """Add a connection to the save."""
```

### Comparing `cm2py-0.2.1/src/cm2py.egg-info/PKG-INFO` & `cm2py-0.2.2/src/cm2py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm2py
-Version: 0.2.1
+Version: 0.2.2
 Summary: Circuit Maker 2 save generation and manipulation package
 Author-email: SKM GEEK <qestudios17@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cm2py-0.2.1/tests/test_app.py` & `cm2py-0.2.2/tests/test_app.py`

 * *Files identical despite different names*

