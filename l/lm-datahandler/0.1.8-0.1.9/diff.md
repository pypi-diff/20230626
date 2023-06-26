# Comparing `tmp/lm_datahandler-0.1.8.tar.gz` & `tmp/lm_datahandler-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lm_datahandler-0.1.8.tar", last modified: Wed Jun 21 03:05:37 2023, max compression
+gzip compressed data, was "lm_datahandler-0.1.9.tar", last modified: Wed Jun 21 04:01:06 2023, max compression
```

## Comparing `lm_datahandler-0.1.8.tar` & `lm_datahandler-0.1.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.648739 lm_datahandler-0.1.8/
--rw-rw-rw-   0        0        0     1104 2023-06-14 03:54:04.000000 lm_datahandler-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       45 2023-06-14 10:58:27.000000 lm_datahandler-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      325 2023-06-21 03:05:37.648739 lm_datahandler-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.626570 lm_datahandler-0.1.8/lm_datahandler/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:11:31.000000 lm_datahandler-0.1.8/lm_datahandler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.635918 lm_datahandler-0.1.8/lm_datahandler/data_download/
--rw-rw-rw-   0        0        0        0 2023-06-20 07:02:42.000000 lm_datahandler-0.1.8/lm_datahandler/data_download/__init__.py
--rw-rw-rw-   0        0        0     3008 2023-06-20 07:59:35.000000 lm_datahandler-0.1.8/lm_datahandler/data_download/data_download.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.639001 lm_datahandler-0.1.8/lm_datahandler/data_load/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:11:51.000000 lm_datahandler-0.1.8/lm_datahandler/data_load/__init__.py
--rw-rw-rw-   0        0        0     2026 2023-06-20 07:11:38.000000 lm_datahandler-0.1.8/lm_datahandler/data_load/data_loader.py
--rw-rw-rw-   0        0        0    12664 2023-06-15 09:43:32.000000 lm_datahandler-0.1.8/lm_datahandler/data_load/loaders.py
--rw-rw-rw-   0        0        0    24249 2023-06-20 03:21:12.000000 lm_datahandler-0.1.8/lm_datahandler/datahandler.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.642013 lm_datahandler-0.1.8/lm_datahandler/functions/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:02.000000 lm_datahandler-0.1.8/lm_datahandler/functions/__init__.py
--rw-rw-rw-   0        0        0    33356 2023-06-21 02:52:28.000000 lm_datahandler-0.1.8/lm_datahandler/functions/biomarker.py
--rw-rw-rw-   0        0        0    29337 2023-06-16 07:10:08.000000 lm_datahandler-0.1.8/lm_datahandler/functions/feature_extract.py
--rw-rw-rw-   0        0        0        0 2023-05-31 12:12:04.000000 lm_datahandler-0.1.8/lm_datahandler/functions/os_detect.py
--rw-rw-rw-   0        0        0      613 2023-06-16 08:37:12.000000 lm_datahandler-0.1.8/lm_datahandler/functions/posture_analyse.py
--rw-rw-rw-   0        0        0     1510 2023-06-15 09:46:15.000000 lm_datahandler-0.1.8/lm_datahandler/functions/sleep_staging.py
--rw-rw-rw-   0        0        0     3828 2023-06-19 09:29:10.000000 lm_datahandler-0.1.8/lm_datahandler/functions/sleep_variable_compute.py
--rw-rw-rw-   0        0        0        0 2023-05-31 12:11:57.000000 lm_datahandler-0.1.8/lm_datahandler/functions/spindle_detect.py
--rw-rw-rw-   0        0        0      832 2023-06-16 07:21:59.000000 lm_datahandler-0.1.8/lm_datahandler/functions/wear_detect.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.643052 lm_datahandler-0.1.8/lm_datahandler/models/
--rw-rw-rw-   0        0        0    59109 2023-03-31 05:25:34.000000 lm_datahandler-0.1.8/lm_datahandler/models/wear_detection_1s.txt
--rw-rw-rw-   0        0        0   376172 2023-05-30 01:59:36.000000 lm_datahandler-0.1.8/lm_datahandler/models/wholenight_sleep_staging.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.644792 lm_datahandler-0.1.8/lm_datahandler/plots/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:16.000000 lm_datahandler-0.1.8/lm_datahandler/plots/__init__.py
--rw-rw-rw-   0        0        0      625 2023-06-07 08:43:30.000000 lm_datahandler-0.1.8/lm_datahandler/plots/biomarker_plot.py
--rw-rw-rw-   0        0        0     6763 2023-06-19 08:57:14.000000 lm_datahandler-0.1.8/lm_datahandler/plots/sleep_staging_plot.py
--rw-rw-rw-   0        0        0     3553 2023-06-19 08:09:09.000000 lm_datahandler-0.1.8/lm_datahandler/plots/stim_plot.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.645798 lm_datahandler-0.1.8/lm_datahandler/postprocess/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:28.000000 lm_datahandler-0.1.8/lm_datahandler/postprocess/__init__.py
--rw-rw-rw-   0        0        0     2358 2023-06-02 05:40:05.000000 lm_datahandler-0.1.8/lm_datahandler/postprocess/label_smooth.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.647519 lm_datahandler-0.1.8/lm_datahandler/preprocess/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:46.000000 lm_datahandler-0.1.8/lm_datahandler/preprocess/__init__.py
--rw-rw-rw-   0        0        0      865 2023-06-19 08:09:38.000000 lm_datahandler-0.1.8/lm_datahandler/preprocess/filter.py
--rw-rw-rw-   0        0        0        0 2023-05-31 10:48:56.000000 lm_datahandler-0.1.8/lm_datahandler/preprocess/tailor.py
--rw-rw-rw-   0        0        0     4843 2023-06-21 03:05:18.000000 lm_datahandler-0.1.8/lm_datahandler/scripts.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.648201 lm_datahandler-0.1.8/lm_datahandler/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 03:12:57.000000 lm_datahandler-0.1.8/lm_datahandler/utils/__init__.py
--rw-rw-rw-   0        0        0     1734 2023-04-20 07:01:30.000000 lm_datahandler-0.1.8/lm_datahandler/utils/numba_func.py
-drwxrwxrwx   0        0        0        0 2023-06-21 03:05:37.634953 lm_datahandler-0.1.8/lm_datahandler.egg-info/
--rw-rw-rw-   0        0        0      325 2023-06-21 03:05:37.000000 lm_datahandler-0.1.8/lm_datahandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1381 2023-06-21 03:05:37.000000 lm_datahandler-0.1.8/lm_datahandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 03:05:37.000000 lm_datahandler-0.1.8/lm_datahandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      179 2023-06-21 03:05:37.000000 lm_datahandler-0.1.8/lm_datahandler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-21 03:05:37.000000 lm_datahandler-0.1.8/lm_datahandler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 03:05:37.648739 lm_datahandler-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      987 2023-06-21 03:05:22.000000 lm_datahandler-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:01:06.774845 lm_datahandler-0.1.9/
+-rw-rw-rw-   0        0        0     1104 2023-06-14 03:54:04.000000 lm_datahandler-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       45 2023-06-14 10:58:27.000000 lm_datahandler-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      325 2023-06-21 04:01:06.774845 lm_datahandler-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-21 04:01:06.745713 lm_datahandler-0.1.9/lm_datahandler/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:11:31.000000 lm_datahandler-0.1.9/lm_datahandler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:01:06.762227 lm_datahandler-0.1.9/lm_datahandler/data_download/
+-rw-rw-rw-   0        0        0        0 2023-06-20 07:02:42.000000 lm_datahandler-0.1.9/lm_datahandler/data_download/__init__.py
+-rw-rw-rw-   0        0        0     3008 2023-06-20 07:59:35.000000 lm_datahandler-0.1.9/lm_datahandler/data_download/data_download.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:01:06.763227 lm_datahandler-0.1.9/lm_datahandler/data_load/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:11:51.000000 lm_datahandler-0.1.9/lm_datahandler/data_load/__init__.py
+-rw-rw-rw-   0        0        0     2026 2023-06-20 07:11:38.000000 lm_datahandler-0.1.9/lm_datahandler/data_load/data_loader.py
+-rw-rw-rw-   0        0        0    12664 2023-06-15 09:43:32.000000 lm_datahandler-0.1.9/lm_datahandler/data_load/loaders.py
+-rw-rw-rw-   0        0        0    24249 2023-06-20 03:21:12.000000 lm_datahandler-0.1.9/lm_datahandler/datahandler.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:01:06.767680 lm_datahandler-0.1.9/lm_datahandler/functions/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:02.000000 lm_datahandler-0.1.9/lm_datahandler/functions/__init__.py
+-rw-rw-rw-   0        0        0    33356 2023-06-21 02:52:28.000000 lm_datahandler-0.1.9/lm_datahandler/functions/biomarker.py
+-rw-rw-rw-   0        0        0    29337 2023-06-16 07:10:08.000000 lm_datahandler-0.1.9/lm_datahandler/functions/feature_extract.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:12:04.000000 lm_datahandler-0.1.9/lm_datahandler/functions/os_detect.py
+-rw-rw-rw-   0        0        0      613 2023-06-16 08:37:12.000000 lm_datahandler-0.1.9/lm_datahandler/functions/posture_analyse.py
+-rw-rw-rw-   0        0        0     1510 2023-06-15 09:46:15.000000 lm_datahandler-0.1.9/lm_datahandler/functions/sleep_staging.py
+-rw-rw-rw-   0        0        0     3828 2023-06-19 09:29:10.000000 lm_datahandler-0.1.9/lm_datahandler/functions/sleep_variable_compute.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:11:57.000000 lm_datahandler-0.1.9/lm_datahandler/functions/spindle_detect.py
+-rw-rw-rw-   0        0        0      832 2023-06-16 07:21:59.000000 lm_datahandler-0.1.9/lm_datahandler/functions/wear_detect.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:01:06.768614 lm_datahandler-0.1.9/lm_datahandler/models/
+-rw-rw-rw-   0        0        0    59109 2023-03-31 05:25:34.000000 lm_datahandler-0.1.9/lm_datahandler/models/wear_detection_1s.txt
+-rw-rw-rw-   0        0        0   376172 2023-05-30 01:59:36.000000 lm_datahandler-0.1.9/lm_datahandler/models/wholenight_sleep_staging.txt
+drwxrwxrwx   0        0        0        0 2023-06-21 04:01:06.770418 lm_datahandler-0.1.9/lm_datahandler/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:16.000000 lm_datahandler-0.1.9/lm_datahandler/plots/__init__.py
+-rw-rw-rw-   0        0        0      625 2023-06-07 08:43:30.000000 lm_datahandler-0.1.9/lm_datahandler/plots/biomarker_plot.py
+-rw-rw-rw-   0        0        0     6763 2023-06-19 08:57:14.000000 lm_datahandler-0.1.9/lm_datahandler/plots/sleep_staging_plot.py
+-rw-rw-rw-   0        0        0     3553 2023-06-19 08:09:09.000000 lm_datahandler-0.1.9/lm_datahandler/plots/stim_plot.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:01:06.770834 lm_datahandler-0.1.9/lm_datahandler/postprocess/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:28.000000 lm_datahandler-0.1.9/lm_datahandler/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     2358 2023-06-02 05:40:05.000000 lm_datahandler-0.1.9/lm_datahandler/postprocess/label_smooth.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:01:06.773844 lm_datahandler-0.1.9/lm_datahandler/preprocess/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:46.000000 lm_datahandler-0.1.9/lm_datahandler/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      865 2023-06-19 08:09:38.000000 lm_datahandler-0.1.9/lm_datahandler/preprocess/filter.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 10:48:56.000000 lm_datahandler-0.1.9/lm_datahandler/preprocess/tailor.py
+-rw-rw-rw-   0        0        0     5081 2023-06-21 03:59:24.000000 lm_datahandler-0.1.9/lm_datahandler/scripts.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:01:06.773844 lm_datahandler-0.1.9/lm_datahandler/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 03:12:57.000000 lm_datahandler-0.1.9/lm_datahandler/utils/__init__.py
+-rw-rw-rw-   0        0        0     1734 2023-04-20 07:01:30.000000 lm_datahandler-0.1.9/lm_datahandler/utils/numba_func.py
+drwxrwxrwx   0        0        0        0 2023-06-21 04:01:06.760227 lm_datahandler-0.1.9/lm_datahandler.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-06-21 04:01:06.000000 lm_datahandler-0.1.9/lm_datahandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1381 2023-06-21 04:01:06.000000 lm_datahandler-0.1.9/lm_datahandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 04:01:06.000000 lm_datahandler-0.1.9/lm_datahandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      179 2023-06-21 04:01:06.000000 lm_datahandler-0.1.9/lm_datahandler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-21 04:01:06.000000 lm_datahandler-0.1.9/lm_datahandler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-21 04:01:06.774845 lm_datahandler-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      987 2023-06-21 04:00:51.000000 lm_datahandler-0.1.9/setup.py
```

### Comparing `lm_datahandler-0.1.8/LICENSE` & `lm_datahandler-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/lm_datahandler/data_download/data_download.py` & `lm_datahandler-0.1.9/lm_datahandler/data_download/data_download.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/lm_datahandler/data_load/data_loader.py` & `lm_datahandler-0.1.9/lm_datahandler/data_load/data_loader.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/lm_datahandler/data_load/loaders.py` & `lm_datahandler-0.1.9/lm_datahandler/data_load/loaders.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/lm_datahandler/datahandler.py` & `lm_datahandler-0.1.9/lm_datahandler/datahandler.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/lm_datahandler/functions/biomarker.py` & `lm_datahandler-0.1.9/lm_datahandler/functions/biomarker.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/lm_datahandler/functions/feature_extract.py` & `lm_datahandler-0.1.9/lm_datahandler/functions/feature_extract.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/lm_datahandler/functions/posture_analyse.py` & `lm_datahandler-0.1.9/lm_datahandler/functions/posture_analyse.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/lm_datahandler/functions/sleep_staging.py` & `lm_datahandler-0.1.9/lm_datahandler/functions/sleep_staging.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/lm_datahandler/functions/sleep_variable_compute.py` & `lm_datahandler-0.1.9/lm_datahandler/functions/sleep_variable_compute.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/lm_datahandler/functions/wear_detect.py` & `lm_datahandler-0.1.9/lm_datahandler/functions/wear_detect.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/lm_datahandler/models/wear_detection_1s.txt` & `lm_datahandler-0.1.9/lm_datahandler/models/wear_detection_1s.txt`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/lm_datahandler/models/wholenight_sleep_staging.txt` & `lm_datahandler-0.1.9/lm_datahandler/models/wholenight_sleep_staging.txt`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/lm_datahandler/plots/biomarker_plot.py` & `lm_datahandler-0.1.9/lm_datahandler/plots/biomarker_plot.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/lm_datahandler/plots/sleep_staging_plot.py` & `lm_datahandler-0.1.9/lm_datahandler/plots/sleep_staging_plot.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/lm_datahandler/plots/stim_plot.py` & `lm_datahandler-0.1.9/lm_datahandler/plots/stim_plot.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/lm_datahandler/postprocess/label_smooth.py` & `lm_datahandler-0.1.9/lm_datahandler/postprocess/label_smooth.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/lm_datahandler/preprocess/filter.py` & `lm_datahandler-0.1.9/lm_datahandler/preprocess/filter.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/lm_datahandler/scripts.py` & `lm_datahandler-0.1.9/lm_datahandler/scripts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,63 @@
 import os.path
 import pandas as pd
 from lm_datahandler.data_download.data_download import download_lm_data_from_server
 from lm_datahandler.datahandler import DataHandler
 
 
 def download_and_full_analyse(download_params):
