# Comparing `tmp/transcriptorthology-2.0.1.tar.gz` & `tmp/transcriptorthology-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transcriptorthology-2.0.1.tar", last modified: Mon Jun 26 05:12:44 2023, max compression
+gzip compressed data, was "dist/transcriptorthology-2.0.2.tar", last modified: Mon Jun 26 05:23:51 2023, max compression
```

## Comparing `transcriptorthology-2.0.1.tar` & `transcriptorthology-2.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/transcriptorthology/
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    23446 2023-06-26 04:44:35.000000 transcriptorthology-2.0.1/transcriptorthology/tsmComputing.py
--rw-------   0 ouew2201 (1811316550) domain^users (1810891265)      123 2023-06-26 04:51:12.000000 transcriptorthology-2.0.1/transcriptorthology/__init__.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2913 2023-06-26 04:44:23.000000 transcriptorthology-2.0.1/transcriptorthology/transcriptOrthology.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    15635 2023-06-26 04:44:42.000000 transcriptorthology-2.0.1/transcriptorthology/Tclustering.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     1072 2023-06-26 05:03:50.000000 transcriptorthology-2.0.1/setup.py
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     3364 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/PKG-INFO
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       38 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/setup.cfg
-drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/transcriptorthology.egg-info/
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)        1 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/transcriptorthology.egg-info/dependency_links.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      378 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/transcriptorthology.egg-info/SOURCES.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       41 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/transcriptorthology.egg-info/requires.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     3364 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/transcriptorthology.egg-info/PKG-INFO
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       20 2023-06-26 05:12:44.000000 transcriptorthology-2.0.1/transcriptorthology.egg-info/top_level.txt
--rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2180 2023-06-26 05:12:33.000000 transcriptorthology-2.0.1/README.md
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/transcriptorthology/
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    23446 2023-06-26 05:22:08.000000 transcriptorthology-2.0.2/transcriptorthology/tsmComputing.py
+-rw-------   0 ouew2201 (1811316550) domain^users (1810891265)      123 2023-06-26 04:51:12.000000 transcriptorthology-2.0.2/transcriptorthology/__init__.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2913 2023-06-26 05:22:02.000000 transcriptorthology-2.0.2/transcriptorthology/transcriptOrthology.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)    15635 2023-06-26 05:21:52.000000 transcriptorthology-2.0.2/transcriptorthology/Tclustering.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     1072 2023-06-26 05:21:31.000000 transcriptorthology-2.0.2/setup.py
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2833 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/PKG-INFO
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       38 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/setup.cfg
+drwxr-xr-x   0 ouew2201 (1811316550) domain^users (1810891265)        0 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/transcriptorthology.egg-info/
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)        1 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/transcriptorthology.egg-info/dependency_links.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)      378 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/transcriptorthology.egg-info/SOURCES.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       41 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/transcriptorthology.egg-info/requires.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2833 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/transcriptorthology.egg-info/PKG-INFO
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)       20 2023-06-26 05:23:51.000000 transcriptorthology-2.0.2/transcriptorthology.egg-info/top_level.txt
+-rw-r--r--   0 ouew2201 (1811316550) domain^users (1810891265)     2180 2023-06-26 05:12:33.000000 transcriptorthology-2.0.2/README.md
```

### Comparing `transcriptorthology-2.0.1/transcriptorthology/tsmComputing.py` & `transcriptorthology-2.0.2/transcriptorthology/tsmComputing.py`

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
-__version__= "2.0.1"
+__version__= "2.0.2"
 
 import pandas as pd
 import argparse
 import time
 import numpy as np
 
 def build_arg_parser():
```

### Comparing `transcriptorthology-2.0.1/transcriptorthology/transcriptOrthology.py` & `transcriptorthology-2.0.2/transcriptorthology/transcriptOrthology.py`

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
-__version__= "2.0.1"
+__version__= "2.0.2"
 
 
 import argparse
 from Tclustering import get_orthology_graph
 from tsmComputing import get_matrix
