# Comparing `tmp/ramanspy-0.0.1.tar.gz` & `tmp/ramanspy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramanspy-0.0.1.tar", last modified: Mon Jun 26 12:05:54 2023, max compression
+gzip compressed data, was "ramanspy-0.0.2.tar", last modified: Mon Jun 26 18:31:16 2023, max compression
```

## Comparing `ramanspy-0.0.1.tar` & `ramanspy-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 12:05:54.951787 ramanspy-0.0.1/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1503 2023-06-26 11:18:57.000000 ramanspy-0.0.1/LICENSE
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       45 2023-06-26 12:05:50.000000 ramanspy-0.0.1/MANIFEST.in
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3983 2023-06-26 12:05:54.951678 ramanspy-0.0.1/PKG-INFO
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1534 2023-06-26 12:05:35.000000 ramanspy-0.0.1/README.md
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1118 2023-06-26 12:01:24.000000 ramanspy-0.0.1/pyproject.toml
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       38 2023-06-26 12:05:54.951829 ramanspy-0.0.1/setup.cfg
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 12:05:54.947521 ramanspy-0.0.1/src/
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 12:05:54.948883 ramanspy-0.0.1/src/ramanspy/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      471 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/__init__.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 12:05:54.950080 ramanspy-0.0.1/src/ramanspy/analysis/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3187 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/analysis/Step.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       85 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/analysis/__init__.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1035 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/analysis/cluster.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2140 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/analysis/decompose.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     6702 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/analysis/unmix.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    11990 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/core.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    18519 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/datasets.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    10006 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/load.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4974 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/metrics.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 12:05:54.950406 ramanspy-0.0.1/src/ramanspy/plot/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      196 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/plot/__init__.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     7777 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/plot/_core.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    25767 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/plot/plot.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 12:05:54.951501 ramanspy-0.0.1/src/ramanspy/preprocessing/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     5493 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/preprocessing/Pipeline.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4862 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/preprocessing/Step.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      262 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/preprocessing/__init__.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    16856 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/preprocessing/baseline.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4168 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/preprocessing/denoise.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2370 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/preprocessing/despike.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2138 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/preprocessing/misc.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3573 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/preprocessing/normalise.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3143 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/preprocessing/protocols.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      473 2023-06-26 11:18:57.000000 ramanspy-0.0.1/src/ramanspy/utils.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 12:05:54.949488 ramanspy-0.0.1/src/ramanspy.egg-info/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3983 2023-06-26 12:05:54.000000 ramanspy-0.0.1/src/ramanspy.egg-info/PKG-INFO
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      950 2023-06-26 12:05:54.000000 ramanspy-0.0.1/src/ramanspy.egg-info/SOURCES.txt
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        1 2023-06-26 12:05:54.000000 ramanspy-0.0.1/src/ramanspy.egg-info/dependency_links.txt
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       90 2023-06-26 12:05:54.000000 ramanspy-0.0.1/src/ramanspy.egg-info/requires.txt
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        9 2023-06-26 12:05:54.000000 ramanspy-0.0.1/src/ramanspy.egg-info/top_level.txt
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 18:31:16.296921 ramanspy-0.0.2/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1503 2023-06-26 11:18:57.000000 ramanspy-0.0.2/LICENSE
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       45 2023-06-26 12:05:50.000000 ramanspy-0.0.2/MANIFEST.in
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3983 2023-06-26 18:31:16.296805 ramanspy-0.0.2/PKG-INFO
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1534 2023-06-26 12:05:35.000000 ramanspy-0.0.2/README.md
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1118 2023-06-26 18:31:05.000000 ramanspy-0.0.2/pyproject.toml
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       38 2023-06-26 18:31:16.296969 ramanspy-0.0.2/setup.cfg
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 18:31:16.291777 ramanspy-0.0.2/src/
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 18:31:16.293201 ramanspy-0.0.2/src/ramanspy/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      471 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/__init__.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 18:31:16.294690 ramanspy-0.0.2/src/ramanspy/analysis/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3187 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/analysis/Step.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       85 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/analysis/__init__.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1035 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/analysis/cluster.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2140 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/analysis/decompose.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     6702 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/analysis/unmix.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    11990 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/core.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    18545 2023-06-26 13:07:02.000000 ramanspy-0.0.2/src/ramanspy/datasets.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    10006 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/load.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4974 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/metrics.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 18:31:16.295218 ramanspy-0.0.2/src/ramanspy/plot/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      196 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/plot/__init__.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     7777 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/plot/_core.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    25767 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/plot/plot.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 18:31:16.296600 ramanspy-0.0.2/src/ramanspy/preprocessing/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     5493 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/preprocessing/Pipeline.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4862 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/preprocessing/Step.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      262 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/preprocessing/__init__.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    16856 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/preprocessing/baseline.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4168 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/preprocessing/denoise.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2370 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/preprocessing/despike.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2138 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/preprocessing/misc.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3573 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/preprocessing/normalise.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3143 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/preprocessing/protocols.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      473 2023-06-26 11:18:57.000000 ramanspy-0.0.2/src/ramanspy/utils.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2023-06-26 18:31:16.294008 ramanspy-0.0.2/src/ramanspy.egg-info/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3983 2023-06-26 18:31:16.000000 ramanspy-0.0.2/src/ramanspy.egg-info/PKG-INFO
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      950 2023-06-26 18:31:16.000000 ramanspy-0.0.2/src/ramanspy.egg-info/SOURCES.txt
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        1 2023-06-26 18:31:16.000000 ramanspy-0.0.2/src/ramanspy.egg-info/dependency_links.txt
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       90 2023-06-26 18:31:16.000000 ramanspy-0.0.2/src/ramanspy.egg-info/requires.txt
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        9 2023-06-26 18:31:16.000000 ramanspy-0.0.2/src/ramanspy.egg-info/top_level.txt
```

### Comparing `ramanspy-0.0.1/LICENSE` & `ramanspy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.1/PKG-INFO` & `ramanspy-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramanspy
-Version: 0.0.1
+Version: 0.0.2
 Summary: RamanSPy: An open-source Python package for integrative Raman spectroscopy data analysis
 Author-email: Dimitar Georgiev <d.georgiev21@imperial.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Dimitar Georgiev
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `ramanspy-0.0.1/README.md` & `ramanspy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.1/pyproject.toml` & `ramanspy-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ramanspy"
-version = "0.0.1"
+version = "0.0.2"
 description = "RamanSPy: An open-source Python package for integrative Raman spectroscopy data analysis"
 readme = "README.md"
 authors = [{ name = "Dimitar Georgiev", email = "d.georgiev21@imperial.ac.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
```

