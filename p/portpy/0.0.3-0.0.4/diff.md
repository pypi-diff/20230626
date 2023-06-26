# Comparing `tmp/portpy-0.0.3.tar.gz` & `tmp/portpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\portpy-0.0.3.tar", last modified: Tue Jun 13 17:00:01 2023, max compression
+gzip compressed data, was "dist\portpy-0.0.4.tar", last modified: Mon Jun 26 20:36:24 2023, max compression
```

## Comparing `portpy-0.0.3.tar` & `portpy-0.0.4.tar`

### file list

```diff
@@ -1,48 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 17:00:01.000000 portpy-0.0.3/
--rw-rw-rw-   0        0        0      142 2023-06-13 16:08:24.000000 portpy-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     7804 2023-06-13 17:00:01.000000 portpy-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6198 2023-06-12 04:36:17.000000 portpy-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/config_files/
-drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/config_files/clinical_criteria/
-drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/config_files/clinical_criteria/Default/
--rw-rw-rw-   0        0        0     2511 2023-01-19 21:58:41.000000 portpy-0.0.3/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json
-drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/config_files/optimization_params/
--rw-rw-rw-   0        0        0     2419 2023-05-13 03:05:59.000000 portpy-0.0.3/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json
-drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/images/
--rw-rw-rw-   0        0        0   184526 2023-05-12 05:53:35.000000 portpy-0.0.3/images/PortPy_logo.jpg
-drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/portpy/
--rw-rw-rw-   0        0        0       52 2023-06-13 16:55:29.000000 portpy-0.0.3/portpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/portpy/config_files/
--rw-rw-rw-   0        0        0        0 2023-06-13 16:25:21.000000 portpy-0.0.3/portpy/config_files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/portpy/config_files/clinical_criteria/
-drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/portpy/config_files/clinical_criteria/Default/
--rw-rw-rw-   0        0        0     2511 2023-01-19 21:58:41.000000 portpy-0.0.3/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json
-drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/portpy/config_files/optimization_params/
--rw-rw-rw-   0        0        0     2419 2023-05-13 03:05:59.000000 portpy-0.0.3/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json
-drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/portpy/photon/
--rw-rw-rw-   0        0        0      395 2023-06-12 21:08:08.000000 portpy-0.0.3/portpy/photon/__init__.py
--rw-rw-rw-   0        0        0     8340 2023-05-15 03:35:09.000000 portpy-0.0.3/portpy/photon/beam.py
--rw-rw-rw-   0        0        0     4994 2023-06-13 15:49:21.000000 portpy-0.0.3/portpy/photon/clinical_criteria.py
--rw-rw-rw-   0        0        0      702 2023-06-13 15:15:28.000000 portpy-0.0.3/portpy/photon/ct.py
--rw-rw-rw-   0        0        0    23345 2023-06-13 16:28:27.000000 portpy-0.0.3/portpy/photon/data_explorer.py
--rw-rw-rw-   0        0        0    15041 2023-06-13 16:20:52.000000 portpy-0.0.3/portpy/photon/evaluation.py
--rw-rw-rw-   0        0        0    48775 2023-06-13 15:28:29.000000 portpy-0.0.3/portpy/photon/influence_matrix.py
--rw-rw-rw-   0        0        0    22066 2023-06-13 16:00:14.000000 portpy-0.0.3/portpy/photon/optimization.py
--rw-rw-rw-   0        0        0     5806 2023-06-13 15:50:40.000000 portpy-0.0.3/portpy/photon/plan.py
--rw-rw-rw-   0        0        0    16378 2023-05-15 03:42:09.000000 portpy-0.0.3/portpy/photon/structures.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/portpy/photon/utils/
--rw-rw-rw-   0        0        0      264 2023-06-12 21:08:08.000000 portpy-0.0.3/portpy/photon/utils/__init__.py
--rw-rw-rw-   0        0        0     2058 2023-05-17 06:00:15.000000 portpy-0.0.3/portpy/photon/utils/get_eclipse_fluence.py
--rw-rw-rw-   0        0        0     2846 2023-05-15 12:19:37.000000 portpy-0.0.3/portpy/photon/utils/save_nrrd.py
--rw-rw-rw-   0        0        0     4887 2023-05-15 11:43:22.000000 portpy-0.0.3/portpy/photon/utils/save_or_load_pickle.py
--rw-rw-rw-   0        0        0     1387 2023-05-09 07:09:19.000000 portpy-0.0.3/portpy/photon/utils/slicer_script.py
--rw-rw-rw-   0        0        0     4188 2023-06-12 16:42:02.000000 portpy-0.0.3/portpy/photon/utils/view_in_slicer_jupyter.py
--rw-rw-rw-   0        0        0    24087 2023-06-13 15:27:59.000000 portpy-0.0.3/portpy/photon/visualization.py
-drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/portpy.egg-info/
--rw-rw-rw-   0        0        0     7804 2023-06-13 16:59:57.000000 portpy-0.0.3/portpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1068 2023-06-13 16:59:57.000000 portpy-0.0.3/portpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 16:59:57.000000 portpy-0.0.3/portpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      352 2023-06-13 16:59:57.000000 portpy-0.0.3/portpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-13 16:59:57.000000 portpy-0.0.3/portpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 17:00:01.000000 portpy-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2502 2023-05-30 02:26:49.000000 portpy-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:36:24.000000 portpy-0.0.4/
+-rw-rw-rw-   0        0        0      142 2023-06-13 16:08:24.000000 portpy-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     8193 2023-06-26 20:36:24.000000 portpy-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6587 2023-06-13 18:42:32.000000 portpy-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 20:36:23.000000 portpy-0.0.4/images/
+-rw-rw-rw-   0        0        0   184526 2023-05-12 05:53:35.000000 portpy-0.0.4/images/PortPy_logo.jpg
+drwxrwxrwx   0        0        0        0 2023-06-26 20:36:23.000000 portpy-0.0.4/portpy/
+-rw-rw-rw-   0        0        0       52 2023-06-26 20:34:12.000000 portpy-0.0.4/portpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:36:23.000000 portpy-0.0.4/portpy/config_files/
+-rw-rw-rw-   0        0        0        0 2023-06-13 16:25:21.000000 portpy-0.0.4/portpy/config_files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:36:23.000000 portpy-0.0.4/portpy/config_files/clinical_criteria/
+drwxrwxrwx   0        0        0        0 2023-06-26 20:36:23.000000 portpy-0.0.4/portpy/config_files/clinical_criteria/Default/
+-rw-rw-rw-   0        0        0     2511 2023-01-19 21:58:41.000000 portpy-0.0.4/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json
+drwxrwxrwx   0        0        0        0 2023-06-26 20:36:23.000000 portpy-0.0.4/portpy/config_files/optimization_params/
+-rw-rw-rw-   0        0        0     2419 2023-06-21 16:45:36.000000 portpy-0.0.4/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json
+drwxrwxrwx   0        0        0        0 2023-06-26 20:36:23.000000 portpy-0.0.4/portpy/photon/
+-rw-rw-rw-   0        0        0      395 2023-06-12 21:08:08.000000 portpy-0.0.4/portpy/photon/__init__.py
+-rw-rw-rw-   0        0        0     8347 2023-06-13 17:33:26.000000 portpy-0.0.4/portpy/photon/beam.py
+-rw-rw-rw-   0        0        0     4994 2023-06-13 15:49:21.000000 portpy-0.0.4/portpy/photon/clinical_criteria.py
+-rw-rw-rw-   0        0        0      702 2023-06-13 15:15:28.000000 portpy-0.0.4/portpy/photon/ct.py
+-rw-rw-rw-   0        0        0    23325 2023-06-26 14:23:50.000000 portpy-0.0.4/portpy/photon/data_explorer.py
+-rw-rw-rw-   0        0        0    15901 2023-06-22 18:40:10.000000 portpy-0.0.4/portpy/photon/evaluation.py
+-rw-rw-rw-   0        0        0    48775 2023-06-13 15:28:29.000000 portpy-0.0.4/portpy/photon/influence_matrix.py
+-rw-rw-rw-   0        0        0    22066 2023-06-22 20:54:30.000000 portpy-0.0.4/portpy/photon/optimization.py
+-rw-rw-rw-   0        0        0     5806 2023-06-13 15:50:40.000000 portpy-0.0.4/portpy/photon/plan.py
+-rw-rw-rw-   0        0        0    16378 2023-06-13 17:27:58.000000 portpy-0.0.4/portpy/photon/structures.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:36:23.000000 portpy-0.0.4/portpy/photon/utils/
+-rw-rw-rw-   0        0        0      342 2023-06-21 21:52:31.000000 portpy-0.0.4/portpy/photon/utils/__init__.py
+-rw-rw-rw-   0        0        0     2931 2023-06-22 16:17:59.000000 portpy-0.0.4/portpy/photon/utils/convert_dose_rt_dicom_to_portpy.py
+-rw-rw-rw-   0        0        0     2058 2023-05-17 06:00:15.000000 portpy-0.0.4/portpy/photon/utils/get_eclipse_fluence.py
+-rw-rw-rw-   0        0        0     2846 2023-05-15 12:19:37.000000 portpy-0.0.4/portpy/photon/utils/save_nrrd.py
+-rw-rw-rw-   0        0        0     4887 2023-05-15 11:43:22.000000 portpy-0.0.4/portpy/photon/utils/save_or_load_pickle.py
+-rw-rw-rw-   0        0        0     1387 2023-05-09 07:09:19.000000 portpy-0.0.4/portpy/photon/utils/slicer_script.py
+-rw-rw-rw-   0        0        0     4188 2023-06-12 16:42:02.000000 portpy-0.0.4/portpy/photon/utils/view_in_slicer_jupyter.py
+-rw-rw-rw-   0        0        0    23970 2023-06-13 17:30:49.000000 portpy-0.0.4/portpy/photon/visualization.py
+drwxrwxrwx   0        0        0        0 2023-06-26 20:36:23.000000 portpy-0.0.4/portpy.egg-info/
+-rw-rw-rw-   0        0        0     8193 2023-06-26 20:36:20.000000 portpy-0.0.4/portpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      993 2023-06-26 20:36:20.000000 portpy-0.0.4/portpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 20:36:20.000000 portpy-0.0.4/portpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      352 2023-06-26 20:36:20.000000 portpy-0.0.4/portpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-26 20:36:20.000000 portpy-0.0.4/portpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 20:36:24.000000 portpy-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2502 2023-05-30 02:26:49.000000 portpy-0.0.4/setup.py
```

### Comparing `portpy-0.0.3/PKG-INFO` & `portpy-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: portpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: First open-source radiation treatment planning system in Python
 Home-page: https://github.com/PortPy-Project/PortPy
 Author: Gourav Jhanwar, Mojtaba Tefagh, Vicki Taasti, Seppo Tuomaala, Saad Nadeem, Masoud Zarepisheh
 Author-email: jhanwarg@mskcc.struct, mtefagh@acm.struct, vicki.taasti@maastro.nl, tuomaals@mskcc.struct, nadeems@mskcc.struct, zarepism@mskcc.struct
 License: Apache License, Version 2.0
 Description: <p align="center">
           <img src="./images/PortPy_logo.jpg" width="50%">
         </p>
         
         # What is PortPy?
         **Note: The package is at its early stages of development (version 0.0.1) and we are now collecting feedback from researchers to further refine the data structure and the main functionality. We are expecting to have a stable version 1.xx around July 2023. We would love to hear your feedback.**
         
         PortPy (**P**lanning and **O**ptimization for **R**adiation **T**herapy) is a community effort to develop the **first opensource python library** to facilitate the development and clinical translation of radiotherapy cancer treatment planning algorithms. PortPy includes:
         1. Research-ready data and code for *benchmarking*, *reproducibility*, and *community-driven* development.
