# Comparing `tmp/portpy-0.0.4.tar.gz` & `tmp/portpy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\portpy-0.0.4.tar", last modified: Mon Jun 26 20:36:24 2023, max compression
+gzip compressed data, was "dist\portpy-0.0.5.tar", last modified: Mon Jun 26 20:41:24 2023, max compression
```

## Comparing `portpy-0.0.4.tar` & `portpy-0.0.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 20:36:24.000000 portpy-0.0.4/
--rw-rw-rw-   0        0        0      142 2023-06-13 16:08:24.000000 portpy-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     8193 2023-06-26 20:36:24.000000 portpy-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     6587 2023-06-13 18:42:32.000000 portpy-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 20:36:23.000000 portpy-0.0.4/images/
--rw-rw-rw-   0        0        0   184526 2023-05-12 05:53:35.000000 portpy-0.0.4/images/PortPy_logo.jpg
-drwxrwxrwx   0        0        0        0 2023-06-26 20:36:23.000000 portpy-0.0.4/portpy/
--rw-rw-rw-   0        0        0       52 2023-06-26 20:34:12.000000 portpy-0.0.4/portpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:36:23.000000 portpy-0.0.4/portpy/config_files/
--rw-rw-rw-   0        0        0        0 2023-06-13 16:25:21.000000 portpy-0.0.4/portpy/config_files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:36:23.000000 portpy-0.0.4/portpy/config_files/clinical_criteria/
-drwxrwxrwx   0        0        0        0 2023-06-26 20:36:23.000000 portpy-0.0.4/portpy/config_files/clinical_criteria/Default/
--rw-rw-rw-   0        0        0     2511 2023-01-19 21:58:41.000000 portpy-0.0.4/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json
-drwxrwxrwx   0        0        0        0 2023-06-26 20:36:23.000000 portpy-0.0.4/portpy/config_files/optimization_params/
--rw-rw-rw-   0        0        0     2419 2023-06-21 16:45:36.000000 portpy-0.0.4/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json
-drwxrwxrwx   0        0        0        0 2023-06-26 20:36:23.000000 portpy-0.0.4/portpy/photon/
--rw-rw-rw-   0        0        0      395 2023-06-12 21:08:08.000000 portpy-0.0.4/portpy/photon/__init__.py
--rw-rw-rw-   0        0        0     8347 2023-06-13 17:33:26.000000 portpy-0.0.4/portpy/photon/beam.py
--rw-rw-rw-   0        0        0     4994 2023-06-13 15:49:21.000000 portpy-0.0.4/portpy/photon/clinical_criteria.py
--rw-rw-rw-   0        0        0      702 2023-06-13 15:15:28.000000 portpy-0.0.4/portpy/photon/ct.py
--rw-rw-rw-   0        0        0    23325 2023-06-26 14:23:50.000000 portpy-0.0.4/portpy/photon/data_explorer.py
--rw-rw-rw-   0        0        0    15901 2023-06-22 18:40:10.000000 portpy-0.0.4/portpy/photon/evaluation.py
--rw-rw-rw-   0        0        0    48775 2023-06-13 15:28:29.000000 portpy-0.0.4/portpy/photon/influence_matrix.py
--rw-rw-rw-   0        0        0    22066 2023-06-22 20:54:30.000000 portpy-0.0.4/portpy/photon/optimization.py
--rw-rw-rw-   0        0        0     5806 2023-06-13 15:50:40.000000 portpy-0.0.4/portpy/photon/plan.py
--rw-rw-rw-   0        0        0    16378 2023-06-13 17:27:58.000000 portpy-0.0.4/portpy/photon/structures.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:36:23.000000 portpy-0.0.4/portpy/photon/utils/
--rw-rw-rw-   0        0        0      342 2023-06-21 21:52:31.000000 portpy-0.0.4/portpy/photon/utils/__init__.py
--rw-rw-rw-   0        0        0     2931 2023-06-22 16:17:59.000000 portpy-0.0.4/portpy/photon/utils/convert_dose_rt_dicom_to_portpy.py
--rw-rw-rw-   0        0        0     2058 2023-05-17 06:00:15.000000 portpy-0.0.4/portpy/photon/utils/get_eclipse_fluence.py
--rw-rw-rw-   0        0        0     2846 2023-05-15 12:19:37.000000 portpy-0.0.4/portpy/photon/utils/save_nrrd.py
--rw-rw-rw-   0        0        0     4887 2023-05-15 11:43:22.000000 portpy-0.0.4/portpy/photon/utils/save_or_load_pickle.py
--rw-rw-rw-   0        0        0     1387 2023-05-09 07:09:19.000000 portpy-0.0.4/portpy/photon/utils/slicer_script.py
--rw-rw-rw-   0        0        0     4188 2023-06-12 16:42:02.000000 portpy-0.0.4/portpy/photon/utils/view_in_slicer_jupyter.py
--rw-rw-rw-   0        0        0    23970 2023-06-13 17:30:49.000000 portpy-0.0.4/portpy/photon/visualization.py
-drwxrwxrwx   0        0        0        0 2023-06-26 20:36:23.000000 portpy-0.0.4/portpy.egg-info/
--rw-rw-rw-   0        0        0     8193 2023-06-26 20:36:20.000000 portpy-0.0.4/portpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      993 2023-06-26 20:36:20.000000 portpy-0.0.4/portpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 20:36:20.000000 portpy-0.0.4/portpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      352 2023-06-26 20:36:20.000000 portpy-0.0.4/portpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-26 20:36:20.000000 portpy-0.0.4/portpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 20:36:24.000000 portpy-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2502 2023-05-30 02:26:49.000000 portpy-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:41:24.000000 portpy-0.0.5/
+-rw-rw-rw-   0        0        0      142 2023-06-13 16:08:24.000000 portpy-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     8193 2023-06-26 20:41:24.000000 portpy-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6587 2023-06-13 18:42:32.000000 portpy-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 20:41:23.000000 portpy-0.0.5/images/
+-rw-rw-rw-   0        0        0   184526 2023-05-12 05:53:35.000000 portpy-0.0.5/images/PortPy_logo.jpg
+drwxrwxrwx   0        0        0        0 2023-06-26 20:41:23.000000 portpy-0.0.5/portpy/
+-rw-rw-rw-   0        0        0       52 2023-06-26 20:40:38.000000 portpy-0.0.5/portpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:41:23.000000 portpy-0.0.5/portpy/config_files/
+-rw-rw-rw-   0        0        0        0 2023-06-13 16:25:21.000000 portpy-0.0.5/portpy/config_files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:41:23.000000 portpy-0.0.5/portpy/config_files/clinical_criteria/
+drwxrwxrwx   0        0        0        0 2023-06-26 20:41:23.000000 portpy-0.0.5/portpy/config_files/clinical_criteria/Default/
+-rw-rw-rw-   0        0        0     2511 2023-01-19 21:58:41.000000 portpy-0.0.5/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json
+drwxrwxrwx   0        0        0        0 2023-06-26 20:41:23.000000 portpy-0.0.5/portpy/config_files/optimization_params/
+-rw-rw-rw-   0        0        0     2419 2023-06-21 16:45:36.000000 portpy-0.0.5/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json
+drwxrwxrwx   0        0        0        0 2023-06-26 20:41:23.000000 portpy-0.0.5/portpy/photon/
+-rw-rw-rw-   0        0        0      395 2023-06-12 21:08:08.000000 portpy-0.0.5/portpy/photon/__init__.py
+-rw-rw-rw-   0        0        0     8347 2023-06-13 17:33:26.000000 portpy-0.0.5/portpy/photon/beam.py
+-rw-rw-rw-   0        0        0     4994 2023-06-13 15:49:21.000000 portpy-0.0.5/portpy/photon/clinical_criteria.py
+-rw-rw-rw-   0        0        0      702 2023-06-13 15:15:28.000000 portpy-0.0.5/portpy/photon/ct.py
+-rw-rw-rw-   0        0        0    23325 2023-06-26 14:23:50.000000 portpy-0.0.5/portpy/photon/data_explorer.py
+-rw-rw-rw-   0        0        0    15901 2023-06-22 18:40:10.000000 portpy-0.0.5/portpy/photon/evaluation.py
+-rw-rw-rw-   0        0        0    48775 2023-06-13 15:28:29.000000 portpy-0.0.5/portpy/photon/influence_matrix.py
+-rw-rw-rw-   0        0        0    22066 2023-06-22 20:54:30.000000 portpy-0.0.5/portpy/photon/optimization.py
+-rw-rw-rw-   0        0        0     5806 2023-06-13 15:50:40.000000 portpy-0.0.5/portpy/photon/plan.py
+-rw-rw-rw-   0        0        0    16378 2023-06-13 17:27:58.000000 portpy-0.0.5/portpy/photon/structures.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:41:23.000000 portpy-0.0.5/portpy/photon/utils/
+-rw-rw-rw-   0        0        0      342 2023-06-21 21:52:31.000000 portpy-0.0.5/portpy/photon/utils/__init__.py
+-rw-rw-rw-   0        0        0     2931 2023-06-22 16:17:59.000000 portpy-0.0.5/portpy/photon/utils/convert_dose_rt_dicom_to_portpy.py
+-rw-rw-rw-   0        0        0     2058 2023-05-17 06:00:15.000000 portpy-0.0.5/portpy/photon/utils/get_eclipse_fluence.py
+-rw-rw-rw-   0        0        0     2846 2023-05-15 12:19:37.000000 portpy-0.0.5/portpy/photon/utils/save_nrrd.py
+-rw-rw-rw-   0        0        0     4887 2023-05-15 11:43:22.000000 portpy-0.0.5/portpy/photon/utils/save_or_load_pickle.py
+-rw-rw-rw-   0        0        0     1387 2023-05-09 07:09:19.000000 portpy-0.0.5/portpy/photon/utils/slicer_script.py
+-rw-rw-rw-   0        0        0     4188 2023-06-12 16:42:02.000000 portpy-0.0.5/portpy/photon/utils/view_in_slicer_jupyter.py
+-rw-rw-rw-   0        0        0    23970 2023-06-13 17:30:49.000000 portpy-0.0.5/portpy/photon/visualization.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:41:23.000000 portpy-0.0.5/portpy.egg-info/
+-rw-rw-rw-   0        0        0     8193 2023-06-26 20:41:21.000000 portpy-0.0.5/portpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      993 2023-06-26 20:41:21.000000 portpy-0.0.5/portpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 20:41:21.000000 portpy-0.0.5/portpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      352 2023-06-26 20:41:21.000000 portpy-0.0.5/portpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-26 20:41:21.000000 portpy-0.0.5/portpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 20:41:24.000000 portpy-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2502 2023-05-30 02:26:49.000000 portpy-0.0.5/setup.py
```

### Comparing `portpy-0.0.4/PKG-INFO` & `portpy-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: First open-source radiation treatment planning system in Python
 Home-page: https://github.com/PortPy-Project/PortPy
 Author: Gourav Jhanwar, Mojtaba Tefagh, Vicki Taasti, Seppo Tuomaala, Saad Nadeem, Masoud Zarepisheh
 Author-email: jhanwarg@mskcc.struct, mtefagh@acm.struct, vicki.taasti@maastro.nl, tuomaals@mskcc.struct, nadeems@mskcc.struct, zarepism@mskcc.struct
 License: Apache License, Version 2.0
 Description: <p align="center">
           <img src="./images/PortPy_logo.jpg" width="50%">