-    save_path = download_params["save_path"]
-    data_list = download_lm_data_from_server(download_params, save_path)
+    data_save_path = download_params["save_path"]
+    data_list = download_lm_data_from_server(download_params, data_save_path)
     sleep_variables_save_file_name = "sleep_variables_" + download_params["dateRange"][0] + "_" + \
                                      download_params["dateRange"][1] + ".csv"
 
     analysis_save_path = download_params["analysis_save_path"]
 
-    local_data_full_analyse(save_path, data_list, analysis_save_path=analysis_save_path, sleep_variables_save_name=sleep_variables_save_file_name)
+    local_data_full_analyse(data_save_path, data_list, analysis_save_path=analysis_save_path, sleep_variables_save_name=sleep_variables_save_file_name)
 
 
 
 
-def local_data_full_analyse(dir_path, data_names, analysis_save_path=None, sleep_variables_save_name=None):
-    assert os.path.exists(dir_path), "The input dir path does not exist."
+def local_datas_full_analyse(data_path, data_names, analysis_save_path=None, sleep_variables_save_name=None):
+    assert os.path.exists(data_path), "The input dir path does not exist."
     sleep_variables_df = pd.DataFrame({
         "data_name": [],
         "TST": [],
         "SOL": [],
         "GU": [],
         "WASO": [],
         "SE": [],
         "AR": []
     })
 
     if analysis_save_path is None:
