# Comparing `tmp/transcriptorthology-2.0.0.tar.gz` & `tmp/transcriptorthology-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transcriptorthology-2.0.0.tar", last modified: Mon Jun 26 04:17:55 2023, max compression
+gzip compressed data, was "dist/transcriptorthology-2.0.1.tar", last modified: Mon Jun 26 05:12:44 2023, max compression
```

## Comparing `transcriptorthology-2.0.0.tar` & `transcriptorthology-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/transcriptorthology/
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    23446 2023-06-26 04:15:24.000000 transcriptorthology-2.0.0/transcriptorthology/tsmComputing.py
--rw-------   0 ouew2201 (1811316550) domain^users (1810891265)      121 2023-03-03 21:12:23.000000 transcriptorthology-2.0.0/transcriptorthology/__init__.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2911 2023-06-26 04:15:32.000000 transcriptorthology-2.0.0/transcriptorthology/transcriptOrthology.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    15635 2023-06-26 04:15:41.000000 transcriptorthology-2.0.0/transcriptorthology/Tclustering.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     1053 2023-06-26 04:09:28.000000 transcriptorthology-2.0.0/setup.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      761 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/PKG-INFO
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       38 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/setup.cfg
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/transcriptorthology.egg-info/
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)        1 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/transcriptorthology.egg-info/dependency_links.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      368 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/transcriptorthology.egg-info/SOURCES.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       41 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/transcriptorthology.egg-info/requires.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      761 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/transcriptorthology.egg-info/PKG-INFO
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       20 2023-06-26 04:17:55.000000 transcriptorthology-2.0.0/transcriptorthology.egg-info/top_level.txt
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/transcriptorthology/
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    23446 2023-06-26 04:44:35.000000 transcriptorthology-2.0.1/transcriptorthology/tsmComputing.py
+-rw-------   0 ouew2201 (1811316550) domain^users (1810891265)      123 2023-06-26 04:51:12.000000 transcriptorthology-2.0.1/transcriptorthology/__init__.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2913 2023-06-26 04:44:23.000000 transcriptorthology-2.0.1/transcriptorthology/transcriptOrthology.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    15635 2023-06-26 04:44:42.000000 transcriptorthology-2.0.1/transcriptorthology/Tclustering.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     1072 2023-06-26 05:03:50.000000 transcriptorthology-2.0.1/setup.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     3364 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/PKG-INFO
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       38 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/setup.cfg
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/transcriptorthology.egg-info/
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)        1 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/transcriptorthology.egg-info/dependency_links.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      378 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/transcriptorthology.egg-info/SOURCES.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       41 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/transcriptorthology.egg-info/requires.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     3364 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/transcriptorthology.egg-info/PKG-INFO
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       20 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/transcriptorthology.egg-info/top_level.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2180 2023-06-26 05:12:33.000000 transcriptorthology-2.0.1/README.md
```

### Comparing `transcriptorthology-2.0.0/transcriptorthology/tsmComputing.py` & `transcriptorthology-2.0.1/transcriptorthology/tsmComputing.py`

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
-__version__= "2.0.0"
+__version__= "2.0.1"
 
 import pandas as pd
 import argparse
 import time
 import numpy as np
 
 def build_arg_parser():
```

### Comparing `transcriptorthology-2.0.0/transcriptorthology/transcriptOrthology.py` & `transcriptorthology-2.0.1/transcriptorthology/transcriptOrthology.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ======
     https://github.com/UdeS-CoBIUS/TranscriptOrthology
 """
 __authors__ = ("Wend Yam Donald Davy Ouedraogo")
 __contact__ = ("wend.yam.donald.davy.usherbrooke.ca")
 __copyright__ = "CoBIUS lab at Université de Sherbrooke, QC, CANADA"
 __date__ = "2023-06-26"
-__version__= "2.0.0"
+__version__= "2.0.1"
 
 
 import argparse
 from Tclustering import get_orthology_graph
 from tsmComputing import get_matrix
 
 
@@ -26,15 +26,15 @@
     parser.add_argument('-gtot', '--genetotranscripts', default=None, help="mappings transcripts to corresponding genes")
     parser.add_argument('-nhxt', '--nhxgenetree', default=None, help='NHX gene tree')
     parser.add_argument('-lowb', '--lowerbound', default=0.7, help='a lower bound for the selection of transcripts RBHs')
     parser.add_argument('-tsm', '--tsmvalue', default=1, help='an integer(1|2|3|4|5|6) that refers to the transcript similarity measure')
     parser.add_argument('-outf', '--outputfolder', default='.', help='the output folder to store the results')
     return parser
 
-def inferring_transcripts_isoortholoy(transcripts_msa_path, gtot_path, gt_path, tsm_conditions, lower_bound, output_folder):
+def inferring_transcripts_isoorthology(transcripts_msa_path, gtot_path, gt_path, tsm_conditions, lower_bound, output_folder):
     """inferring transcript isoorthologies"""
     try:
         tsm_matrix, df_blocks_transcripts, df_blocks_genes = get_matrix(transcripts_msa_path, gtot_path, tsm_conditions, output_folder)
     except:
         raise('Impossible to retrieve the matrix ! Errors occured ...')
     
     try:
@@ -52,15 +52,15 @@
     gt_path = args.nhxgenetree
     lower_bound = float(args.lowerbound)
     transcripts_msa_path = args.tralignment
     tsm_conditions = args.tsmvalue
     output_folder = args.outputfolder
 
     #compute the main algorithm
-    tsm_matrix, df_blocks_transcripts, df_blocks_genes, clusters, df, df_orthology = inferring_transcripts_isoortholoy(transcripts_msa_path, gtot_path, gt_path, tsm_conditions, lower_bound, output_folder)
+    tsm_matrix, df_blocks_transcripts, df_blocks_genes, clusters, df, df_orthology = inferring_transcripts_isoorthology(transcripts_msa_path, gtot_path, gt_path, tsm_conditions, lower_bound, output_folder)
     
     # finish
     print('++++++++++++++++Finished \n\n Succesful. Data results can be found in {}'.format(output_folder))
```

### Comparing `transcriptorthology-2.0.0/transcriptorthology/Tclustering.py` & `transcriptorthology-2.0.1/transcriptorthology/Tclustering.py`

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
-__version__= "2.0.0"
+__version__= "2.0.1"
 
 import pandas as pd
 import networkx as nx
 import time
 from ete3 import Tree
 import matplotlib.pyplot as plt
 import argparse
```

### Comparing `transcriptorthology-2.0.0/setup.py` & `transcriptorthology-2.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from setuptools import setup, find_packages
+from pathlib import Path
 
-VERSION = '2.0.0'
+this_directory = Path(__file__).parent
+
+VERSION = '2.0.1'
 DESCRIPTION = 'A transcript orthologies inferring package'
-LONG_DESCRIPTION = 'A package that using Gene-level homology relationships to define different types of homology relationships between homologous transcripts'
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="transcriptorthology",
     version=VERSION,
     description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     author="Wend Yam Donald Davy Ouedraogo",
     author_email="wend.yam.donald.davy.ouedraogo@usherbrooke.ca",
     url='https://github.com/UdeS-CoBIUS/TranscriptOrthology',
     license='MIT',
     packages=find_packages(),
     install_requires=["pandas","ete3","networkx","matplotlib","argparse"],
     keywords=['clustering','alternative-splicing','orthoogy-inference','isoorthology','algorithm','evolution','computational-biology'],
```

