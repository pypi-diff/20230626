# Comparing `tmp/neuroshape-0.0.4.6.4.tar.gz` & `tmp/neuroshape-0.0.4.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroshape-0.0.4.6.4.tar", last modified: Tue Jun 20 06:26:43 2023, max compression
+gzip compressed data, was "neuroshape-0.0.4.6.5.tar", last modified: Mon Jun 26 01:55:49 2023, max compression
```

## Comparing `neuroshape-0.0.4.6.4.tar` & `neuroshape-0.0.4.6.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:26:43.516731 neuroshape-0.0.4.6.4/
--rw-r--r--   0 nik        (502) admin       (80)     1501 2023-06-07 02:08:37.000000 neuroshape-0.0.4.6.4/LICENSE
--rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-20 06:26:43.514754 neuroshape-0.0.4.6.4/PKG-INFO
--rw-r--r--   0 nik        (502) admin       (80)     4445 2023-06-08 03:48:59.000000 neuroshape-0.0.4.6.4/README.rst
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:26:43.482499 neuroshape-0.0.4.6.4/neuroshape/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)    22407 2023-06-15 03:59:02.000000 neuroshape-0.0.4.6.4/neuroshape/connectopic_laplacian.py
--rw-r--r--   0 nik        (502) admin       (80)    22913 2023-06-18 23:49:14.000000 neuroshape-0.0.4.6.4/neuroshape/eigenmodes.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:26:43.487650 neuroshape-0.0.4.6.4/neuroshape/nulls/
--rw-r--r--   0 nik        (502) admin       (80)       44 2023-06-08 03:48:59.000000 neuroshape-0.0.4.6.4/neuroshape/nulls/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/nulls/burt.py
--rw-r--r--   0 nik        (502) admin       (80)    20808 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.4/neuroshape/nulls/eigenshuff.py
--rw-r--r--   0 nik        (502) admin       (80)    11987 2023-06-20 06:06:13.000000 neuroshape-0.0.4.6.4/neuroshape/nulls/eigensphere.py
--rw-r--r--   0 nik        (502) admin       (80)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/nulls/nulls.py
--rw-r--r--   0 nik        (502) admin       (80)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/nulls/spins.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:26:43.492738 neuroshape-0.0.4.6.4/neuroshape/nulls/tests/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/nulls/tests/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     5042 2023-06-19 01:29:34.000000 neuroshape-0.0.4.6.4/neuroshape/nulls/tests/eigenmode_replication.py
--rw-r--r--   0 nik        (502) admin       (80)      530 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/nulls/tests/test_burt.py
--rw-r--r--   0 nik        (502) admin       (80)     4137 2023-06-17 23:29:12.000000 neuroshape-0.0.4.6.4/neuroshape/nulls/tests/test_eigenresamp.py
--rw-r--r--   0 nik        (502) admin       (80)      695 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/nulls/tests/test_nulls.py
--rw-r--r--   0 nik        (502) admin       (80)      814 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/nulls/tests/test_spins.py
--rw-r--r--   0 nik        (502) admin       (80)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/nulls/waveshuff.py
--rw-r--r--   0 nik        (502) admin       (80)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/permutation.py
--rw-r--r--   0 nik        (502) admin       (80)    13180 2023-06-18 23:49:14.000000 neuroshape-0.0.4.6.4/neuroshape/recon.py
--rw-r--r--   0 nik        (502) admin       (80)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/stats.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:26:43.508639 neuroshape-0.0.4.6.4/neuroshape/utils/
--rw-r--r--   0 nik        (502) admin       (80)       25 2023-06-07 00:31:38.000000 neuroshape-0.0.4.6.4/neuroshape/utils/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/utils/check_fs_subjid.py
--rw-r--r--   0 nik        (502) admin       (80)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/utils/check_map.py
--rw-r--r--   0 nik        (502) admin       (80)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/utils/checks.py
--rw-r--r--   0 nik        (502) admin       (80)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/utils/compare_parallel.py
--rw-r--r--   0 nik        (502) admin       (80)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/utils/compute_geodesic_distance.py
--rw-r--r--   0 nik        (502) admin       (80)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/utils/concavehull.py
--rw-r--r--   0 nik        (502) admin       (80)    11844 2023-06-20 04:35:08.000000 neuroshape-0.0.4.6.4/neuroshape/utils/eigen.py
--rw-r--r--   0 nik        (502) admin       (80)      763 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.4/neuroshape/utils/fetch_atlas.py
--rw-r--r--   0 nik        (502) admin       (80)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/utils/fs_shapeDNA.py
--rw-r--r--   0 nik        (502) admin       (80)    31133 2023-06-18 23:49:14.000000 neuroshape-0.0.4.6.4/neuroshape/utils/geometry.py
--rw-r--r--   0 nik        (502) admin       (80)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/utils/load_mesh_vertices.py
--rw-r--r--   0 nik        (502) admin       (80)     2639 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/utils/meshtransforms.py
--rw-r--r--   0 nik        (502) admin       (80)      222 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.4/neuroshape/utils/normalize_data.py
--rw-r--r--   0 nik        (502) admin       (80)      201 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/utils/swap_single_row.py
--rw-r--r--   0 nik        (502) admin       (80)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/utils/tmpname.py
--rw-r--r--   0 nik        (502) admin       (80)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.4/neuroshape/utils/zscore_avg_method.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:26:43.484351 neuroshape-0.0.4.6.4/neuroshape.egg-info/
--rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-20 06:26:43.000000 neuroshape-0.0.4.6.4/neuroshape.egg-info/PKG-INFO
--rw-r--r--   0 nik        (502) admin       (80)     1383 2023-06-20 06:26:43.000000 neuroshape-0.0.4.6.4/neuroshape.egg-info/SOURCES.txt
--rw-r--r--   0 nik        (502) admin       (80)        1 2023-06-20 06:26:43.000000 neuroshape-0.0.4.6.4/neuroshape.egg-info/dependency_links.txt
--rw-r--r--   0 nik        (502) admin       (80)       11 2023-06-20 06:26:43.000000 neuroshape-0.0.4.6.4/neuroshape.egg-info/top_level.txt
--rw-r--r--   0 nik        (502) admin       (80)      670 2023-06-20 06:26:35.000000 neuroshape-0.0.4.6.4/pyproject.toml
--rw-r--r--   0 nik        (502) admin       (80)       38 2023-06-20 06:26:43.517349 neuroshape-0.0.4.6.4/setup.cfg
--rw-r--r--   0 nik        (502) admin       (80)     1048 2023-06-20 06:26:38.000000 neuroshape-0.0.4.6.4/setup.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-20 06:26:43.512311 neuroshape-0.0.4.6.4/src/
--rw-r--r--   0 nik        (502) admin       (80)     5389 2023-06-09 06:16:05.000000 neuroshape-0.0.4.6.4/src/eta_squared.c
--rw-r--r--   0 nik        (502) admin       (80)     2545 2023-06-06 05:49:54.000000 neuroshape-0.0.4.6.4/src/euler_threshold.c
--rw-r--r--   0 nik        (502) admin       (80)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4.6.4/src/glmfit.c
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-26 01:55:49.129194 neuroshape-0.0.4.6.5/
+-rw-r--r--   0 nik        (502) admin       (80)     1501 2023-06-07 02:08:37.000000 neuroshape-0.0.4.6.5/LICENSE
+-rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-26 01:55:49.128908 neuroshape-0.0.4.6.5/PKG-INFO
+-rw-r--r--   0 nik        (502) admin       (80)     4445 2023-06-08 03:48:59.000000 neuroshape-0.0.4.6.5/README.rst
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-26 01:55:48.821233 neuroshape-0.0.4.6.5/neuroshape/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)    22407 2023-06-15 03:59:02.000000 neuroshape-0.0.4.6.5/neuroshape/connectopic_laplacian.py
+-rw-r--r--   0 nik        (502) admin       (80)    22913 2023-06-18 23:49:14.000000 neuroshape-0.0.4.6.5/neuroshape/eigenmodes.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-26 01:55:48.884516 neuroshape-0.0.4.6.5/neuroshape/nulls/
+-rw-r--r--   0 nik        (502) admin       (80)       44 2023-06-08 03:48:59.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/burt.py
+-rw-r--r--   0 nik        (502) admin       (80)    20808 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/eigenshuff.py
+-rw-r--r--   0 nik        (502) admin       (80)    15330 2023-06-21 07:38:08.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/eigensphere.py
+-rw-r--r--   0 nik        (502) admin       (80)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/nulls.py
+-rw-r--r--   0 nik        (502) admin       (80)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/spins.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-26 01:55:48.907978 neuroshape-0.0.4.6.5/neuroshape/nulls/tests/
+-rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/tests/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     5042 2023-06-19 01:29:34.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/tests/eigenmode_replication.py
+-rw-r--r--   0 nik        (502) admin       (80)      530 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/tests/test_burt.py
+-rw-r--r--   0 nik        (502) admin       (80)     4137 2023-06-17 23:29:12.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/tests/test_eigenresamp.py
+-rw-r--r--   0 nik        (502) admin       (80)      695 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/tests/test_nulls.py
+-rw-r--r--   0 nik        (502) admin       (80)      814 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/tests/test_spins.py
+-rw-r--r--   0 nik        (502) admin       (80)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/nulls/waveshuff.py
+-rw-r--r--   0 nik        (502) admin       (80)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/permutation.py
+-rw-r--r--   0 nik        (502) admin       (80)    13180 2023-06-18 23:49:14.000000 neuroshape-0.0.4.6.5/neuroshape/recon.py
+-rw-r--r--   0 nik        (502) admin       (80)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/stats.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-26 01:55:49.068850 neuroshape-0.0.4.6.5/neuroshape/utils/
+-rw-r--r--   0 nik        (502) admin       (80)       25 2023-06-07 00:31:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/__init__.py
+-rw-r--r--   0 nik        (502) admin       (80)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/check_fs_subjid.py
+-rw-r--r--   0 nik        (502) admin       (80)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/check_map.py
+-rw-r--r--   0 nik        (502) admin       (80)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/checks.py
+-rw-r--r--   0 nik        (502) admin       (80)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/compare_parallel.py
+-rw-r--r--   0 nik        (502) admin       (80)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/compute_geodesic_distance.py
+-rw-r--r--   0 nik        (502) admin       (80)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/concavehull.py
+-rw-r--r--   0 nik        (502) admin       (80)    11784 2023-06-21 03:32:59.000000 neuroshape-0.0.4.6.5/neuroshape/utils/eigen.py
+-rw-r--r--   0 nik        (502) admin       (80)      763 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.5/neuroshape/utils/fetch_atlas.py
+-rw-r--r--   0 nik        (502) admin       (80)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/fs_shapeDNA.py
+-rw-r--r--   0 nik        (502) admin       (80)    31133 2023-06-18 23:49:14.000000 neuroshape-0.0.4.6.5/neuroshape/utils/geometry.py
+-rw-r--r--   0 nik        (502) admin       (80)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/load_mesh_vertices.py
+-rw-r--r--   0 nik        (502) admin       (80)     2639 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/meshtransforms.py
+-rw-r--r--   0 nik        (502) admin       (80)      222 2023-06-13 01:26:03.000000 neuroshape-0.0.4.6.5/neuroshape/utils/normalize_data.py
+-rw-r--r--   0 nik        (502) admin       (80)      201 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/swap_single_row.py
+-rw-r--r--   0 nik        (502) admin       (80)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/tmpname.py
+-rw-r--r--   0 nik        (502) admin       (80)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4.6.5/neuroshape/utils/zscore_avg_method.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-26 01:55:48.837562 neuroshape-0.0.4.6.5/neuroshape.egg-info/
+-rw-r--r--   0 nik        (502) admin       (80)      470 2023-06-26 01:55:48.000000 neuroshape-0.0.4.6.5/neuroshape.egg-info/PKG-INFO
+-rw-r--r--   0 nik        (502) admin       (80)     1383 2023-06-26 01:55:48.000000 neuroshape-0.0.4.6.5/neuroshape.egg-info/SOURCES.txt
+-rw-r--r--   0 nik        (502) admin       (80)        1 2023-06-26 01:55:48.000000 neuroshape-0.0.4.6.5/neuroshape.egg-info/dependency_links.txt
+-rw-r--r--   0 nik        (502) admin       (80)       11 2023-06-26 01:55:48.000000 neuroshape-0.0.4.6.5/neuroshape.egg-info/top_level.txt
+-rw-r--r--   0 nik        (502) admin       (80)      670 2023-06-26 01:55:37.000000 neuroshape-0.0.4.6.5/pyproject.toml
+-rw-r--r--   0 nik        (502) admin       (80)       38 2023-06-26 01:55:49.129277 neuroshape-0.0.4.6.5/setup.cfg
+-rw-r--r--   0 nik        (502) admin       (80)     1048 2023-06-26 01:55:25.000000 neuroshape-0.0.4.6.5/setup.py
+drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-26 01:55:49.109092 neuroshape-0.0.4.6.5/src/
+-rw-r--r--   0 nik        (502) admin       (80)     5389 2023-06-09 06:16:05.000000 neuroshape-0.0.4.6.5/src/eta_squared.c
+-rw-r--r--   0 nik        (502) admin       (80)     2545 2023-06-06 05:49:54.000000 neuroshape-0.0.4.6.5/src/euler_threshold.c
+-rw-r--r--   0 nik        (502) admin       (80)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4.6.5/src/glmfit.c
```

### Comparing `neuroshape-0.0.4.6.4/LICENSE` & `neuroshape-0.0.4.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/README.rst` & `neuroshape-0.0.4.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/connectopic_laplacian.py` & `neuroshape-0.0.4.6.5/neuroshape/connectopic_laplacian.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/eigenmodes.py` & `neuroshape-0.0.4.6.5/neuroshape/eigenmodes.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/nulls/burt.py` & `neuroshape-0.0.4.6.5/neuroshape/nulls/burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/nulls/eigenshuff.py` & `neuroshape-0.0.4.6.5/neuroshape/nulls/eigenshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/nulls/eigensphere.py` & `neuroshape-0.0.4.6.5/neuroshape/nulls/eigensphere.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     reconstruct_data,
     )
 
 import numpy as np
 import nibabel as nib
 import matplotlib.pyplot as plt
 from nilearn import plotting
