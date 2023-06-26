# Comparing `tmp/gistdawater-0.0.2.tar.gz` & `tmp/gistdawater-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gistdawater-0.0.2.tar", last modified: Mon Jun 26 04:22:24 2023, max compression
+gzip compressed data, was "gistdawater-0.0.3.tar", last modified: Mon Jun 26 04:27:57 2023, max compression
```

## Comparing `gistdawater-0.0.2.tar` & `gistdawater-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 04:22:24.739784 gistdawater-0.0.2/
--rw-rw-rw-   0        0        0     1068 2022-07-25 06:10:12.000000 gistdawater-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1089 2022-07-25 06:10:12.000000 gistdawater-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       38 2023-04-27 03:39:29.000000 gistdawater-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2210 2023-06-26 04:22:24.740779 gistdawater-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1540 2023-06-22 07:56:15.000000 gistdawater-0.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-26 04:22:24.311435 gistdawater-0.0.2/gistdawater/
--rw-rw-rw-   0        0        0      180 2023-06-26 04:21:27.000000 gistdawater-0.0.2/gistdawater/__init__.py
--rw-rw-rw-   0        0        0    20811 2023-06-26 03:28:40.000000 gistdawater-0.0.2/gistdawater/mainfile.py
-drwxrwxrwx   0        0        0        0 2023-06-26 04:22:24.738781 gistdawater-0.0.2/gistdawater.egg-info/
--rw-rw-rw-   0        0        0     2210 2023-06-26 04:22:23.000000 gistdawater-0.0.2/gistdawater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-26 04:22:24.000000 gistdawater-0.0.2/gistdawater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 04:22:23.000000 gistdawater-0.0.2/gistdawater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-26 04:22:23.000000 gistdawater-0.0.2/gistdawater.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-26 04:22:23.000000 gistdawater-0.0.2/gistdawater.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-26 04:22:24.742782 gistdawater-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1497 2023-06-26 04:21:49.000000 gistdawater-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 04:27:57.521493 gistdawater-0.0.3/
+-rw-rw-rw-   0        0        0     1068 2022-07-25 06:10:12.000000 gistdawater-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1089 2022-07-25 06:10:12.000000 gistdawater-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       38 2023-04-27 03:39:29.000000 gistdawater-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2081 2023-06-26 04:27:57.521493 gistdawater-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1540 2023-06-22 07:56:15.000000 gistdawater-0.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-26 04:27:57.064618 gistdawater-0.0.3/gistdawater/
+-rw-rw-rw-   0        0        0      180 2023-06-26 04:26:11.000000 gistdawater-0.0.3/gistdawater/__init__.py
+-rw-rw-rw-   0        0        0    20826 2023-06-26 04:25:02.000000 gistdawater-0.0.3/gistdawater/mainfile.py
+drwxrwxrwx   0        0        0        0 2023-06-26 04:27:57.519490 gistdawater-0.0.3/gistdawater.egg-info/
+-rw-rw-rw-   0        0        0     2081 2023-06-26 04:27:56.000000 gistdawater-0.0.3/gistdawater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-26 04:27:56.000000 gistdawater-0.0.3/gistdawater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 04:27:56.000000 gistdawater-0.0.3/gistdawater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-26 04:27:56.000000 gistdawater-0.0.3/gistdawater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-26 04:27:56.000000 gistdawater-0.0.3/gistdawater.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-26 04:27:57.523488 gistdawater-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1319 2023-06-26 04:26:16.000000 gistdawater-0.0.3/setup.py
```

### Comparing `gistdawater-0.0.2/LICENSE` & `gistdawater-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gistdawater-0.0.2/LICENSE.txt` & `gistdawater-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gistdawater-0.0.2/PKG-INFO` & `gistdawater-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: gistdawater
-Version: 0.0.2
+Version: 0.0.3
 Summary: Waterdetection for landsat8
-Home-page: https://github.com/Tun555/lazyearth
-Download-URL: https://github.com/Tun555/lazyearth/archive/refs/tags/v0.0.15.zip
 Author: Gistda
 Author-email: gistdathailand@gmail.com
 License: MIT
 Keywords: geo,oepn data cube,earth
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `gistdawater-0.0.2/README.rst` & `gistdawater-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `gistdawater-0.0.2/gistdawater/mainfile.py` & `gistdawater-0.0.3/gistdawater/mainfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from sklearn.model_selection import train_test_split
 from sklearn.cluster import AgglomerativeClustering
 from sklearn.metrics import calinski_harabasz_score
 from sklearn.naive_bayes import GaussianNB
 from sklearn import cluster
 import numpy as np
 from matplotlib import colorbar
+import xarray
 
 class water:
         #fix
         required_bands = {'mndi','Green','ndwi','Mir2','mbwi'}
         required_indices = {'ndwi','mbwi','mndwi'}
         bands_keys = ['mndwi','ndwi','Mir2']
         invalid_mask = None
```

### Comparing `gistdawater-0.0.2/gistdawater.egg-info/PKG-INFO` & `gistdawater-0.0.3/gistdawater.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: gistdawater
-Version: 0.0.2
+Version: 0.0.3
 Summary: Waterdetection for landsat8
-Home-page: https://github.com/Tun555/lazyearth
-Download-URL: https://github.com/Tun555/lazyearth/archive/refs/tags/v0.0.15.zip
 Author: Gistda
 Author-email: gistdathailand@gmail.com
 License: MIT
 Keywords: geo,oepn data cube,earth
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `gistdawater-0.0.2/setup.py` & `gistdawater-0.0.3/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,22 +8,20 @@
 DESCRIPTION = '\n\n'.join(LOAD_TEXT(_) for _ in [
     'README.rst'
 ])
 
 setup(
   name = 'gistdawater',                # Name project the same with folder
   packages = ['gistdawater'],          # Name project the same with folder
-  version = '0.0.2',                   # version
+  version = '0.0.3',                   # version
   license='MIT', 
   description = 'Waterdetection for landsat8',    #Show on PyPi
   long_description=DESCRIPTION,
   author = 'Gistda',            #          
-  author_email = 'gistdathailand@gmail.com',      #
-  url = 'https://github.com/Tun555/lazyearth',  #
-  download_url = 'https://github.com/Tun555/lazyearth/archive/refs/tags/v0.0.15.zip',                                      #  
+  author_email = 'gistdathailand@gmail.com',     #  
   keywords = ['geo','oepn data cube','earth'],      # When someone search
   # Dont add any library bz It's gonna error waiting
   include_package_data=True,         # Create another file (models)
   install_requires=[                 # Package that use
         'numpy',
         'matplotlib'
     ],
```