-        analysis_save_path = dir_path
+        analysis_save_path = data_path
+    else:
+        if not os.path.exists(analysis_save_path):
+            os.mkdir(analysis_save_path)
     for i, data_name in enumerate(data_names):
-        if not os.path.exists(os.path.join(dir_path, data_name)):
-            print("data: \"{}\" not found, skipped.")
+        if not os.path.exists(os.path.join(data_path, data_name)):
+            print("data: \"{}\" not found, skipped.".format(data_name))
             continue
         data_handler = DataHandler()
 
-        data_path = os.path.join(dir_path, data_name)
+        temp_data_path = os.path.join(data_path, data_name)
 
         data_analysis_save_path = os.path.join(analysis_save_path, data_name)
-        if os.path.exists(data_analysis_save_path):
+
+        if not os.path.exists(data_analysis_save_path):
             os.mkdir(data_analysis_save_path)
         sleep_fig_save_path = os.path.join(data_analysis_save_path, "sleep_fig.png")
         slow_wave_stim_sham_plot = os.path.join(data_analysis_save_path, "sw_stim_sham_fig.png")
 
         slow_wave_excel_save_path = os.path.join(data_analysis_save_path, "sw.csv")
         spindle_excel_save_path = os.path.join(data_analysis_save_path, "sp.csv")
 
         # 数据加载
