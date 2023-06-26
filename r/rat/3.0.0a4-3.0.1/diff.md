# Comparing `tmp/rat-3.0.0a4.tar.gz` & `tmp/rat-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rat-3.0.0a4.tar", last modified: Tue May  2 17:36:27 2023, max compression
+gzip compressed data, was "rat-3.0.1.tar", last modified: Mon Jun 26 17:19:25 2023, max compression
```

## Comparing `rat-3.0.0a4.tar` & `rat-3.0.1.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.148266 rat-3.0.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-02 17:36:15.000000 rat-3.0.0a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    43730 2023-05-02 17:36:27.144266 rat-3.0.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-02 17:36:15.000000 rat-3.0.0a4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-02 17:36:15.000000 rat-3.0.0a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:36:27.148266 rat-3.0.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-02 17:36:15.000000 rat-3.0.0a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.132266 rat-3.0.0a4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.136266 rat-3.0.0a4/src/rat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.136266 rat-3.0.0a4/src/rat/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/cli/rat_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/cli/rat_init_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/cli/rat_test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.140266 rat-3.0.0a4/src/rat/core/
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/run_altimetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/run_metsim.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/run_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/run_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/run_sarea.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/run_vic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.140266 rat-3.0.0a4/src/rat/core/sarea/
--rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/sarea/TMS.py
--rw-r--r--   0 runner    (1001) docker     (123)    19904 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/sarea/sarea_cli_l8.py
--rw-r--r--   0 runner    (1001) docker     (123)    20478 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/sarea/sarea_cli_l9.py
--rw-r--r--   0 runner    (1001) docker     (123)    18180 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/sarea/sarea_cli_s2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/core/sarea/sarea_cli_sar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.144266 rat-3.0.0a4/src/rat/data_processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/data_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32463 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/data_processing/altimetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/data_processing/metsim_input_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    28327 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/data_processing/newdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.144266 rat-3.0.0a4/src/rat/ee_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/ee_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/ee_utils/ee_aec_file_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/ee_utils/ee_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/ee_utils/ee_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    40632 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/rat_basin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/run_rat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.144266 rat-3.0.0a4/src/rat/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/convert_to_final_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/files_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/metsim_param_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/route_param_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/run_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/science.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-05-02 17:36:15.000000 rat-3.0.0a4/src/rat/utils/vic_param_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.136266 rat-3.0.0a4/src/rat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    43730 2023-05-02 17:36:27.000000 rat-3.0.0a4/src/rat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-02 17:36:27.000000 rat-3.0.0a4/src/rat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:36:27.000000 rat-3.0.0a4/src/rat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 17:36:27.000000 rat-3.0.0a4/src/rat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:36:27.144266 rat-3.0.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-02 17:36:15.000000 rat-3.0.0a4/tests/test_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:19:25.265086 rat-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-26 17:19:13.000000 rat-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    43728 2023-06-26 17:19:25.261086 rat-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-26 17:19:13.000000 rat-3.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-26 17:19:17.000000 rat-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:19:25.265086 rat-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-26 17:19:17.000000 rat-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:19:25.253086 rat-3.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:19:25.253086 rat-3.0.1/src/rat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:19:25.257086 rat-3.0.1/src/rat/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    20754 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/cli/rat_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/cli/rat_init_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/cli/rat_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/cli/rat_test_verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:19:25.257086 rat-3.0.1/src/rat/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/core/run_altimetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/core/run_metsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12737 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/core/run_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14507 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/core/run_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/core/run_sarea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/core/run_vic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:19:25.257086 rat-3.0.1/src/rat/core/sarea/
+-rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/core/sarea/TMS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19904 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/core/sarea/sarea_cli_l8.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20478 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/core/sarea/sarea_cli_l9.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18180 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/core/sarea/sarea_cli_s2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/core/sarea/sarea_cli_sar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:19:25.257086 rat-3.0.1/src/rat/data_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/data_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32463 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/data_processing/altimetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13032 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/data_processing/metsim_input_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30156 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/data_processing/newdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:19:25.261086 rat-3.0.1/src/rat/ee_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/ee_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/ee_utils/ee_aec_file_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/ee_utils/ee_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/ee_utils/ee_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42918 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/rat_basin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/run_rat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:19:25.261086 rat-3.0.1/src/rat/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/utils/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/utils/convert_to_final_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/utils/files_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/utils/metsim_param_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/utils/route_param_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/utils/run_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/utils/science.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23887 2023-06-26 17:19:13.000000 rat-3.0.1/src/rat/utils/vic_param_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:19:25.253086 rat-3.0.1/src/rat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43728 2023-06-26 17:19:25.000000 rat-3.0.1/src/rat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-26 17:19:25.000000 rat-3.0.1/src/rat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:19:25.000000 rat-3.0.1/src/rat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-26 17:19:25.000000 rat-3.0.1/src/rat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:19:25.261086 rat-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 17:19:13.000000 rat-3.0.1/tests/test_imports.py
```

### Comparing `rat-3.0.0a4/LICENSE` & `rat-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a4/PKG-INFO` & `rat-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rat
-Version: 3.0.0a4
+Version: 3.0.1
 Summary: Resevoir Monitoring using Satellite Remote Sensing
 Author-email: Pritam Das <pdas47@uw.edu>, Sanchit Minocha <msanchit@uw.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -681,15 +681,15 @@
 Project-URL: Bug Tracker, https://github.com/UW-SASWE/RAT/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![Reservoir Assessment Tool](docs/logos/Rat%20Logo_black_360p.png)