```

### Comparing `portpy-0.0.4/README.md` & `portpy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/images/PortPy_logo.jpg` & `portpy-0.0.5/images/PortPy_logo.jpg`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json` & `portpy-0.0.5/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json` & `portpy-0.0.5/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/portpy/photon/beam.py` & `portpy-0.0.5/portpy/photon/beam.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/portpy/photon/clinical_criteria.py` & `portpy-0.0.5/portpy/photon/clinical_criteria.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/portpy/photon/ct.py` & `portpy-0.0.5/portpy/photon/ct.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/portpy/photon/data_explorer.py` & `portpy-0.0.5/portpy/photon/data_explorer.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/portpy/photon/evaluation.py` & `portpy-0.0.5/portpy/photon/evaluation.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/portpy/photon/influence_matrix.py` & `portpy-0.0.5/portpy/photon/influence_matrix.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/portpy/photon/optimization.py` & `portpy-0.0.5/portpy/photon/optimization.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/portpy/photon/plan.py` & `portpy-0.0.5/portpy/photon/plan.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/portpy/photon/structures.py` & `portpy-0.0.5/portpy/photon/structures.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/portpy/photon/utils/convert_dose_rt_dicom_to_portpy.py` & `portpy-0.0.5/portpy/photon/utils/convert_dose_rt_dicom_to_portpy.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/portpy/photon/utils/get_eclipse_fluence.py` & `portpy-0.0.5/portpy/photon/utils/get_eclipse_fluence.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/portpy/photon/utils/save_nrrd.py` & `portpy-0.0.5/portpy/photon/utils/save_nrrd.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/portpy/photon/utils/save_or_load_pickle.py` & `portpy-0.0.5/portpy/photon/utils/save_or_load_pickle.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/portpy/photon/utils/slicer_script.py` & `portpy-0.0.5/portpy/photon/utils/slicer_script.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/portpy/photon/utils/view_in_slicer_jupyter.py` & `portpy-0.0.5/portpy/photon/utils/view_in_slicer_jupyter.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/portpy/photon/visualization.py` & `portpy-0.0.5/portpy/photon/visualization.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/portpy.egg-info/PKG-INFO` & `portpy-0.0.5/portpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portpy
-Version: 0.0.4
+Version: 0.0.5
 Summary: First open-source radiation treatment planning system in Python
 Home-page: https://github.com/PortPy-Project/PortPy
 Author: Gourav Jhanwar, Mojtaba Tefagh, Vicki Taasti, Seppo Tuomaala, Saad Nadeem, Masoud Zarepisheh
 Author-email: jhanwarg@mskcc.struct, mtefagh@acm.struct, vicki.taasti@maastro.nl, tuomaals@mskcc.struct, nadeems@mskcc.struct, zarepism@mskcc.struct
 License: Apache License, Version 2.0
 Description: <p align="center">
           <img src="./images/PortPy_logo.jpg" width="50%">
```

### Comparing `portpy-0.0.4/portpy.egg-info/SOURCES.txt` & `portpy-0.0.5/portpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `portpy-0.0.4/setup.py` & `portpy-0.0.5/setup.py`

 * *Files identical despite different names*