```

### Comparing `transcriptorthology-2.0.1/transcriptorthology/Tclustering.py` & `transcriptorthology-2.0.2/transcriptorthology/Tclustering.py`

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
-__version__= "2.0.1"
+__version__= "2.0.2"
 
 import pandas as pd
 import networkx as nx
 import time
 from ete3 import Tree
 import matplotlib.pyplot as plt
 import argparse
```

### Comparing `transcriptorthology-2.0.1/setup.py` & `transcriptorthology-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 
-VERSION = '2.0.1'
+VERSION = '2.0.2'
 DESCRIPTION = 'A transcript orthologies inferring package'
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="transcriptorthology",
     version=VERSION,
     description=DESCRIPTION,
-    long_description=long_description,
     long_description_content_type="text/markdown",
+    long_description=long_description,
     author="Wend Yam Donald Davy Ouedraogo",
     author_email="wend.yam.donald.davy.ouedraogo@usherbrooke.ca",
     url='https://github.com/UdeS-CoBIUS/TranscriptOrthology',
     license='MIT',
     packages=find_packages(),
     install_requires=["pandas","ete3","networkx","matplotlib","argparse"],
     keywords=['clustering','alternative-splicing','orthoogy-inference','isoorthology','algorithm','evolution','computational-biology'],
```

### Comparing `transcriptorthology-2.0.1/PKG-INFO` & `transcriptorthology-2.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,83 @@
 Metadata-Version: 2.1
 Name: transcriptorthology
-Version: 2.0.1
+Version: 2.0.2
 Summary: A transcript orthologies inferring package
 Home-page: https://github.com/UdeS-CoBIUS/TranscriptOrthology
 Author: Wend Yam Donald Davy Ouedraogo
 Author-email: wend.yam.donald.davy.ouedraogo@usherbrooke.ca
 License: MIT