### Comparing `ramanspy-0.0.1/src/ramanspy/analysis/Step.py` & `ramanspy-0.0.2/src/ramanspy/analysis/Step.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.1/src/ramanspy/analysis/cluster.py` & `ramanspy-0.0.2/src/ramanspy/analysis/cluster.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.1/src/ramanspy/analysis/decompose.py` & `ramanspy-0.0.2/src/ramanspy/analysis/decompose.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.1/src/ramanspy/analysis/unmix.py` & `ramanspy-0.0.2/src/ramanspy/analysis/unmix.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.1/src/ramanspy/core.py` & `ramanspy-0.0.2/src/ramanspy/core.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.1/src/ramanspy/datasets.py` & `ramanspy-0.0.2/src/ramanspy/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,15 +289,15 @@
 
 def volumetric_cells(cell_type='THP-1', folder=None) -> List[core.SpectralVolume]:
     """
     A single volumetric scan of hiPSC cells.
 
     Data from `Kallepitis et al. (2017) <https://www.nature.com/articles/ncomms14843>`_.
 
-    Provided by authors on `Zenodo <https://zenodo.org/record/256329#.Y7wpc3bP1D_>`_.
+    Must be downloaded first. Provided by authors on `Zenodo <https://zenodo.org/record/256329#.Y7wpc3bP1D_>`_.
 
     Parameters
     ----------
     cell_type : str, default='THP-1'
         The cell type to load. Supported cell types are:
 
         - ``'THP-1'`` - THP-1 cells (n=4);
```

### Comparing `ramanspy-0.0.1/src/ramanspy/load.py` & `ramanspy-0.0.2/src/ramanspy/load.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.1/src/ramanspy/metrics.py` & `ramanspy-0.0.2/src/ramanspy/metrics.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.1/src/ramanspy/plot/_core.py` & `ramanspy-0.0.2/src/ramanspy/plot/_core.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.1/src/ramanspy/plot/plot.py` & `ramanspy-0.0.2/src/ramanspy/plot/plot.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.1/src/ramanspy/preprocessing/Pipeline.py` & `ramanspy-0.0.2/src/ramanspy/preprocessing/Pipeline.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.1/src/ramanspy/preprocessing/Step.py` & `ramanspy-0.0.2/src/ramanspy/preprocessing/Step.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.1/src/ramanspy/preprocessing/baseline.py` & `ramanspy-0.0.2/src/ramanspy/preprocessing/baseline.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.1/src/ramanspy/preprocessing/denoise.py` & `ramanspy-0.0.2/src/ramanspy/preprocessing/denoise.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.1/src/ramanspy/preprocessing/despike.py` & `ramanspy-0.0.2/src/ramanspy/preprocessing/despike.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.1/src/ramanspy/preprocessing/misc.py` & `ramanspy-0.0.2/src/ramanspy/preprocessing/misc.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.1/src/ramanspy/preprocessing/normalise.py` & `ramanspy-0.0.2/src/ramanspy/preprocessing/normalise.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.1/src/ramanspy/preprocessing/protocols.py` & `ramanspy-0.0.2/src/ramanspy/preprocessing/protocols.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.0.1/src/ramanspy.egg-info/PKG-INFO` & `ramanspy-0.0.2/src/ramanspy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramanspy
-Version: 0.0.1
+Version: 0.0.2
 Summary: RamanSPy: An open-source Python package for integrative Raman spectroscopy data analysis
 Author-email: Dimitar Georgiev <d.georgiev21@imperial.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Dimitar Georgiev
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `ramanspy-0.0.1/src/ramanspy.egg-info/SOURCES.txt` & `ramanspy-0.0.2/src/ramanspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

