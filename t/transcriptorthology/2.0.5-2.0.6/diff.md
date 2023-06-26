# Comparing `tmp/transcriptorthology-2.0.5.tar.gz` & `tmp/transcriptorthology-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transcriptorthology-2.0.5.tar", last modified: Mon Jun 26 06:16:59 2023, max compression
+gzip compressed data, was "dist/transcriptorthology-2.0.6.tar", last modified: Mon Jun 26 06:21:30 2023, max compression
```

## Comparing `transcriptorthology-2.0.5.tar` & `transcriptorthology-2.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 06:16:59.000000 transcriptorthology-2.0.5/
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 06:16:59.000000 transcriptorthology-2.0.5/transcriptorthology/
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    23446 2023-06-26 06:15:40.000000 transcriptorthology-2.0.5/transcriptorthology/tsmComputing.py
--rw-------   0 ouew2201 (1811316550) domain^users (1810891265)      123 2023-06-26 04:51:12.000000 transcriptorthology-2.0.5/transcriptorthology/__init__.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2915 2023-06-26 06:15:33.000000 transcriptorthology-2.0.5/transcriptorthology/transcriptOrthology.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    15635 2023-06-26 06:15:25.000000 transcriptorthology-2.0.5/transcriptorthology/Tclustering.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     1091 2023-06-26 06:16:39.000000 transcriptorthology-2.0.5/setup.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      777 2023-06-26 06:16:59.000000 transcriptorthology-2.0.5/PKG-INFO
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       38 2023-06-26 06:16:59.000000 transcriptorthology-2.0.5/setup.cfg
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 06:16:59.000000 transcriptorthology-2.0.5/transcriptorthology.egg-info/
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)        1 2023-06-26 06:16:59.000000 transcriptorthology-2.0.5/transcriptorthology.egg-info/dependency_links.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      378 2023-06-26 06:16:59.000000 transcriptorthology-2.0.5/transcriptorthology.egg-info/SOURCES.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       41 2023-06-26 06:16:59.000000 transcriptorthology-2.0.5/transcriptorthology.egg-info/requires.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      777 2023-06-26 06:16:59.000000 transcriptorthology-2.0.5/transcriptorthology.egg-info/PKG-INFO
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       20 2023-06-26 06:16:59.000000 transcriptorthology-2.0.5/transcriptorthology.egg-info/top_level.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2180 2023-06-26 05:12:33.000000 transcriptorthology-2.0.5/README.md
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/transcriptorthology/
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    23446 2023-06-26 06:21:09.000000 transcriptorthology-2.0.6/transcriptorthology/tsmComputing.py
+-rw-------   0 ouew2201 (1811316550) domain^users (1810891265)      123 2023-06-26 06:21:16.000000 transcriptorthology-2.0.6/transcriptorthology/__init__.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2915 2023-06-26 06:21:03.000000 transcriptorthology-2.0.6/transcriptorthology/transcriptOrthology.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    15635 2023-06-26 06:20:56.000000 transcriptorthology-2.0.6/transcriptorthology/Tclustering.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     1071 2023-06-26 06:20:45.000000 transcriptorthology-2.0.6/setup.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2833 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/PKG-INFO
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       38 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/setup.cfg
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/transcriptorthology.egg-info/
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)        1 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/transcriptorthology.egg-info/dependency_links.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      378 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/transcriptorthology.egg-info/SOURCES.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       41 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/transcriptorthology.egg-info/requires.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2833 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/transcriptorthology.egg-info/PKG-INFO
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       20 2023-06-26 06:21:30.000000 transcriptorthology-2.0.6/transcriptorthology.egg-info/top_level.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2180 2023-06-26 05:12:33.000000 transcriptorthology-2.0.6/README.md
```

### Comparing `transcriptorthology-2.0.5/transcriptorthology/tsmComputing.py` & `transcriptorthology-2.0.6/transcriptorthology/tsmComputing.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ======
     https://github.com/UdeS-CoBIUS/TranscriptOrthology
 """
 __authors__ = ("Wend Yam Donald Davy Ouedraogo")
 __contact__ = ("wend.yam.donald.davy.usherbrooke.ca")
 __copyright__ = "CoBIUS lab at Université de Sherbrooke, QC, CANADA"
 __date__ = "2023-06-26"
-__version__= "2.0.5"
+__version__= "2.0.6"
 
 import pandas as pd
 import argparse
 import time
 import numpy as np
 
 def build_arg_parser():
```

### Comparing `transcriptorthology-2.0.5/transcriptorthology/transcriptOrthology.py` & `transcriptorthology-2.0.6/transcriptorthology/transcriptOrthology.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ======
     https://github.com/UdeS-CoBIUS/TranscriptOrthology
 """
 __authors__ = ("Wend Yam Donald Davy Ouedraogo")
 __contact__ = ("wend.yam.donald.davy.usherbrooke.ca")
 __copyright__ = "CoBIUS lab at Université de Sherbrooke, QC, CANADA"
 __date__ = "2023-06-26"
-__version__= "2.0.5"
+__version__= "2.0.6"
 
 
 import argparse
 from .Tclustering import get_orthology_graph
 from .tsmComputing import get_matrix
```

### Comparing `transcriptorthology-2.0.5/transcriptorthology/Tclustering.py` & `transcriptorthology-2.0.6/transcriptorthology/Tclustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ======
     https://github.com/UdeS-CoBIUS/TranscriptOrthology
 """
 __authors__ = ("Wend Yam Donald Davy Ouedraogo")
 __contact__ = ("wend.yam.donald.davy.usherbrooke.ca")
 __copyright__ = "CoBIUS lab at Université de Sherbrooke, QC, CANADA"
 __date__ = "2023-06-26"
-__version__= "2.0.5"
+__version__= "2.0.6"
 
 import pandas as pd
 import networkx as nx
 import time
 from ete3 import Tree
 import matplotlib.pyplot as plt
 import argparse
```

### Comparing `transcriptorthology-2.0.5/setup.py` & `transcriptorthology-2.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from setuptools import setup, find_packages
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
-VERSION = '2.0.5'
+VERSION = '2.0.6'
 DESCRIPTION = 'A transcript orthologies inferring package'
-long_description = 'Algorithm to infer clusters of isoorthologous transcripts using gene-level homology relationships and a Reciprocal Best Hits approach'
 
 setup(
     name="transcriptorthology",
     version=VERSION,
     description=DESCRIPTION,
-    long_description_content_type="text",
+    long_description_content_type="text/markdown",
     long_description=long_description,
     author="Wend Yam Donald Davy Ouedraogo",
     author_email="wend.yam.donald.davy.ouedraogo@usherbrooke.ca",
     url='https://github.com/UdeS-CoBIUS/TranscriptOrthology',
     license='MIT',
     packages=find_packages(),
     install_requires=["pandas","ete3","networkx","matplotlib","argparse"],
```

### Comparing `transcriptorthology-2.0.5/README.md` & `transcriptorthology-2.0.6/README.md`

 * *Files identical despite different names*