-Description: 
-        # :dna: Inferring clusters of orthologous and paralogous transcripts
-        
-        ``Algorithm to infer clusters of isoorthologous transcripts using gene-level homology relationships and a Reciprocal Best Hits approach``
-        
-        ![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
-        
-        <!-- ABOUT THE PROJECT -->
-        <h2 id="about-the-project"> :pencil: About The Project</h2>
-        
-        
-        <!-- OVERVIEW -->
-        <h3 id="overview"> :cloud: Overview</h3>
-        
-        `A graph-based method to infer isoorthology & recent paralogy relations in a set of homologous transcripts:dna:`
-        
-        ---
-        
-        
-        <!-- Requirements -->
-        <h3 id="requirements"> :hammer_and_pick: Requirements</h3>
-        
-        *   __`python3 (at leat python 3.6)`__
-        *   __`NetworkX`__
-        *   __`Pandas`__
-        *   __`Numpy`__
-        *   __`ETE toolkit`__
-        
-        
-        ![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
-        
-        <!-- Package -->
-        <h3 id="package"> :package: About the package</h3>
-        
-        ``install the package``
-        <pre><code>pip3 install transcriptorthology</code></pre>
-        
-        ``import package and use the main function``
-        <pre><code>from transcriptorthology.transcriptOrthology import inferring_transcripts_isoorthology
-        
-        if __name__ == '__main__':
-          gtot_path = './execution/mapping_gene_to_transcripts/ENSGT00390000000080.fasta'
-          gt_path = './execution/NHX_trees/ENSGT00390000000080.nwk'
-          lower_bound = 0.7
-          transcripts_msa_path = './execution/transcripts_alignments/ENSGT00390000000080.alg'
-          tsm_conditions = 2
-          output_folder = './execution/output_folder'
-          
-          <span style="color:red;">inferring_transcripts_isoorthology</span>(<span style="color:red;">transcripts_msa_path</span>, <span style="color:green;">gtot_path</span>, <span style="color:purple;">gt_path</span>,<span style="color:orange;">tsm_conditions</span>,<span style="color:yellow;">lower_bound</span>,<span style="color:gray;">output_folder</span>)</code></pre>
-        
-        
-        ![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
-        
-        ---
-        <br>
-        <br>
-        <br>
-        <br>
-        <br>
-        <br>
-        Copyright © 2023 CoBIUS LAB
-        
-        
-        
-        
-        
 Keywords: clustering,alternative-splicing,orthoogy-inference,isoorthology,algorithm,evolution,computational-biology
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+
+
+# :dna: Inferring clusters of orthologous and paralogous transcripts
+
+``Algorithm to infer clusters of isoorthologous transcripts using gene-level homology relationships and a Reciprocal Best Hits approach``
+
+![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
+
+<!-- ABOUT THE PROJECT -->
+<h2 id="about-the-project"> :pencil: About The Project</h2>
+
+
+<!-- OVERVIEW -->
+<h3 id="overview"> :cloud: Overview</h3>
+
+`A graph-based method to infer isoorthology & recent paralogy relations in a set of homologous transcripts:dna:`
+
+---
+
+
+<!-- Requirements -->
+<h3 id="requirements"> :hammer_and_pick: Requirements</h3>
+
+*   __`python3 (at leat python 3.6)`__
+*   __`NetworkX`__
+*   __`Pandas`__
+*   __`Numpy`__
+*   __`ETE toolkit`__
+
+
+![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
+
+<!-- Package -->
+<h3 id="package"> :package: About the package</h3>
+
+``install the package``
+<pre><code>pip3 install transcriptorthology</code></pre>
+
+``import package and use the main function``
+<pre><code>from transcriptorthology.transcriptOrthology import inferring_transcripts_isoorthology
+
+if __name__ == '__main__':
+  gtot_path = './execution/mapping_gene_to_transcripts/ENSGT00390000000080.fasta'
+  gt_path = './execution/NHX_trees/ENSGT00390000000080.nwk'
+  lower_bound = 0.7
+  transcripts_msa_path = './execution/transcripts_alignments/ENSGT00390000000080.alg'
+  tsm_conditions = 2
+  output_folder = './execution/output_folder'
+  
+  <span style="color:red;">inferring_transcripts_isoorthology</span>(<span style="color:red;">transcripts_msa_path</span>, <span style="color:green;">gtot_path</span>, <span style="color:purple;">gt_path</span>,<span style="color:orange;">tsm_conditions</span>,<span style="color:yellow;">lower_bound</span>,<span style="color:gray;">output_folder</span>)</code></pre>
+
+
+![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
+
+---
+<br>
+<br>
+<br>
+<br>
+<br>
+<br>
+Copyright © 2023 CoBIUS LAB
+
+
+
+
+
+
```

### Comparing `transcriptorthology-2.0.1/transcriptorthology.egg-info/PKG-INFO` & `transcriptorthology-2.0.2/transcriptorthology.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,83 @@
 Metadata-Version: 2.1
 Name: transcriptorthology
-Version: 2.0.1
+Version: 2.0.2
 Summary: A transcript orthologies inferring package
 Home-page: https://github.com/UdeS-CoBIUS/TranscriptOrthology
 Author: Wend Yam Donald Davy Ouedraogo
 Author-email: wend.yam.donald.davy.ouedraogo@usherbrooke.ca
 License: MIT
-Description: 
-        # :dna: Inferring clusters of orthologous and paralogous transcripts
-        
-        ``Algorithm to infer clusters of isoorthologous transcripts using gene-level homology relationships and a Reciprocal Best Hits approach``
-        
-        ![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
-        
-        <!-- ABOUT THE PROJECT -->
-        <h2 id="about-the-project"> :pencil: About The Project</h2>
-        
-        
-        <!-- OVERVIEW -->
-        <h3 id="overview"> :cloud: Overview</h3>
-        
-        `A graph-based method to infer isoorthology & recent paralogy relations in a set of homologous transcripts:dna:`
-        
-        ---
-        
-        
-        <!-- Requirements -->
-        <h3 id="requirements"> :hammer_and_pick: Requirements</h3>
-        
-        *   __`python3 (at leat python 3.6)`__
-        *   __`NetworkX`__
-        *   __`Pandas`__
-        *   __`Numpy`__
-        *   __`ETE toolkit`__
-        
-        
-        ![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
-        
-        <!-- Package -->
-        <h3 id="package"> :package: About the package</h3>
-        
-        ``install the package``
-        <pre><code>pip3 install transcriptorthology</code></pre>
-        
-        ``import package and use the main function``
-        <pre><code>from transcriptorthology.transcriptOrthology import inferring_transcripts_isoorthology
-        
-        if __name__ == '__main__':
-          gtot_path = './execution/mapping_gene_to_transcripts/ENSGT00390000000080.fasta'
-          gt_path = './execution/NHX_trees/ENSGT00390000000080.nwk'
-          lower_bound = 0.7
-          transcripts_msa_path = './execution/transcripts_alignments/ENSGT00390000000080.alg'
-          tsm_conditions = 2
-          output_folder = './execution/output_folder'
-          
-          <span style="color:red;">inferring_transcripts_isoorthology</span>(<span style="color:red;">transcripts_msa_path</span>, <span style="color:green;">gtot_path</span>, <span style="color:purple;">gt_path</span>,<span style="color:orange;">tsm_conditions</span>,<span style="color:yellow;">lower_bound</span>,<span style="color:gray;">output_folder</span>)</code></pre>
-        
-        
-        ![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
-        
-        ---
-        <br>
-        <br>
-        <br>
-        <br>
-        <br>
-        <br>
-        Copyright © 2023 CoBIUS LAB
-        
-        
-        
-        
-        
 Keywords: clustering,alternative-splicing,orthoogy-inference,isoorthology,algorithm,evolution,computational-biology
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+
+
+# :dna: Inferring clusters of orthologous and paralogous transcripts
+
+``Algorithm to infer clusters of isoorthologous transcripts using gene-level homology relationships and a Reciprocal Best Hits approach``
+
+![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
+
+<!-- ABOUT THE PROJECT -->
+<h2 id="about-the-project"> :pencil: About The Project</h2>
+
+
+<!-- OVERVIEW -->
+<h3 id="overview"> :cloud: Overview</h3>
+
+`A graph-based method to infer isoorthology & recent paralogy relations in a set of homologous transcripts:dna:`
+
+---
+
+
+<!-- Requirements -->
+<h3 id="requirements"> :hammer_and_pick: Requirements</h3>
+
+*   __`python3 (at leat python 3.6)`__
+*   __`NetworkX`__
+*   __`Pandas`__
+*   __`Numpy`__
+*   __`ETE toolkit`__
+
+
+![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
+
+<!-- Package -->
+<h3 id="package"> :package: About the package</h3>
+
+``install the package``
+<pre><code>pip3 install transcriptorthology</code></pre>
+
+``import package and use the main function``
+<pre><code>from transcriptorthology.transcriptOrthology import inferring_transcripts_isoorthology
+
+if __name__ == '__main__':
+  gtot_path = './execution/mapping_gene_to_transcripts/ENSGT00390000000080.fasta'
+  gt_path = './execution/NHX_trees/ENSGT00390000000080.nwk'
+  lower_bound = 0.7
+  transcripts_msa_path = './execution/transcripts_alignments/ENSGT00390000000080.alg'
+  tsm_conditions = 2
+  output_folder = './execution/output_folder'
+  
+  <span style="color:red;">inferring_transcripts_isoorthology</span>(<span style="color:red;">transcripts_msa_path</span>, <span style="color:green;">gtot_path</span>, <span style="color:purple;">gt_path</span>,<span style="color:orange;">tsm_conditions</span>,<span style="color:yellow;">lower_bound</span>,<span style="color:gray;">output_folder</span>)</code></pre>
+
+
+![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
+
+---
+<br>
+<br>
+<br>
+<br>
+<br>
+<br>
+Copyright © 2023 CoBIUS LAB
+
+
+
+
+
+
```

### Comparing `transcriptorthology-2.0.1/README.md` & `transcriptorthology-2.0.2/README.md`

 * *Files identical despite different names*