-        data_handler.load_data(data_name=data_name, data_path=data_path)
+        data_handler.load_data(data_name=data_name, data_path=temp_data_path)
 
         # 绘制慢波增强对比图，并保存
         data_handler.plot_sw_stim_sham(savefig=slow_wave_stim_sham_plot)
 
         # 进行睡眠分期，计算睡眠指标，绘制睡眠综合情况图，并保存
         data_handler.preprocess().sleep_staging().compute_sleep_variables().plot_sleep_data(savefig=sleep_fig_save_path)
 
@@ -63,50 +67,53 @@
         # spindle检测和慢波检测，并导出结果成excel
         data_handler.spindle_detect().export_sp_results(slow_wave_excel_save_path)
         data_handler.sw_detect().export_sw_results(spindle_excel_save_path)
 
         data_handler.show_plots()
 
 
-        sleep_variables_df.to_csv(os.path.join(dir_path, sleep_variables_save_name))
+        sleep_variables_df.to_csv(os.path.join(temp_data_path, sleep_variables_save_name))
 
 
-if __name__ == '__main__':
-    # download_param = {
-    #     # 刺激范式：1. 手动刺激，2. 音频刺激，3. N3闭环刺激，4. 纯记录模式，5. 记录模式， 6. 音频刺激
-    #     'paradigms': [],
-    #     # 用户手机号
-    #     'phones': None,
-    #     # 基座mac
-    #     'macs': None,
-    #     # 服务版本
-    #     'serviceVersions': None,
-    #     # 睡眠主观评分，1~5，-1表示未评分
-    #     'sleepScores': None,
-    #     # 停止类型， 0. 断连超时, 1. 用户手动, 2. 头贴放到基座上停止, 3. 关机指令触发, 4. 低电量, 5. 崩溃
-    #     'stopTypes': None,
-    #     # 时间范围，以停止记录的时间为准
-    #     'dateRange': ['20230621', '20230621'],
-    #     # 数据时长范围
-    #     'dataLengthRange': [60 * 1, 60 * 12],
-    #     # 翻身次数范围
-    #     'turnoverCountRange': None,
-    #     # 刺激次数范围
-    #     'stimulationCountRange': None,
-    #     # 下载保存路径
-    #     'save_path': 'E:/dataset/x7_new/matlab_data',
-    #     # 分析结果保存路径（为None表示保存在数据下载路径中）
-    #     'analysis_save_path': None
-    # }
-    # download_and_full_analyse(download_param)
-
-    data_names = [
-        "13651856616_0428-21_35_53_0429-06_16_38_0.00_4",
-        "13651856616_0429-22_38_30_0430-05_06_56_0.00_4",
-        "13651856616_0430-22_07_51_0501-05_44_42_0.00_4",
-        "13651856616_0501-22_02_30_0502-05_03_52_0.00_4",
-        "13651856616_0502-22_15_44_0503-05_29_35_0.02_4",
-        "13651856616_0503-21_39_36_0504-05_05_05_0.00_4",
-        "13651856616_20210102_20_05_07_20210103_04_21_55",
 
-    ]
-    local_data_full_analyse(r"E:\dataset\sleep_disorders\1_13651856616_ZLZ", data_names, None, "sleep_variables_13651856616_ZLZ.csv")
+
+if __name__ == '__main__':
+    day = '20230621'
+    download_param = {
+        # 刺激范式：1. 手动刺激，2. 音频刺激，3. N3闭环刺激，4. 纯记录模式，5. 记录模式， 6. 音频刺激
+        'paradigms': None,
+        # 用户手机号
+        'phones': None,
+        # 基座mac
+        'macs': None,
+        # 服务版本
+        'serviceVersions': None,
+        # 睡眠主观评分，1~5，-1表示未评分
+        'sleepScores': None,
+        # 停止类型， 0. 断连超时, 1. 用户手动, 2. 头贴放到基座上停止, 3. 关机指令触发, 4. 低电量, 5. 崩溃
+        'stopTypes': None,
+        # 时间范围，以停止记录的时间为准
+        'dateRange': ['20230621', '20230621'],
+        # 数据时长范围
+        'dataLengthRange': [60 * 8, 60 * 12],
+        # 翻身次数范围
+        'turnoverCountRange': None,
+        # 刺激次数范围
+        'stimulationCountRange': None,
+        # 下载保存路径
+        'save_path': os.path.join('E:/dataset/x7_data_by_days/data', day),
+        # 分析结果保存路径（为None表示保存在数据下载路径中）
+        'analysis_save_path': os.path.join('E:/dataset/x7_data_by_days/analysis', day)
+    }
+    download_and_full_analyse(download_param)
+
+    # data_names = [
+    #     "13651856616_0428-21_35_53_0429-06_16_38_0.00_4",
+    #     "13651856616_0429-22_38_30_0430-05_06_56_0.00_4",
+    #     "13651856616_0430-22_07_51_0501-05_44_42_0.00_4",
+    #     "13651856616_0501-22_02_30_0502-05_03_52_0.00_4",
+    #     "13651856616_0502-22_15_44_0503-05_29_35_0.02_4",
+    #     "13651856616_0503-21_39_36_0504-05_05_05_0.00_4",
+    #     "13651856616_20210102_20_05_07_20210103_04_21_55",
+    #
+    # ]
+    # local_data_full_analyse(r"E:\dataset\sleep_disorders\1_13651856616_ZLZ", data_names, None, "sleep_variables_13651856616_ZLZ.csv")
```

### Comparing `lm_datahandler-0.1.8/lm_datahandler/utils/numba_func.py` & `lm_datahandler-0.1.9/lm_datahandler/utils/numba_func.py`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/lm_datahandler.egg-info/SOURCES.txt` & `lm_datahandler-0.1.9/lm_datahandler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lm_datahandler-0.1.8/setup.py` & `lm_datahandler-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'lm_datahandler',
-    version = '0.1.8',
+    version = '0.1.9',
     keywords='eeg sleep staging analysis',
     description = 'a python analyse tool for LM Data Recorder data',
     license = 'MIT License',
     url = 'https://github.com/zx950618/lm_datahandler',
     author = 'Eric Zheng',
     author_email = '1248471980@qq.com',
     packages = find_packages(),
```

