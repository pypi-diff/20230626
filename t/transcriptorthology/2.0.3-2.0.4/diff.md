# Comparing `tmp/transcriptorthology-2.0.3.tar.gz` & `tmp/transcriptorthology-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transcriptorthology-2.0.3.tar", last modified: Mon Jun 26 05:54:12 2023, max compression
+gzip compressed data, was "dist/transcriptorthology-2.0.4.tar", last modified: Mon Jun 26 06:11:38 2023, max compression
```

## Comparing `transcriptorthology-2.0.3.tar` & `transcriptorthology-2.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/transcriptorthology/
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    23446 2023-06-26 05:53:08.000000 transcriptorthology-2.0.3/transcriptorthology/tsmComputing.py
--rw-------   0 ouew2201 (1811316550) domain^users (1810891265)      123 2023-06-26 04:51:12.000000 transcriptorthology-2.0.3/transcriptorthology/__init__.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2944 2023-06-26 05:53:03.000000 transcriptorthology-2.0.3/transcriptorthology/transcriptOrthology.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    15635 2023-06-26 05:52:56.000000 transcriptorthology-2.0.3/transcriptorthology/Tclustering.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     1072 2023-06-26 05:53:19.000000 transcriptorthology-2.0.3/setup.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2833 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/PKG-INFO
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       38 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/setup.cfg
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/transcriptorthology.egg-info/
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)        1 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/transcriptorthology.egg-info/dependency_links.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      378 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/transcriptorthology.egg-info/SOURCES.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       41 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/transcriptorthology.egg-info/requires.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2833 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/transcriptorthology.egg-info/PKG-INFO
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       20 2023-06-26 05:54:12.000000 transcriptorthology-2.0.3/transcriptorthology.egg-info/top_level.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2180 2023-06-26 05:12:33.000000 transcriptorthology-2.0.3/README.md
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 06:11:38.000000 transcriptorthology-2.0.4/
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 06:11:38.000000 transcriptorthology-2.0.4/transcriptorthology/
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    23446 2023-06-26 06:09:46.000000 transcriptorthology-2.0.4/transcriptorthology/tsmComputing.py
+-rw-------   0 ouew2201 (1811316550) domain^users (1810891265)      123 2023-06-26 04:51:12.000000 transcriptorthology-2.0.4/transcriptorthology/__init__.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2913 2023-06-26 06:09:24.000000 transcriptorthology-2.0.4/transcriptorthology/transcriptOrthology.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    15635 2023-06-26 06:09:04.000000 transcriptorthology-2.0.4/transcriptorthology/Tclustering.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     1096 2023-06-26 06:11:21.000000 transcriptorthology-2.0.4/setup.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      794 2023-06-26 06:11:38.000000 transcriptorthology-2.0.4/PKG-INFO
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       38 2023-06-26 06:11:38.000000 transcriptorthology-2.0.4/setup.cfg
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 06:11:38.000000 transcriptorthology-2.0.4/transcriptorthology.egg-info/
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)        1 2023-06-26 06:11:38.000000 transcriptorthology-2.0.4/transcriptorthology.egg-info/dependency_links.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      378 2023-06-26 06:11:38.000000 transcriptorthology-2.0.4/transcriptorthology.egg-info/SOURCES.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       41 2023-06-26 06:11:38.000000 transcriptorthology-2.0.4/transcriptorthology.egg-info/requires.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      794 2023-06-26 06:11:38.000000 transcriptorthology-2.0.4/transcriptorthology.egg-info/PKG-INFO
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       20 2023-06-26 06:11:38.000000 transcriptorthology-2.0.4/transcriptorthology.egg-info/top_level.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2180 2023-06-26 05:12:33.000000 transcriptorthology-2.0.4/README.md
```

### Comparing `transcriptorthology-2.0.3/transcriptorthology/tsmComputing.py` & `transcriptorthology-2.0.4/transcriptorthology/tsmComputing.py`

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
-__version__= "2.0.3"
+__version__= "2.0.4"
 
 import pandas as pd
 import argparse
 import time
 import numpy as np
 
 def build_arg_parser():
```

### Comparing `transcriptorthology-2.0.3/transcriptorthology/transcriptOrthology.py` & `transcriptorthology-2.0.4/transcriptorthology/transcriptOrthology.py`

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
-__version__= "2.0.3"
+__version__= "2.0.4"
 
 
 import argparse
-from Tclustering.get_orthology_graph import get_orthology_graph
-from tsmComputing.get_matrix import get_matrix
+from Tclustering import get_orthology_graph
+from tsmComputing import get_matrix
 
 
 def build_arg_parser():
     '''Parsing function'''
     parser = argparse.ArgumentParser(description="program parameters")
     parser.add_argument('-talg', '--tralignment', default=None, help='Multiple Sequences Alignment of transcripts in FASTA format')
     parser.add_argument('-gtot', '--genetotranscripts', default=None, help="mappings transcripts to corresponding genes")
```

### Comparing `transcriptorthology-2.0.3/transcriptorthology/Tclustering.py` & `transcriptorthology-2.0.4/transcriptorthology/Tclustering.py`

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
-__version__= "2.0.3"
+__version__= "2.0.4"
 
 import pandas as pd
 import networkx as nx
 import time
 from ete3 import Tree
 import matplotlib.pyplot as plt
 import argparse
```

### Comparing `transcriptorthology-2.0.3/setup.py` & `transcriptorthology-2.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 from setuptools import setup, find_packages
-from pathlib import Path
 
-this_directory = Path(__file__).parent
-
-VERSION = '2.0.3'
+VERSION = '2.0.4'
 DESCRIPTION = 'A transcript orthologies inferring package'
-long_description = (this_directory / "README.md").read_text()
-
+long_description = 'Algorithm to infer clusters of isoorthologous transcripts using gene-level homology relationships and a Reciprocal Best Hits approach'
 setup(
     name="transcriptorthology",
     version=VERSION,
     description=DESCRIPTION,
-    long_description_content_type="text/markdown",
+    long_description_content_type="text/plain",
     long_description=long_description,
     author="Wend Yam Donald Davy Ouedraogo",
     author_email="wend.yam.donald.davy.ouedraogo@usherbrooke.ca",
     url='https://github.com/UdeS-CoBIUS/TranscriptOrthology',
     license='MIT',
     packages=find_packages(),
     install_requires=["pandas","ete3","networkx","matplotlib","argparse"],
```

### Comparing `transcriptorthology-2.0.3/PKG-INFO` & `transcriptorthology-2.0.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: transcriptorthology
-Version: 2.0.3
-Summary: A transcript orthologies inferring package
-Home-page: https://github.com/UdeS-CoBIUS/TranscriptOrthology
-Author: Wend Yam Donald Davy Ouedraogo
-Author-email: wend.yam.donald.davy.ouedraogo@usherbrooke.ca
-License: MIT
-Keywords: clustering,alternative-splicing,orthoogy-inference,isoorthology,algorithm,evolution,computational-biology
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-
 
 # :dna: Inferring clusters of orthologous and paralogous transcripts
 
 ``Algorithm to infer clusters of isoorthologous transcripts using gene-level homology relationships and a Reciprocal Best Hits approach``
 
 ![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
 
@@ -75,9 +59,7 @@
 <br>
 <br>
 Copyright © 2023 CoBIUS LAB
 
 
 
 
-
-
```

