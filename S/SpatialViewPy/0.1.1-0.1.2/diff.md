# Comparing `tmp/SpatialViewPy-0.1.1.tar.gz` & `tmp/SpatialViewPy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpatialViewPy-0.1.1.tar", last modified: Thu Jun  8 08:07:57 2023, max compression
+gzip compressed data, was "SpatialViewPy-0.1.2.tar", last modified: Mon Jun 26 14:50:23 2023, max compression
```

## Comparing `SpatialViewPy-0.1.1.tar` & `SpatialViewPy-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-08 08:07:57.700486 SpatialViewPy-0.1.1/
--rw-r--r--   0 cmohanty2   (503) staff       (20)     1073 2023-06-07 20:55:25.000000 SpatialViewPy-0.1.1/LICENSE.txt
--rw-r--r--   0 cmohanty2   (503) staff       (20)       36 2023-06-08 03:39:33.000000 SpatialViewPy-0.1.1/MANIFEST.in
--rw-r--r--   0 cmohanty2   (503) staff       (20)     1014 2023-06-08 08:07:57.700291 SpatialViewPy-0.1.1/PKG-INFO
--rw-r--r--   0 cmohanty2   (503) staff       (20)      666 2023-06-08 06:56:19.000000 SpatialViewPy-0.1.1/README.md
-drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-08 08:07:57.698095 SpatialViewPy-0.1.1/notebooks/
--rw-r--r--   0 cmohanty2   (503) staff       (20)   420498 2023-06-08 08:03:00.000000 SpatialViewPy-0.1.1/notebooks/tutorial.ipynb
--rw-r--r--   0 cmohanty2   (503) staff       (20)       38 2023-06-08 08:07:57.700533 SpatialViewPy-0.1.1/setup.cfg
--rw-r--r--   0 cmohanty2   (503) staff       (20)     1005 2023-06-08 08:07:31.000000 SpatialViewPy-0.1.1/setup.py
-drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-08 08:07:57.696876 SpatialViewPy-0.1.1/src/
-drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-08 08:07:57.699242 SpatialViewPy-0.1.1/src/SpatialViewPy.egg-info/
--rw-r--r--   0 cmohanty2   (503) staff       (20)     1014 2023-06-08 08:07:57.000000 SpatialViewPy-0.1.1/src/SpatialViewPy.egg-info/PKG-INFO
--rw-r--r--   0 cmohanty2   (503) staff       (20)      365 2023-06-08 08:07:57.000000 SpatialViewPy-0.1.1/src/SpatialViewPy.egg-info/SOURCES.txt
--rw-r--r--   0 cmohanty2   (503) staff       (20)        1 2023-06-08 08:07:57.000000 SpatialViewPy-0.1.1/src/SpatialViewPy.egg-info/dependency_links.txt
--rw-r--r--   0 cmohanty2   (503) staff       (20)      126 2023-06-08 08:07:57.000000 SpatialViewPy-0.1.1/src/SpatialViewPy.egg-info/requires.txt
--rw-r--r--   0 cmohanty2   (503) staff       (20)       14 2023-06-08 08:07:57.000000 SpatialViewPy-0.1.1/src/SpatialViewPy.egg-info/top_level.txt
-drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-08 08:07:57.699915 SpatialViewPy-0.1.1/src/spatialviewpy/
--rw-r--r--   0 cmohanty2   (503) staff       (20)       82 2023-06-08 06:37:49.000000 SpatialViewPy-0.1.1/src/spatialviewpy/__init__.py
--rw-r--r--   0 cmohanty2   (503) staff       (20)       21 2023-06-08 06:36:09.000000 SpatialViewPy-0.1.1/src/spatialviewpy/__version.py
--rw-r--r--   0 cmohanty2   (503) staff       (20)    16484 2023-06-08 08:04:35.000000 SpatialViewPy-0.1.1/src/spatialviewpy/prepare_viz.py
+drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-26 14:50:23.275130 SpatialViewPy-0.1.2/
+-rw-r--r--   0 cmohanty2   (503) staff       (20)     1073 2023-06-07 20:55:25.000000 SpatialViewPy-0.1.2/LICENSE.txt
+-rw-r--r--   0 cmohanty2   (503) staff       (20)       36 2023-06-08 03:39:33.000000 SpatialViewPy-0.1.2/MANIFEST.in
+-rw-r--r--   0 cmohanty2   (503) staff       (20)     1014 2023-06-26 14:50:23.274951 SpatialViewPy-0.1.2/PKG-INFO
+-rw-r--r--   0 cmohanty2   (503) staff       (20)      666 2023-06-08 06:56:19.000000 SpatialViewPy-0.1.2/README.md
+drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-26 14:50:23.272983 SpatialViewPy-0.1.2/notebooks/
+-rw-r--r--   0 cmohanty2   (503) staff       (20)   421515 2023-06-26 14:29:32.000000 SpatialViewPy-0.1.2/notebooks/tutorial.ipynb
+-rw-r--r--   0 cmohanty2   (503) staff       (20)       38 2023-06-26 14:50:23.275176 SpatialViewPy-0.1.2/setup.cfg
+-rw-r--r--   0 cmohanty2   (503) staff       (20)     1005 2023-06-26 14:40:39.000000 SpatialViewPy-0.1.2/setup.py
+drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-26 14:50:23.272252 SpatialViewPy-0.1.2/src/
+drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-26 14:50:23.274028 SpatialViewPy-0.1.2/src/SpatialViewPy.egg-info/
+-rw-r--r--   0 cmohanty2   (503) staff       (20)     1014 2023-06-26 14:50:23.000000 SpatialViewPy-0.1.2/src/SpatialViewPy.egg-info/PKG-INFO
+-rw-r--r--   0 cmohanty2   (503) staff       (20)      365 2023-06-26 14:50:23.000000 SpatialViewPy-0.1.2/src/SpatialViewPy.egg-info/SOURCES.txt
+-rw-r--r--   0 cmohanty2   (503) staff       (20)        1 2023-06-26 14:50:23.000000 SpatialViewPy-0.1.2/src/SpatialViewPy.egg-info/dependency_links.txt
+-rw-r--r--   0 cmohanty2   (503) staff       (20)      126 2023-06-26 14:50:23.000000 SpatialViewPy-0.1.2/src/SpatialViewPy.egg-info/requires.txt
+-rw-r--r--   0 cmohanty2   (503) staff       (20)       14 2023-06-26 14:50:23.000000 SpatialViewPy-0.1.2/src/SpatialViewPy.egg-info/top_level.txt
+drwxr-xr-x   0 cmohanty2   (503) staff       (20)        0 2023-06-26 14:50:23.274690 SpatialViewPy-0.1.2/src/spatialviewpy/
+-rw-r--r--   0 cmohanty2   (503) staff       (20)       82 2023-06-08 06:37:49.000000 SpatialViewPy-0.1.2/src/spatialviewpy/__init__.py
+-rw-r--r--   0 cmohanty2   (503) staff       (20)       21 2023-06-26 14:40:48.000000 SpatialViewPy-0.1.2/src/spatialviewpy/__version.py
+-rw-r--r--   0 cmohanty2   (503) staff       (20)    16521 2023-06-26 14:01:05.000000 SpatialViewPy-0.1.2/src/spatialviewpy/prepare_viz.py
```

### Comparing `SpatialViewPy-0.1.1/LICENSE.txt` & `SpatialViewPy-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SpatialViewPy-0.1.1/PKG-INFO` & `SpatialViewPy-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpatialViewPy
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/kendziorski-lab/SpatialViewPy
 Author: Chitrasen Mohanty
 Author-email: mohantychitraen@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `SpatialViewPy-0.1.1/README.md` & `SpatialViewPy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `SpatialViewPy-0.1.1/notebooks/tutorial.ipynb` & `SpatialViewPy-0.1.2/notebooks/tutorial.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9893194444444444%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(13, '\\n'), (14, 'from scipy.io import mmwrite\\n'), (15, "*

 * *            "'from zipfile import ZipFile\\n'), (16, 'import requests\\n'), (17, 'import os\\n'), "*

 * *            "(18, 'import shutil\\n'), (19, 'import json\\n'), (20, 'import gzip\\n')]}}, 4: "*

 * *            "{'source': ['In this tutorial, we are using Spatial Transcriptomics (ST) data "*

 * *            'published in (Barkley *et al.*, 2022). This data contains multiple ST samples from '*

 * *            'different canc […]*

```diff
@@ -50,43 +50,35 @@
                 "import scanorama\n",
                 "\n",
                 "from spatialviewpy import prepare10x_from_scanpy\n",
                 "\n",
                 "from os import listdir, path\n",
                 "from collections import OrderedDict\n",
                 "\n",
+                "from scipy.io import mmwrite\n",
+                "from zipfile import ZipFile\n",
+                "import requests\n",
+                "import os\n",
+                "import shutil\n",
+                "import json\n",
+                "import gzip\n",
+                "\n",
                 "import warnings\n",
                 "warnings.filterwarnings('ignore')"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 4,
-            "id": "43e47497",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# import numpy as np\n",
-                "# from scipy.io import mmwrite\n",
-                "# from zipfile import ZipFile\n",
-                "# import seaborn as sns\n",
-                "# import requests\n",
-                "# import os\n",
-                "# import shutil\n",
-                "# import json\n",
-                "# import gzip"
-            ]
-        },
-        {
             "attachments": {},
             "cell_type": "markdown",
             "id": "f5fcfffc",
             "metadata": {},
             "source": [
-                "In this tutorial we are using Spatial Transcriptomics (ST) data published in (Barkley et al. 2022). This data contains multiple samples from different cancer types, such as breast, gastrointestinal, liver, ovary, pancreas, endometrium, and others. This data is helpful to understand the heterogeneity in tumor micro environment (TME) among different cancer types. For this demonstration, we will be using the ten samples (three breast, two gastrointestinal, one liver, two ovarian, one pancreas, and one endometrium) generated using 10x SpaceRanger. We will use Scanpy (Wolf *et al*., 2018) for data pre-processing and Scanorama (Hie *et al*., 2019) for integrating the samples. With the integrated data, we will do clustering followed by differential expression (DE) analysis to identify the marker genes of the clusters. Finally, we will export the analyzed data to SpatialView (Mohanty et al., 2023) for interactive visualization. Note that analysis steps are for demonstration purpose only."
+                "In this tutorial, we are using Spatial Transcriptomics (ST) data published in (Barkley *et al.*, 2022). This data contains multiple ST samples from different cancer types, such as breast, gastrointestinal, liver, ovary, pancreas, endometrium, and others. The data may be helpful to understand the heterogeneity in tumor micro environment (TME) among different cancer types. For this demonstration, we will be using ten samples (three breast, two gastrointestinal, one liver, two ovarian, one pancreas, and one endometrium) generated using 10x SpaceRanger. We will use Scanpy (Wolf *et al*., 2018) for data pre-processing and Scanorama (Hie *et al*., 2019) for integrating the samples. With the integrated data, we will do clustering followed by differential expression (DE) analysis to identify the marker genes of the clusters. Finally, we will export the analyzed data to SpatialView (Mohanty et al., 2023) for interactive visualization. Note that analysis steps are for demonstration purpose only.\n",
+                "\n",
+                "[Check the running demo application](https://www.biostat.wisc.edu/~kendzior/spatialviewdemo/)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "a1b29046",
             "metadata": {},
@@ -501,16 +493,30 @@
                 "\n",
                 "prepare10x_from_scanpy(adata_spatial, data_paths = sample_paths,\n",
                 "                       export_path = \"TME\",\n",
                 "                       cluster_genes = de_genes,\n",
                 "                       layer = 'normalized_counts',\n",
                 "                       download_repo = True,\n",
                 "                       launch_app = True,\n",
+                "                       port = 8878,\n",
                 "                       verbose= True)"
             ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "6bb5d6b5",
+            "metadata": {},
+            "source": [
+                "## Citations\n",
+                "\n",
+                "1. Barkley, Dalia, Reuben Moncada, Maayan Pour, Deborah A. Liberman, Ian Dryg, Gregor Werba, Wei Wang, et al. 2022. \u201cCancer Cell States Recur Across Tumor Types and Form Specific Interactions with the Tumor Microenvironment.\u201d Nature Genetics 54 (8): 1192\u20131201. https://doi.org/10.1038/s41588-022-01141-9.\n",
+                "2. Hao, Yuhan, Stephanie Hao, Erica Andersen-Nissen, William M. Mauck, Shiwei Zheng, Andrew Butler, Maddie J. Lee, et al. 2021. \u201cIntegrated Analysis of Multimodal Single-Cell Data.\u201d Cell 184 (13): 3573\u20133587.e29. https://doi.org/10.1016/j.cell.2021.04.048.\n",
+                "3. Mohanty, Chitrasen, Aman Prasad, Lingxin Cheng, Lisa M. Arkin, Bridget E. Shields, Beth Drolet, and Christina Kendziorski. 2023. \u201cSpatialView: An Interactive Web Application for Visualization of Multiple Samples in Spatial Transcriptomics Experiments.\u201d http://dx.doi.org/10.1101/2023.06.13.544836."
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `SpatialViewPy-0.1.1/setup.py` & `SpatialViewPy-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='SpatialViewPy',
-      version='0.1.1',
+      version='0.1.2',
       descriptiopn = 'Visualizing multi-sample spatial transcriptimic data using SpatialView',
       py_module='spatialviewpy/prepare_viz',
       package_dir = {'':'src'},
       classifiers=[
           "Programming Language :: Python :: 3.6",
           "Operating System :: OS Independent",
       ],
```

### Comparing `SpatialViewPy-0.1.1/src/SpatialViewPy.egg-info/PKG-INFO` & `SpatialViewPy-0.1.2/src/SpatialViewPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpatialViewPy
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/kendziorski-lab/SpatialViewPy
 Author: Chitrasen Mohanty
 Author-email: mohantychitraen@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `SpatialViewPy-0.1.1/src/spatialviewpy/prepare_viz.py` & `SpatialViewPy-0.1.2/src/spatialviewpy/prepare_viz.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,15 +304,15 @@
                                         'color' : clust_colors,
                                         'name' : cluster_names, 
                                         'genes' : cluster_genes})
         clusterInfo_df.to_csv(path.join(export_path_sample, 'cluster_info.csv'),
                               index = False)
             
     if download_repo and launch_app:
-        start_httpserver(path, port = port, verbose = False)
+        start_httpserver(path.join(orign_export_path,project_name), port = port, verbose = False)
         
 
 def start_httpserver(appPath, port = None, verbose = False, launch = True):
     from subprocess import Popen
     import webbrowser
     
     server = None
```