+![Reservoir Assessment Tool](docs/logos/Rat_Logo_black_github.png)
 # Reservoir Assessment Tool 3.0
 [![Documentation Status](https://readthedocs.org/projects/rat-satellitedams/badge/?version=latest)](https://rat-satellitedams.readthedocs.io/en/latest/?badge=latest)
 
 The Reservoir Assessment Tool (RAT) uses satellite remote sensing data to monitor water surface area and water level changes in artificial reservoirs. It uses this information, along with topographical information (either derived from satellite data, or in-situ topo maps) to estimate the **Storage Change (∆S)** in the reservoirs. Additionally, RAT models the **Inflow (I)** and the **Evaporation (E)** of each reservoir. Finally, RAT uses the modeled I, and E, and estimated ∆S, to estimate the **Outflow (O)** from reservoirs.
 
 RAT 3.0 makes numerous improvements to the code structure, performance optimizations, added configurations, ability to run RAT for multiple basins, among some introduced features. It also introduces packaging of RAT as a conda package, allowing for quick and easy installation.
```

### Comparing `rat-3.0.0a4/README.md` & `rat-3.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Reservoir Assessment Tool](docs/logos/Rat%20Logo_black_360p.png)
+![Reservoir Assessment Tool](docs/logos/Rat_Logo_black_github.png)
 # Reservoir Assessment Tool 3.0
 [![Documentation Status](https://readthedocs.org/projects/rat-satellitedams/badge/?version=latest)](https://rat-satellitedams.readthedocs.io/en/latest/?badge=latest)
 
 The Reservoir Assessment Tool (RAT) uses satellite remote sensing data to monitor water surface area and water level changes in artificial reservoirs. It uses this information, along with topographical information (either derived from satellite data, or in-situ topo maps) to estimate the **Storage Change (∆S)** in the reservoirs. Additionally, RAT models the **Inflow (I)** and the **Evaporation (E)** of each reservoir. Finally, RAT uses the modeled I, and E, and estimated ∆S, to estimate the **Outflow (O)** from reservoirs.
 
 RAT 3.0 makes numerous improvements to the code structure, performance optimizations, added configurations, ability to run RAT for multiple basins, among some introduced features. It also introduces packaging of RAT as a conda package, allowing for quick and easy installation.
```

### Comparing `rat-3.0.0a4/pyproject.toml` & `rat-3.0.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rat"
-version = "3.0.0.alpha.4"
+version = "3.0.1"
 authors = [
   { name="Pritam Das", email="pdas47@uw.edu" },
   { name="Sanchit Minocha", email="msanchit@uw.edu" },
 ]
 description = "Resevoir Monitoring using Satellite Remote Sensing"
 requires-python = ">=3.6"
 readme = "README.md"
```

### Comparing `rat-3.0.0a4/src/rat/cli/rat_test_config.py` & `rat-3.0.1/src/rat/cli/rat_test_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from datetime import datetime
 
-DOWNLOAD_LINK = {
-    'test_data': "https://www.dropbox.com/s/huen14qwzphya61/test_data.zip?dl=1"
+DOWNLOAD_LINK_DROPBOX = {
+    'test_data': "https://www.dropbox.com/scl/fi/f1pnyz9mo178kweh3agtf/test_data.zip?dl=1&rlkey=qxvsfrhc2li55dh4yj4a03bq2"
+}
+DOWNLOAD_LINK_GOOGLE = {
+    'test_data': "https://drive.google.com/uc?id=1F5Z6f4rX7nBSXXo7XYGK_XC0i5-G6zBF"
 }
 
 PATHS = {
     'GUNNISON' : {
         'GLOBAL': {
             'data_dir': 'data/test_output',
             'basin_shpfile': 'data/test_data/gunnison/gunnison_boundary/gunnison_boundary.shp',
@@ -35,18 +38,14 @@
             'uh': 'params/routing/uh.txt'
         },
 
         'GEE': {
             'reservoir_vector_file': 'data/test_data/gunnison/gunnison_reservoirs/gunnison_reservoirs_named.geojson',
         },
 
-        'ALTIMETER': {
-            'altimeter_tracks': 'global_data/global_altimetry/j3_tracks.geojson',
-            'geoid_grid': 'global_data/global_altimetry/geoidegm2008grid.mat'
-        },
     },
     'NUECES':{
         'GLOBAL': {
             'data_dir': 'data/test_output',
             'basin_shpfile': 'data/test_data/Nueces/basin_shapefile/Nueces_polygon.json',
         },
 
@@ -73,19 +72,15 @@
             'flow_direction_file': 'data/test_data/Nueces/fl/fl.asc',
             'uh': 'params/routing/uh.txt'
         },
 
         'GEE': {
             'reservoir_vector_file': 'data/test_data/Nueces/reservoirs/basin_reservoirs.shp',
         },
-
-        'ALTIMETER': {
-            'altimeter_tracks': 'global_data/global_altimetry/j3_tracks.geojson',
-            'geoid_grid': 'global_data/global_altimetry/geoidegm2008grid.mat'
-        },
+        
         }
 }
 
 PARAMS = {
     'GUNNISON':{
         'GLOBAL': {
             'steps':[1,2,3,4,5,6,7,8,9,10,12,13,14],
@@ -144,8 +139,19 @@
                                     'area_column'     : 'AREA_SKM'} 
         },
 
         'ROUTING': {
             'station_global_data': False
         }
     }
-}
+}
+
+TEST_PATHS = {
+    'GUNNISON':{
+        'expected_outputs': 'data/test_data/gunnison/expected_outputs',
+        'rat_produced_outputs': 'data/test_output/colorado/basins/gunnison/final_outputs'
+    },
+    'NUECES':{
+        'expected_outputs': 'data/test_data/Nueces/expected_outputs',
+        'rat_produced_outputs': 'data/test_output/Texas/basins/Nueces/final_outputs'
+    }
+}
```

### Comparing `rat-3.0.0a4/src/rat/core/run_altimetry.py` & `rat-3.0.1/src/rat/core/run_altimetry.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a4/src/rat/core/run_metsim.py` & `rat-3.0.1/src/rat/core/run_metsim.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a4/src/rat/core/run_postprocessing.py` & `rat-3.0.1/src/rat/core/run_postprocessing.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 import geopandas as gpd
 import warnings
 import datetime
 
 warnings.filterwarnings("ignore")
 
 from logging import getLogger
-from rat.utils.logging import LOG_NAME, NOTIFICATION
+from rat.utils.logging import LOG_NAME,LOG_LEVEL1_NAME,NOTIFICATION
 from rat.utils.science import penman
 
 log = getLogger(f"{LOG_NAME}.{__name__}")
+log_level1 = getLogger(f"{LOG_LEVEL1_NAME}.{__name__}")
 
 
 def calc_dels(aecpath, sareapath, savepath):
     aec = pd.read_csv(aecpath)
     df = pd.read_csv(sareapath, parse_dates=['date'])
 
     df = df.drop_duplicates('date')
@@ -94,17 +95,17 @@
 
         P = forcings.sel(lat=centroid.y, lon=centroid.x, method='nearest')
         P = P.to_dataframe().reset_index().set_index('time')['air_pressure'].resample('1D').mean()[1:]
         P.head()
 
     else:
         # print(f"[!] {len(points_within)} Grid cells inside reservoir found, averaging their values")
-        data = reqvars.sel(lat=points_within.y, lon=points_within.x, method='nearest').to_dataframe().reset_index().groupby('time').mean()[1:]
+        data = reqvars.sel(lat=np.array(points_within.y), lon=np.array(points_within.x), method='nearest').to_dataframe().reset_index().groupby('time').mean()[1:]
 
-        P = forcings.sel(lat=points_within.y, lon=points_within.x, method='nearest').resample({'time':'1D'}).mean().to_dataframe().groupby('time').mean()[1:]
+        P = forcings.sel(lat=np.array(points_within.y), lon=np.array(points_within.x), method='nearest').resample({'time':'1D'}).mean().to_dataframe().groupby('time').mean()[1:]
 
     data['area'] = sarea_interpolated['area']
     data['P'] = P
     data = data.dropna()
     if (data.empty):
         print('After removal of NAN values, no data left to calculate evaporation.')
         return None
@@ -125,25 +126,25 @@
             data[['time', 'penman_E']].rename({'penman_E': 'OUT_EVAP'}, axis=1).to_csv(savepath, index=False)
 
 
 def calc_outflow(inflowpath, dspath, epath, area, savepath):
     if os.path.isfile(inflowpath):
         inflow = pd.read_csv(inflowpath, parse_dates=["date"])
     else:
-        print('Inflow file does not exist and Outflow cannot be calculated.')
+        raise Exception('Inflow file does not exist. Outflow cannot be calculated.')
     if os.path.isfile(epath):
         E = pd.read_csv(epath, parse_dates=['time'])
     else:
-        print('Evaporation file does not exist and Outflow cannot be calculated.')
+        raise Exception('Evaporation file does not exist. Outflow cannot be calculated.')
 
     if isinstance(dspath, str):
         if os.path.isfile(dspath):
             df = pd.read_csv(dspath, parse_dates=['date'])
         else:
-            print('Storage Change file does not exist and Outflow cannot be calculated.')
+            raise Exception('Storage Change file does not exist. Outflow cannot be calculated.')
     else:
         df = dspath
     
     inflow = inflow[inflow['date']>=df['date'].iloc[0]]
     inflow = inflow[inflow['date']<=df['date'].iloc[-1]]
     inflow = inflow.set_index('date')
 
@@ -184,42 +185,48 @@
     EVAP_STATUS = 0
     DELS_STATUS = 0
     OUTFLOW_STATUS = 0
 
     # SArea
     sarea_raw_dir = os.path.join(basin_data_dir,'gee', "gee_sarea_tmsos")
 
+    ## No of failed files (no_failed_files) is tracked and used to print a warning message in log level 1 file.
     # DelS
     if(gee_status):
         log.debug("Calculating ∆S")
+        no_failed_files = 0
         aec_dir = aec_dir_path
 
         for reservoir_no,reservoir in reservoirs.iterrows():
             try:
                 # Reading reservoir information
                 reservoir_name = str(reservoir[reservoir_shpfile_column_dict['unique_identifier']])
                 sarea_path = os.path.join(sarea_raw_dir, reservoir_name + ".csv")
                 savepath = os.path.join(dels_savedir, reservoir_name + ".csv")
                 aecpath = os.path.join(aec_dir, reservoir_name + ".csv")
 
                 if os.path.isfile(sarea_path):
                     log.debug(f"Calculating ∆S for {reservoir_name}, saving at: {savepath}")
                     calc_dels(aecpath, sarea_path, savepath)
                 else:
-                    log.debug(f"{sarea_path} not found; skipping ∆S calculation")
+                    raise Exception("Surface area file not found; skipping ∆S calculation")
             except:
                 log.exception(f"∆S for {reservoir_name} could not be calculated.")
+                no_failed_files += 1 
         DELS_STATUS=1
+        if no_failed_files:
+            log_level1.warning(f"∆S was not calculated for {no_failed_files} reservoir(s). Please check Level-2 log file for more details.")
     else:
         log.debug("Cannot Calculate ∆S because GEE Run Failed.")
         
 
     # Evaporation
     if(vic_status and gee_status):
         log.debug("Retrieving Evaporation")
+        no_failed_files = 0
         if(use_rout_state):
             vic_results_path = rout_init_state_save_file
         else:
             vic_results_path = os.path.join(basin_data_dir,'vic', "vic_outputs/nc_fluxes."+start_date_str+".nc")
         forcings_path = os.path.join(basin_data_dir,'vic', "vic_inputs/*.nc")
 
         for reservoir_no,reservoir in reservoirs.iterrows():
@@ -230,45 +237,52 @@
                 e_path = os.path.join(evap_datadir, reservoir_name + ".csv")
                 
                 if os.path.isfile(sarea_path):
                     log.debug(f"Calculating Evaporation for {reservoir_name}")
                     # calc_E(e_path, respath, vic_results_path)
                     calc_E(reservoir, start_date_str_evap, end_date_str, forcings_path, vic_results_path, sarea_path, e_path)
                 else:
-                    log.debug(f"{sarea_path} not found; skipping evaporation calculation")
+                    raise Exception("Surface area file not found; skipping evaporation calculation")          
             except:
                 log.exception(f"Evaporation for {reservoir_name} could not be calculated.")
+                no_failed_files +=1
         EVAP_STATUS = 1
+        if no_failed_files:
+            log_level1.warning(f"Evapotration was not calculated for {no_failed_files} reservoir(s). Please check Level-2 log file for more details.")
     elif((not vic_status) and (not gee_status)):
         log.debug("Cannot Retrieve Evaporation because both VIC and GEE Run Failed.")
     elif(vic_status):
         log.debug("Cannot Retrieve Evaporation because VIC Run Failed.")
     else:
         log.debug("Cannot Retrieve Evaporation because GEE Run Failed.")
 
     # Outflow
     if((routing_status) and (EVAP_STATUS) and (DELS_STATUS)):
         log.debug("Calculating Outflow")
-        inflow_dir = os.path.join(basin_data_dir,'ro', "rout_inflow")
+        no_failed_files = 0
+        inflow_dir = os.path.join(basin_data_dir, "rat_outputs", "inflow")
 
         for reservoir_no,reservoir in reservoirs.iterrows():
             try:
                 # Reading reservoir information
                 reservoir_name = str(reservoir[reservoir_shpfile_column_dict['unique_identifier']])
                 deltaS = os.path.join(dels_savedir, reservoir_name + ".csv")
-                inflowpath = os.path.join(inflow_dir, reservoir_name[:5] + ".csv")  ## Routing model keeps only first 5 letters of the reservoir name as file name
+                inflowpath = os.path.join(inflow_dir, reservoir_name + ".csv")
                 epath = os.path.join(evap_datadir, reservoir_name + ".csv")
                 a = float(reservoir[reservoir_shpfile_column_dict['area_column']])
 
                 savepath = os.path.join(outflow_savedir, reservoir_name + ".csv")
                 log.debug(f"Calculating Outflow for {reservoir_name} saving at: {savepath}")
                 calc_outflow(inflowpath, deltaS, epath, a, savepath)
             except:
                 log.exception(f"Outflow for {reservoir_name} could not be calculated")
+                no_failed_files+=1
         OUTFLOW_STATUS = 1
+        if no_failed_files:
+            log_level1.warning(f"Outflow was not calculated for {no_failed_files} reservoir(s). Please check Level-2 log file for more details.")
     else:
         log.debug("Cannot Calculate Outflow because either evaporation, ∆S or Inflow is missing.")
     
     return (DELS_STATUS, EVAP_STATUS, OUTFLOW_STATUS)
 def main():
     pass
```

### Comparing `rat-3.0.0a4/src/rat/core/run_sarea.py` & `rat-3.0.1/src/rat/core/run_sarea.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 import os
 import geopandas as gpd
 
 from logging import getLogger
-from rat.utils.logging import LOG_NAME, NOTIFICATION
+from rat.utils.logging import LOG_NAME, NOTIFICATION, LOG_LEVEL1_NAME
 
 from rat.core.sarea.sarea_cli_s2 import sarea_s2
 from rat.core.sarea.sarea_cli_l8 import sarea_l8
 from rat.core.sarea.sarea_cli_l9 import sarea_l9
 from rat.core.sarea.sarea_cli_sar import sarea_s1
 from rat.core.sarea.TMS import TMS
 
 log = getLogger(f"{LOG_NAME}.{__name__}")
+log_level1 = getLogger(f"{LOG_LEVEL1_NAME}.{__name__}")
 
 
 def run_sarea(start_date, end_date, datadir, reservoirs_shpfile, shpfile_column_dict):
     reservoirs_polygon = gpd.read_file(reservoirs_shpfile)
+    no_failed_files = 0
     
     for reservoir_no,reservoir in reservoirs_polygon.iterrows():
-        # Reading reservoir information
-        reservoir_name = str(reservoir[shpfile_column_dict['unique_identifier']])
-        reservoir_area = float(reservoir[shpfile_column_dict['area_column']])
-        reservoir_polygon = reservoir.geometry
-        run_sarea_for_res(reservoir_name, reservoir_area, reservoir_polygon, start_date, end_date, datadir)
-
-
+        try:
+            # Reading reservoir information
+            reservoir_name = str(reservoir[shpfile_column_dict['unique_identifier']]).replace(" ","_")
+            reservoir_area = float(reservoir[shpfile_column_dict['area_column']])
+            reservoir_polygon = reservoir.geometry
+            log.info(f"Calculating surface area for {reservoir_name}.")
+            run_sarea_for_res(reservoir_name, reservoir_area, reservoir_polygon, start_date, end_date, datadir)
+            log.info(f"Calculated surface area for {reservoir_name} successfully.")
+        except:
+            log.exception(f"Surface area calculation failed for {reservoir_name}.")
+            no_failed_files += 1
+    if no_failed_files:
+        log_level1.warning(f"Surface area was not calculated for {no_failed_files} reservoirs.")
+        
 def run_sarea_for_res(reservoir_name, reservoir_area, reservoir_polygon, start_date, end_date, datadir):
 
     # Obtain surface areas
     # Sentinel-2
     log.debug(f"Reservoir: {reservoir_name}; Downloading Sentinel-2 data from {start_date} to {end_date}")
     sarea_s2(reservoir_name, reservoir_polygon, start_date, end_date, os.path.join(datadir, 's2'))
     s2_dfpath = os.path.join(datadir, 's2', reservoir_name+'.csv')
```

### Comparing `rat-3.0.0a4/src/rat/core/run_vic.py` & `rat-3.0.1/src/rat/core/run_vic.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 import time
 import math
 import datetime
 from pathlib import Path
 from functools import partial
 
 from logging import getLogger
-from rat.utils.logging import LOG_NAME, NOTIFICATION
+from rat.utils.logging import LOG_NAME, LOG_LEVEL, NOTIFICATION
 from rat.utils.utils import create_directory
 from rat.utils.run_command import run_command
 from rat.utils.vic_param_reader import VICParameterFile
 
 log = getLogger(LOG_NAME)
-
+log.setLevel(LOG_LEVEL)
 
 class VICRunner():
     def __init__(self, vic_env, param_file, vic_result_file, rout_input_dir, conda_hook = None) -> None:
         self.vic_env = vic_env
         self.param_file = param_file
         self.vic_result = vic_result_file
         self.rout_input = rout_input_dir
```

### Comparing `rat-3.0.0a4/src/rat/core/sarea/TMS.py` & `rat-3.0.1/src/rat/core/sarea/TMS.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a4/src/rat/core/sarea/sarea_cli_l8.py` & `rat-3.0.1/src/rat/core/sarea/sarea_cli_l8.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a4/src/rat/core/sarea/sarea_cli_l9.py` & `rat-3.0.1/src/rat/core/sarea/sarea_cli_l9.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a4/src/rat/core/sarea/sarea_cli_s2.py` & `rat-3.0.1/src/rat/core/sarea/sarea_cli_s2.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a4/src/rat/core/sarea/sarea_cli_sar.py` & `rat-3.0.1/src/rat/core/sarea/sarea_cli_sar.py`

 * *Files 15% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 def detectWaterSAR(d, ref_image):
     d = ee.Date(d)
     s1_subset = s1.filterDate(d, d.advance(REVISIT_TIME, 'days')) \
         .filterBounds(ROI) \
         .filter(ee.Filter.listContains('transmitterReceiverPolarisation', 'VV')) \
         .filter(ee.Filter.eq('instrumentMode', 'IW'))
-
+        
     vv = s1_subset.map(mask_by_angle)
     vv = vv.map(focal_median);
     vv_median = vv.select("Smooth").median();
     
     def in_case_we_have_obs():
         clas = vv_median.lt(-13);
         mask = vv_median.gt(-32);
@@ -73,43 +73,62 @@
         in_case_we_have_obs()
     )
     
     return res
 
 # client side code
 def ee_get_data(ee_Date_Start, ee_Date_End):
+    date_start_str = ee_Date_Start
+    date_end_str = ee_Date_End
     ee_Date_Start, ee_Date_End = ee.Date(ee_Date_Start), ee.Date(ee_Date_End)
     S1 = s1.filterDate(ee_Date_Start, ee_Date_End) \
             .filterBounds(ROI) \
             .filter(ee.Filter.listContains('transmitterReceiverPolarisation', 'VV')) \
             .filter(ee.Filter.eq('instrumentMode', 'IW'))
     
-    ref_image = S1.first()
-    first_date = getfirstobs(S1)
+     ## Checking if time interval is small then the image collection should not be empty in GEE
+    if (days_between(date_start_str,date_end_str) < 30):     # less than a month difference
+        number_of_images = S1.size().getInfo()
+    else:
+        number_of_images = 1     # more than a month difference simply run, so no need to calculate number_of_images
 
-    n_days = ee_Date_End.difference(ee_Date_Start, 'day').round()
-    dates = ee.List.sequence(0, n_days, REVISIT_TIME)
-    dates = dates.map(lambda n: first_date.advance(n, 'day'))
+    if number_of_images:
+        ref_image = S1.first()
+        first_date = getfirstobs(S1)
+
+        n_days = ee_Date_End.difference(ee_Date_Start, 'day').round()
+        dates = ee.List.sequence(0, n_days, REVISIT_TIME)
+        dates = dates.map(lambda n: first_date.advance(n, 'day'))
 
-    classified_water_sar = ee.ImageCollection(dates.map(lambda d: detectWaterSAR(d, ref_image)))
-    classified_water_sar = classified_water_sar.map(calcWaterPix)
+        classified_water_sar = ee.ImageCollection(dates.map(lambda d: detectWaterSAR(d, ref_image)))
+        classified_water_sar = classified_water_sar.map(calcWaterPix)
 
-    wc = ee.Array(classified_water_sar.aggregate_array('water_pixels')).multiply(0.0001).getInfo() # area in sq. km
-    d = classified_water_sar.aggregate_array('system:time_start').getInfo() # convert from miliseconds to seconds from epoch
-    
-    df = pd.DataFrame({
-        'time': d,  # https://stackoverflow.com/a/15056365
-        'sarea': wc
-    })
-    df['time'] = df['time'].apply(lambda t: np.datetime64(t, 'ms'))
-    
-    return df
+        # print('size line 103:',classified_water_sar.size().getInfo())
+        # print('size line 104:',ee.Array(classified_water_sar.aggregate_array('water_pixels')).multiply(0.0001).size().getInfo())
+
+        wc = ee.Array(classified_water_sar.aggregate_array('water_pixels')).multiply(0.0001).getInfo() # area in sq. km
+        d = classified_water_sar.aggregate_array('system:time_start').getInfo() # convert from miliseconds to seconds from epoch
+        
+        df = pd.DataFrame({
+            'time': d,  # https://stackoverflow.com/a/15056365
+            'sarea': wc
+        })
+        df['time'] = df['time'].apply(lambda t: np.datetime64(t, 'ms'))
+        
+        return df
+    else:
+        df = pd.DataFrame({
+            'time': [],  # https://stackoverflow.com/a/15056365
+            'sarea': []
+        })
+        print('No image observed. Returning empty dataframe.')
+        return df
 
-def retrieve_sar(start_date, end_date, res='ys'):
-    date_ranges = list((pd.date_range(start_date, end_date, freq=res).union([pd.to_datetime(start_date), pd.to_datetime(end_date)])).strftime("%Y-%m-%d").tolist()) 
+def retrieve_sar(start_date, end_date, res='ys'): #ys-year-start frequency
+    date_ranges = list((pd.date_range(start_date, end_date, freq=res).union([pd.to_datetime(start_date), pd.to_datetime(end_date)])).strftime("%Y-%m-%d").tolist()) #ys-year-start frequency
     print(date_ranges)
     dfs = []
     # for begin, end in zip(date_ranges[:-1], date_ranges.shift(1)[:-1]):
     for begin, end in zip(date_ranges[:-1], date_ranges[1:]):
         # begin_str, end_str = begin.strftime('%Y-%m-%d'), end.strftime('%Y-%m-%d')
         print(f"Processing: {begin} - {end} ")
         dfs.append(ee_get_data(begin, end))
@@ -153,15 +172,15 @@
             print(f"No. of days passed since: {days_passed}")
             if days_passed < TEMPORAL_RESOLUTION:
                 print(f"No new observation expected. Quitting early")
                 return savepath
         else:
             to_combine = []
 
-        results = retrieve_sar(start_date, end_date, res='6MS')
+        results = retrieve_sar(start_date, end_date, res='6MS') #MS-month start frequency
         to_combine.append(results)
         data = pd.concat(to_combine).drop_duplicates().sort_values("time")
         
         if not os.path.isdir(datadir):
             os.makedirs(datadir)
         data.to_csv(savepath, index=False)
```

### Comparing `rat-3.0.0a4/src/rat/data_processing/altimetry.py` & `rat-3.0.1/src/rat/data_processing/altimetry.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a4/src/rat/data_processing/metsim_input_processing.py` & `rat-3.0.1/src/rat/data_processing/metsim_input_processing.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 from logging import getLogger
 import numpy as np
 import rasterio as rio
 import numpy as np
 import xarray as xr
 import os
 import pandas as pd
+import shutil
 
-from rat.utils.logging import LOG_NAME, NOTIFICATION
+from rat.utils.logging import LOG_NAME, LOG_LEVEL, NOTIFICATION
 
 log = getLogger(LOG_NAME)
+log.setLevel(LOG_LEVEL)
 
 class CombinedNC:
-    def __init__(self, start, end, datadir, basingridpath, outputdir, use_previous):
+    def __init__(self, start, end, datadir, basingridpath, outputdir, use_previous, climatological_data=None, z_lim=3):
         """
         Parameters:
             start: Start date in YYYY-MM-DD format
             :
             :
             datadir: Directory path of ascii format files
         """
@@ -41,15 +43,76 @@
         self.tmaxes = np.zeros((self._total_days+1, self._rast.height, self._rast.width))
         self.tmins = np.zeros((self._total_days+1, self._rast.height, self._rast.width))
         self.winds = np.zeros((self._total_days+1, self._rast.height, self._rast.width))
         self.dates = pd.date_range(start, end)
 
         self._read()
         self._write()
-
+        # If climatological data is passed, then run the climatological data correction
+        if climatological_data:
+            self._climatological_data = climatological_data
+            self._z_lim = z_lim
+            log.debug(f"Running climatological corection of satellite precipitation")
+            self.satellite_precip_correction()
+
+    def satellite_precip_correction(self):
+        # UPDATE (2023-06-02): Seems like this function isn't able to filter out some very high precipitation values (Jan 6, Jan 7 2022).
+        # from https://github.com/pritamd47/2022_05_04-extreme_precip/blob/1baa1319513abbecfb89f7a7269a1214b50cdca0/notebooks/Extreme-Precip.ipynb
+        daily_precip = xr.open_dataset(self._climatological_data)
+        log_precip = daily_precip.copy()
+        # Take the natural log to convert to normal from log-normal distribution
+        log_precip['tp'] = np.log(log_precip['tp'], where=log_precip['tp']>0)
+
+        weekly_log_precip_mean = log_precip.groupby(log_precip['time'].dt.isocalendar().week).mean()
+        weekly_log_precip_std = log_precip.groupby(log_precip['time'].dt.isocalendar().week).std()
+
+        forcings = xr.open_dataset(self._outputpath)
+        forcings_precip = forcings[['precip']]
+
+        log_forcings_precip = forcings_precip.copy()
+        log_forcings_precip['precip'] = np.log(forcings_precip['precip'], where=forcings_precip['precip']>0)
+
+        # Align both the datasets, so that the final z-scores, means and std devs can be calculated and compared easily.
+        weekly_log_precip_mean_sampled = weekly_log_precip_mean.sel(longitude=log_forcings_precip.lon, latitude=log_forcings_precip.lat, method='nearest')
+        weekly_log_precip_std_sampled = weekly_log_precip_std.sel(longitude=log_forcings_precip.lon, latitude=log_forcings_precip.lat, method='nearest')
+
+        log_forcings_precip['weekly_mean_precip'] = weekly_log_precip_mean_sampled['tp']
+        log_forcings_precip['weekly_std_precip'] = weekly_log_precip_std_sampled['tp']
+
+        # build daily clim precip
+        times = []
+        clim_precip_mean = []
+        clim_precip_std = []
+
+        for t in log_forcings_precip.time:
+            time = pd.to_datetime(t.values)
+            times.append(time)
+            # clim_precip_std.append(log_forcings_precip['weekly_std_precip'].sel(week=time.weekofyear))
+            clim_precip_mean.append(log_forcings_precip['weekly_mean_precip'].sel(week=time.weekofyear).values)
+            clim_precip_std.append(log_forcings_precip['weekly_std_precip'].sel(week=time.weekofyear).values)
+
+        mean = xr.DataArray(np.array(clim_precip_mean), coords=({'time': times, 'lon': log_forcings_precip.lon, 'lat': log_forcings_precip.lat}), dims=["time", "lat", "lon"])
+        std = xr.DataArray(np.array(clim_precip_std), coords=({'time': times, 'lon': log_forcings_precip.lon, 'lat': log_forcings_precip.lat}), dims=["time", "lat", "lon"])
+
+        log_forcings_precip['climatological_precip_mean'] = mean
+        log_forcings_precip['climatological_precip_std'] = std
+
+        # calculate z-scores
+        z_scores = (log_forcings_precip['precip'] - log_forcings_precip['climatological_precip_mean'])/log_forcings_precip['climatological_precip_std']
+
+        high_precip = log_forcings_precip['climatological_precip_mean']
+        precip_extremes_handled = np.where((z_scores.data>self._z_lim)|(z_scores.data<-self._z_lim), high_precip.data, log_forcings_precip['precip'].data)
+        log_forcings_precip['precip'].data = precip_extremes_handled
+        forcings['precip'].data = np.exp(log_forcings_precip['precip'].data)  # Convert to precipitation 
+        forcings.attrs['precip_filtering'] = f">{self._z_lim}sigma | <-{self._z_lim}sigma"
+
+        forcings.to_netcdf(self._outputpath.replace(".nc", "_precip_handled.nc"))
+        forcings.close()
+        daily_precip.close()
+        shutil.move(self._outputpath.replace(".nc", "_precip_handled.nc"), self._outputpath)
 
     def _get_lat_long_1d(self):
         x_res, y_res = self._rast.res
         r_lon_0, r_lat_0 = self._rast.xy(self._rast.height-1, 0)
         longitudes1d = (np.arange(0, self._rast.shape[1])*x_res + r_lon_0).round(5)
         latitudes1d = (np.arange(0, self._rast.shape[0])*y_res + r_lat_0).round(5)
 
@@ -93,24 +156,28 @@
             # self.dates.append(fileDate)
             self.precips[day, :, :] = precipitation
             self.tmaxes[day, :, :] = tmax
             self.tmins[day, :, :] = tmin
             self.winds[day, :, :] = wind
             # pbar.update(1)
 
+    # Imputes missing data by interpolation in the order of dimensions time, lon, lat.
     def _impute_basin_missing_data(self, combined_data):
-        combine_nomiss_data = combined_data.where(combined_data['extent']==1,-9999)
+        combine_nomiss_data = combined_data
         try:
-            combine_nomiss_data = combine_nomiss_data.interpolate_na(dim="time", method="linear", fill_value="extrapolate")
+            #Interpolation using time dimension - if unsuccesful values will still be NaN
+            combine_nomiss_data = combine_nomiss_data.interpolate_na(dim="time", method="linear", fill_value="extrapolate", limit = 30)
+            #Interpolation using lon dimension - if unsuccesful values will still be NaN
+            combine_nomiss_data = combine_nomiss_data.interpolate_na(dim="lon", method="linear", fill_value="extrapolate")
+            #Interpolation using lat dimension - if unsuccesful values will still be NaN
+            combine_nomiss_data = combine_nomiss_data.interpolate_na(dim="lat", method="linear", fill_value="extrapolate", use_coordinate=False)
         except:
-            try:
-                combine_nomiss_data = combine_nomiss_data.interpolate_na(dim="lon", method="linear", fill_value="extrapolate")
-            except:
-                print("No inter or extra polation can be done.")
-        combine_nomiss_data = combine_nomiss_data.where(combine_nomiss_data!=-9999,combined_data)
+            print("No inter or extra polation is possible.")
+        #Restoring original values outside basin extent. This ensures that ocean tiles remain to be NaN/-9999
+        combine_nomiss_data = combine_nomiss_data.where(combined_data['extent']==1,combined_data)
         return combine_nomiss_data
 
     def _write(self):
         precip_da = xr.DataArray(
             data = self.precips,
             coords=[self.dates, np.flip(self._latitudes1d), self._longitudes1d],
             dims=['time', 'lat', 'lon']
```

### Comparing `rat-3.0.0a4/src/rat/data_processing/newdata.py` & `rat-3.0.1/src/rat/data_processing/newdata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import subprocess
 import requests
 from datetime import datetime, timedelta
+import calendar
 import os
 import time
 import shutil
 import tempfile
 import rioxarray as rxr
 import xarray as xr
 from logging import getLogger
 import pandas as pd
 from concurrent.futures import ProcessPoolExecutor, as_completed
 from pathlib import Path
 from dask.distributed import Semaphore
 import dask
+import pandas as pd
 
-from rat.utils.logging import LOG_NAME, NOTIFICATION
+from rat.utils.logging import LOG_NAME, LOG_LEVEL, NOTIFICATION
 from rat.utils.utils import create_directory
 import configparser
 
 log = getLogger(LOG_NAME)
+log.setLevel(LOG_LEVEL)
 
 def run_command(cmd,shell_bool=False):
     """Safely runs a command, and returns the returncode silently in case of no error. Otherwise,
     raises an Exception
     """
     res = subprocess.run(cmd, check=True, capture_output=True,shell=shell_bool)
     
@@ -93,222 +96,232 @@
 
 def download_precip(date, version, outputpath, secrets, interpolate=True):
     """
     Parameters:
         date: datetime object that defines the date for which data is required
         version: which version of data to download - IMERG-LATE or IMERG-EARLY
         outputpath: path where the data should be downloaded
+    Returns:
+        STATUS: Can have the following values:
+            STARTED: Download has started
+            SUCCESS: Download was successful
+            FAILED: Download failed
+            INTERPOLATION_STARTED: Download failed, but interpolation was started
+            INTERPOLATED: Download failed, but interpolation was successful
+            INTERPOLATION_FAILED: Download failed, and interpolation failed
+            NOT_FOUND: Download link not found. Data can be interpolated if `interpolate` is set to True
     =======
     TODO: Add ability to select either CHIRPS or IMERG data
     """
+    STATUS = "STARTED"
     if not(os.path.exists(outputpath)):
         link,version_ = _determine_precip_link_and_version(date)
         response = requests.head(link,auth=(secrets["imerg"]["username"], secrets["imerg"]["pwd"]))
         
         if response.status_code == 200 :  
         # Define the command (different for FINAL, same for EARLY and LATE)
             cmd = _get_cmd_precip_download(outputpath,link,version,secrets)
             log.debug("Downloading precipitation 1-day file: %s (%s)", date.strftime('%Y-%m-%d'), version)
-            return run_command(cmd)
+            exit_code = run_command(cmd)
+            STATUS = "SUCCESS" if exit_code == 0 else "FAILED"
         else:
             if(interpolate):
-                print('Link for 1day file does not exist. Trying to interpolate data using previous and next date.')
+                STATUS="INTERPOLATION_STARTED"
+                log.debug('Link for 1day file does not exist. Trying to interpolate data using previous and next date.')
                 pre_date = date - timedelta(days=1)
                 pre_link, pre_version = _determine_precip_link_and_version(pre_date)
                 pre_response = requests.head(pre_link,auth=(secrets["imerg"]["username"], secrets["imerg"]["pwd"]))
 
                 post_date = date + timedelta(days=1)
                 post_link, post_version = _determine_precip_link_and_version(post_date)
                 post_response = requests.head(post_link,auth=(secrets["imerg"]["username"], secrets["imerg"]["pwd"]))
                 if(pre_response.status_code==200 and post_response.status_code==200):
                     pre_outputpath = ('').join(outputpath.split('.')[:-1])+'_pretemp.tif'
                     pre_cmd = _get_cmd_precip_download(pre_outputpath,pre_link,pre_version,secrets)
                     log.debug("Downloading pre-precipitation 1-day file: %s (%s)", date.strftime('%Y-%m-%d'), version)
-                    run_command(pre_cmd)
+                    exit_code1 = run_command(pre_cmd)
 
                     post_outputpath = ('').join(outputpath.split('.')[:-1])+'_posttemp.tif'
                     post_cmd = _get_cmd_precip_download(post_outputpath,post_link,post_version,secrets)
                     log.debug("Downloading post-precipitation 1-day file: %s (%s)", date.strftime('%Y-%m-%d'), version)
-                    run_command(post_cmd)
+                    exit_code2 = run_command(post_cmd)
+
+                    STATUS = "INTERPOLATED" if (exit_code1 == 0) & (exit_code2 == 0) else "INTERPOLATION_FAILED"
 
                     ## taking mean of pre and post date
                     pre_precip = rxr.open_rasterio(pre_outputpath)
                     post_precip = rxr.open_rasterio(post_outputpath)
                     precip = (pre_precip+post_precip)/2 
                     precip.rio.to_raster(outputpath)
 
                     ## Removing pre and post date files after
                     if os.path.isfile(pre_outputpath):
                         os.remove(pre_outputpath)
                     if os.path.isfile(post_outputpath):
                         os.remove(post_outputpath)
-                    print(f"Precipitation file interpolated using previous and next date : {date.strftime('%Y-%m-%d')}")
+                    log.debug(f"Precipitation file interpolated using previous and next date : {date.strftime('%Y-%m-%d')}")
 
                 elif (pre_response.status_code==200):
                     pre_cmd = _get_cmd_precip_download(outputpath,pre_link,pre_version,secrets)
                     log.debug("Being Replaced by pre-precipitation 1-day file: %s (%s)", date.strftime('%Y-%m-%d'), version)
-                    run_command(pre_cmd)
+                    exit_code = run_command(pre_cmd)
+                    STATUS = "INTERPOLATED" if exit_code == 0 else "INTERPOLATION_FAILED"
                 
                 elif (post_response.status_code==200):
                     post_cmd = _get_cmd_precip_download(outputpath,post_link,post_version,secrets)
                     log.debug("Being Replaced by post-precipitation 1-day file: %s (%s)", date.strftime('%Y-%m-%d'), version)
-                    run_command(post_cmd)
+                    exit_code = run_command(post_cmd)
+                    STATUS = "INTERPOLATED" if exit_code == 0 else "INTERPOLATION_FAILED"
                 else:
-                    print(f"Precipitation file cannnot be interpolated from pre/post date. Skipping downloading: {date.strftime('%Y-%m-%d')}")
+                    log.warning(f"Precipitation file cannnot be interpolated from pre/post date. Skipping downloading: {date.strftime('%Y-%m-%d')}")
+                    STATUS = "INTERPOLATION_FAILED"
             else:
-                print(f"Precipitation download link not found. Skipping downloading: {date.strftime('%Y-%m-%d')}")
+                log.warning(f"Precipitation download link not found. Skipping downloading: {date.strftime('%Y-%m-%d')}")
+                STATUS = "NOT_FOUND"
     else:
-        print(f"Precipitation file already exits: {date.strftime('%Y-%m-%d')}")
+        STATUS = "SKIPPED"
+        log.debug(f"Precipitation file already exits: {date.strftime('%Y-%m-%d')}")
+
+    return STATUS
 
 def download_tmax(year, outputpath):
     """
     Parameters:
         year: year for which data is to be downloaded, as a string
         outputpath: path where the data has to be saved
     """
     ## New data will keep on coming in the year going on i.e. recent year
-    tod = datetime.now()  #today date
-    days_ago_20 = tod - timedelta(days=20)  # date 20 days back
-    today_year = str(tod.year)    # today year 
-    recent_year_20day_ago = str(days_ago_20.year)  # year for 20 days back 
     if (not(os.path.exists(outputpath))):
         cmd = [
             'wget', 
             '-O', 
             f'{outputpath}', 
             f'ftp://ftp.cdc.noaa.gov/Datasets/cpc_global_temp/tmax.{year}.nc'
         ]
         log.debug("Downloading tmax: %s", year)
         return run_command(cmd)
     else:
         log.info("File already exists tmax: %s", year)
-        date_of_file_modification = time.ctime(os.path.getmtime(outputpath))
-        log.info(f"Last modified date:{date_of_file_modification}")
-        if ((year == recent_year_20day_ago) or (year == today_year)):
-            if(datetime.strptime(date_of_file_modification, "%c").date()==tod.date()):
-                log.info("No data since last modified date. No need to download.")
-            else:
-                cmd = [
+        # Checking days in year and in file. 
+        days_in_year=366 if calendar.isleap(int(year)) else 365
+        with xr.open_dataset(outputpath) as nc_data:
+            days_in_file = len(nc_data['time'])
+        if(days_in_file<days_in_year):
+            log.info(f"The file has only data for {days_in_file} days which is less than the days in the year ({days_in_year}).So, updating the tmax file: {year}")
+            cmd = [
                     'wget', 
                     '-O', 
                     f'{outputpath}', 
                     f'ftp://ftp.cdc.noaa.gov/Datasets/cpc_global_temp/tmax.{year}.nc'
                 ]
-                log.debug("Last modified date is not today. So, updating tmax: %s", year)
-                return run_command(cmd)
+            return run_command(cmd)
+        else:
+            log.info(f"The tmax file has complete data for {days_in_file} days of the year. No need to download for {year}.")
                 
 
 def download_tmin(year, outputpath):
     """
     Parameters:
         year: year for which data is to be downloaded, as a string
         outputpath: path where the data has to be saved
     """
     ## New data will keep on coming in the year going on i.e. recent year
-    tod = datetime.now()  #today date
-    days_ago_20 = tod - timedelta(days=20)  # date 20 days back
-    today_year = str(tod.year)    # today year 
-    recent_year_20day_ago = str(days_ago_20.year)  # year for 20 days back 
     if (not(os.path.exists(outputpath))):
         cmd = [
             'wget', 
             '-O', 
             f'{outputpath}', 
             f'ftp://ftp.cdc.noaa.gov/Datasets/cpc_global_temp/tmin.{year}.nc'
         ]
         log.debug("Downloading tmin: %s", year)
         return run_command(cmd)
     else:
         log.info("File already exists tmin: %s", year)
-        date_of_file_modification = time.ctime(os.path.getmtime(outputpath))
-        log.info(f"Last modified date:{date_of_file_modification}")
-        if ((year == recent_year_20day_ago) or (year == today_year)):
-            if(datetime.strptime(date_of_file_modification, "%c").date()==tod.date()):
-                log.info("No data since last modified date. No need to download.")
-            else:
-                cmd = [
+        # Checking days in year and in file. 
+        days_in_year=366 if calendar.isleap(int(year)) else 365
+        with xr.open_dataset(outputpath) as nc_data:
+            days_in_file = len(nc_data['time'])
+        if(days_in_file<days_in_year):
+            log.info(f"The file has only data for {days_in_file} days which is less than the days in the year ({days_in_year}).So, updating the tmin file: {year}")
+            cmd = [
                     'wget', 
                     '-O', 
                     f'{outputpath}', 
                     f'ftp://ftp.cdc.noaa.gov/Datasets/cpc_global_temp/tmin.{year}.nc'
                 ]
-                log.debug("Last modified date is not today. So, updating tmin: %s", year)
-                return run_command(cmd)
+            return run_command(cmd)
+        else:
+            log.info(f"The tmin file has complete data for {days_in_file} days of the year. No need to download for {year}.")
 
 def download_uwnd(year, outputpath):
     """
     Parameters:
         year: year for which data is to be downloaded, as a string
         outputpath: path where the data has to be saved
     """
     ## New data will keep on coming in the year going on i.e. recent year
-    tod = datetime.now()  #today date
-    days_ago_20 = tod - timedelta(days=20)  # date 20 days back
-    today_year = str(tod.year)    # today year 
-    recent_year_20day_ago = str(days_ago_20.year)  # year for 20 days back 
     if (not(os.path.exists(outputpath))):
         cmd = [
             'wget', 
             '-O', 
             f'{outputpath}', 
             f'ftp://ftp2.psl.noaa.gov/Datasets/ncep.reanalysis/surface_gauss/uwnd.10m.gauss.{year}.nc'
         ]
         log.debug("Downloading uwnd: %s", year)
         return run_command(cmd)
     else:
         log.info("File already exists uwnd: %s", year)
-        date_of_file_modification = time.ctime(os.path.getmtime(outputpath))
-        log.info(f"Last modified date:{date_of_file_modification}")
-        if ((year == recent_year_20day_ago) or (year == today_year)):
-            if(datetime.strptime(date_of_file_modification, "%c").date()==tod.date()):
-                log.info("No data since last modified date. No need to download.")
-            else:
-                cmd = [
+        # Checking days in year and in file. 
+        days_in_year=366 if calendar.isleap(int(year)) else 365
+        with xr.open_dataset(outputpath) as nc_data:
+            days_in_file = int(len(nc_data['time'])/4)  # daily 4 times data at 6hr frequency
+        if(days_in_file<days_in_year):
+            log.info(f"The file has only data for {days_in_file} days which is less than the days in the year ({days_in_year}).So, updating the uwnd file: {year}")
+            cmd = [
                     'wget', 
                     '-O', 
                     f'{outputpath}', 
                     f'ftp://ftp2.psl.noaa.gov/Datasets/ncep.reanalysis/surface_gauss/uwnd.10m.gauss.{year}.nc'
                 ]
-                log.debug("Last modified date is not today. So, updating uwnd: %s", year)
-                return run_command(cmd)
+            return run_command(cmd)
+        else:
+            log.info(f"The uwnd file has complete data for {days_in_file} days of the year. No need to download for {year}.")
 
 def download_vwnd(year, outputpath):
     """
     Parameters:
         year: year for which data is to be downloaded, as a string
         outputpath: path where the data has to be saved
     """
     ## New data will keep on coming in the year going on i.e. recent year
-    tod = datetime.now()  #today date
-    days_ago_20 = tod - timedelta(days=20)  # date 20 days back
-    today_year = str(tod.year)    # today year 
-    recent_year_20day_ago = str(days_ago_20.year)  # year for 20 days back 
     if (not(os.path.exists(outputpath))):
         cmd = [
             'wget', 
             '-O', 
             f'{outputpath}', 
             f'ftp://ftp2.psl.noaa.gov/Datasets/ncep.reanalysis/surface_gauss/vwnd.10m.gauss.{year}.nc']
         log.debug("Downloading vwnd: %s", year)
         return run_command(cmd)
     else:
         log.info("File already exists vwnd: %s", year)
-        date_of_file_modification = time.ctime(os.path.getmtime(outputpath))
-        log.info(f"Last modified date:{date_of_file_modification}")
-        if ((year == recent_year_20day_ago) or (year == today_year)):
-            if(datetime.strptime(date_of_file_modification, "%c").date()==tod.date()):
-                log.info("No data since last modified date. No need to download.")
-            else:
-                cmd = [
+        # Checking days in year and in file. 
+        days_in_year=366 if calendar.isleap(int(year)) else 365
+        with xr.open_dataset(outputpath) as nc_data:
+            days_in_file = int(len(nc_data['time'])/4) # daily 4 times data at 6hr frequency
+        if(days_in_file<days_in_year):
+            log.info(f"The file has only data for {days_in_file} days which is less than the days in the year ({days_in_year}).So, updating the vwnd file: {year}")
+            cmd = [
                     'wget', 
                     '-O', 
                     f'{outputpath}', 
-                    f'ftp://ftp2.psl.noaa.gov/Datasets/ncep.reanalysis/surface_gauss/vwnd.10m.gauss.{year}.nc']
-                log.debug("Last modified date is not today. So, updating vwnd: %s", year)
-                return run_command(cmd)
+                    f'ftp://ftp2.psl.noaa.gov/Datasets/ncep.reanalysis/surface_gauss/vwnd.10m.gauss.{year}.nc'
+                ]
+            return run_command(cmd)
+        else:
+            log.info(f"The vwnd file has complete data for {days_in_file} days of the year. No need to download for {year}.")
 
 def download_data(begin, end, datadir, secrets):
     """Downloads the data between dates defined by begin and end
 
     Parameters:
         begin: Data will start downloading from this date, including this date
         end: Data will be downloaded until this date, including this date
@@ -318,29 +331,40 @@
     # Obtain list of dates to be downloaded
     # required_dates = [begin+timedelta(days=n) for n in range((end-begin).days)]
     required_dates = pd.date_range(begin, end)
     required_years = list(set([d.strftime("%Y") for d in required_dates]))
     # Download Precipitation
     log.debug("Downloading Precipitation")
 
+    precip_statuses = {
+        "Date": [],
+        "Status": []
+    }
+
     sem = Semaphore(max_leases=4, name="IMERG-Downloader")
     def download_precip_with_semaphore(date, version, outputpath, secrets, sem):
         with sem:
-            result = download_precip(date, version, outputpath, secrets)
-            return result
+            STATUS = download_precip(date, version, outputpath, secrets)
+            return date, STATUS
     
     futures = []
     for date in required_dates:
         data_version = _determine_precip_version(date)
         outputpath = os.path.join(datadir, "precipitation", f"{date.strftime('%Y-%m-%d')}_IMERG.tif")
-        if not os.path.isfile(outputpath):
-            future = dask.delayed(download_precip_with_semaphore)(date, data_version, outputpath, secrets, sem)
-            futures.append(future)
+        # if not os.path.isfile(outputpath):
+        future = dask.delayed(download_precip_with_semaphore)(date, data_version, outputpath, secrets, sem)
+        futures.append(future)
 
     results = dask.compute(*futures) # downloading precipitation files first
+    precip_statuses["Date"] = [r[0] for r in results]
+    precip_statuses["Status"] = [r[1] for r in results]
+    precip_statuses = pd.DataFrame(precip_statuses)
+    precip_statuses.sort_values(by="Date", inplace=True)
+    log.debug("Precipitation download statuses:\n%s", precip_statuses.to_string(index=False, col_space=25))
+
     futures = []
 
     # Download other forcing data
     log.debug("Downloading TMax, TMin, UWnd, and VWnd")
     for year in required_years:
         futures.append(dask.delayed(download_tmax)(year, os.path.join(datadir, "tmax", year+'.nc')))
         futures.append(dask.delayed(download_tmin)(year, os.path.join(datadir, "tmin", year+'.nc')))
@@ -350,20 +374,24 @@
     results = dask.compute(*futures)
 
 def process_precip(basin_bounds, srcpath, dstpath, secrets=None, temp_datadir=None, itry=0):
     """For any IMERG Precipitation file located at `srcpath` is clipped, scaled and converted to
     ASCII grid file and saved at `dstpath`. All of this is done in a temporarily created directory
     which can be controlled by the `datadir` path
     """
+    src_fn = Path(srcpath)
+    date = pd.to_datetime(src_fn.stem.split('_')[0])
     if temp_datadir is not None and not os.path.isdir(temp_datadir):
-        raise Exception(f"ERROR: {temp_datadir} directory doesn't exist")
+        log.warning(f"ERROR: {temp_datadir} directory doesn't exist")
+        STATUS='FAILED'
+        return date, 'Precipitaion', STATUS
     
     if not(os.path.exists(dstpath)):
         log.debug("Processing Precipitation file: %s", srcpath)
-
+        STATUS = 'STARTED'
         with tempfile.TemporaryDirectory(dir=temp_datadir) as tempdir:
             clipped_temp_file = os.path.join(tempdir, 'clipped.tif')
             cmd = [
                 "gdalwarp",
                 "-dstnodata", 
                 "-9999.0",
                 "-tr",
@@ -378,30 +406,30 @@
                 'GTiff',
                 '-overwrite', 
                 f'{srcpath}',
                 clipped_temp_file
             ]
             try:
                 run_command(cmd)
+                
             except subprocess.CalledProcessError as e:
-                src_fn = Path(srcpath)
-                date = pd.to_datetime(src_fn.stem.split('_')[0])
                 log.error(f"subprocess.CalledProcessError in {date}: ", e)
-                
                 # delete old precipitation file and redownload. retry once
-                if itry <= 1:
+                try:
                     src_fn = Path(srcpath)
                     src_fn.unlink(missing_ok=True)
 
                     version = _determine_precip_version(date)
 
                     download_precip(date, version, srcpath, secrets)
                     run_command(cmd)
-                else:
-                    raise e
+                except:
+                    log.warning('Processing failed. Downloaded file might be corrupted.')
+                    STATUS='FAILED'
+                    return date, 'Precipitaion', STATUS
 
             # Scale down (EARLY)
             scaled_temp_file = os.path.join(tempdir, 'scaled.tif')
             cmd = [
                 "gdal_calc.py", 
                 "-A", 
                 clipped_temp_file, 
@@ -421,33 +449,38 @@
                 scaled_temp_file, 
                 aai_temp_file
             ]
             run_command(cmd)
 
             # Move to destination
             shutil.move(aai_temp_file, dstpath)
+            STATUS = 'SUCCESS'
     else:
-        print(f"Processing Precipitation file exist: {srcpath}")
-
+        STATUS = 'SKIPPED'
+        log.debug(f"Processing Precipitation file exist: {srcpath}")
+    return date, 'Precipitaion', STATUS
 
-def process_nc(basin_bounds,date, srcpath, dstpath, temp_datadir=None, itry=0):
+def process_nc(basin_bounds,date, srcpath, dstpath, temp_datadir=None, var='---'):
     """For TMax, TMin, UWnd and VWnd, the processing steps are same, and can be performed using
     this function.
 
     Parameters:
         date: Datetime object of the date of data
         srcpath: path of the nc file
         dstpath: path where the final ascii file will be saved
         temp_datadir: directory where the temporary data will be stored
     """
     if temp_datadir is not None and not os.path.isdir(temp_datadir):
-        raise Exception(f"ERROR: {temp_datadir} directory doesn't exist")
+        log.warning(f"ERROR: {temp_datadir} directory doesn't exist")
+        STATUS='FAILED'
+        return date, var, STATUS
+
     if not(os.path.exists(dstpath)):
         log.debug("Processing NC file: %s for date %s", srcpath, date.strftime('%Y-%m-%d'))
-
+        STATUS = 'STARTED'
         with tempfile.TemporaryDirectory(dir=temp_datadir) as tempdir:
             # Convert from NC to Tif
             band = date.strftime("%-j")   # required band number is defined by `day of year`
             converted_tif_temp_file = os.path.join(tempdir, "converted.tif")
 
             # NC to tiff format
             cmd = ["gdal_translate", "-of", "Gtiff", "-b", band, srcpath, converted_tif_temp_file]
@@ -500,31 +533,35 @@
             # Convert GeoTiff to AAI
             aai_temp_file = os.path.join(tempdir, "final_aai.tif")
             cmd = ["gdal_translate", "-of", "aaigrid", scaled_temp_file, aai_temp_file]
             run_command(cmd)
 
             # Move file to destination
             shutil.move(aai_temp_file, dstpath)
+            STATUS='SUCCESS' 
     else:
-        print(f"Processing NC file exists: {srcpath} for date {date.strftime('%Y-%m-%d')}")
+        STATUS='SKIPPED'
+        log.debug(f"Processing NC file exists: {srcpath} for date {date.strftime('%Y-%m-%d')}")
+    return date, var, STATUS
 
 def process_data(basin_bounds,raw_datadir, processed_datadir, begin, end, secrets, temp_datadir):
     if not os.path.isdir(temp_datadir):
         os.makedirs(temp_datadir)
 
     #### Process precipitation ####
     log.debug("Processing Precipitation")
     raw_datadir_precip = os.path.join(raw_datadir, "precipitation")
     processed_datadir_precip = os.path.join(processed_datadir, "precipitation")
 
     # with tqdm(os.listdir(raw_datadir_precip)) as pbar:
     ds = pd.date_range(begin, end)
 
     futures = []
-    
+    processed_statuses = []
+
     for srcname in os.listdir(raw_datadir_precip):
         if datetime.strptime(srcname.split(os.sep)[-1].split("_")[0], "%Y-%m-%d") in ds:
             srcpath = os.path.join(raw_datadir_precip, srcname)
             dstpath = os.path.join(processed_datadir_precip, srcname.replace("tif", "asc"))
 
             # pbar.set_description(f"Precipitation: {srcname.split('_')[0]}")
             future = dask.delayed(process_precip)(basin_bounds, srcpath, dstpath, secrets, temp_datadir)
@@ -538,30 +575,28 @@
     raw_datadir_tmax = os.path.join(raw_datadir, "tmax")
     processed_datadir_tmax = os.path.join(processed_datadir, "tmax")
 
     for date in required_dates:
         srcpath = os.path.join(raw_datadir_tmax, date.strftime('%Y')+'.nc')
         dstpath = os.path.join(processed_datadir_tmax, f"{date.strftime('%Y-%m-%d')}_TMAX.asc")
 
-        future = dask.delayed(process_nc)(basin_bounds,date, srcpath, dstpath, temp_datadir)
+        future = dask.delayed(process_nc)(basin_bounds,date, srcpath, dstpath, temp_datadir, "tmax")
         futures.append(future)
-    
+
     #### Process TMin ####
     log.debug("Processing TMIN")
     raw_datadir_tmin = os.path.join(raw_datadir, "tmin")
     processed_datadir_tmin = os.path.join(processed_datadir, "tmin")
 
     for date in required_dates:
         srcpath = os.path.join(raw_datadir_tmin, date.strftime('%Y')+'.nc')
         dstpath = os.path.join(processed_datadir_tmin, f"{date.strftime('%Y-%m-%d')}_TMIN.asc")
 
-        future = dask.delayed(process_nc)(basin_bounds,date, srcpath, dstpath, temp_datadir)
+        future = dask.delayed(process_nc)(basin_bounds,date, srcpath, dstpath, temp_datadir, "tmin")
         futures.append(future)
-    
-    results = dask.compute(*futures)
 
     #### Process UWND ####
     log.debug("Processing UWND")
     raw_datadir_uwnd = os.path.join(raw_datadir, "uwnd")
     daily_datadir_uwnd = os.path.join(raw_datadir, "uwnd_daily")
     processed_datadir_uwnd = os.path.join(processed_datadir, "uwnd")
 
@@ -571,15 +606,15 @@
         xr.open_dataset(uwnd_f).resample(time='1D').mean().to_netcdf(os.path.join(daily_datadir_uwnd, uwnd_f.split(os.sep)[-1]))
         # xr.open_dataset(vwnd_f).resample(time='1D').mean().to_netcdf(os.path.join(vwnd_outdir, vwnd_f.split(os.sep)[-1]))
 
     for date in required_dates:
         srcpath = os.path.join(daily_datadir_uwnd, date.strftime('%Y')+'.nc')
         dstpath = os.path.join(processed_datadir_uwnd, f"{date.strftime('%Y-%m-%d')}_UWND.asc")
 
-        future = dask.delayed(process_nc)(basin_bounds,date, srcpath, dstpath, temp_datadir)
+        future = dask.delayed(process_nc)(basin_bounds,date, srcpath, dstpath, temp_datadir, "uwnd")
         futures.append(future)
 
     #### Process VWND ####
     log.debug("Processing VWND")
     raw_datadir_vwnd = os.path.join(raw_datadir, "vwnd")
     daily_datadir_vwnd = os.path.join(raw_datadir, "vwnd_daily")
     processed_datadir_vwnd = os.path.join(processed_datadir, "vwnd")
@@ -589,18 +624,21 @@
     for vwnd_f in vwnd_files:
         xr.open_dataset(vwnd_f).resample(time='1D').mean().to_netcdf(os.path.join(daily_datadir_vwnd, vwnd_f.split(os.sep)[-1]))
 
     for date in required_dates:
         srcpath = os.path.join(daily_datadir_vwnd, date.strftime('%Y')+'.nc')
         dstpath = os.path.join(processed_datadir_vwnd, f"{date.strftime('%Y-%m-%d')}_VWND.asc")
 
-        future = dask.delayed(process_nc)(basin_bounds,date, srcpath, dstpath, temp_datadir)
+        future = dask.delayed(process_nc)(basin_bounds,date, srcpath, dstpath, temp_datadir, "vwnd")
         futures.append(future)
-    results = dask.compute(*futures)
 
+    processed_statuses = dask.compute(*futures)
+    processed_statuses = pd.DataFrame(processed_statuses, columns=['Date','Variable','Status'])
+    processed_statuses.sort_values(by=["Date","Variable"], inplace=True)
+    log.debug("Files processed statuses:\n%s", processed_statuses.to_string(index=False, col_space=25))
 
 def get_newdata(basin_name,basin_bounds,data_dir, basin_data_dir,startdate, enddate, secrets_file, download=True, process=True):
     raw_datadir = os.path.join(data_dir,"raw",'')
     processed_datadir = os.path.join(basin_data_dir,"pre_processing","processed",'')
     temp_datadir = os.path.join(basin_data_dir,"pre_processing","temp",'')
     
     ####Creating the required directories####
```

### Comparing `rat-3.0.0a4/src/rat/ee_utils/ee_aec_file_creator.py` & `rat-3.0.1/src/rat/ee_utils/ee_aec_file_creator.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,8 +82,9 @@
         areas_list = list(chain(*areas_list))
         areas_list = np.round(areas_list,3)
         ## Preparing dataframe to write down to csv 
         aec_df = pd.DataFrame(data = {'Elevation' :elevs_list, 'CumArea':areas_list})
         aec_df.to_csv(os.path.join(aec_dir_path,reservoir_name+'.csv'),index=False)
         print(f"AEC file created succesfully for {reservoir_name}")
   print("AEC file exists for all reservoirs in this basin")
+  return 1
```

### Comparing `rat-3.0.0a4/src/rat/ee_utils/ee_utils.py` & `rat-3.0.1/src/rat/ee_utils/ee_utils.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a4/src/rat/rat_basin.py` & `rat-3.0.1/src/rat/rat_basin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 from datetime import datetime
 import os
 from logging import getLogger
 import datetime
 import geopandas as gpd
 import numpy as np
 import xarray as xr
+import shutil
+from pathlib import Path
+import warnings
 
 from rat.utils.utils import create_directory
 from rat.utils.logging import init_logger,close_logger,NOTIFICATION
-from rat.utils.files_creator import create_basingridfile, create_basin_domain_nc_file ,create_vic_domain_param_file, create_basin_grid_flow_asc
+from rat.utils.files_creator import create_basingridfile, create_basin_domain_nc_file ,create_vic_domain_param_file, create_basin_grid_flow_asc, create_basin_station_geojson
 from rat.utils.files_creator import create_basin_station_latlon_csv, create_basin_reservoir_shpfile
 from rat.utils.clean import Clean
 
 from rat.data_processing.newdata import get_newdata
 
 from rat.data_processing.metsim_input_processing import CombinedNC,generate_state_and_inputs
 from rat.utils.metsim_param_reader import MSParameterFile
 from rat.core.run_metsim import MetSimRunner
 
 from rat.utils.vic_param_reader import VICParameterFile
 from rat.core.run_vic import VICRunner
 
 from rat.utils.route_param_reader import RouteParameterFile
-from rat.core.run_routing import RoutingRunner
+from rat.core.run_routing import RoutingRunner, generate_inflow, run_routing
 
 from rat.core.run_altimetry import run_altimetry
 
 from rat.core.run_postprocessing import run_postprocessing
 
-from rat.utils.convert_to_final_outputs import convert_sarea, convert_inflow, convert_dels, convert_evaporation, convert_outflow, convert_altimeter
+from rat.utils.convert_to_final_outputs import convert_sarea, convert_inflow, convert_dels, convert_evaporation, convert_outflow, convert_altimeter, copy_aec_files
 
 # Step-(-1): Reading Configuration settings to run RAT
 # Step-0: Creating required directory structure for RAT
 # Step-1: Downloading and Pre-processing of meteorolgical data
 # Step-2: Pre-processing of data and preparation of MetSim Input
 # Step-3: Preparation of MetSim Parameter Files
 # Step-4: Running MetSim & preparation of VIC input
 # Step-5: Preparation of VIC Parameter Files
 # Step-6: Running of VIC and preparation of Routing input
 # Step-7: Preparation of Routing Parameter Files
-# Step-8: Runnning Routing and generating Inflow
+# Step-8: Runnning Routing model
 # Step-9: Preparation of parameter files for Surface Area Calculation
 # Step-10: TMS-OS Surface Area Calculation from GEE 
 # Step-11: Elevation extraction from Altimeter
 # Step-12: Generating Area Elevation Curves for reservoirs
-# Step-13: Calculation of Outflow, Evaporation and Storage change
+# Step-13: Calculation of Inflow, Outflow, Evaporation and Storage change
 # Step-14: Conversion of output data to final format as time series
 
 #TODO: Converting steps to separate modules to make RAT more robust and generalized
 #module-1 step-1,2 data_preparation_vic
 #module-2 step-3to8 inflow_vic
 #module-3 step- NA evaporation
 #module-4 step-10to12 storage_change
@@ -120,22 +123,25 @@
         # Changing start date if running RAT for first time for the particular basin to give VIC and MetSim to have their spin off periods
         if(config['BASIN']['spin_up']):
             user_given_start = config['BASIN']['start']
             config['BASIN']['start'] = user_given_start-datetime.timedelta(days=800)  # Running RAT for extra 800 days before the user-given start date for VIC to give reliable results starting from user-given start date
             data_download_start = config['BASIN']['start']-datetime.timedelta(days=90)    # Downloading 90 days of extra meteorological data for MetSim to prepare it's initial state
             vic_init_state_date = None    # No initial state of VIC is present as running RAT for first time in this basin
             use_state = False            # Routing state file won't be used
+            gee_start_date = user_given_start  # Run gee from the date provided by user and not spin-off start date.
         elif(config['BASIN'].get('vic_init_state_date')):
             data_download_start = config['BASIN']['start']    # Downloading data from the same date as we want to run RAT from
             vic_init_state_date = config['BASIN']['vic_init_state_date'] # Date of which initial state of VIC for the particular basin exists
             use_state = True           # Routing state file will be used
+            gee_start_date = config['BASIN']['start'] # Run gee from the date provided by user.
         else:
             data_download_start = config['BASIN']['start']-datetime.timedelta(days=90)    # Downloading 90 days of extra meteorological data for MetSim to prepare it's initial state
             vic_init_state_date = None    # No initial state of VIC is present as running RAT for first time in this basin
             use_state = False            # Routing state file won't be used
+            gee_start_date = config['BASIN']['start']  # Run gee from the date provided by user.
 
         # Defining logger
         log = init_logger(
             log_dir= log_dir,
             verbose= False,
             # notify= True,
             notify= False,
@@ -156,23 +162,24 @@
         VIC_STATUS = 1
         ROUTING_STATUS = 1
         GEE_STATUS = 1
         ALTIMETER_STATUS = 1
         DELS_STATUS = 0
         EVAP_STATUS = 0
         OUTFLOW_STATUS = 0
+        AEC_STATUS = 0
     except:
         no_errors = -1
         rat_logger.exception("Error in Configuration parameters defined to run RAT.")
         return (no_errors, latest_altimetry_cycle)
     else:
         rat_logger.info("Read Configuration settings to run RAT.")
         ##--------------------- Read and initialised global parameters ----------------------##
 
-    rat_logger.info(f"Running RAT from {config['BASIN']['start'] } to {config['BASIN']['end']}")
+    rat_logger.info(f"Running RAT from {config['BASIN']['start'] } to {config['BASIN']['end']} which might include spin-up.")
 
     ######### Step-0 Mandatory Step
     try:
         rat_logger.info("Creating required directory structure for RAT")
         
         ##--------------------- Defining global paths and variables ----------------------##
 
@@ -207,23 +214,29 @@
         #----------- Paths Necessary for running of VIC  -----------#
 
         #----------- Paths Necessary for running of Routing  -----------#
         # Routing_input files prefix path
         rout_input_path_prefix = os.path.join(rout_input_path,'fluxes_')
         # Creating routing parameter directory
         rout_param_dir = create_directory(os.path.join(basin_data_dir,'ro','pars',''), True)
+        # Creating routing and its inflow directory
+        rout_dir = Path(config['GLOBAL']['data_dir']) / f'{config["BASIN"]["region_name"]}' / 'basins' / f'{config["BASIN"]["basin_name"]}' / 'ro'
+        rout_dir.mkdir(parents=True, exist_ok=True)
+        routing_output_dir = Path(config['GLOBAL']['data_dir']).joinpath(config['BASIN']['region_name'], 'basins', basin_name, 'ro','ou')
+        routing_output_dir.mkdir(parents=True, exist_ok=True)
+        inflow_dst_dir = Path(config['GLOBAL']['data_dir']).joinpath(config['BASIN']['region_name'], 'basins', basin_name, 'rat_outputs', 'inflow')
+        inflow_dst_dir.mkdir(parents=True, exist_ok=True)
         # Defining path and name for basin flow direction file
         basin_flow_dir_file = os.path.join(rout_param_dir,'fl.asc')
         # Defining Basin station latlon file path
         if (config['ROUTING']['station_global_data']):
             basin_station_latlon_file = os.path.join(rout_param_dir,'basin_station_latlon.csv')
         else:
             basin_station_latlon_file = config['ROUTING']['station_latlon_path']
-        # Creating routing inflow directory
-        rout_inflow_dir = create_directory(os.path.join(basin_data_dir,'ro', 'rout_inflow',''), True)
+            basin_station_geojson_file = os.path.join(rout_param_dir,'station.geojson')
         #----------- Paths Necessary for running of Routing  -----------#
 
         #----------- Paths Necessary for running of Surface Area Calculation and Altimetry-----------#
         # Defining routing station file
         if(config['ROUTING PARAMETERS'].get('station_file')):
             basin_station_xy_path = config['ROUTING PARAMETERS'].get('station_file')
         else:
@@ -249,14 +262,15 @@
             aec_dir_path = config['POST_PROCESSING'].get('aec_dir')
         else:
             aec_dir_path = create_directory(os.path.join(basin_data_dir,'post_processing','post_processing_gee_aec',''), True)
         ## Paths for storing post-processed data and in webformat data
         evap_savedir = create_directory(os.path.join(basin_data_dir,'rat_outputs', "Evaporation"), True)
         dels_savedir = create_directory(os.path.join(basin_data_dir,'rat_outputs', "dels"), True)
         outflow_savedir = create_directory(os.path.join(basin_data_dir,'rat_outputs', "rat_outflow"),True)
+        aec_savedir = Path(create_directory(os.path.join(basin_data_dir,'rat_outputs', "aec"),True))
         final_output_path = create_directory(os.path.join(basin_data_dir,'final_outputs',''),True)
         ## End of defining paths for storing post-processed data and webformat data
         #----------- Paths Necessary for running of Post-Processing-----------#
     except:
         no_errors = -1
         rat_logger.exception("Error in creating required directory structure for RAT")
         return (no_errors, latest_altimetry_cycle)
@@ -306,14 +320,15 @@
             CombinedNC(
                 start= data_download_start,
                 end= config['BASIN']['end'],
                 datadir= processed_datadir,
                 basingridpath= basingridfile_path,
                 outputdir= combined_datapath,
                 use_previous= use_state,
+                climatological_data=config['METSIM'].get('historical_precipitation')
             )
             #----------- Process Data End and combined data created -----------#
 
             #------ MetSim Input Data Preparation Begin ------#
             # Prepare data to metsim input format
             ms_state, ms_input_data = generate_state_and_inputs(
                 forcings_startdate= config['BASIN']['start'],
@@ -463,85 +478,77 @@
             ##--------------- Preparation of Routing Parameter Files begin--------------##
             ### Basin Grid Flow Firection File
             # Creating basin grid flow diretion file if not present
             if (config['ROUTING'].get('global_flow_dir_tif_file')):
                 if not os.path.exists(basin_flow_dir_file):
                     create_basin_grid_flow_asc(config['ROUTING']['global_flow_dir_tif_file'], basingridfile_path, basin_flow_dir_file[:-4],
                                                                     config['ROUTING'].get('replace_flow_directions'))
-            ### Basin Station File
+            ### Basin Station CSV File and Geojson File (for front-end purposes)
             if (config['ROUTING']['station_global_data']):
                 if not os.path.exists(basin_station_latlon_file):
                     create_basin_station_latlon_csv(region_name,basin_name, config['ROUTING']['stations_vector_file'], basin_data, 
                                                         config['ROUTING']['stations_vector_file_columns_dict'], basin_station_latlon_file)
+            else:
+                if(config['ROUTING'].get('station_latlon_path')):
+                    create_basin_station_geojson(region_name,basin_name,config['ROUTING']['station_latlon_path'],basin_station_geojson_file)
         except:
             no_errors = no_errors+1
             rat_logger.exception("Error Executing Step-7: Preparation of Routing Parameter Files")
         else:    
             rat_logger.info("Finished Step-7: Preparation of Routing Parameter Files")
             ##--------------- Preparation of Routing Parameter Files end--------------##
 
     ######### Step-8
     if(8 in steps):
         try:
             if(VIC_STATUS):
-                rat_logger.info("Starting Step-8: Runnning Routing and generating Inflow")
+                rat_logger.info("Starting Step-8: Runnning Routing model")
                 ### Extracting routing start date ###
                 if(config['BASIN']['spin_up']):
                     rout_input_state_start_date = config['BASIN']['start']
                 elif(config['BASIN'].get('vic_init_state_date')): 
                     rout_state_data = xr.open_dataset(rout_init_state_save_file).load()
                     rout_input_state_start_date = rout_state_data.time[0].values.astype('datetime64[us]').astype(datetime.datetime)
                     rout_state_data.close()
                 else:
                     rout_input_state_start_date = config['BASIN']['start']
                 ### Extracted routing start date ###
                 #------------- Routing Begins and Pre processing for Mass Balance --------------#
-                with RouteParameterFile(
+                output_paths, basin_station_xy_path, routing_statuses = run_routing(
                     config = config,
-                    basin_name = basin_name,
                     start = rout_input_state_start_date,
                     end = config['BASIN']['end'],
                     basin_flow_direction_file = basin_flow_dir_file,
+                    rout_input_path_prefix = rout_input_path_prefix,
                     clean=False,
-                    rout_input_path_prefix = rout_input_path_prefix
-                    ) as r:
-                    route = RoutingRunner(    
-                        project_dir = config['GLOBAL']['project_dir'], 
-                        result_dir = r.params['output_dir'], 
-                        inflow_dir = rout_inflow_dir, 
-                        model_path = config['ROUTING']['route_model'],
-                        param_path = r.route_param_path, 
-                        fdr_path = r.params['flow_direction_file'], 
-                        station_path_latlon = basin_station_latlon_file,
-                        station_xy = r.params['station']
-                    )
-                    route.create_station_file()
-                    route.run_routing()
-                    route.generate_inflow()
-                    basin_station_xy_path = route.station_path_xy
+                    inflow_dir = inflow_dst_dir,
+                    station_path_latlon = basin_station_latlon_file,
+                    route_dir=rout_dir,
+                    route_output_dir=routing_output_dir
+                )
                 ROUTING_STATUS=1
+                
             else:
                 rat_logger.info("VIC Run Failed. Skipping Step-8: Runnning Routing and generating Inflow")
         except:
             no_errors = no_errors+1
             rat_logger.exception("Error Executing Step-8: Runnning Routing and generating Inflow")
         else:
-            rat_logger.info("Finished Step-8: Runnning Routing and generating Inflow")
-            #------------- Routing Ends and Inflow pre-processed for Mass Balance --------------#
+            rat_logger.info("Finished Step-8: Runnning Routing model")
+            #------------- Routing Ends --------------#
 
     ######### Step-9
     if(9 in steps):
         try:
             rat_logger.info("Starting Step-9: Preparation of parameter files for Surface Area Calculation")
             #------------- Selection of Reservoirs within the basin begins--------------#
             ###### Preparing basin's reservoir shapefile and it's associated column dictionary for calculating surface area #####
             ### Creating Basin Reservoir Shapefile, if not exists ###
             if not os.path.exists(basin_reservoir_shpfile_path):
-                if os.path.exists(basin_station_xy_path):
-                    create_basin_reservoir_shpfile(config['GEE']['reservoir_vector_file'], reservoirs_gdf_column_dict, basin_station_xy_path,
+                    create_basin_reservoir_shpfile(config['GEE']['reservoir_vector_file'], reservoirs_gdf_column_dict, basin_data,
                                                                                 config['ROUTING']['station_global_data'], basin_reservoir_shpfile_path)
             ###### Prepared basin's reservoir shapefile and it's associated column dictionary #####
         except:
             no_errors = no_errors+1
             rat_logger.exception("Error Executing Step-9: Preparation of parameter files for Surface Area Calculation")
         else:
             rat_logger.info("Finished Step-9: Preparation of parameter files for Surface Area Calculation")
@@ -553,17 +560,17 @@
             from rat.core.run_sarea import run_sarea
             rat_logger.info("Starting Step-10: TMS-OS Surface Area Calculation from GEE")
             ##----------- Remote Sensing to estimate surface area begins -----------##
             if (not os.path.exists(basin_reservoir_shpfile_path)):
                 if (not config['ROUTING']['station_global_data']):
                     basin_reservoir_shpfile_path = config['GEE']['reservoir_vector_file']
                 else: 
-                    raise Exception('There was an error in creating reservoir shapefile using spatial join for this basin from the global reservoir vector file.')
+                    raise Exception('Step-9 was not run OR There was an error in creating reservoir shapefile using spatial join for this basin from the global reservoir vector file.')
             # Get Sarea
-            run_sarea(config['BASIN']['start'].strftime("%Y-%m-%d"), config['BASIN']['end'].strftime("%Y-%m-%d"), sarea_savepath, 
+            run_sarea(gee_start_date.strftime("%Y-%m-%d"), config['BASIN']['end'].strftime("%Y-%m-%d"), sarea_savepath, 
                                                                                     basin_reservoir_shpfile_path, reservoirs_gdf_column_dict)
             GEE_STATUS = 1
         except:
             no_errors = no_errors+1
             rat_logger.exception("Error Executing Step-10: TMS-OS Surface Area Calculation from GEE")
         else:
             rat_logger.info("Finished Step-10: TMS-OS Surface Area Calculation from GEE")                                                                        
@@ -588,35 +595,45 @@
     ######### Step-12
     if(12 in steps):
         try:
             from rat.ee_utils.ee_aec_file_creator import aec_file_creator
             rat_logger.info("Starting Step-12: Generating Area Elevation Curves for reservoirs")
             ##--------------------------------Area Elevation Curves Extraction begins ------------------- ##
             ## Creating AEC files if not present for post-processing dels calculation
-            aec_file_creator(basin_reservoir_shpfile_path,reservoirs_gdf_column_dict,aec_dir_path)
+            AEC_STATUS = aec_file_creator(basin_reservoir_shpfile_path,reservoirs_gdf_column_dict,aec_dir_path)
         except:
             rat_logger.exception("Finished Step-12: Generating Area Elevation Curves for reservoirs")
         else:
             rat_logger.info("Finished Step-12: Generating Area Elevation Curves for reservoirs")
             ##--------------------------------Area Elevation Curves Extraction ends ------------------- ##
 
     ######### Step-13
     if(13 in steps):
         try:
-            rat_logger.info("Starting Step-13: Calculation of Outflow, Evaporation and Storage change")
+            rat_logger.info("Starting Step-13: Calculation of Outflow, Evaporation, Storage change and Inflow")
             
             ##---------- Mass-balance Approach begins and then post-processing ----------## 
+            # Generate inflow files from RAT routing outputs
+            try:
+                generate_inflow(routing_output_dir, inflow_dst_dir)
+            except:
+                rat_logger.warning("Inflow could not be calculated. Moving forward to calculate storage change and evaporation.", exc_info=True)
+            # Copying AEC files to RAT output directory
+            try:
+                copy_aec_files(aec_dir_path, aec_savedir)
+            except:
+                rat_logger.warning("AEC files could not be copied to rat_outputs directory.", exc_info=True)
+            #Generating evaporation, storage change and outflow.    
             DELS_STATUS, EVAP_STATUS, OUTFLOW_STATUS = run_postprocessing(basin_name, basin_data_dir, basin_reservoir_shpfile_path, reservoirs_gdf_column_dict,
                                 aec_dir_path, config['BASIN']['start'], config['BASIN']['end'], rout_init_state_save_file, use_state, evap_savedir, dels_savedir, outflow_savedir, VIC_STATUS, ROUTING_STATUS, GEE_STATUS)
-
         except:
             no_errors = no_errors+1
-            rat_logger.exception("Error Executing Step-13: Calculation of Outflow, Evaporation and Storage change")
+            rat_logger.exception("Error Executing Step-13: Calculation of Outflow, Evaporation, Storage change and Inflow")
         else:
-            rat_logger.info("Finished Step-13: Calculation of Outflow, Evaporation and Storage change")
+            rat_logger.info("Finished Step-13: Calculation of Outflow, Evaporation, Storage change and Inflow")
             ##---------- Mass-balance Approach ends and then post-processed outputs to obtain timeseries  -----------------##
     
     ######### Step-14
     if(14 in steps):
         try:
             rat_logger.info("Starting Step-14: Creating final outputs in a timeseries format and cleaning up.")
 
@@ -626,15 +643,15 @@
                 convert_sarea(sarea_savepath,final_output_path)
                 rat_logger.info("Converted Surface Area to the Output Format.")
             else:
                 rat_logger.info("Could not convert Surface Area to the Output Format as GEE run failed.")
             
             ## Inflow
             if(ROUTING_STATUS):
-                convert_inflow(rout_inflow_dir, basin_reservoir_shpfile_path, reservoirs_gdf_column_dict, final_output_path)
+                convert_inflow(inflow_dst_dir, basin_reservoir_shpfile_path, reservoirs_gdf_column_dict, final_output_path)
                 rat_logger.info("Converted Inflow to the Output Format.")
             else:
                 rat_logger.info("Could not convert Inflow to the Output Format as Routing run failed.")
             
             ## Dels 
             if(DELS_STATUS):
                 convert_dels(dels_savedir, final_output_path)
@@ -659,14 +676,30 @@
             ## Altimeter
             if(ALTIMETER_STATUS):
                 convert_altimeter(altimetry_savepath, final_output_path)
                 rat_logger.info("Converted Extracted Height from Altimeter to the Output Format.")
             else:
                 rat_logger.info("Could not convert Extracted Height from Altimeter to the Output Format as Altimeter Run failed.")
             
+            ## AEC
+            if(AEC_STATUS):
+                aec_final_output_path = Path(final_output_path,'aec')
+                try:
+                    shutil.copytree(aec_savedir, aec_final_output_path)
+                except:
+                    try:
+                        shutil.rmtree(aec_final_output_path)
+                        shutil.copytree(aec_savedir, aec_final_output_path)
+                    except:
+                        rat_logger.warning("No AEC curves to convert into Output Format.")
+                    else:
+                        rat_logger.info("Converted Area Elevation Curve to the Output Format.")
+                else:
+                    rat_logger.info("Converted Area Elevation Curve to the Output Format.")
+            
             # Clearing out memory space as per user input 
             if(config['CLEAN_UP'].get('clean_metsim')):
                 rat_logger.info("Clearing up memory space: Removal of metsim output files")
                 cleaner.clean_metsim()
             if(config['CLEAN_UP'].get('clean_vic')):
                 rat_logger.info("Clearing up memory space: Removal of vic input, output files and previous init_state_files")
                 cleaner.clean_vic()
```

### Comparing `rat-3.0.0a4/src/rat/run_rat.py` & `rat-3.0.1/src/rat/run_rat.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import ee
 import ruamel_yaml as ryaml
 from pathlib import Path 
 import datetime
 import copy
 from dask.distributed import Client, LocalCluster
 
-from rat.utils.logging import init_logger,close_logger
+from rat.utils.logging import init_logger,close_logger,LOG_LEVEL1_NAME
 import rat.ee_utils.ee_config as ee_configuration
 from rat.rat_basin import rat_basin
 
 #------------ Define Variables ------------#
 def run_rat(config_fn, operational_latency=None):
     """Runs RAT as per configuration defined in `config_fn`.
 
@@ -33,20 +33,22 @@
     log_dir = os.path.join(config['GLOBAL']['data_dir'],'runs','logs','')
     log = init_logger(
         log_dir,
         verbose=False,
         # notify=True,
         notify=False,
         log_level='DEBUG',
-        logger_name='run_rat',
+        logger_name=LOG_LEVEL1_NAME,
         for_basin=False
     )
 
-    cluster = LocalCluster(name="RAT", n_workers=config['GLOBAL']['multiprocessing'])
+    log.debug("Initiating Dask Client ... ")
+    cluster = LocalCluster(name="RAT", n_workers=config['GLOBAL']['multiprocessing'], threads_per_worker=1)
     client = Client(cluster)
+    client.forward_logging(logger_name='rat-logger', level='DEBUG')
 
     log.debug(f"Started client with {config['GLOBAL']['multiprocessing']} workers. Dashboard link: {client.dashboard_link}")
 
     # Trying the ee credentials given by user
     try:
         log.info("Checking earth engine credentials")
         secrets = configparser.ConfigParser()
@@ -86,15 +88,15 @@
             # Run RAT for basin
             no_errors, latest_altimetry_cycle = rat_basin(config, log)
         # Displaying and storing RAT function outputs in the copy (non-mutabled as it was not passes to function)
         if(latest_altimetry_cycle):
             config_copy['ALTIMETER']['last_cycle_number'] = latest_altimetry_cycle
             ryaml_client.dump(config_copy, config_fn.open('w'))
         if(no_errors>0):
-            log.info('############## RAT run finished for '+config['BASIN']['basin_name']+ 'with '+str(no_errors)+' errors. #################')
+            log.info('############## RAT run finished for '+config['BASIN']['basin_name']+ ' with '+str(no_errors)+' error(s). #################')
         elif(no_errors==0):
             log.info('############## Succesfully run RAT for '+config['BASIN']['basin_name']+' #################')
         else:
             log.error('############## RAT run failed for '+config['BASIN']['basin_name']+' #################')
 
     ############ ----------- Multiple basin run ---------------- ################
     else:
@@ -146,22 +148,33 @@
             if(latest_altimetry_cycle):
                 # If column doesn't exist in basins_metadata, create one
                 if ('ALTIMETER','last_cycle_number') not in basins_metadata.columns:
                     basins_metadata['ALTIMETER','last_cycle_number'] = None    
                 basins_metadata['ALTIMETER','last_cycle_number'].where(basins_metadata['BASIN','basin_name']!= basin, latest_altimetry_cycle, inplace=True)
                 basins_metadata.to_csv(config_copy['GLOBAL']['basins_metadata'], index=False)
             if(no_errors>0):
-                log.info('############## RAT run finished for '+config_copy['BASIN']['basin_name']+ 'with '+str(no_errors)+' errors. #################')
+                log.info('############## RAT run finished for '+config_copy['BASIN']['basin_name']+ ' with '+str(no_errors)+' error(s). #################')
             elif(no_errors==0):
                 log.info('############## Succesfully run RAT for '+config_copy['BASIN']['basin_name']+' #################')
             else:
                 log.error('############## RAT run failed for '+config_copy['BASIN']['basin_name']+' #################')
 
-    # Clsoing logger
+    # Closing logger
     close_logger('rat_run')
+    # Closing Dask workers
+    try:
+        client.close()
+        client.retire_workers()
+    except:
+        print("####################### Finished executing RAT! ##########################")
+        print("Please ignore any below error related to distributed.worker or closed stream.")
+        print("####################### Finished executing RAT! ##########################")
+        print('\n\n')
+    # cluster.close()
+    
 
 def main():
     parser = argparse.ArgumentParser(description='Run RAT')
     parser.add_argument('--config', type=str, required=True,
                     help='Config file required to run RAT')
     args = parser.parse_args()
```

### Comparing `rat-3.0.0a4/src/rat/utils/clean.py` & `rat-3.0.1/src/rat/utils/clean.py`

 * *Files 7% similar despite different names*

```diff
@@ -104,20 +104,14 @@
 
     def clean_previous_outputs(self):
         try:
             rat_outputs_path = os.path.join(self.basin_data_dir,'rat_outputs')
             shutil.rmtree(rat_outputs_path)
         except:
             print("No previous rat_outputs folder to delete")
-        
-        try:
-            rat_inflow_path = os.path.join(self.basin_data_dir,'ro','rout_inflow')
-            shutil.rmtree(rat_inflow_path)
-        except:
-            print("No previous rout_inflow folder to delete")
 
         try:
             gee_sarea_path = os.path.join(self.basin_data_dir,'gee','gee_sarea_tmsos')
             shutil.rmtree(gee_sarea_path)
         except:
             print("No previous gee extracted surface area data folder to delete")
```

### Comparing `rat-3.0.0a4/src/rat/utils/convert_to_final_outputs.py` & `rat-3.0.1/src/rat/utils/convert_to_final_outputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import pandas as pd
 import geopandas as gpd
 import numpy as np
+from pathlib import Path
 from rat.utils.utils import create_directory
 
 def convert_sarea(sarea_dir, website_v_dir):
     # Surface Area
     sarea_paths = [os.path.join(sarea_dir, f) for f in os.listdir(sarea_dir) if f.endswith(".csv")]
     sarea_web_dir = create_directory(os.path.join(website_v_dir,'sarea_tmsos' ),True)
     for sarea_path in sarea_paths:
@@ -18,28 +19,28 @@
         df = df[['date', 'area']]
         df['area'] = np.round(df['area'], 3)
         df.rename({'area':'area (km2)'}, axis=1, inplace=True)
         print(f"Converting [Surface Area]: {res_name}")
         df.to_csv(savepath, index=False)
 
 
-def convert_inflow(inflow_dir, reservoir_shpfile, reservoir_shpfile_column_dict,  website_v_dir):
+def convert_inflow(inflow_dir, reservoir_shpfile, reservoir_shpfile_column_dict,  final_out_dir):
     # Inflow
     reservoirs = gpd.read_file(reservoir_shpfile)
-    reservoirs['Inflow_filename'] = reservoirs[reservoir_shpfile_column_dict['unique_identifier']].astype(str).str[:5]
+    reservoirs['Inflow_filename'] = reservoirs[reservoir_shpfile_column_dict['unique_identifier']].astype(str)
 
-    inflow_paths = [os.path.join(inflow_dir, f) for f in os.listdir(inflow_dir) if f.endswith(".csv")]
-    inflow_web_dir = create_directory(os.path.join(website_v_dir,'inflow' ),True)
+    inflow_paths = list(Path(inflow_dir).glob('*.csv'))
+    final_out_inflow_dir = Path(final_out_dir) / 'inflow'
+    final_out_inflow_dir.mkdir(exist_ok=True)
 
     for inflow_path in inflow_paths:
         res_name = os.path.splitext(os.path.split(inflow_path)[-1])[0]
 
         if res_name in reservoirs['Inflow_filename'].tolist():
-            savename = reservoirs[reservoirs['Inflow_filename'] == res_name][reservoir_shpfile_column_dict['unique_identifier']].values[0]
-            savepath = os.path.join(inflow_web_dir ,f"{savename}.csv")
+            savepath = final_out_inflow_dir / inflow_path.name
 
             df = pd.read_csv(inflow_path, parse_dates=['date'])
             df['inflow (m3/d)'] = df['streamflow'] * (24*60*60)        # indicate units, convert from m3/s to m3/d
             df = df[['date', 'inflow (m3/d)']]
 
             print(f"Converting [Inflow]: {res_name}")
             df.to_csv(savepath, index=False)
@@ -119,14 +120,27 @@
             df['date'] = df['date'].dt.strftime("%Y-%m-%d")
             df['H [m w.r.t. EGM2008 Geoid]'] = np.round(df['H [m w.r.t. EGM2008 Geoid]'], 2)
             df.rename({'H [m w.r.t. EGM2008 Geoid]':'height (m)'}, axis=1, inplace=True)
 
             print(f"Converting [Heights]: {res_name}")
             df.to_csv(savepath, index=False)
 
+def copy_aec_files(src_dir, dst_dir):
+    src_dir = Path(src_dir)
+    dst_dir = Path(dst_dir)
+
+    for src_path in src_dir.glob('*.csv'):
+        aec = pd.read_csv(src_path)
+        aec.rename({
+            'Elevation': 'elevation',
+            'CumArea': 'area'
+        }, axis=1, inplace=True)
+        aec.to_csv(dst_dir / src_path.name, index=False)
+
+
 def convert_v2_frontend(basin_data_dir, res_name, inflow_src, sarea_src, dels_src, outflow_src):
     """Converts the files according to the newer version of the frontend (v2).
 
     Args:
         basin_data_dir (str): path of basin data directory
         res_name (str): name of reservoir
         inflow_src (str): source .csv file containing inflow in cumecs
```

### Comparing `rat-3.0.0a4/src/rat/utils/files_creator.py` & `rat-3.0.1/src/rat/utils/files_creator.py`

 * *Files 26% similar despite different names*

```diff
@@ -100,18 +100,20 @@
     basins_station_spatialjoin = gpd.sjoin(basins_station, basin_data_crs_changed, "inner")[[
                         column_dict['id_column'],
                         column_dict['name_column'],
                         column_dict['lon_column'],
                         column_dict['lat_column'],
                         'geometry']]
     if(geojson_file):
+        ## Creates a geojson file of stations with columns 'DAM_NAME', 'regionname', 'basinname' and 'filename', used by frontend.
         basins_station_spatialjoin['regionname'] = str(region_name)
         basins_station_spatialjoin['basinname'] = str(basin_name)
         basins_station_spatialjoin['filename'] = basins_station_spatialjoin[column_dict['id_column']].astype(str)+'_'+ \
                                         basins_station_spatialjoin[column_dict['name_column']].str.replace(' ','_')
+        basins_station_spatialjoin.rename(columns={column_dict['name_column']: "DAM_NAME"})
         geojson_save_path = os.path.join(os.path.dirname(savepath),basin_name+'_station.geojson')
         basins_station_spatialjoin.to_file(geojson_save_path, driver= "GeoJSON")
 
     basins_station_lat_lon = basins_station_spatialjoin[[
                             column_dict['id_column'],
                             column_dict['name_column'],
                             column_dict['lon_column'],
@@ -119,26 +121,57 @@
     basins_station_lat_lon['name'] = basins_station_lat_lon[column_dict['id_column']].astype(str
                                                                 )+'_'+basins_station_lat_lon[column_dict['name_column']].astype(str).str.replace(' ','_')
     basins_station_lat_lon['run'] = 1
     basins_station_lat_lon['lon'] = basins_station_lat_lon[column_dict['lon_column']]
     basins_station_lat_lon['lat'] = basins_station_lat_lon[column_dict['lat_column']]
     basins_station_lat_lon[['run','name','lon','lat']].to_csv(savepath,index=False)
 
-def create_basin_reservoir_shpfile(reservoir_shpfile,reservoir_shpfile_column_dict,station_xy_file,routing_station_global_data,savepath):
+def create_basin_station_geojson(region_name, basin_name, station_csv_file, savepath):
+    '''
+    Creates a geojson shape file for the stations(reservoirs) for a particular basin with the following columns:
+        DAM_NAME: the name of the station
+        basinname: the name of the basin in which the station is located
+        regionname: the name of the region in which the basin of that station is located
+        filename: the name which will be used to save a station's output data like inflow, outflow etc.
+    '''
+    # Reading the station csv file
+    basin_station_df =  pd.read_csv(station_csv_file)
+    # Converting pandas df to geopandas dataframe
+    basin_station_gdf= gpd.GeoDataFrame(
+        basin_station_df, geometry=gpd.points_from_xy(basin_station_df.lon, basin_station_df.lat))
+    # Removing unwanted columns
+    basin_station_gdf = basin_station_gdf.drop(columns='run')
+    # Adding the desired columns
+    basin_station_gdf['regionname'] = str(region_name)
+    basin_station_gdf['basinname'] = str(basin_name)
+    basin_station_gdf['filename'] = basin_station_gdf['name']
+    basin_station_gdf['DAM_NAME'] = basin_station_gdf['name'].str.replace('_',' ')
+    # Setting crs of the geopandas dataframe
+    basin_station_gdf = basin_station_gdf.set_crs('epsg:4326')
+    # Saving the geopandas datframe as geojson file
+    geojson_save_path = os.path.join(os.path.dirname(savepath),basin_name+'_station.geojson')
+    basin_station_gdf.to_file(geojson_save_path, driver= "GeoJSON")
+
+def create_basin_reservoir_shpfile(reservoir_shpfile,reservoir_shpfile_column_dict,basin_gpd_df,routing_station_global_data,savepath):
     reservoirs = gpd.read_file(reservoir_shpfile)
-    stations_df = pd.read_csv(station_xy_file,sep='\t',header=None,names=['run','name','x','y','area']).dropna().reset_index(drop=True)
+    basin_data_crs_changed = basin_gpd_df.to_crs(reservoirs.crs)
+    #stations_df = pd.read_csv(station_xy_file,sep='\t',header=None,names=['run','name','x','y','area']).dropna().reset_index(drop=True)
     reservoirs_gdf_column_dict = reservoir_shpfile_column_dict
 
     if routing_station_global_data:
-        reservoirs['uniq_id'] = reservoirs[reservoirs_gdf_column_dict['id_column']].astype(str)+'_'+ \
-                            reservoirs[reservoirs_gdf_column_dict['dam_name_column']].astype(str).str.replace(' ','_')
-        stations_df = stations_df.rename(columns={'name':'uniq_id'})                                            
-        reservoirs_gdf = reservoirs.merge(stations_df['uniq_id'], how='inner', on='uniq_id')
+        reservoirs_spatialjoin = gpd.sjoin(reservoirs, basin_data_crs_changed, "inner")[[
+                        reservoirs_gdf_column_dict['id_column'],
+                        reservoirs_gdf_column_dict['dam_name_column'],
+                        reservoirs_gdf_column_dict['area_column'],
+                        'geometry']]
+        reservoirs_spatialjoin['uniq_id'] = reservoirs_spatialjoin[reservoirs_gdf_column_dict['id_column']].astype(str)+'_'+ \
+                            reservoirs_spatialjoin[reservoirs_gdf_column_dict['dam_name_column']].astype(str).str.replace(' ','_')
     else:
-        stations_df = stations_df.rename(columns={'name':reservoirs_gdf_column_dict['dam_name_column']})
-        reservoirs_gdf = reservoirs.merge(stations_df[reservoirs_gdf_column_dict['dam_name_column']], 
-                                        how='inner', on=reservoirs_gdf_column_dict['dam_name_column'])
+        reservoirs_spatialjoin = gpd.sjoin(reservoirs, basin_data_crs_changed, "inner")[[
+                        reservoirs_gdf_column_dict['dam_name_column'],
+                        reservoirs_gdf_column_dict['area_column'],
+                        'geometry']]
     
-    if(reservoirs_gdf.empty):
+    if(reservoirs_spatialjoin.empty):
         raise Exception('Reservoir names in reservoir shapefile are not matching with the station names in the station file used for routing.')
-    reservoirs_gdf.to_file(savepath, index=False)
+    reservoirs_spatialjoin.to_file(savepath, index=False)
```

### Comparing `rat-3.0.0a4/src/rat/utils/logging.py` & `rat-3.0.1/src/rat/utils/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from time import gmtime, strftime
 import datetime
 import logging
 import subprocess
 from rat.utils.utils import create_directory
 
 # -------------------------------------------------------------------- #
+LOG_LEVEL1_NAME = 'run_rat'
 LOG_NAME = 'rat-logger'
-FORMATTER = logging.Formatter('%(levelname)s:%(funcName)s>> %(message)s')
-
+LOG_LEVEL = 'DEBUG'
 NOTIFICATION = 25    # Setting level above INFO, below WARNING
 logging.addLevelName(NOTIFICATION, "NOTIFICATION")
 NOTIFICATION_FOMATTER = logging.Formatter(
     '%(asctime)s>> %(message)s',
     datefmt='%Y-%m-%d %I:%M:%S %p')
 # -------------------------------------------------------------------- #
 
@@ -41,14 +41,33 @@
         pass
 
 class NotificationHandler(logging.Handler):
     def emit(self, record):
         subprocess.run(['/houston2/pritam/rat_mekong_v3/.condaenv/bin/ntfy', '-b', 'telegram', 'send', self.format(record)])
 # -------------------------------------------------------------------- #
 
+class Formatter(logging.Formatter):
+    def __init__(self, fmt="%(asctime)s %(levelname)s:%(funcName)s>> %(message)s", datefmt="%Y-%m-%d %H:%M:%S"):
+        super().__init__(fmt, datefmt=datefmt, style='%')
+
+    def format(self, record):
+        original_fmt = self._style._fmt
+
+        if hasattr(record, 'worker'):
+            self._style._fmt = '%(asctime)s %(levelname)s [worker %(worker)s]:%(funcName)s>> %(message)s'
+
+        # Call the original formatter class to do the grunt work
+        result = logging.Formatter.format(self, record)
+
+        # Restore the original format configured by the user
+        self._style._fmt = original_fmt
+
+        return result
+
+FORMATTER = Formatter()
 
 def init_logger(log_dir='./', log_level='DEBUG', verbose=False, notify=False, logger_name=LOG_NAME, for_basin=True):
     ''' Setup the logger '''
     #Creating log directory if does not exist
     create_directory(log_dir)
 
     #Extracting basin name from the log_dir_path
```

### Comparing `rat-3.0.0a4/src/rat/utils/metsim_param_reader.py` & `rat-3.0.1/src/rat/utils/metsim_param_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import yaml
 import datetime
 from logging import getLogger
 import os
 
-from rat.utils.logging import LOG_NAME, NOTIFICATION
+from rat.utils.logging import LOG_NAME, LOG_LEVEL, NOTIFICATION
 from rat.utils.utils import create_directory
 
 log = getLogger(LOG_NAME)
-
+log.setLevel(LOG_LEVEL)
 
 class MSParameterFile:
     def __init__(self, start, end, init_param, out_dir, forcings=None, state=None, domain=None, workspace=None, runname=None):
         self.params = yaml.safe_load(open(init_param, 'r'))   # Initialize from a parameter file
         
         self.params['MetSim']['start'] = start.strftime("%Y-%-m-%d")
         self.params['MetSim']['stop'] = end.strftime("%Y-%-m-%d")
```

### Comparing `rat-3.0.0a4/src/rat/utils/route_param_reader.py` & `rat-3.0.1/src/rat/utils/route_param_reader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 import os
 import datetime
 from logging import getLogger
 import yaml
 import shutil
-
+from pathlib import Path
 from rat.utils.utils import create_directory
-from rat.utils.logging import LOG_NAME, NOTIFICATION
+from rat.utils.logging import LOG_NAME, NOTIFICATION, LOG_LEVEL
 
 log = getLogger(LOG_NAME)
+log.setLevel(LOG_LEVEL)
 
 class RouteParameterFile:
-    def __init__(self, config, basin_name, start, end, basin_flow_direction_file=None, clean=False, runname=None, rout_input_path_prefix=None,
-                                config_section='ROUTING', intermediate_files=False):
+    def __init__(self, config, basin_name, start, end, route_param_path=None, basin_flow_direction_file=None, clean=False, runname=None, rout_input_path_prefix=None,
+                                station_path=None, config_section='ROUTING', intermediate_files=False, output_dst=None, uh=None):
         self.params = {
             'flow_direction_file': None,
             'velocity': None,
             'diff': None,
             'xmask': None,
             'fraction': None,
             'station': None,
             'input_files_prefix': None,
             'input_file_precision': None,
             'output_dir': None,
             'start_date': start.strftime("%Y %m %d"),
             'end_date': end.strftime("%Y %m %d"),
             'uh': None
         }
-        self.route_param_path = None
+        self.route_param_path = route_param_path
         self.workspace = None
         self.clean = clean
 
         self.basin_name = basin_name
+        self.station_path = station_path
         self.intermediate_files = intermediate_files
         self.rout_input_path_prefix = rout_input_path_prefix
         self.basin_flow_direction_file = basin_flow_direction_file
         self.project_dir = config['GLOBAL']['project_dir']
+        self.output_dir = output_dst
+        self.uh = uh
 
         self.startdate = start
         self.enddate = end
         self.config_section = config_section
 
         self.config = config
         if runname is None:
@@ -63,115 +67,127 @@
             self.params['start_date'] = self.startdate.strftime('%Y %m %d')
 
         if self.enddate:
             self.params['end_date'] = self.enddate.strftime('%Y %m %d')
 
         # setup workspace
         if (config[self.config_section].get('route_workspace')):
-            self.workspace = create_directory(os.path.join(config[self.config_section]['route_workspace'],
-                                                                 f'run_{self.runname}'))
+            self.workspace = Path(config[self.config_section]['route_workspace']) / f'run_{self.runname}'
+            self.workspace.mkdir(exist_ok=True)
         else:
             if(self.intermediate_files):
-                self.workspace = create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['region_name'],'basins',
-                                                                self.basin_name,'ro','rout_workspace',f'run_{self.runname}'))
+                self.workspace = Path(config['GLOBAL']['data_dir']).joinpath(config['BASIN']['region_name'],'basins',self.basin_name,'ro','rout_workspace',f'run_{self.runname}')
+                self.workspace.mkdir(exist_ok=True)
         
         ## Route parameter file, this is where the parameter file will be saved
         if (self.intermediate_files):
             self.route_param_path = os.path.relpath(os.path.join(self.workspace, 'route_param.txt'),self.project_dir)
-        else:
+        elif self.route_param_path is None:
             # Replacing the init_route_param_file
             if(config[self.config_section].get('route_param_file')):
                 self.route_param_path = os.path.relpath(config[self.config_section].get('route_param_file'),self.project_dir)
             # Or storing it in route basin params dir and replace it from next cycle
             else:
                 self.route_param_path = create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['region_name'],
-                                                            'basins',self.basin_name,'rout_basin_params'),True)
+                                                            'basins',self.basin_name,'ro','pars'),True)
                 self.route_param_path = os.path.relpath(os.path.join(self.route_param_path,'route_param.txt'),self.project_dir)
         
         ## flow direction file
         self.params['flow_direction_file'] = self.basin_flow_direction_file
 
         ## output dir
-        self.params['output_dir'] = create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['region_name'],
+        if self.output_dir is not None: # if output dir is passed as parameter use it
+            self.params['output_dir'] = self.output_dir
+        else: # if output dir is not passed as parameter, create it in default location
+            self.params['output_dir'] = create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['region_name'],
                                                             'basins',self.basin_name,'ro','ou'),True)
         
         ## stations
-        if (self.intermediate_files):
-            self.params['station'] = os.path.join(self.workspace, 'sta_xy.txt')
+        if self.station_path: # if station path is passed as parameter
+            self.params['station'] = self.station_path # use it
+        elif (self.intermediate_files): # if intermediate files are to be generated (on-the-fly workspace folder creation)
+            self.params['station'] = os.path.join(self.workspace, 'sta_xy.txt') # use the workspace folder
         else:
             self.params['station'] = create_directory(os.path.join(config['GLOBAL']['data_dir'],config['BASIN']['region_name'],
-                                                        'basins',self.basin_name,'ro','pars'),True)
+                                                        'basins',self.basin_name,'ro','pars'),True) # else use the default folder
             self.params['station'] = os.path.join(self.params['station'],'sta_xy.txt')
 
         # Routing Input file prefix path   
         self.params['input_files_prefix'] = self.rout_input_path_prefix
         
         # load from config
         for key in config[f'{self.config_section} PARAMETERS']:
             val = config[f'{self.config_section} PARAMETERS'][key]
             self.params[key] = val
+
+        # if uh is passed as parameter (override the value from rat_config)
+        if self.uh:
+            self.params['uh'] = self.uh
+        # if basin_flow_direction file is passed as parameter (override the value from rat_config)
+        if self.basin_flow_direction_file:
+            self.params['flow_direction_file'] = self.basin_flow_direction_file
     
     # TODO create _load_from_param
 
     def _out_format_params(self):
         res = []
 
         res.append(f"# ROUTE PARAMETER FILE created by RouteParameterFile() on {datetime.datetime.now().strftime('%Y-%m-%d %X')} - run_{self.runname}")
         
         res.append(f"# FLOW DIRECTION FILE")
-        res.append(f"{os.path.relpath(self.params['flow_direction_file'],self.project_dir)}")
+        res.append(f"{self.params['flow_direction_file']}")
         
         res.append(f"# VELOCITY FILE")
         if not isinstance(self.params['velocity'], str): # if not a velocity file path
             res.append(f".false.")
             res.append(f"{self.params['velocity']}")
         else:
             res.append(f".true.")
-            res.append(f"{os.path.relpath(self.params['velocity'],self.project_dir)}")
+            res.append(f"{self.params['velocity']}")
 
         res.append(f"# DIFFUSION FILE")
         if not isinstance(self.params['diff'], str): # if not a velocity file path
             res.append(f".false.")
             res.append(f"{self.params['diff']}")
         else:
             res.append(f".true.")
-            res.append(f"{os.path.relpath(self.params['diff'],self.project_dir)}")
+            res.append(f"{self.params['diff']}")
 
         res.append(f"# XMASK FILE")
         if not isinstance(self.params['xmask'], str): # if not a velocity file path
             res.append(f".false.")
             res.append(f"{self.params['xmask']}")
         else:
             res.append(f".true.")
-            res.append(f"{os.path.relpath(self.params['xmask'],self.project_dir)}")
+            res.append(f"{self.params['xmask']}")
 
         res.append(f"# FRACTION FILE")
         if not isinstance(self.params['fraction'], str): # if not a velocity file path
             res.append(f".false.")
             res.append(f"{self.params['fraction']}")
         else:
             res.append(f".true.")
-            res.append(f"{os.path.relpath(self.params['fraction'],self.project_dir)}")
+            res.append(f"{self.params['fraction']}")
 
         res.append(f"# STATION FILE")
-        res.append(f"{os.path.relpath(self.params['station'],self.project_dir)}")
+        res.append(f"{self.params['station']}")
 
         res.append(f"# INPUTS and PRECISION")
-        res.append(f"{os.path.relpath(self.params['input_files_prefix'],self.project_dir)}")
+        res.append(f"{self.params['input_files_prefix']}")
         res.append(f"{self.params['input_file_precision']}")
 
         res.append(f"# OUTPUT FILES")
-        res.append(f"{os.path.relpath(self.params['output_dir'],self.project_dir)}/")
+        res.append(f"{self.params['output_dir']}")
 
         res.append(f"# START and END")
         res.append(f"{self.params['start_date']}")
         res.append(f"{self.params['end_date']}")
 
         res.append(f"# UH")
-        res.append(f"{os.path.relpath(self.params['uh'],self.project_dir)}")
+        res.append(f"{self.params['uh']}")
 
         return '\n'.join(res)
 
     def _write(self):
         with open(os.path.join(self.project_dir,self.route_param_path), 'w') as f:
             param = self._out_format_params()
             log.debug(param)
```

### Comparing `rat-3.0.0a4/src/rat/utils/run_command.py` & `rat-3.0.1/src/rat/utils/run_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,14 @@
         for line in iter(p.stdout.readline, b''): # b'\n'-separated lines
             log.debug("%r", line)
         
     exitcode = p.wait()
 
     if exitcode == 0:
         log.debug("Finished running command successfully: EXIT CODE %s", exitcode)
-    elif (exitcode == 1 and metsim==True):
+    elif (exitcode == 0 and metsim==True):
         log.debug("Finished running metsim successfully: EXIT CODE %s", exitcode)
     else:
         log.error("ERROR Occurred with exit code: %s", exitcode)
         raise Exception
     
     return exitcode
```

### Comparing `rat-3.0.0a4/src/rat/utils/science.py` & `rat-3.0.1/src/rat/utils/science.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a4/src/rat/utils/utils.py` & `rat-3.0.1/src/rat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `rat-3.0.0a4/src/rat/utils/vic_param_reader.py` & `rat-3.0.1/src/rat/utils/vic_param_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import datetime
 import os
 from logging import getLogger
 
 import yaml
 
-from rat.utils.logging import LOG_NAME, NOTIFICATION
+from rat.utils.logging import LOG_NAME, NOTIFICATION, LOG_LEVEL
 from rat.utils.utils import create_directory
 
 log = getLogger(LOG_NAME)
+log.setLevel(LOG_LEVEL)
 
 class VICParameterFile:
     def __init__(self, config, basin_name, startdate=None, enddate=None, vic_output_path=None, vic_section='VIC',
                                      forcing_prefix=None, runname=None, init_state_date=None, save_init_state=True,
                                       intermediate_files= False):
         
         self.params = {
```

### Comparing `rat-3.0.0a4/src/rat.egg-info/PKG-INFO` & `rat-3.0.1/src/rat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rat
-Version: 3.0.0a4
+Version: 3.0.1
 Summary: Resevoir Monitoring using Satellite Remote Sensing
 Author-email: Pritam Das <pdas47@uw.edu>, Sanchit Minocha <msanchit@uw.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -681,15 +681,15 @@
 Project-URL: Bug Tracker, https://github.com/UW-SASWE/RAT/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![Reservoir Assessment Tool](docs/logos/Rat%20Logo_black_360p.png)
+![Reservoir Assessment Tool](docs/logos/Rat_Logo_black_github.png)
 # Reservoir Assessment Tool 3.0
 [![Documentation Status](https://readthedocs.org/projects/rat-satellitedams/badge/?version=latest)](https://rat-satellitedams.readthedocs.io/en/latest/?badge=latest)
 
 The Reservoir Assessment Tool (RAT) uses satellite remote sensing data to monitor water surface area and water level changes in artificial reservoirs. It uses this information, along with topographical information (either derived from satellite data, or in-situ topo maps) to estimate the **Storage Change (∆S)** in the reservoirs. Additionally, RAT models the **Inflow (I)** and the **Evaporation (E)** of each reservoir. Finally, RAT uses the modeled I, and E, and estimated ∆S, to estimate the **Outflow (O)** from reservoirs.
 
 RAT 3.0 makes numerous improvements to the code structure, performance optimizations, added configurations, ability to run RAT for multiple basins, among some introduced features. It also introduces packaging of RAT as a conda package, allowing for quick and easy installation.
```

### Comparing `rat-3.0.0a4/src/rat.egg-info/SOURCES.txt` & `rat-3.0.1/src/rat.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/rat.egg-info/PKG-INFO
 src/rat.egg-info/SOURCES.txt
 src/rat.egg-info/dependency_links.txt
 src/rat.egg-info/top_level.txt
 src/rat/cli/rat_cli.py
 src/rat/cli/rat_init_config.py
 src/rat/cli/rat_test_config.py
+src/rat/cli/rat_test_verify.py
 src/rat/core/run_altimetry.py
 src/rat/core/run_metsim.py
 src/rat/core/run_postprocessing.py
 src/rat/core/run_routing.py
 src/rat/core/run_sarea.py
 src/rat/core/run_vic.py
 src/rat/core/sarea/TMS.py
```