+from brainsmash.utils.dataio import is_string_like, dataio
 
 cmap = plt.get_cmap('viridis')
 
 global norm_types
 norm_types = [
     'constant',
     'number',
@@ -30,15 +31,32 @@
 
 global methods
 methods = [
     'matrix',
     'regression',
     ]
 
-def eigenmode_resample(surface, data, evals, emodes, angles=None, decomp_method='matrix', resample=True):
+def gram_schmidt(A):
+    """Orthogonalize a set of vectors stored as the columns of matrix A."""
+    # get the number of vectors
+    n = A.shape[1]
+    for j in range(n):
+        # To orthogonalize the vector in column j with respect to the
+        # previous vectors, subtract from it its projection onto
+        # each of the previous vectors
+        for k in range(j):
+            A[:, j] -= np.dot(A[:, k], A[:, j]) * A[:, k]
+        
+        A[:, j] = A[:, j] / np.linalg.norm(A[:, j])
+        
+    return A
+
+def eigenmode_resample(surface, data, evals, emodes, 
+                       angles=None, decomp_method='matrix', 
+                       medial=None, resample=True):
     """
     Resample the hypersphere bounded by the eigengroups contained within `emodes`,
     and reconstruct the data using coefficients conditioned on the original data
     Based on the degenerate solutions of solving the Laplace-Beltrami operator 
     on the cortex. The power spectrum is perfectly retained (the square of the 
     eigenvalues).
     
@@ -61,15 +79,15 @@
             by the ellipsoid axes
         - finds the set of points `p` on the hypersphere given by the basis 
             modes (the eigenmodes) by normalizing them to unit length
         - rotate the set of points `p` by cos(angle) for 
             even dimensions and sin(angle) for odd dims (resampling step)
         - find the unit vectors of the points `p` by dividing by the 
             Euclidean norm (equivalent to the eigenmodes)
-        - make the new unit vectors orthonormal using QR decomposition
+        - make the new unit vectors orthonormal using Gram-Schmidt process
         - return the new eigenmodes of that eigengroup until all eigengroups
             are computed
         - reconstruct the null data by multiplying the original coefficients
             by the new eigenmodes
         - resamples the original data to the new distribution by performing
             a rank order of both the surrogate and the empirical data and
             subsitutes the empirical data into the new array, then returns the
@@ -92,15 +110,15 @@
         coordinates. The American Mathematical Monthly, 67(1), 63-66.
         <https://www.jstor.org/stable/2308932>
         
         5. Trefethen, Lloyd N., Bau, David III, (1997). Numerical linear algebra. 
         Philadelphia, PA: Society for Industrial and Applied Mathematics. 
         ISBN 978-0-898713-61-9.
         
-        6. <https://en.wikipedia.org/wiki/QR_decomposition>
+        6. https://en.wikipedia.org/wiki/QR_decomposition
         
         7. Chen, Y. C. et al., (2022). The individuality of shape asymmetries 
         of the human cerebral cortex. Elife, 11, e75056. 
         <https://doi.org/10.7554/eLife.75056>
         
 
     Parameters
@@ -127,14 +145,27 @@
         
     decomp_method : str, optional
         method of calculation of coefficients: 'matrix', 'matrix_separate', 
         'regression'.
         
         The default is 'matrix'.
         
+    medial : np.logical_array or str of path to file, default None
+        Medial wall mask for the input surface `surface`. Will use the labels
+        for the medial wall to mask out of the surrogates. If None, uses the
+        naive implementation of finding the medial wall by finding 0.0 values
+        in `data` - prone to errors if `data` has zero values outside of the
+        medial wall. Can also pass `False` to not attempt masking of medial wall
+        at all. 
+        
+        WARNING: If passing `False` to medial and `True` to resample,
+        resulting surrogates may have strange distributions since the 
+        rank-ordering step may assign medial-wall values outside of the 
+        medial wall. USE AT YOUR OWN RISK.
+        
     resample : bool, optional
         Set whether to resample surrogate map from original map to preserve
         values, default True
 
     Returns
     -------
     new_surface : nib.GiftiImage class
@@ -192,54 +223,99 @@
         if len(groups[idx]) == 3:
             # do simple rotation
             # initialize the points
             p = group_modes / np.linalg.norm(group_modes)
             p *= np.sin(angles[m])
             
             # ensure orthonormal
-            group_new_modes = p
+            group_new_modes = gram_schmidt(p)
              # get the index for the angles
-            new_modes[:, groups[idx]] = group_new_modes / np.linalg.norm(group_new_modes)
+            new_modes[:, groups[idx]] = group_new_modes
         
         m += 1
         # else, transform to spheroid and index the angles properly
         group_new_modes = transform_to_spheroid(group_evals, group_modes)
         group_spherical_modes = resample_spheroid(group_new_modes, angles[m])
         
+        # ensure orthonormal
+        group_spherical_modes = gram_schmidt(group_spherical_modes)
+        
         # transform back to ellipsoid
         group_ellipsoid_modes = transform_to_ellipsoid(group_evals, group_spherical_modes)
-        new_modes[:, groups[idx]] = group_ellipsoid_modes / np.linalg.norm(group_ellipsoid_modes)
         
+        new_modes[:, groups[idx]] = group_ellipsoid_modes / np.linalg.norm(group_ellipsoid_modes)
         
-    # reconstruct the new surface
-    # if normalize == 'constant':
-    #     if norm_factor > 0.:
-    #         new_surface = reconstruct_surface(surface, new_modes, normalize=normalize, norm_factor=norm_factor, method=method)
-    #     else:
-    #         raise ValueError("Normalization factor must be greater than zero")
-    # else:
-    #     new_surface = reconstruct_surface(surface, new_modes, n=new_modes.shape[1], normalize=normalize, method=method)
-    
+    # find the coefficents of the modes to the data by solving the OLS
+    # decomposition, either through the normal equation solution or regression    
     coeffs = eigen_decomposition(data, emodes, method=method)
-            
+    
+    # matrix multiply the estimated coefficients by the new modes
     surrogate_data = reconstruct_data(coeffs, new_modes)
     
-    if resample is True:
-        data_ranks = np.argsort(data)
-        surr_copy = np.copy(surrogate_data)
-        surr_ranks = np.argsort(surrogate_data)
-        surr_copy[surr_ranks] = data[data_ranks]
-        surrogate_data[surr_ranks] = surr_copy
+    # mask out medial wall
+    if medial is None:
+        # get index of medial wall hopefully
+        medial_wall = np.abs(data) == 0.0
+        
+    elif medial is False:
+        if resample is True:
+            raise RuntimeWarning("Resampling without masking out the medial wall "
+                                 "may result in erroneous surrogate distributions. "
+                                 "The authors of this code do not take responsibility for "
+                                 "improper usage.\n"
+                                 "USE AT YOUR OWN RISK.")
+            
+            medial_wall = np.zeros_like(data)
         
-    # get index of medial wall
-    medial_wall = np.where(data == 0.0)
+    else: # if given medial array
+        if is_string_like(medial) == True:
+            try:
+                medial = dataio(medial)
+            except:
+                raise RuntimeError("Could not load medial wall file, please check")
+        
+        if isinstance(medial, np.ndarray) == True:
+            if medial.ndim != 1:
+                raise ValueError("Medial wall array must be a vector")
+            if medial.shape[0] != surface.darrays[0].data.shape[0]:
+                # try transpose
+                if medial.shape[1] != surface.darrays[0].data.shape[0]:
+                    raise ValueError("Medial wall array must have the same number of vertices as the brain map")
+                else:
+                    medial_wall = medial.T
+            if not np.array_equal(medial, medial.astype(bool)):
+                raise RuntimeError("Medial wall array must be 1 for the ROI (medial wall) and 0 elsewhere")
+            else:    
+                medial_wall = medial
+        else:
+            raise ValueError("Could not use provided medial wall array or "
+                             "file, please check")
+    
+    medial_wall = medial_wall.astype(bool)
     
     # mask out medial wall from surrogate
     surrogate_data[medial_wall] = 0.0
     
+    if resample is True:
+        mask = np.logical_not(medial_wall)
+
+        # Mask the data and surrogate_data excluding the medial wall
+        data_no_mwall = data[mask]
+        surr_no_mwall = surrogate_data[mask]
+        
+        # Get the rank ordered indices
+        data_ranks = np.argsort(data_no_mwall)
+        surr_ranks = np.argsort(surr_no_mwall)
+        
+        # Resample surr_no_mwall according to the rank ordering of data_no_mwall
+        surr_no_mwall[surr_ranks] = data_no_mwall[data_ranks]
+        output_surr = np.copy(surrogate_data)
+        output_surr[mask] = surr_no_mwall
+        surrogate_data = output_surr
+    
     return surrogate_data
 
 
 def plot_data(surface, data, hemi='left', view='lateral', cmap='gray', show=True):
     """
     Plots a data map using nilearn.plotting, returns fig and ax handles
     from matplotlib.pyplot for further use. Can also plot values on the
```

### Comparing `neuroshape-0.0.4.6.4/neuroshape/nulls/nulls.py` & `neuroshape-0.0.4.6.5/neuroshape/nulls/nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/nulls/spins.py` & `neuroshape-0.0.4.6.5/neuroshape/nulls/spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/nulls/tests/eigenmode_replication.py` & `neuroshape-0.0.4.6.5/neuroshape/nulls/tests/eigenmode_replication.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/nulls/tests/test_burt.py` & `neuroshape-0.0.4.6.5/neuroshape/nulls/tests/test_burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/nulls/tests/test_eigenresamp.py` & `neuroshape-0.0.4.6.5/neuroshape/nulls/tests/test_eigenresamp.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/nulls/tests/test_nulls.py` & `neuroshape-0.0.4.6.5/neuroshape/nulls/tests/test_nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/nulls/tests/test_spins.py` & `neuroshape-0.0.4.6.5/neuroshape/nulls/tests/test_spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/nulls/waveshuff.py` & `neuroshape-0.0.4.6.5/neuroshape/nulls/waveshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/permutation.py` & `neuroshape-0.0.4.6.5/neuroshape/permutation.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/recon.py` & `neuroshape-0.0.4.6.5/neuroshape/recon.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/stats.py` & `neuroshape-0.0.4.6.5/neuroshape/stats.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/utils/check_fs_subjid.py` & `neuroshape-0.0.4.6.5/neuroshape/utils/check_fs_subjid.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/utils/check_map.py` & `neuroshape-0.0.4.6.5/neuroshape/utils/check_map.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/utils/checks.py` & `neuroshape-0.0.4.6.5/neuroshape/utils/checks.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/utils/compare_parallel.py` & `neuroshape-0.0.4.6.5/neuroshape/utils/compare_parallel.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/utils/compute_geodesic_distance.py` & `neuroshape-0.0.4.6.5/neuroshape/utils/compute_geodesic_distance.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/utils/concavehull.py` & `neuroshape-0.0.4.6.5/neuroshape/utils/concavehull.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/utils/eigen.py` & `neuroshape-0.0.4.6.5/neuroshape/utils/eigen.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,34 +314,32 @@
     Resample the N-D hypersphere generated by the N orthogonal unit modes
 
     """
     # ensure the eigenmodes are normalized on the unit hypersphere
     spheroid_eigenmodes = spheroid_eigenmodes / np.linalg.norm(spheroid_eigenmodes, axis=0)
     
     # length of group to determine evenness or oddness of dimensions
-    dims = spheroid_eigenmodes.shape[0]
+    #dims = spheroid_eigenmodes.shape[0]
     
     # initialize the new points p
     p = spheroid_eigenmodes
     
+    # compute the coordinates for the new points
+    for i in range(1, spheroid_eigenmodes.shape[1]):
+        p[:, i] *= np.sin(angle)
+    
     # Compute the coordinates for new points p
-    print("Computing the coordinates for each dimension, multiplying by single angle per group")
-    if dims % 2 == 0: # EVEN
-        p *= np.cos(angle)
-    else: #dims % 2 == 1 ODD
-        p *= np.sin(angle)
-        
-    # find the unit modes that describe the points p
-    if np.linalg.norm(p) == 0.0:
-        new_modes = p
-    else:
-        new_modes = p / np.linalg.norm(p)
+    # print("Computing the coordinates for each dimension, multiplying by single angle per group")
+    # if dims % 2 == 0: # EVEN
+    #     p *= np.cos(angle)
+    # else: #dims % 2 == 1 ODD
+    #     p *= np.sin(angle)
     
     # ensure that the unit modes are orthonormal (QR decomposition)
-    #new_modes = np.linalg.qr(new_modes, mode='reduced')[0]
+    new_modes = p
     
     return new_modes
 
 def _cartesian_to_spherical(x, y, z):
     """
     Convert Cartesian coordinates to spherical coordinates.
```

### Comparing `neuroshape-0.0.4.6.4/neuroshape/utils/fetch_atlas.py` & `neuroshape-0.0.4.6.5/neuroshape/utils/fetch_atlas.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/utils/fs_shapeDNA.py` & `neuroshape-0.0.4.6.5/neuroshape/utils/fs_shapeDNA.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/utils/geometry.py` & `neuroshape-0.0.4.6.5/neuroshape/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/utils/meshtransforms.py` & `neuroshape-0.0.4.6.5/neuroshape/utils/meshtransforms.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape/utils/tmpname.py` & `neuroshape-0.0.4.6.5/neuroshape/utils/tmpname.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/neuroshape.egg-info/SOURCES.txt` & `neuroshape-0.0.4.6.5/neuroshape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/pyproject.toml` & `neuroshape-0.0.4.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "setuptools>=42",
     "wheel",
 ]
 
 
 [project]
 name = "neuroshape"