-        2. Interface to an open-source optimization package [CVXPy](https://www.cvxpy.org/) for easy/quick prototyping and out-of-the-box access to commercial/opensource optimization engines (e.g., Mosek, Gorubi, CPLEX, IPOPT).
+        2. Interface to an open-source optimization package [CVXPy](https://www.cvxpy.org/) for easy/quick prototyping and out-of-the-box access to commercial/opensource optimization engines (e.g., Mosek, Gorubi, CPLEX).
         3. Visualization modules to visualize relevant plan information (e.g, dose volume histograms, dose distribution, fluence map).
         4. Evaluation modules to quantify plan quality with respect to established clinical metrics (e.g., RTOG metrics, dose conformality, tumor control probability, normal tissue control probability).
         # Data
-        Data needed for optimization and algorithm development (e.g., a set of beams/beamlets/voxels, dose contribution of each beamlet to each voxel) are provided for a set of pre-specified machine parameters (e.g., beam/collimator/couch angles). We will initially provide these for a set of publicly available datasets from [TCIA](https://www.cancerimagingarchive.net/). We hope to expand our dataset in the future. The data needed for optimization is extracted from the research version of Eclipse<sup>TM</sup> treatment planning system ([Varian Medical Systems](https://www.varian.com/)) using its API. 
+        Data needed for optimization and algorithm development (e.g., a set of beams/beamlets/voxels, dose contribution of each beamlet to each voxel) are provided for a set of pre-specified machine parameters (e.g., beam/collimator/couch angles). We will initially provide these for a set of publicly available datasets from [TCIA](https://www.cancerimagingarchive.net/). We initially start with two lung patients to get feedback and then expand to about 100 patients in version 1.xx (about end of July). We hope to further expand our dataset in the future. The data needed for optimization is extracted from Eclipse<sup>TM</sup>, a FDA-approved commerical treatment planning system ([Varian Medical Systems](https://www.varian.com/)), using its API. 
         
         You can download the sample patient data [here](https://drive.google.com/drive/folders/1nA1oHEhlmh2Hk8an9e0Oi0ye6LRPREit?usp=sharing).
         
         Create a directory named './data' in the current project directory and copy the downloaded file to it, e.g ./data/Lung_Phantom_Patient_1
         
         # Quick Start
         Please see below for understanding the basic functionalities of PortPy. For advance usage of PortPy, we recommend navigating through [examples](https://github.com/PortPy-Project/PortPy/tree/master/examples) folder.
-        1. To understand the most important features of PortPy, we highly recommend to go through notebook [ex_1_introduction.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_1_introduction.ipynb)
-        2. One of the major computational issues while optimizing the plan arise due to large size of influence matrix. We suggest you to follow [ex_2_down_sampling.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_2_downsampling.py) to understand how PortPy can assist in resolving it.
+        1. To understand the most important features of PortPy, we highly recommend going through notebook [ex_1_introduction.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_1_introduction.ipynb)
+        2. One of the major computational issues while optimizing the plan arise due to large size of influence matrix. We suggest you to follow [ex_2_down_sampling.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_2_down_sampling.py) and [ex_4_inf_matrix_sparsification.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_4_inf_matrix_sparsification.py) to understand how PortPy can assist in resolving it. 
         3. You can check out [ex_3_structure_operations.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_3_structure_operations.py) to know how to perform different structure operations (e.g., boolean, margin).
-        4. For algorithm benchmarking, the global optimal solution is provided for non-convex optimization problems resulting from beam angle optimization [ex_6_boo_benchmark.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_boo_benchmark.ipynb) and incorporating DVH constraints [ex_6_dvh_benchmark.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_dvh_benchmark.py) using the mixed-integer programming on down-sampled data.
-        5. In addition to basic visualization capabilities, PortPy provide advanced visualization by integration with 3D Slicer. Please look out notebook [ex_7_Slicer.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_7_Slicer.ipynb)
+        4. For algorithm benchmarking, the global optimal solution is provided for non-convex optimization problems resulting from beam angle optimization [ex_6_boo_benchmark.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_boo_benchmark.ipynb), incorporating DVH constraints [ex_5_dvh_benchmark.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_5_dvh_benchmark.py), and VMAT optimization [ex_8_VMAT.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_8_VMAT.py) using the mixed-integer programming on down-sampled data.
+        5. In addition to basic visualization capabilities, PortPy provide advanced visualization by integration with 3D Slicer. Please check out notebook [ex_7_Slicer.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_7_Slicer.ipynb)
         
         # Installing PortPy
         
         1. Installing using pip
           ```bash
           pip install portpy
           ```
```

### Comparing `portpy-0.0.3/README.md` & `portpy-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 </p>
 
 # What is PortPy?
 **Note: The package is at its early stages of development (version 0.0.1) and we are now collecting feedback from researchers to further refine the data structure and the main functionality. We are expecting to have a stable version 1.xx around July 2023. We would love to hear your feedback.**
 
 PortPy (**P**lanning and **O**ptimization for **R**adiation **T**herapy) is a community effort to develop the **first opensource python library** to facilitate the development and clinical translation of radiotherapy cancer treatment planning algorithms. PortPy includes:
 1. Research-ready data and code for *benchmarking*, *reproducibility*, and *community-driven* development.
-2. Interface to an open-source optimization package [CVXPy](https://www.cvxpy.org/) for easy/quick prototyping and out-of-the-box access to commercial/opensource optimization engines (e.g., Mosek, Gorubi, CPLEX, IPOPT).
+2. Interface to an open-source optimization package [CVXPy](https://www.cvxpy.org/) for easy/quick prototyping and out-of-the-box access to commercial/opensource optimization engines (e.g., Mosek, Gorubi, CPLEX).
 3. Visualization modules to visualize relevant plan information (e.g, dose volume histograms, dose distribution, fluence map).
 4. Evaluation modules to quantify plan quality with respect to established clinical metrics (e.g., RTOG metrics, dose conformality, tumor control probability, normal tissue control probability).
 # Data
-Data needed for optimization and algorithm development (e.g., a set of beams/beamlets/voxels, dose contribution of each beamlet to each voxel) are provided for a set of pre-specified machine parameters (e.g., beam/collimator/couch angles). We will initially provide these for a set of publicly available datasets from [TCIA](https://www.cancerimagingarchive.net/). We hope to expand our dataset in the future. The data needed for optimization is extracted from the research version of Eclipse<sup>TM</sup> treatment planning system ([Varian Medical Systems](https://www.varian.com/)) using its API. 
+Data needed for optimization and algorithm development (e.g., a set of beams/beamlets/voxels, dose contribution of each beamlet to each voxel) are provided for a set of pre-specified machine parameters (e.g., beam/collimator/couch angles). We will initially provide these for a set of publicly available datasets from [TCIA](https://www.cancerimagingarchive.net/). We initially start with two lung patients to get feedback and then expand to about 100 patients in version 1.xx (about end of July). We hope to further expand our dataset in the future. The data needed for optimization is extracted from Eclipse<sup>TM</sup>, a FDA-approved commerical treatment planning system ([Varian Medical Systems](https://www.varian.com/)), using its API. 
 
 You can download the sample patient data [here](https://drive.google.com/drive/folders/1nA1oHEhlmh2Hk8an9e0Oi0ye6LRPREit?usp=sharing).
 
 Create a directory named './data' in the current project directory and copy the downloaded file to it, e.g ./data/Lung_Phantom_Patient_1
 
 # Quick Start
 Please see below for understanding the basic functionalities of PortPy. For advance usage of PortPy, we recommend navigating through [examples](https://github.com/PortPy-Project/PortPy/tree/master/examples) folder.
-1. To understand the most important features of PortPy, we highly recommend to go through notebook [ex_1_introduction.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_1_introduction.ipynb)
-2. One of the major computational issues while optimizing the plan arise due to large size of influence matrix. We suggest you to follow [ex_2_down_sampling.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_2_downsampling.py) to understand how PortPy can assist in resolving it.
+1. To understand the most important features of PortPy, we highly recommend going through notebook [ex_1_introduction.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_1_introduction.ipynb)
+2. One of the major computational issues while optimizing the plan arise due to large size of influence matrix. We suggest you to follow [ex_2_down_sampling.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_2_down_sampling.py) and [ex_4_inf_matrix_sparsification.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_4_inf_matrix_sparsification.py) to understand how PortPy can assist in resolving it. 
 3. You can check out [ex_3_structure_operations.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_3_structure_operations.py) to know how to perform different structure operations (e.g., boolean, margin).
-4. For algorithm benchmarking, the global optimal solution is provided for non-convex optimization problems resulting from beam angle optimization [ex_6_boo_benchmark.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_boo_benchmark.ipynb) and incorporating DVH constraints [ex_6_dvh_benchmark.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_dvh_benchmark.py) using the mixed-integer programming on down-sampled data.
-5. In addition to basic visualization capabilities, PortPy provide advanced visualization by integration with 3D Slicer. Please look out notebook [ex_7_Slicer.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_7_Slicer.ipynb)
+4. For algorithm benchmarking, the global optimal solution is provided for non-convex optimization problems resulting from beam angle optimization [ex_6_boo_benchmark.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_boo_benchmark.ipynb), incorporating DVH constraints [ex_5_dvh_benchmark.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_5_dvh_benchmark.py), and VMAT optimization [ex_8_VMAT.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_8_VMAT.py) using the mixed-integer programming on down-sampled data.
+5. In addition to basic visualization capabilities, PortPy provide advanced visualization by integration with 3D Slicer. Please check out notebook [ex_7_Slicer.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_7_Slicer.ipynb)
 
 # Installing PortPy
 
 1. Installing using pip
   ```bash
   pip install portpy
   ```
```

### Comparing `portpy-0.0.3/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json` & `portpy-0.0.4/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json`

 * *Files identical despite different names*

### Comparing `portpy-0.0.3/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json` & `portpy-0.0.4/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json`

 * *Files identical despite different names*

### Comparing `portpy-0.0.3/images/PortPy_logo.jpg` & `portpy-0.0.4/images/PortPy_logo.jpg`

 * *Files identical despite different names*

### Comparing `portpy-0.0.3/portpy/photon/beam.py` & `portpy-0.0.4/portpy/photon/beam.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     def preprocess_beams(self):
         for i, beam_id in enumerate(self.beams_dict['ID']):
             ind = self.beams_dict['ID'].index(beam_id)
             beam_2d_grid = self.create_beamlet_idx_2d_finest_grid(beam_id=beam_id)
             self.beams_dict.setdefault('beamlet_idx_2d_finest_grid', []).append(beam_2d_grid)
 
     @staticmethod
-    def get_original_map(beam_map):
+    def get_beamlet_idx_2d_grid(beam_map):
         rowsNoRepeat = [0]
         for i in range(1, np.size(beam_map, 0)):
             if (beam_map[i, :] != beam_map[rowsNoRepeat[-1], :]).any():
                 rowsNoRepeat.append(i)
         colsNoRepeat = [0]
         for j in range(1, np.size(beam_map, 1)):
             if (beam_map[:, j] != beam_map[:, colsNoRepeat[-1]]).any():
```

### Comparing `portpy-0.0.3/portpy/photon/clinical_criteria.py` & `portpy-0.0.4/portpy/photon/clinical_criteria.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.3/portpy/photon/ct.py` & `portpy-0.0.4/portpy/photon/ct.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.3/portpy/photon/data_explorer.py` & `portpy-0.0.4/portpy/photon/data_explorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,186 @@
     def __init__(self, data_dir: str = None, patient_id: str = None):
         if data_dir is None:
             data_dir = os.path.join('..', 'data')
         self.data_dir = data_dir
         if patient_id is not None:
             self.patient_id = patient_id
 
+    def display_patient_metadata(self, in_browser: bool = False, return_beams_df: bool = False,
+                                 return_structs_df: bool = False):
+        """Displays the patient information in console or browser. If in_browser is true,
+        it creates a temporary html file and lnunches your browser
+
+        :param in_browser: visualize in pretty way in browser. default to False. If false, plot table in console
+        :param return_beams_df: return dataframe containing beams metadata
+        :param return_structs_df: return dataframe containing structures metadata
+        :raises invalid directory error: raises an exception if invalid data directory
+
+        :Example:
+        >>> DataExplorer.display_patient_metadata(in_browser=False, return_beams_df=False, return_structs_df=False)
+        """
+
+        pat_dir = os.path.join(self.data_dir, self.patient_id)
+        if not os.path.exists(pat_dir):  # check if valid directory
+            raise Exception("Invalid data directory. Please input valid directory")
+
+        meta_data = self.load_metadata(pat_dir)
+        # if show_beams:
+        # check if full and/or sparse influence matrices are provided.
+        # Sparse matrix is just a truncated version of the full matrix (zeroing out small elements)
+        # often used in the optimization for computational efficiency
+        beams = meta_data['beams']  # get beams metadata
+        beams_df = pd.DataFrame.from_dict(beams)  # using Pandas data struct_name
+        is_full = beams_df['influenceMatrixFull_File'].str.contains('full',
+                                                                    na=False)  # does the data include the full influence matrix
+        is_sparse = beams_df['influenceMatrixSparse_File'].str.contains('sparse',
+                                                                        na=False)  # does the data include the sparse influence matrix
+        for ind, (sparse, full) in enumerate(zip(is_full, is_sparse)):  # create column for sparse/full check
+            if sparse and full:
+                beams_df.at[ind, 'influence_matrix(sparse/full)'] = 'Both'
+            elif sparse and not full:
+                beams_df.at[ind, 'influence_matrix(sparse/full)'] = 'Only Sparse'
+            elif not sparse and full:
+                beams_df.at[ind, 'influence_matrix(sparse/full)'] = 'Only Full'
+        #  pick information to include in the table
+        keep_columns = ['ID', 'gantry_angle', 'collimator_angle', 'couch_angle', 'beam_modality', 'energy_MV',
+                        'influence_matrix(sparse/full)',
+                        'iso_center', 'MLC_name',
+                        'machine_name']
+        beams_df = beams_df[keep_columns]
+
+        structures = meta_data['structures']
+        struct_df = pd.DataFrame.from_dict(structures)
+        keep_columns = ['name', 'volume_cc']  # discard the columns except this columns
+        struct_df = struct_df[keep_columns]
+
+        if return_beams_df and return_structs_df:
+            return beams_df, struct_df
+        elif return_beams_df:
+            return beams_df
+        elif return_structs_df:
+            return struct_df
+        # Write the results in a temporary html file in the current directory and launch a browser to display
+        if in_browser:
+            style_file = os.path.join('../..', 'df_style.css')
+            html_string = '''
+                    <html>
+                      <head><title>Portpy MetaData</title></head>
+                      <link rel="stylesheet" type="text/css" href="{style}"/>
+                      <body>
+                      <h1> PortPy Metadata </h1> 
+                      <h4> Beams Metadata </h4>
+                        {table_1}
+                      <h4> Structures Metadata </h4>
+                        {table_2}
+                      </body>
+                    </html>.
+                    '''  # create html body and append table to it
+            # create a temporary html file to store data for visualization in browser
+            with open('temp.html', 'w') as f:
+                f.write(html_string.format(table_1=beams_df.to_html(index=False, header=True, classes='mystyle'),
+                                           table_2=struct_df.to_html(index=False, header=True, classes='mystyle'),
+                                           style=style_file))
+            webbrowser.open('file://' + os.path.realpath('temp.html'))
+        else:
+            if DataExplorer.is_notebook():
+                from IPython.display import display
+                print('Beams table..')
+                with pd.option_context('display.max_rows', None,
+                                       'display.max_columns', None,
+                                       'display.precision', 3,
+                                       'display.colheader_justify', 'center',
+                                       ):
+                    beams_df = beams_df.style.set_properties(**{'text-align': 'center'})
+                    display(beams_df)
+                print('Structure table..')
+                with pd.option_context('display.max_rows', None,
+                                       'display.max_columns', None,
+                                       'display.precision', 3,
+                                       'display.colheader_justify', 'center',
+                                       ):
+                    struct_df = struct_df.style.set_properties(**{'text-align': 'center'})
+                    display(struct_df)
+            else:
+                print('Beams table..')
+                print(tabulate(beams_df, headers='keys', tablefmt='psql'))  # print the table in console using tabulate
+                print('\n\nStructures table..')
+                print(tabulate(struct_df, headers='keys', tablefmt='psql'))
+
+    def display_list_of_patients(self, in_browser: bool = False, return_df: bool = False):
+        """
+        Displays the list of patients included in data_dir folder in console (by default) or browser (if in_browser=true).
+        If in_browser is true, it creates a temporary html file and lunches your browser
+
+        :param data_dir: folder including patient data.
+            If it is None, then it assumes the data is in the current directory under sub-folder named "data"
+        :param in_browser: If true, it first saves the data in a temporary html file and then lunches the browser to visualize the data (this provides better visualization). Default to False. If false, plot table in console
+        :param return_df: return dataframe instead of visualization
+        :raises invalid directory error: raises an exception if invalid data directory.
+
+        :return patient data in Panda table
+
+        :Example:
+        >>> DataExplorer.display_list_of_patients(data_dir='path/to/data', in_browser=True)
+
+        """
+
+        display_dict = {}  # we add all the relevant information from meta_data to this dictionary
+        data_dir = self.data_dir
+        if not os.path.exists(data_dir):  # check if valid directory
+            raise Exception("Invalid data directory. Please input valid directory")
+        pat_ids = os.listdir(data_dir)
+        for i, pat_id in enumerate(pat_ids):  # Loop through patients in path
+            if "Patient" in pat_id:  # ignore irrelevant folders
+                display_dict.setdefault('patient_id', []).append(pat_id)
+                meta_data = self.load_metadata(os.path.join(data_dir, pat_id))  # load metadata for the patients
+                # set the keys and append to display dict
+                display_dict.setdefault('disease_site', []).append(pat_id.split('_')[0])
+                ind = meta_data['structures']['name'].index('PTV')
+                display_dict.setdefault('ptv_vol_cc', []).append(meta_data['structures']['volume_cc'][ind])
+                display_dict.setdefault('num_beams', []).append(len(meta_data['beams']['ID']))
+                # check if all the iso centers are same for beams
+                # res = all(
+                #     ele == meta_data['beams']['iso_center'][0] for ele in meta_data['beams']['iso_center'])
+                # if res:
+                #     display_dict.setdefault('iso_center_shift ', []).append('No')
+                # else:
+                #     display_dict.setdefault('iso_center_shift ', []).append('Yes')
+        df = pd.DataFrame.from_dict(display_dict)  # convert dictionary to dataframe
+        if return_df:
+            return df
+        if in_browser:
+            style_file = os.path.join('..', 'df_style.css')  # get style file path
+            html_string = '''
+                    <html>
+                      <head><title>Portpy MetaData</title></head>
+                      <link rel="stylesheet" type="text/css" href="{style}"/>
+                      <body>
+                      <h4> Patients Metadata </h4>
+                        {table}
+                      </body>
+                    </html>.
+                    '''  # create html body and append table to it
+            # create a temporary html file to store data for visualization in browser
+            with open('temp.html', 'w') as f:
+                f.write(
+                    html_string.format(table=df.to_html(index=False, header=True, classes='mystyle'), style=style_file))
+            webbrowser.open('file://' + os.path.realpath('temp.html'))
+        else:
+            if DataExplorer.is_notebook():
+                from IPython.display import display
+                with pd.option_context('display.max_rows', None,
+                                       'display.max_columns', None,
+                                       'display.precision', 3,
+                                       ):
+
+                    display(df)
+            else:
+                print(tabulate(df, headers='keys', tablefmt='psql'))  # print in console using tabulate
+
     def load_metadata(self, pat_dir: str = None) -> dict:
         """Loads metadata of a patient located in path and returns the metadata as a dictionary
 
         The data are loaded from the following .Json files:
         1- StructureSet_MetaData.json
             including data about the structures (e.g., PTV, Kidney, Lung)
         2- OptimizationVoxels_MetaData.json
@@ -81,17 +253,17 @@
         fname = os.path.join(pat_dir, 'PlannerBeams.json')
         if os.path.isfile(fname):
             # Opening JSON file
             json_data = self.load_json(fname)
             meta_data['planner_beam_ids'] = DataExplorer.list_to_dict(json_data)
 
         # read information regarding the clinical evaluation metrics
-        fname = os.path.join(pat_dir, 'ClinicalCriteria_MetaData.json')
-        json_data = self.load_json(fname)
-        meta_data['clinical_criteria'] = DataExplorer.list_to_dict(json_data)
+        # fname = os.path.join(pat_dir, 'ClinicalCriteria_MetaData.json')
+        # json_data = self.load_json(fname)
+        # meta_data['clinical_criteria'] = DataExplorer.list_to_dict(json_data)
 
         # read information regarding the beams_dict
         beamFolder = os.path.join(pat_dir, 'Beams')
         beamsJson = [pos_json for pos_json in os.listdir(beamFolder) if pos_json.endswith('.json')]
 
         beamsJson = natsorted(beamsJson)
         meta_data['beams'] = dict()
@@ -231,186 +403,14 @@
                                 print('Problem reading data: {}'.format(meta_data[key][i]))
                                 success = 0
                 if success:
                     del meta_data[key]
 
         return meta_data
 
-    def display_patient_metadata(self, in_browser: bool = False, return_beams_df: bool = False,
-                                 return_structs_df: bool = False):
-        """Displays the patient information in console or browser. If in_browser is true,
-        it creates a temporary html file and lnunches your browser
-
-        :param in_browser: visualize in pretty way in browser. default to False. If false, plot table in console
-        :param return_beams_df: return dataframe containing beams metadata
-        :param return_structs_df: return dataframe containing structures metadata
-        :raises invalid directory error: raises an exception if invalid data directory
-
-        :Example:
-        >>> DataExplorer.display_patient_metadata(in_browser=False, return_beams_df=False, return_structs_df=False)
-        """
-
-        pat_dir = os.path.join(self.data_dir, self.patient_id)
-        if not os.path.exists(pat_dir):  # check if valid directory
-            raise Exception("Invalid data directory. Please input valid directory")
-
-        meta_data = self.load_metadata(pat_dir)
-        # if show_beams:
-        # check if full and/or sparse influence matrices are provided.
-        # Sparse matrix is just a truncated version of the full matrix (zeroing out small elements)
-        # often used in the optimization for computational efficiency
-        beams = meta_data['beams']  # get beams metadata
-        beams_df = pd.DataFrame.from_dict(beams)  # using Pandas data struct_name
-        is_full = beams_df['influenceMatrixFull_File'].str.contains('full',
-                                                                    na=False)  # does the data include the full influence matrix
-        is_sparse = beams_df['influenceMatrixSparse_File'].str.contains('sparse',
-                                                                        na=False)  # does the data include the sparse influence matrix
-        for ind, (sparse, full) in enumerate(zip(is_full, is_sparse)):  # create column for sparse/full check
-            if sparse and full:
-                beams_df.at[ind, 'influence_matrix(sparse/full)'] = 'Both'
-            elif sparse and not full:
-                beams_df.at[ind, 'influence_matrix(sparse/full)'] = 'Only Sparse'
-            elif not sparse and full:
-                beams_df.at[ind, 'influence_matrix(sparse/full)'] = 'Only Full'
-        #  pick information to include in the table
-        keep_columns = ['ID', 'gantry_angle', 'collimator_angle', 'couch_angle', 'beam_modality', 'energy_MV',
-                        'influence_matrix(sparse/full)',
-                        'iso_center', 'MLC_name',
-                        'machine_name']
-        beams_df = beams_df[keep_columns]
-
-        structures = meta_data['structures']
-        struct_df = pd.DataFrame.from_dict(structures)
-        keep_columns = ['name', 'volume_cc']  # discard the columns except this columns
-        struct_df = struct_df[keep_columns]
-
-        if return_beams_df and return_structs_df:
-            return beams_df, struct_df
-        elif return_beams_df:
-            return beams_df
-        elif return_structs_df:
-            return struct_df
-        # Write the results in a temporary html file in the current directory and launch a browser to display
-        if in_browser:
-            style_file = os.path.join('../..', 'df_style.css')
-            html_string = '''
-                    <html>
-                      <head><title>Portpy MetaData</title></head>
-                      <link rel="stylesheet" type="text/css" href="{style}"/>
-                      <body>
-                      <h1> PortPy Metadata </h1> 
-                      <h4> Beams Metadata </h4>
-                        {table_1}
-                      <h4> Structures Metadata </h4>
-                        {table_2}
-                      </body>
-                    </html>.
-                    '''  # create html body and append table to it
-            # create a temporary html file to store data for visualization in browser
-            with open('temp.html', 'w') as f:
-                f.write(html_string.format(table_1=beams_df.to_html(index=False, header=True, classes='mystyle'),
-                                           table_2=struct_df.to_html(index=False, header=True, classes='mystyle'),
-                                           style=style_file))
-            webbrowser.open('file://' + os.path.realpath('temp.html'))
-        else:
-            if DataExplorer.is_notebook():
-                from IPython.display import display
-                print('Beams table..')
-                with pd.option_context('display.max_rows', None,
-                                       'display.max_columns', None,
-                                       'display.precision', 3,
-                                       'display.colheader_justify', 'center',
-                                       ):
-                    beams_df = beams_df.style.set_properties(**{'text-align': 'center'})
-                    display(beams_df)
-                print('Structure table..')
-                with pd.option_context('display.max_rows', None,
-                                       'display.max_columns', None,
-                                       'display.precision', 3,
-                                       'display.colheader_justify', 'center',
-                                       ):
-                    struct_df = struct_df.style.set_properties(**{'text-align': 'center'})
-                    display(struct_df)
-            else:
-                print('Beams table..')
-                print(tabulate(beams_df, headers='keys', tablefmt='psql'))  # print the table in console using tabulate
-                print('\n\nStructures table..')
-                print(tabulate(struct_df, headers='keys', tablefmt='psql'))
-
-    def display_list_of_patients(self, in_browser: bool = False, return_df: bool = False):
-        """
-        Displays the list of patients included in data_dir folder in console (by default) or browser (if in_browser=true).
-        If in_browser is true, it creates a temporary html file and lunches your browser
-
-        :param data_dir: folder including patient data.
-            If it is None, then it assumes the data is in the current directory under sub-folder named "data"
-        :param in_browser: If true, it first saves the data in a temporary html file and then lunches the browser to visualize the data (this provides better visualization). Default to False. If false, plot table in console
-        :param return_df: return dataframe instead of visualization
-        :raises invalid directory error: raises an exception if invalid data directory.
-
-        :return patient data in Panda table
-
-        :Example:
-        >>> DataExplorer.display_list_of_patients(data_dir='path/to/data', in_browser=True)
-
-        """
-
-        display_dict = {}  # we add all the relevant information from meta_data to this dictionary
-        data_dir = self.data_dir
-        if not os.path.exists(data_dir):  # check if valid directory
-            raise Exception("Invalid data directory. Please input valid directory")
-        pat_ids = os.listdir(data_dir)
-        for i, pat_id in enumerate(pat_ids):  # Loop through patients in path
-            if "Patient" in pat_id:  # ignore irrelevant folders
-                display_dict.setdefault('patient_id', []).append(pat_id)
-                meta_data = self.load_metadata(os.path.join(data_dir, pat_id))  # load metadata for the patients
-                # set the keys and append to display dict
-                display_dict.setdefault('disease_site', []).append(meta_data['clinical_criteria']['disease_site'])
-                ind = meta_data['structures']['name'].index('PTV')
-                display_dict.setdefault('ptv_vol_cc', []).append(meta_data['structures']['volume_cc'][ind])
-                display_dict.setdefault('num_beams', []).append(len(meta_data['beams']['ID']))
-                # check if all the iso centers are same for beams
-                # res = all(
-                #     ele == meta_data['beams']['iso_center'][0] for ele in meta_data['beams']['iso_center'])
-                # if res:
-                #     display_dict.setdefault('iso_center_shift ', []).append('No')
-                # else:
-                #     display_dict.setdefault('iso_center_shift ', []).append('Yes')
-        df = pd.DataFrame.from_dict(display_dict)  # convert dictionary to dataframe
-        if return_df:
-            return df
-        if in_browser:
-            style_file = os.path.join('..', 'df_style.css')  # get style file path
-            html_string = '''
-                    <html>
-                      <head><title>Portpy MetaData</title></head>
-                      <link rel="stylesheet" type="text/css" href="{style}"/>
-                      <body>
-                      <h4> Patients Metadata </h4>
-                        {table}
-                      </body>
-                    </html>.
-                    '''  # create html body and append table to it
-            # create a temporary html file to store data for visualization in browser
-            with open('temp.html', 'w') as f:
-                f.write(
-                    html_string.format(table=df.to_html(index=False, header=True, classes='mystyle'), style=style_file))
-            webbrowser.open('file://' + os.path.realpath('temp.html'))
-        else:
-            if DataExplorer.is_notebook():
-                from IPython.display import display
-                with pd.option_context('display.max_rows', None,
-                                       'display.max_columns', None,
-                                       'display.precision', 3,
-                                       ):
-
-                    display(df)
-            else:
-                print(tabulate(df, headers='keys', tablefmt='psql'))  # print in console using tabulate
-
     @staticmethod
     def is_notebook() -> bool:
         try:
             from IPython import get_ipython
             shell = get_ipython().__class__.__name__
             if shell == 'ZMQInteractiveShell':
                 return True  # Jupyter notebook or qtconsole
```

### Comparing `portpy-0.0.3/portpy/photon/evaluation.py` & `portpy-0.0.4/portpy/photon/evaluation.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,117 +50,14 @@
         """
         x, y = Evaluation.get_dvh(sol, dose_1d=dose_1d, struct=struct, weight_flag=weight_flag)
         f = interpolate.interp1d(100 * y, x)
 
         return f(volume_per)
 
     @staticmethod
-    def get_volume(sol: dict, struct: str, dose_value_gy: float, dose_1d: np.ndarray = None,
-                   weight_flag: bool = True) -> float:
-        """
-        Get volume at dose_1d value in Gy
-
-        :param sol: solution dictionary
-        :param dose_1d: dose_1d in 1d
-        :param struct: struct_name name for which to get the dose_1d
-        :param dose_value_gy: query the volume at dose_value
-        :param weight_flag: for non uniform voxels weight flag always True
-        :return: dose_1d at volume_percentage
-
-        :Example:
-
-        >>> Evaluation.get_volume(sol=sol, struct='PTV', dose_value_gy=60)
-
-        """
-        x, y = Evaluation.get_dvh(sol, dose_1d=dose_1d, struct=struct, weight_flag=weight_flag)
-        x1, indices = np.unique(x, return_index=True)
-        y1 = y[indices]
-        f = interpolate.interp1d(x1, 100 * y1)
-        if dose_value_gy > max(x1):
-            print('Warning: dose_1d value {} is greater than max dose_1d for {}'.format(dose_value_gy, struct))
-            return 0
-        else:
-            return f(dose_value_gy)
-
-    @staticmethod
-    def get_dvh(sol: dict, struct: str, dose_1d: np.ndarray = None, weight_flag: bool = True):
-        """
-        Get dvh for the struct_name
-
-        :param sol: optimal solution dictionary
-        :param dose_1d: dose_1d which is not in solution dictionary
-        :param struct: struct_name name
-        :param weight_flag: for non uniform voxels weight flag always True
-        :return: x, y --> dvh for the struct_name
-
-        :Example:
-
-        >>> Evaluation.get_dvh(sol=sol, struct='PTV')
-
-        """
-        inf_matrix = sol['inf_matrix']
-        vox = inf_matrix.get_opt_voxels_idx(struct)
-        if dose_1d is None:
-            dose_1d = sol['dose_1d']
-        org_sort_dose = np.sort(dose_1d[vox])
-        sort_ind = np.argsort(dose_1d[vox])
-        org_sort_dose = np.append(org_sort_dose, org_sort_dose[-1] + 0.01)
-        x = org_sort_dose
-        if weight_flag:
-            # org_points_sort_spacing = my_plan._structures.opt_voxels_dict['dose_voxel_resolution_XYZ_mm']
-            # org_points_sort_volume = org_points_sort_spacing[:, 0] * org_points_sort_spacing[:,
-            #                                                          1] * org_points_sort_spacing[:, 2]
-            # sum_weight = np.sum(org_points_sort_volume)
-            org_weights = inf_matrix.get_opt_voxels_volume_cc(struct)
-            org_sort_weights = org_weights[sort_ind]
-            sum_weight = np.sum(org_sort_weights)
-            y = [1]
-            for j in range(len(org_sort_weights)):
-                y.append(y[-1] - org_sort_weights[j] / sum_weight)
-        else:
-            y = np.ones(len(vox) + 1) - np.arange(0, len(vox) + 1) / len(vox)
-        y[-1] = 0
-        y = np.array(y)
-        return x, y
-
-    @staticmethod
-    def get_max_dose(sol: dict, struct: str, dose_1d=None) -> float:
-        """
-        Get maximum dose_1d for the struct_name
-
-        :param sol: optimal solution dictionary
-        :param dose_1d: dose_1d which is not in solution dictionary
-        :param struct: struct_name name
-
-        :return: maximum dose_1d for the struct_name
-        """
-        inf_matrix = sol['inf_matrix']
-        vox = inf_matrix.get_opt_voxels_idx(struct)
-        if dose_1d is None:
-            dose_1d = sol['dose_1d']
-        return np.max(dose_1d[vox])
-
-    @staticmethod
-    def get_mean_dose(sol: dict, struct: str, dose_1d=None) -> np.ndarray:
-        """
-                Get mean dose_1d for the struct_name
-
-                :param sol: optimal solution dictionary
-                :param dose_1d: dose_1d which is not in solution dictionary
-                :param struct: struct_name name
-
-                :return: mean dose_1d for the struct_name
-                """
-        inf_matrix = sol['inf_matrix']
-        vox = inf_matrix.get_opt_voxels_idx(struct)
-        if dose_1d is None:
-            dose_1d = sol['dose_1d']
-        return np.mean(dose_1d[vox])
-
-    @staticmethod
     def display_clinical_criteria(my_plan: Plan, sol: Union[dict, List[dict]], html_file_name='temp.html',
                                   sol_names: List[str] = None, clinical_criteria: ClinicalCriteria = None,
                                   return_df: bool = False, in_browser: bool = False):
         """
         Visualization the plan metrics for clinical criteria in browser.
         It evaluate the plan by comparing the metrics against required criteria.
 
@@ -269,29 +166,29 @@
         styled_df = df.style.apply(color_plan_value, subset=sol_names, axis=1)  # apply
         # color to dataframe using df.style method
         if return_df:
             return styled_df
         if in_browser:
             html = styled_df.render()  # render to html
             html_string = '''
-                                            <html>
-                                              <head><title>Portpy Clinical Criteria Evaluation</title></head>
-                                              <style> 
-                                                table, th, td {{font-size:10pt; border:1px solid black; border-collapse:collapse; text-align:left;}}
-                                                th, td {{padding: 5px;}}
-                                              </style>
-                                              <body>
-                                              <h1> Clinical Criteria</h1>
-                                              <h4 style="color: green">Meets limit and goal</h4>
-                                              <h4 style="color: orange">Meets limit but not goal</h4>
-                                              <h4 style="color: red">Violate both limit and goal</h4>
-                                                {table}
-                                              </body>
-                                            </html>.
-                                            '''
+                                                <html>
+                                                  <head><title>Portpy Clinical Criteria Evaluation</title></head>
+                                                  <style> 
+                                                    table, th, td {{font-size:10pt; border:1px solid black; border-collapse:collapse; text-align:left;}}
+                                                    th, td {{padding: 5px;}}
+                                                  </style>
+                                                  <body>
+                                                  <h1> Clinical Criteria</h1>
+                                                  <h4 style="color: green">Meets limit and goal</h4>
+                                                  <h4 style="color: orange">Meets limit but not goal</h4>
+                                                  <h4 style="color: red">Violate both limit and goal</h4>
+                                                    {table}
+                                                  </body>
+                                                </html>.
+                                                '''
             with open(html_file_name, 'w') as f:
                 f.write(html_string.format(table=html))
             webbrowser.open('file://' + os.path.realpath(html_file_name))
 
         else:
             if Evaluation.is_notebook():
                 from IPython.display import display
@@ -301,14 +198,136 @@
                                        ):
 
                     display(styled_df)
             else:
                 print(tabulate(df, headers='keys', tablefmt='psql'))  # print in console using tabulate
 
     @staticmethod
+    def get_volume(sol: dict, struct: str, dose_value_gy: float, dose_1d: np.ndarray = None,
+                   weight_flag: bool = True) -> float:
+        """
+        Get volume at dose_1d value in Gy
+
+        :param sol: solution dictionary
+        :param dose_1d: dose_1d in 1d
+        :param struct: struct_name name for which to get the dose_1d
+        :param dose_value_gy: query the volume at dose_value
+        :param weight_flag: for non uniform voxels weight flag always True
+        :return: dose_1d at volume_percentage
+
+        :Example:
+
+        >>> Evaluation.get_volume(sol=sol, struct='PTV', dose_value_gy=60)
+
+        """
+        x, y = Evaluation.get_dvh(sol, dose_1d=dose_1d, struct=struct, weight_flag=weight_flag)
+        x1, indices = np.unique(x, return_index=True)
+        y1 = y[indices]
+        f = interpolate.interp1d(x1, 100 * y1)
+        if dose_value_gy > max(x1):
+            print('Warning: dose_1d value {} is greater than max dose_1d for {}'.format(dose_value_gy, struct))
+            return 0
+        else:
+            return f(dose_value_gy)
+
+    @staticmethod
+    def get_dvh(sol: dict, struct: str, dose_1d: np.ndarray = None, weight_flag: bool = True):
+        """
+        Get dvh for the struct_name
+
+        :param sol: optimal solution dictionary
+        :param dose_1d: dose_1d which is not in solution dictionary
+        :param struct: struct_name name
+        :param weight_flag: for non uniform voxels weight flag always True
+        :return: x, y --> dvh for the struct_name
+
+        :Example:
+
+        >>> Evaluation.get_dvh(sol=sol, struct='PTV')
+
+        """
+        inf_matrix = sol['inf_matrix']
+        vox = inf_matrix.get_opt_voxels_idx(struct)
+        if dose_1d is None:
+            dose_1d = sol['dose_1d']
+        org_sort_dose = np.sort(dose_1d[vox])
+        sort_ind = np.argsort(dose_1d[vox])
+        org_sort_dose = np.append(org_sort_dose, org_sort_dose[-1] + 0.01)
+        x = org_sort_dose
+        if weight_flag:
+            # org_points_sort_spacing = my_plan._structures.opt_voxels_dict['dose_voxel_resolution_XYZ_mm']
+            # org_points_sort_volume = org_points_sort_spacing[:, 0] * org_points_sort_spacing[:,
+            #                                                          1] * org_points_sort_spacing[:, 2]
+            # sum_weight = np.sum(org_points_sort_volume)
+            org_weights = inf_matrix.get_opt_voxels_volume_cc(struct)
+            org_sort_weights = org_weights[sort_ind]
+            sum_weight = np.sum(org_sort_weights)
+            y = [1]
+            for j in range(len(org_sort_weights)):
+                y.append(y[-1] - org_sort_weights[j] / sum_weight)
+        else:
+            y = np.ones(len(vox) + 1) - np.arange(0, len(vox) + 1) / len(vox)
+        y[-1] = 0
+        y = np.array(y)
+        return x, y
+
+    @staticmethod
+    def get_max_dose(sol: dict, struct: str, dose_1d=None) -> float:
+        """
+        Get maximum dose_1d for the struct_name
+
+        :param sol: optimal solution dictionary
+        :param dose_1d: dose_1d which is not in solution dictionary
+        :param struct: struct_name name
+
+        :return: maximum dose_1d for the struct_name
+        """
+        inf_matrix = sol['inf_matrix']
+        vox = inf_matrix.get_opt_voxels_idx(struct)
+        if dose_1d is None:
+            dose_1d = sol['dose_1d']
+        return np.max(dose_1d[vox])
+
+    @staticmethod
+    def get_mean_dose(sol: dict, struct: str, dose_1d=None) -> np.ndarray:
+        """
+                Get mean dose_1d for the struct_name
+
+                :param sol: optimal solution dictionary
+                :param dose_1d: dose_1d which is not in solution dictionary
+                :param struct: struct_name name
+
+                :return: mean dose_1d for the struct_name
+                """
+        inf_matrix = sol['inf_matrix']
+        vox = inf_matrix.get_opt_voxels_idx(struct)
+        if dose_1d is None:
+            dose_1d = sol['dose_1d']
+        return np.mean(dose_1d[vox])
+
+    @staticmethod
+    def get_BED(my_plan: Plan, sol: dict = None, dose_per_fraction_1d: np.ndarray = None, alpha=1, beta=1) -> np.ndarray:
+        """
+        Get Biologically equivalent dose (BED) for the struct_name
+
+        :param my_plan: Object of class Plan
+        :param sol: optimal solution dictionary
+        :param dose_per_fraction_1d: dose_1d which is not in solution dictionary
+
+        :return: BED
+        """
+
+        if dose_per_fraction_1d is None:
+            dose_per_fraction_1d = sol['inf_matrix'].A @ (sol['optimal_intensity'])
+        bed_d = np.zeros_like(dose_per_fraction_1d)
+        for i in range(int(my_plan.get_num_of_fractions())):
+            bed_d = bed_d + (dose_per_fraction_1d + (dose_per_fraction_1d**2/(alpha/beta)))
+        return bed_d
+
+    @staticmethod
     def is_notebook() -> bool:
         try:
             from IPython import get_ipython
             shell = get_ipython().__class__.__name__
             if shell == 'ZMQInteractiveShell':
                 return True  # Jupyter notebook or qtconsole
             elif shell == 'TerminalInteractiveShell':
```

### Comparing `portpy-0.0.3/portpy/photon/influence_matrix.py` & `portpy-0.0.4/portpy/photon/influence_matrix.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.3/portpy/photon/optimization.py` & `portpy-0.0.4/portpy/photon/optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
                             (obj_funcs[i]['weight'] * cp.sum_squares(dU))]
                     constraints += [A[st.get_opt_voxels_idx(struct), :] @ x >= dose_gy - dU]
             elif obj_funcs[i]['type'] == 'quadratic':
                 if obj_funcs[i]['structure_name'] in my_plan.structures.get_structures():
                     struct = obj_funcs[i]['structure_name']
                     obj += [(1 / len(st.get_opt_voxels_idx(struct))) * (
                             obj_funcs[i]['weight'] * cp.sum_squares(A[st.get_opt_voxels_idx(struct), :] @ x))]
-            elif obj_funcs[i]['type'] == 'quadratic-smoothness':
+            elif obj_funcs[i]['type'] == 'smoothness-quadratic':
                 [Qx, Qy, num_rows, num_cols] = self.get_smoothness_matrix(inf_matrix.beamlets_dict)
                 smoothness_X_weight = 0.6
                 smoothness_Y_weight = 0.4
                 obj += [obj_funcs[i]['weight'] * (smoothness_X_weight * (1 / num_cols) * cp.sum_squares(Qx @ x) +
                                                   smoothness_Y_weight * (1 / num_rows) * cp.sum_squares(Qy @ x))]
 
         print('Objective done')
```

### Comparing `portpy-0.0.3/portpy/photon/plan.py` & `portpy-0.0.4/portpy/photon/plan.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.3/portpy/photon/structures.py` & `portpy-0.0.4/portpy/photon/structures.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -68,71 +68,14 @@
 
          :param structure_name: name of the struct_name in plan
          :return: volume of the struct_name
          """
         ind = self.structures_dict['name'].index(structure_name)
         return self.structures_dict['fraction_of_vol_in_calc_box'][ind]
 
-    def preprocess_structures(self):
-        """
-        preprocess structures to create optimization voxel indices for the struct_name
-        :return:
-        """
-        self.opt_voxels_dict['voxel_idx'] = [None] * len(self.structures_dict['name'])
-        self.opt_voxels_dict['voxel_volume_cc'] = [None] * len(self.structures_dict['name'])
-        for i in range(len(self.structures_dict['name'])):
-            vox_3d = self.structures_dict['structure_mask_3d'][i] * self.opt_voxels_dict['ct_to_dose_voxel_map'][0]
-            # my_plan.structures_dict['voxel_idx'][i] = np.unique(vox_3d[vox_3d > 0])
-            vox, counts = np.unique(vox_3d[vox_3d > 0], return_counts=True)
-            self.opt_voxels_dict['voxel_idx'][i] = vox
-            self.opt_voxels_dict['voxel_volume_cc'][i] = counts * np.prod(
-                self._ct_voxel_resolution_xyz_mm)/1000  # calculate weight for each voxel
-            # dividing by 1000 due to conversion from mm3 to cm3
-            # self.opt_voxels_dict['voxel_volume_cc'][i] = counts / np.max(counts)  # calculate weight for each voxel
-
-    def create_structure(self, new_struct_name: str, mask_3d: np.ndarray) -> None:
-        """
-        Create a new struct_name and append its mask to the structures_dict
-
-        :param new_struct_name: name of the new struct_name
-        :param mask_3d: 3d mask for the struct_name
-        :return: create new_struct_name
-        """
-        for key in self.structures_dict.keys():
-            if key == 'name':
-                self.structures_dict['name'].append(new_struct_name)
-            elif key == 'structure_mask_3d':
-                self.structures_dict['structure_mask_3d'].append(mask_3d)
-            else:
-                self.structures_dict[key].append(None)
-
-    def modify_structure(self, struct_name: str, mask_3d: np.ndarray) -> None:
-        """
-        :param struct_name: name of the struct_name to be modified
-        :param mask_3d: 3d mask for the struct_name
-        :return: modify struct_name
-        """
-        ind = self.structures_dict['name'].index(struct_name)
-        for key in self.structures_dict.keys():
-            if key == 'name':
-                self.structures_dict['name'][ind] = struct_name
-            elif key == 'structure_mask_3d':
-                self.structures_dict['structure_mask_3d'][ind] = mask_3d
-            else:
-                self.structures_dict[key][ind] = None
-
-    def delete_structure(self, structure: str):
-        """
-        :param structure: struct_name to be removed
-        :return:
-        """
-        ind = self.structures_dict['name'].index(structure)
-        for key in self.structures_dict.keys():
-            del self.structures_dict[key][ind]
-
     def union(self, struct_1_name: str, struct_2_name: str, new_struct_name: str) -> None:
         """
         Create union of two structures struct_1_name and struct_2_name. If str1_or_str2 is not in structures dict,
         it will create new structures. If str1_or_str2 is in structure_dict, it will modify the struct_name
 
         :param struct_1_name: struct_name name for the 1st struct_name
         :param struct_2_name: struct_name name for the 2nd struct_name
@@ -303,14 +246,71 @@
         self.delete_structure('dose_mask')
 
         print('rinds created!!')
         # for param in rind_params:
         #     self.set_opt_voxel_idx(struct_name=param['name'])
         self.preprocess_structures()
 
+    def preprocess_structures(self):
+        """
+        preprocess structures to create optimization voxel indices for the struct_name
+        :return:
+        """
+        self.opt_voxels_dict['voxel_idx'] = [None] * len(self.structures_dict['name'])
+        self.opt_voxels_dict['voxel_volume_cc'] = [None] * len(self.structures_dict['name'])
+        for i in range(len(self.structures_dict['name'])):
+            vox_3d = self.structures_dict['structure_mask_3d'][i] * self.opt_voxels_dict['ct_to_dose_voxel_map'][0]
+            # my_plan.structures_dict['voxel_idx'][i] = np.unique(vox_3d[vox_3d > 0])
+            vox, counts = np.unique(vox_3d[vox_3d > 0], return_counts=True)
+            self.opt_voxels_dict['voxel_idx'][i] = vox
+            self.opt_voxels_dict['voxel_volume_cc'][i] = counts * np.prod(
+                self._ct_voxel_resolution_xyz_mm)/1000  # calculate weight for each voxel
+            # dividing by 1000 due to conversion from mm3 to cm3
+            # self.opt_voxels_dict['voxel_volume_cc'][i] = counts / np.max(counts)  # calculate weight for each voxel
+
+    def create_structure(self, new_struct_name: str, mask_3d: np.ndarray) -> None:
+        """
+        Create a new struct_name and append its mask to the structures_dict
+
+        :param new_struct_name: name of the new struct_name
+        :param mask_3d: 3d mask for the struct_name
+        :return: create new_struct_name
+        """
+        for key in self.structures_dict.keys():
+            if key == 'name':
+                self.structures_dict['name'].append(new_struct_name)
+            elif key == 'structure_mask_3d':
+                self.structures_dict['structure_mask_3d'].append(mask_3d)
+            else:
+                self.structures_dict[key].append(None)
+
+    def modify_structure(self, struct_name: str, mask_3d: np.ndarray) -> None:
+        """
+        :param struct_name: name of the struct_name to be modified
+        :param mask_3d: 3d mask for the struct_name
+        :return: modify struct_name
+        """
+        ind = self.structures_dict['name'].index(struct_name)
+        for key in self.structures_dict.keys():
+            if key == 'name':
+                self.structures_dict['name'][ind] = struct_name
+            elif key == 'structure_mask_3d':
+                self.structures_dict['structure_mask_3d'][ind] = mask_3d
+            else:
+                self.structures_dict[key][ind] = None
+
+    def delete_structure(self, structure: str):
+        """
+        :param structure: struct_name to be removed
+        :return:
+        """
+        ind = self.structures_dict['name'].index(structure)
+        for key in self.structures_dict.keys():
+            del self.structures_dict[key][ind]
+
     def set_opt_voxel_idx(self, struct_name):
         ind = self.structures_dict['name'].index(struct_name)
         vox_3d = self.structures_dict['structure_mask_3d'][ind] * \
                  self.opt_voxels_dict['ct_to_dose_voxel_map'][0]
         # my_plan.structures_dict['voxel_idx'][i] = np.unique(vox_3d[vox_3d > 0])
         vox, counts = np.unique(vox_3d[vox_3d > 0], return_counts=True)
         self.opt_voxels_dict['voxel_idx'].append(vox)
```

### Comparing `portpy-0.0.3/portpy/photon/utils/get_eclipse_fluence.py` & `portpy-0.0.4/portpy/photon/utils/get_eclipse_fluence.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.3/portpy/photon/utils/save_nrrd.py` & `portpy-0.0.4/portpy/photon/utils/save_nrrd.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.3/portpy/photon/utils/save_or_load_pickle.py` & `portpy-0.0.4/portpy/photon/utils/save_or_load_pickle.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.3/portpy/photon/utils/slicer_script.py` & `portpy-0.0.4/portpy/photon/utils/slicer_script.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.3/portpy/photon/utils/view_in_slicer_jupyter.py` & `portpy-0.0.4/portpy/photon/utils/view_in_slicer_jupyter.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.3/portpy/photon/visualization.py` & `portpy-0.0.4/portpy/photon/visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,49 +162,14 @@
         if show:
             plt.show()
         if filename is not None:
             plt.savefig(filename, bbox_inches="tight", dpi=300)
         return ax
 
     @staticmethod
-    def plot_binary_mask_points(my_plan, structure: str, show: bool = True, color: List[str] = None):
-        fig = plt.figure()
-        ax = fig.add_subplot(111, projection='3d')
-        ind = my_plan.structures.structures_dict['name'].index(structure)
-        mask_3d = my_plan.structures.structures_dict['structure_mask_3d'][ind]
-        pos = np.where(mask_3d == 1)
-        if color is None:
-            color = Visualization.get_colors()
-        ax.scatter(pos[0], pos[1], pos[2], c=color)
-        if show:
-            plt.show()
-
-    @staticmethod
-    def get_colors():
-        """
-
-        :return: return list of 20 colors
-        """
-        colors = ['#ffe119', '#4363d8', '#f58231', '#911eb4',
-                  '#46f0f0', '#f032e6', '#bcf60c', '#fabebe', '#008080', '#e6beff',
-                  '#9a6324', '#fffac8', '#800000', '#aaffc3', '#808000', '#ffd8b1',
-                  '#000075', '#808080', '#ffffff', '#000000', '#e6194b', '#3cb44b']
-        return colors
-
-    @staticmethod
-    def surface_plot(matrix: np.ndarray, **kwargs):
-        # acquire the cartesian coordinate matrices from the matrix
-        # x is cols, y is rows
-        (x, y) = np.meshgrid(np.arange(matrix.shape[0]), np.arange(matrix.shape[1]))
-        fig = plt.figure()
-        ax = fig.add_subplot(111, projection='3d')
-        surf = ax.plot_surface(x, y, np.transpose(matrix), **kwargs)
-        return ax, surf
-
-    @staticmethod
     def plot_fluence_2d(beam_id: int, sol: dict = None, optimal_fluence_2d: List[np.ndarray] = None,
                         inf_matrix: InfluenceMatrix = None, **options):
         """
 
         Displays fluence in 2d for the given beam_id
 
         :param beam_id: beam_id of the beam
@@ -273,15 +238,15 @@
 
         ind = [i for i in range(len(inf_matrix.beamlets_dict)) if inf_matrix.beamlets_dict[i]['beam_id'] == beam_id]
         if len(ind) == 0:
             raise IndexError('invalid beam id {}'.format(beam_id))
         if sol is not None:
             optimal_fluence_2d = inf_matrix.fluence_1d_to_2d(sol=sol)
         (ax, surf) = Visualization.surface_plot(optimal_fluence_2d[ind[0]], ax=ax, figsize=figsize,
-                                                  cmap='viridis', edgecolor='black')
+                                                cmap='viridis', edgecolor='black')
         plt.colorbar(surf, ax=ax, pad=0.2)
         ax.set_zlabel('Fluence Intensity')
         ax.set_xlabel('x-axis (beamlets column)')
         ax.set_ylabel('y-axis (beamlets row)')
 
         if title is not None:
             ax.set_title('{}'.format(title))
@@ -391,37 +356,14 @@
         if show:
             plt.show()
         if filename is not None:
             plt.savefig(filename, bbox_inches="tight", dpi=300)
         return ax
 
     @staticmethod
-    def get_cmap_colors(n, name='hsv'):
-        """Returns a function that maps each index in 0, 1, ..., n-1 to a distinct
-        RGB color; the keyword argument name must be a standard mpl colormap name."""
-        return plt.cm.get_cmap(name, n)
-
-    @staticmethod
-    def legend_dose_storage(my_plan: Plan) -> dict:
-        # dose_color = [[0.55, 0, 1], [0, 0, 1], [0, 0.5, 1], [0, 1, 0],
-        #               [1, 1, 0], [1, 0.65, 0], [1, 0, 0], [0.55, 0, 0]]
-        dose_color = [[0.55, 0, 0], [0, 0, 1], [0.55, 0, 1], [0, 0.5, 1], [0, 1, 0], [1, 0, 0]]
-        dose_level = [0.3, 0.5, 0.7, 0.9, 1.0, 1.1]
-        dose_prescription = my_plan.clinical_criteria.clinical_criteria_dict['pres_per_fraction_gy'] * \
-                            my_plan.clinical_criteria.clinical_criteria_dict['num_of_fractions']
-        dose_value = [item * dose_prescription for item in dose_level]
-        dose_name = []
-        for item in range(0, len(dose_level)):
-            dose_name.append(str(round(dose_level[item] * 100, 2)) + ' % / ' +
-                             str(round(dose_value[item], 3)) + ' ' + 'Gy')
-        dose_storage_legend = {'dose_1d color': dose_color, 'dose_1d level': dose_level, 'dose_1d value': dose_value,
-                               'dose_1d name': dose_name}
-        return dose_storage_legend
-
-    @staticmethod
     def view_in_slicer(my_plan: Plan, slicer_path: str = None, data_dir: str = None) -> None:
         """
 
         :param my_plan: object of class Plan
         :param slicer_path: slicer executable path on your local machine
         :param data_dir: the folder path where data located, defaults to None.
                 If path = None, then it assumes the data is in sub-folder named data in the current directory
@@ -464,19 +406,77 @@
         :param dose_name: Default to 'dose'. name of the dose node in 3D slicer
         :param struct_set_name: name of the rtstruct
         :param show_structs: default to True. If false, will not create struct_name node
         :param show_dose: default to True. If false, will not create dose node
         :param show_ct:default to True. If false, will not create ct node
         :return: visualize in slicer jupyter
         """
-        view_in_slicer_jupyter.view_in_slicer_jupyter(my_plan, dose_1d=dose_1d, sol=sol, ct_name=ct_name,
-                                                      dose_name=dose_name,
-                                                      struct_set_name=struct_set_name, show_ct=show_ct,
-                                                      show_dose=show_dose,
-                                                      show_structs=show_structs)
+        view_in_slicer_jupyter(my_plan, dose_1d=dose_1d, sol=sol, ct_name=ct_name,
+                               dose_name=dose_name,
+                               struct_set_name=struct_set_name, show_ct=show_ct,
+                               show_dose=show_dose,
+                               show_structs=show_structs)
+
+    @staticmethod
+    def plot_binary_mask_points(my_plan, structure: str, show: bool = True, color: List[str] = None):
+        fig = plt.figure()
+        ax = fig.add_subplot(111, projection='3d')
+        ind = my_plan.structures.structures_dict['name'].index(structure)
+        mask_3d = my_plan.structures.structures_dict['structure_mask_3d'][ind]
+        pos = np.where(mask_3d == 1)
+        if color is None:
+            color = Visualization.get_colors()
+        ax.scatter(pos[0], pos[1], pos[2], c=color)
+        if show:
+            plt.show()
+
+    @staticmethod
+    def get_colors():
+        """
+
+        :return: return list of 20 colors
+        """
+        colors = ['#ffe119', '#4363d8', '#f58231', '#911eb4',
+                  '#46f0f0', '#f032e6', '#bcf60c', '#fabebe', '#008080', '#e6beff',
+                  '#9a6324', '#fffac8', '#800000', '#aaffc3', '#808000', '#ffd8b1',
+                  '#000075', '#808080', '#ffffff', '#000000', '#e6194b', '#3cb44b']
+        return colors
+
+    @staticmethod
+    def surface_plot(matrix: np.ndarray, **kwargs):
+        # acquire the cartesian coordinate matrices from the matrix
+        # x is cols, y is rows
+        (x, y) = np.meshgrid(np.arange(matrix.shape[0]), np.arange(matrix.shape[1]))
+        fig = plt.figure()
+        ax = fig.add_subplot(111, projection='3d')
+        surf = ax.plot_surface(x, y, np.transpose(matrix), **kwargs)
+        return ax, surf
+
+    @staticmethod
+    def get_cmap_colors(n, name='hsv'):
+        """Returns a function that maps each index in 0, 1, ..., n-1 to a distinct
+        RGB color; the keyword argument name must be a standard mpl colormap name."""
+        return plt.cm.get_cmap(name, n)
+
+    @staticmethod
+    def legend_dose_storage(my_plan: Plan) -> dict:
+        # dose_color = [[0.55, 0, 1], [0, 0, 1], [0, 0.5, 1], [0, 1, 0],
+        #               [1, 1, 0], [1, 0.65, 0], [1, 0, 0], [0.55, 0, 0]]
+        dose_color = [[0.55, 0, 0], [0, 0, 1], [0.55, 0, 1], [0, 0.5, 1], [0, 1, 0], [1, 0, 0]]
+        dose_level = [0.3, 0.5, 0.7, 0.9, 1.0, 1.1]
+        dose_prescription = my_plan.clinical_criteria.clinical_criteria_dict['pres_per_fraction_gy'] * \
+                            my_plan.clinical_criteria.clinical_criteria_dict['num_of_fractions']
+        dose_value = [item * dose_prescription for item in dose_level]
+        dose_name = []
+        for item in range(0, len(dose_level)):
+            dose_name.append(str(round(dose_level[item] * 100, 2)) + ' % / ' +
+                             str(round(dose_value[item], 3)) + ' ' + 'Gy')
+        dose_storage_legend = {'dose_1d color': dose_color, 'dose_1d level': dose_level, 'dose_1d value': dose_value,
+                               'dose_1d name': dose_name}
+        return dose_storage_legend
 
     @staticmethod
     def is_notebook() -> bool:
         try:
             from IPython import get_ipython
             shell = get_ipython().__class__.__name__
             if shell == 'ZMQInteractiveShell':
```

### Comparing `portpy-0.0.3/portpy.egg-info/PKG-INFO` & `portpy-0.0.4/portpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: portpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: First open-source radiation treatment planning system in Python
 Home-page: https://github.com/PortPy-Project/PortPy
 Author: Gourav Jhanwar, Mojtaba Tefagh, Vicki Taasti, Seppo Tuomaala, Saad Nadeem, Masoud Zarepisheh
 Author-email: jhanwarg@mskcc.struct, mtefagh@acm.struct, vicki.taasti@maastro.nl, tuomaals@mskcc.struct, nadeems@mskcc.struct, zarepism@mskcc.struct
 License: Apache License, Version 2.0
 Description: <p align="center">
           <img src="./images/PortPy_logo.jpg" width="50%">
         </p>
         
         # What is PortPy?
         **Note: The package is at its early stages of development (version 0.0.1) and we are now collecting feedback from researchers to further refine the data structure and the main functionality. We are expecting to have a stable version 1.xx around July 2023. We would love to hear your feedback.**
         
         PortPy (**P**lanning and **O**ptimization for **R**adiation **T**herapy) is a community effort to develop the **first opensource python library** to facilitate the development and clinical translation of radiotherapy cancer treatment planning algorithms. PortPy includes:
         1. Research-ready data and code for *benchmarking*, *reproducibility*, and *community-driven* development.
-        2. Interface to an open-source optimization package [CVXPy](https://www.cvxpy.org/) for easy/quick prototyping and out-of-the-box access to commercial/opensource optimization engines (e.g., Mosek, Gorubi, CPLEX, IPOPT).
+        2. Interface to an open-source optimization package [CVXPy](https://www.cvxpy.org/) for easy/quick prototyping and out-of-the-box access to commercial/opensource optimization engines (e.g., Mosek, Gorubi, CPLEX).
         3. Visualization modules to visualize relevant plan information (e.g, dose volume histograms, dose distribution, fluence map).
         4. Evaluation modules to quantify plan quality with respect to established clinical metrics (e.g., RTOG metrics, dose conformality, tumor control probability, normal tissue control probability).
         # Data
-        Data needed for optimization and algorithm development (e.g., a set of beams/beamlets/voxels, dose contribution of each beamlet to each voxel) are provided for a set of pre-specified machine parameters (e.g., beam/collimator/couch angles). We will initially provide these for a set of publicly available datasets from [TCIA](https://www.cancerimagingarchive.net/). We hope to expand our dataset in the future. The data needed for optimization is extracted from the research version of Eclipse<sup>TM</sup> treatment planning system ([Varian Medical Systems](https://www.varian.com/)) using its API. 
+        Data needed for optimization and algorithm development (e.g., a set of beams/beamlets/voxels, dose contribution of each beamlet to each voxel) are provided for a set of pre-specified machine parameters (e.g., beam/collimator/couch angles). We will initially provide these for a set of publicly available datasets from [TCIA](https://www.cancerimagingarchive.net/). We initially start with two lung patients to get feedback and then expand to about 100 patients in version 1.xx (about end of July). We hope to further expand our dataset in the future. The data needed for optimization is extracted from Eclipse<sup>TM</sup>, a FDA-approved commerical treatment planning system ([Varian Medical Systems](https://www.varian.com/)), using its API. 
         
         You can download the sample patient data [here](https://drive.google.com/drive/folders/1nA1oHEhlmh2Hk8an9e0Oi0ye6LRPREit?usp=sharing).
         
         Create a directory named './data' in the current project directory and copy the downloaded file to it, e.g ./data/Lung_Phantom_Patient_1
         
         # Quick Start
         Please see below for understanding the basic functionalities of PortPy. For advance usage of PortPy, we recommend navigating through [examples](https://github.com/PortPy-Project/PortPy/tree/master/examples) folder.
-        1. To understand the most important features of PortPy, we highly recommend to go through notebook [ex_1_introduction.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_1_introduction.ipynb)
-        2. One of the major computational issues while optimizing the plan arise due to large size of influence matrix. We suggest you to follow [ex_2_down_sampling.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_2_downsampling.py) to understand how PortPy can assist in resolving it.
+        1. To understand the most important features of PortPy, we highly recommend going through notebook [ex_1_introduction.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_1_introduction.ipynb)
+        2. One of the major computational issues while optimizing the plan arise due to large size of influence matrix. We suggest you to follow [ex_2_down_sampling.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_2_down_sampling.py) and [ex_4_inf_matrix_sparsification.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_4_inf_matrix_sparsification.py) to understand how PortPy can assist in resolving it. 
         3. You can check out [ex_3_structure_operations.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_3_structure_operations.py) to know how to perform different structure operations (e.g., boolean, margin).
-        4. For algorithm benchmarking, the global optimal solution is provided for non-convex optimization problems resulting from beam angle optimization [ex_6_boo_benchmark.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_boo_benchmark.ipynb) and incorporating DVH constraints [ex_6_dvh_benchmark.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_dvh_benchmark.py) using the mixed-integer programming on down-sampled data.
-        5. In addition to basic visualization capabilities, PortPy provide advanced visualization by integration with 3D Slicer. Please look out notebook [ex_7_Slicer.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_7_Slicer.ipynb)
+        4. For algorithm benchmarking, the global optimal solution is provided for non-convex optimization problems resulting from beam angle optimization [ex_6_boo_benchmark.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_boo_benchmark.ipynb), incorporating DVH constraints [ex_5_dvh_benchmark.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_5_dvh_benchmark.py), and VMAT optimization [ex_8_VMAT.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_8_VMAT.py) using the mixed-integer programming on down-sampled data.
+        5. In addition to basic visualization capabilities, PortPy provide advanced visualization by integration with 3D Slicer. Please check out notebook [ex_7_Slicer.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_7_Slicer.ipynb)
         
         # Installing PortPy
         
         1. Installing using pip
           ```bash
           pip install portpy
           ```
```

### Comparing `portpy-0.0.3/portpy.egg-info/SOURCES.txt` & `portpy-0.0.4/portpy.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 MANIFEST.in
 README.md
 setup.py
-config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json
-config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json
 images/PortPy_logo.jpg
 portpy/__init__.py
 portpy.egg-info/PKG-INFO
 portpy.egg-info/SOURCES.txt
 portpy.egg-info/dependency_links.txt
 portpy.egg-info/requires.txt
 portpy.egg-info/top_level.txt
@@ -21,12 +19,13 @@
 portpy/photon/evaluation.py
 portpy/photon/influence_matrix.py
 portpy/photon/optimization.py
 portpy/photon/plan.py
 portpy/photon/structures.py
 portpy/photon/visualization.py
 portpy/photon/utils/__init__.py
+portpy/photon/utils/convert_dose_rt_dicom_to_portpy.py
 portpy/photon/utils/get_eclipse_fluence.py
 portpy/photon/utils/save_nrrd.py
 portpy/photon/utils/save_or_load_pickle.py
 portpy/photon/utils/slicer_script.py
 portpy/photon/utils/view_in_slicer_jupyter.py
```

### Comparing `portpy-0.0.3/setup.py` & `portpy-0.0.4/setup.py`

 * *Files identical despite different names*

