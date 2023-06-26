# Comparing `tmp/transcriptorthology-2.0.2.tar.gz` & `tmp/transcriptorthology-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transcriptorthology-2.0.2.tar", last modified: Mon Jun 26 05:23:51 2023, max compression
+gzip compressed data, was "dist/transcriptorthology-2.0.3.tar", last modified: Mon Jun 26 05:54:12 2023, max compression
```

## Comparing `transcriptorthology-2.0.2.tar` & `transcriptorthology-2.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/transcriptorthology/
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    23446 2023-06-26 05:22:08.000000 transcriptorthology-2.0.2/transcriptorthology/tsmComputing.py
--rw-------   0 ouew2201 (1811316550) domain^users (1810891265)      123 2023-06-26 04:51:12.000000 transcriptorthology-2.0.2/transcriptorthology/__init__.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2913 2023-06-26 05:22:02.000000 transcriptorthology-2.0.2/transcriptorthology/transcriptOrthology.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    15635 2023-06-26 05:21:52.000000 transcriptorthology-2.0.2/transcriptorthology/Tclustering.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     1072 2023-06-26 05:21:31.000000 transcriptorthology-2.0.2/setup.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2833 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/PKG-INFO
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       38 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/setup.cfg
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/transcriptorthology.egg-info/
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)        1 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/transcriptorthology.egg-info/dependency_links.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      378 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/transcriptorthology.egg-info/SOURCES.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       41 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/transcriptorthology.egg-info/requires.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2833 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/transcriptorthology.egg-info/PKG-INFO
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       20 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/transcriptorthology.egg-info/top_level.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2180 2023-06-26 05:12:33.000000 transcriptorthology-2.0.2/README.md
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/transcriptorthology/
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    23446 2023-06-26 05:53:08.000000 transcriptorthology-2.0.3/transcriptorthology/tsmComputing.py
+-rw-------   0 ouew2201 (1811316550) domain^users (1810891265)      123 2023-06-26 04:51:12.000000 transcriptorthology-2.0.3/transcriptorthology/__init__.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2944 2023-06-26 05:53:03.000000 transcriptorthology-2.0.3/transcriptorthology/transcriptOrthology.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    15635 2023-06-26 05:52:56.000000 transcriptorthology-2.0.3/transcriptorthology/Tclustering.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     1072 2023-06-26 05:53:19.000000 transcriptorthology-2.0.3/setup.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2833 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/PKG-INFO
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       38 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/setup.cfg
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/transcriptorthology.egg-info/
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)        1 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/transcriptorthology.egg-info/dependency_links.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      378 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/transcriptorthology.egg-info/SOURCES.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       41 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/transcriptorthology.egg-info/requires.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2833 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/transcriptorthology.egg-info/PKG-INFO
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       20 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/transcriptorthology.egg-info/top_level.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2180 2023-06-26 05:12:33.000000 transcriptorthology-2.0.3/README.md
```

### Comparing `transcriptorthology-2.0.2/transcriptorthology/tsmComputing.py` & `transcriptorthology-2.0.3/transcriptorthology/tsmComputing.py`

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
-__version__= "2.0.2"
+__version__= "2.0.3"
 
 import pandas as pd
 import argparse
 import time
 import numpy as np
 
 def build_arg_parser():
```

### Comparing `transcriptorthology-2.0.2/transcriptorthology/transcriptOrthology.py` & `transcriptorthology-2.0.3/transcriptorthology/transcriptOrthology.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 ======
     https://github.com/UdeS-CoBIUS/TranscriptOrthology
 """
 __authors__ = ("Wend Yam Donald Davy Ouedraogo")
 __contact__ = ("wend.yam.donald.davy.usherbrooke.ca")
 __copyright__ = "CoBIUS lab at Université de Sherbrooke, QC, CANADA"
 __date__ = "2023-06-26"
-__version__= "2.0.2"
+__version__= "2.0.3"
 
 
 import argparse
-from Tclustering import get_orthology_graph
-from tsmComputing import get_matrix
+from Tclustering.get_orthology_graph import get_orthology_graph
+from tsmComputing.get_matrix import get_matrix
 
 
 def build_arg_parser():
     '''Parsing function'''
     parser = argparse.ArgumentParser(description="program parameters")
     parser.add_argument('-talg', '--tralignment', default=None, help='Multiple Sequences Alignment of transcripts in FASTA format')
     parser.add_argument('-gtot', '--genetotranscripts', default=None, help="mappings transcripts to corresponding genes")
```

### Comparing `transcriptorthology-2.0.2/transcriptorthology/Tclustering.py` & `transcriptorthology-2.0.3/transcriptorthology/Tclustering.py`

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
-__version__= "2.0.2"
+__version__= "2.0.3"
 
 import pandas as pd
 import networkx as nx
 import time
 from ete3 import Tree
 import matplotlib.pyplot as plt
 import argparse
```

### Comparing `transcriptorthology-2.0.2/setup.py` & `transcriptorthology-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 
-VERSION = '2.0.2'
+VERSION = '2.0.3'
 DESCRIPTION = 'A transcript orthologies inferring package'
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="transcriptorthology",
     version=VERSION,
     description=DESCRIPTION,
```

### Comparing `transcriptorthology-2.0.2/PKG-INFO` & `transcriptorthology-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transcriptorthology
-Version: 2.0.2
+Version: 2.0.3
 Summary: A transcript orthologies inferring package
 Home-page: https://github.com/UdeS-CoBIUS/TranscriptOrthology
 Author: Wend Yam Donald Davy Ouedraogo
 Author-email: wend.yam.donald.davy.ouedraogo@usherbrooke.ca
 License: MIT
 Keywords: clustering,alternative-splicing,orthoogy-inference,isoorthology,algorithm,evolution,computational-biology
 Platform: UNKNOWN
```

### Comparing `transcriptorthology-2.0.2/transcriptorthology.egg-info/PKG-INFO` & `transcriptorthology-2.0.3/transcriptorthology.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transcriptorthology
-Version: 2.0.2
+Version: 2.0.3
 Summary: A transcript orthologies inferring package
 Home-page: https://github.com/UdeS-CoBIUS/TranscriptOrthology
 Author: Wend Yam Donald Davy Ouedraogo
 Author-email: wend.yam.donald.davy.ouedraogo@usherbrooke.ca
 License: MIT
 Keywords: clustering,alternative-splicing,orthoogy-inference,isoorthology,algorithm,evolution,computational-biology
 Platform: UNKNOWN
```

### Comparing `transcriptorthology-2.0.2/README.md` & `transcriptorthology-2.0.3/README.md`

 * *Files identical despite different names*