-version = "0.0.4.6.4"
+version = "0.0.4.6.5"
 description = "For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change."
 readme = "README.rst"
 authors = [
     {name = "Nikitas C. Koussis", email = "nikitas.koussis@gmail.com"},
 ]
 license = { file = "LICENSE" }
```

### Comparing `neuroshape-0.0.4.6.4/setup.py` & `neuroshape-0.0.4.6.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 #                   include_dirs=[numpy.get_include()])
 
 #euler = Extension('neuroshape.euler', sources=['src/euler_threshold.c'],
 #                  include_dirs=[numpy.get_include()])
 
 # run the setup
 setup(name='neuroshape',
-      version='0.0.4.6.4',
+      version='0.0.4.6.5',
       description="For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change.",
       author='Nikitas C. Koussis, Systems Neuroscience Group Newcastle',
       author_email='nikitas.koussis@gmail.com',
       url='https://github.com/nikitas-k/neuroshape-dev',
       packages=find_packages())
       #ext_modules=[eta, glmfit, euler])
```

### Comparing `neuroshape-0.0.4.6.4/src/eta_squared.c` & `neuroshape-0.0.4.6.5/src/eta_squared.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/src/euler_threshold.c` & `neuroshape-0.0.4.6.5/src/euler_threshold.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.6.4/src/glmfit.c` & `neuroshape-0.0.4.6.5/src/glmfit.c`

 * *Files identical despite different names*

