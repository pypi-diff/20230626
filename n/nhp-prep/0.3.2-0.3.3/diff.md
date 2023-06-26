# Comparing `tmp/nhp-prep-0.3.2.tar.gz` & `tmp/nhp-prep-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhp-prep-0.3.2.tar", last modified: Fri Mar 31 19:21:40 2023, max compression
+gzip compressed data, was "nhp-prep-0.3.3.tar", last modified: Mon Jun 26 13:01:59 2023, max compression
```

## Comparing `nhp-prep-0.3.2.tar` & `nhp-prep-0.3.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-03-31 19:21:40.467262 nhp-prep-0.3.2/
--rw-r--r--   0 hugo       (501) staff       (20)       64 2023-03-31 19:18:02.000000 nhp-prep-0.3.2/MANIFEST.in
--rw-r--r--   0 hugo       (501) staff       (20)     3633 2023-03-31 19:21:40.467072 nhp-prep-0.3.2/PKG-INFO
--rw-r--r--   0 hugo       (501) staff       (20)     2980 2023-03-24 12:42:19.000000 nhp-prep-0.3.2/README.md
-drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-03-31 19:21:40.465006 nhp-prep-0.3.2/app/
--rw-r--r--   0 hugo       (501) staff       (20)      325 2023-03-31 19:20:59.000000 nhp-prep-0.3.2/app/__init__.py
--rw-r--r--   0 hugo       (501) staff       (20)    16315 2023-03-31 19:18:02.000000 nhp-prep-0.3.2/app/__main__.py
--rw-r--r--   0 hugo       (501) staff       (20)       57 2022-11-20 13:33:19.000000 nhp-prep-0.3.2/app/cli.py
--rw-r--r--   0 hugo       (501) staff       (20)      830 2022-11-20 13:33:19.000000 nhp-prep-0.3.2/app/column_mapper.py
-drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-03-31 19:21:40.465563 nhp-prep-0.3.2/app/config/
--rw-r--r--   0 hugo       (501) staff       (20)     1244 2023-02-24 03:59:57.000000 nhp-prep-0.3.2/app/config/columns__std_format.csv
--rw-r--r--   0 hugo       (501) staff       (20)      677 2022-11-22 20:27:38.000000 nhp-prep-0.3.2/app/config/logs.yaml
--rw-r--r--   0 hugo       (501) staff       (20)      274 2022-12-20 16:45:39.000000 nhp-prep-0.3.2/app/main_logger.py
--rw-r--r--   0 hugo       (501) staff       (20)     8007 2022-12-20 14:26:32.000000 nhp-prep-0.3.2/app/rename_files.py
--rw-r--r--   0 hugo       (501) staff       (20)     4300 2023-03-24 20:17:31.000000 nhp-prep-0.3.2/app/subject_changer.py
--rw-r--r--   0 hugo       (501) staff       (20)     1639 2023-02-27 04:12:49.000000 nhp-prep-0.3.2/app/timestamp_estimator.py
-drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-03-31 19:21:40.465879 nhp-prep-0.3.2/app/util/
--rw-r--r--   0 hugo       (501) staff       (20)     2481 2023-02-28 17:18:12.000000 nhp-prep-0.3.2/app/util/rough_estimate_std_files.py
-drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-03-31 19:21:40.466823 nhp-prep-0.3.2/nhp_prep.egg-info/
--rw-r--r--   0 hugo       (501) staff       (20)     3633 2023-03-31 19:21:40.000000 nhp-prep-0.3.2/nhp_prep.egg-info/PKG-INFO
--rw-r--r--   0 hugo       (501) staff       (20)      487 2023-03-31 19:21:40.000000 nhp-prep-0.3.2/nhp_prep.egg-info/SOURCES.txt
--rw-r--r--   0 hugo       (501) staff       (20)        1 2023-03-31 19:21:40.000000 nhp-prep-0.3.2/nhp_prep.egg-info/dependency_links.txt
--rw-r--r--   0 hugo       (501) staff       (20)       47 2023-03-31 19:21:40.000000 nhp-prep-0.3.2/nhp_prep.egg-info/entry_points.txt
--rw-r--r--   0 hugo       (501) staff       (20)       39 2023-03-31 19:21:40.000000 nhp-prep-0.3.2/nhp_prep.egg-info/requires.txt
--rw-r--r--   0 hugo       (501) staff       (20)       13 2023-03-31 19:21:40.000000 nhp-prep-0.3.2/nhp_prep.egg-info/top_level.txt
--rw-r--r--   0 hugo       (501) staff       (20)       38 2023-02-28 17:18:12.000000 nhp-prep-0.3.2/requirements.txt
--rw-r--r--   0 hugo       (501) staff       (20)       38 2023-03-31 19:21:40.467312 nhp-prep-0.3.2/setup.cfg
--rw-r--r--   0 hugo       (501) staff       (20)     1268 2023-03-31 19:20:40.000000 nhp-prep-0.3.2/setup.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-06-26 13:01:59.549883 nhp-prep-0.3.3/
+-rw-r--r--   0 hugo       (501) staff       (20)       64 2023-03-31 19:18:02.000000 nhp-prep-0.3.3/MANIFEST.in
+-rw-r--r--   0 hugo       (501) staff       (20)     3483 2023-06-26 13:01:59.549698 nhp-prep-0.3.3/PKG-INFO
+-rw-r--r--   0 hugo       (501) staff       (20)     2830 2023-06-26 12:45:36.000000 nhp-prep-0.3.3/README.md
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-06-26 13:01:59.548194 nhp-prep-0.3.3/app/
+-rw-r--r--   0 hugo       (501) staff       (20)      325 2023-06-26 13:00:06.000000 nhp-prep-0.3.3/app/__init__.py
+-rw-r--r--   0 hugo       (501) staff       (20)    17482 2023-06-26 12:45:36.000000 nhp-prep-0.3.3/app/__main__.py
+-rw-r--r--   0 hugo       (501) staff       (20)       57 2022-11-20 13:33:19.000000 nhp-prep-0.3.3/app/cli.py
+-rw-r--r--   0 hugo       (501) staff       (20)      830 2022-11-20 13:33:19.000000 nhp-prep-0.3.3/app/column_mapper.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-06-26 13:01:59.548457 nhp-prep-0.3.3/app/config/
+-rw-r--r--   0 hugo       (501) staff       (20)     1244 2023-02-24 03:59:57.000000 nhp-prep-0.3.3/app/config/columns__std_format.csv
+-rw-r--r--   0 hugo       (501) staff       (20)      677 2022-11-22 20:27:38.000000 nhp-prep-0.3.3/app/config/logs.yaml
+-rw-r--r--   0 hugo       (501) staff       (20)      274 2022-12-20 16:45:39.000000 nhp-prep-0.3.3/app/main_logger.py
+-rw-r--r--   0 hugo       (501) staff       (20)     8045 2023-06-26 12:45:36.000000 nhp-prep-0.3.3/app/rename_files.py
+-rw-r--r--   0 hugo       (501) staff       (20)     4300 2023-03-24 20:17:31.000000 nhp-prep-0.3.3/app/subject_changer.py
+-rw-r--r--   0 hugo       (501) staff       (20)     1639 2023-02-27 04:12:49.000000 nhp-prep-0.3.3/app/timestamp_estimator.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-06-26 13:01:59.548616 nhp-prep-0.3.3/app/util/
+-rw-r--r--   0 hugo       (501) staff       (20)     2519 2023-06-26 12:45:36.000000 nhp-prep-0.3.3/app/util/rough_estimate_std_files.py
+drwxr-xr-x   0 hugo       (501) staff       (20)        0 2023-06-26 13:01:59.549471 nhp-prep-0.3.3/nhp_prep.egg-info/
+-rw-r--r--   0 hugo       (501) staff       (20)     3483 2023-06-26 13:01:59.000000 nhp-prep-0.3.3/nhp_prep.egg-info/PKG-INFO
+-rw-r--r--   0 hugo       (501) staff       (20)      487 2023-06-26 13:01:59.000000 nhp-prep-0.3.3/nhp_prep.egg-info/SOURCES.txt
+-rw-r--r--   0 hugo       (501) staff       (20)        1 2023-06-26 13:01:59.000000 nhp-prep-0.3.3/nhp_prep.egg-info/dependency_links.txt
+-rw-r--r--   0 hugo       (501) staff       (20)       47 2023-06-26 13:01:59.000000 nhp-prep-0.3.3/nhp_prep.egg-info/entry_points.txt
+-rw-r--r--   0 hugo       (501) staff       (20)       39 2023-06-26 13:01:59.000000 nhp-prep-0.3.3/nhp_prep.egg-info/requires.txt
+-rw-r--r--   0 hugo       (501) staff       (20)       13 2023-06-26 13:01:59.000000 nhp-prep-0.3.3/nhp_prep.egg-info/top_level.txt
+-rw-r--r--   0 hugo       (501) staff       (20)       38 2023-02-28 17:18:12.000000 nhp-prep-0.3.3/requirements.txt
+-rw-r--r--   0 hugo       (501) staff       (20)       38 2023-06-26 13:01:59.549935 nhp-prep-0.3.3/setup.cfg
+-rw-r--r--   0 hugo       (501) staff       (20)     1268 2023-06-26 12:59:48.000000 nhp-prep-0.3.3/setup.py
```

### Comparing `nhp-prep-0.3.2/PKG-INFO` & `nhp-prep-0.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhp-prep
-Version: 0.3.2
+Version: 0.3.3
 Summary: Pre-processing data tool for NHP Lab @ CMU
 Home-page: https://caoslab.psy.cmu.edu:32443/monkeylab/preprocessing-scripts
 Author: Hugo Angulo, Zijun Zhao
 Author-email: hugoanda@andrew.cmu.edu, zijunzha@andrew.cmu.edu
 License: MIT
 Keywords: nhp-prep,caoslab,cmu,pre-processing
 Classifier: Development Status :: 5 - Production/Stable
@@ -69,29 +69,23 @@
 ```
 nhp-prep reorder-columns -i <directory_with_files_to_reorder_columns_OR_unique_CSV_file> -o <output_directory> -r <file_with_reference_columns>
 ```
 
 2. Rename the files to follow current standard (`rename`)
 
 ```
-nhp-prep rename -i <directory_files_to_rename_OR_uniques_CSV_file> -o <output_directory>
+nhp-prep rename -i <directory_files_to_rename> -o <output_directory>
 ```
 
 The current format for the file is: `YYYY-MM-DD_HHmmh_<experiment_name>_<Subject_name>_<Researcher_name_or_initials>_data.csv`
 
 3. Timestamp estimation trials from historical data files based on column <X> (`timestamp-estimate`)
 
 ```
-nhp-prep --timestamp-estimate -i <input_file>
-```
-
-Alternatively, you can pass the directory of the files to estimate the timestamp of each trial:
-
-```
-nhp-prep timestamp-estimate -i <directory_with_files_OR_unique_CSV_file>
+nhp-prep timestamp-estimate -i <directory_with_files_OR_unique_CSV_file> -o <output_directory>
 ```
 
 ##### **Since v0.3.0**
 
 Since the previous 3 steps are common across the different datasets collected, the dev team decided to merge them into one single command (`preparation-steps`):
 
 ```
```

### Comparing `nhp-prep-0.3.2/README.md` & `nhp-prep-0.3.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -52,29 +52,23 @@
 ```
 nhp-prep reorder-columns -i <directory_with_files_to_reorder_columns_OR_unique_CSV_file> -o <output_directory> -r <file_with_reference_columns>
 ```
 
 2. Rename the files to follow current standard (`rename`)
 
 ```
-nhp-prep rename -i <directory_files_to_rename_OR_uniques_CSV_file> -o <output_directory>
+nhp-prep rename -i <directory_files_to_rename> -o <output_directory>
 ```
 
 The current format for the file is: `YYYY-MM-DD_HHmmh_<experiment_name>_<Subject_name>_<Researcher_name_or_initials>_data.csv`
 
 3. Timestamp estimation trials from historical data files based on column <X> (`timestamp-estimate`)
 
 ```
-nhp-prep --timestamp-estimate -i <input_file>
-```
-
-Alternatively, you can pass the directory of the files to estimate the timestamp of each trial:
-
-```
-nhp-prep timestamp-estimate -i <directory_with_files_OR_unique_CSV_file>
+nhp-prep timestamp-estimate -i <directory_with_files_OR_unique_CSV_file> -o <output_directory>
 ```
 
 ##### **Since v0.3.0**
 
 Since the previous 3 steps are common across the different datasets collected, the dev team decided to merge them into one single command (`preparation-steps`):
 
 ```
```

### Comparing `nhp-prep-0.3.2/app/__main__.py` & `nhp-prep-0.3.3/app/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,30 +92,50 @@
     exists.
     """
     if not os.path.exists(output):
         os.makedirs(output)
 
     _files_to_process = 0
     _error_files = 0
-    # TODO: Needs a validation for a directory or a file.
-    for _, _, files in os.walk(input):
-        for each in files:
-            if each.endswith(FILE_TYPE):
-                _files_to_process += 1
-                filename = os.path.join(input, each)
-                out_filename = os.path.join(output, each)
-                try:
-                    df_reordered = map_columns(
-                        columns=ref_columns, filename=filename)
-                    df_reordered.to_csv(out_filename, index=False)
-                    logger.info(f'File reordered successfully: {out_filename}')
-                except Exception as e:
-                    logger.error(
-                        f'An error has been detected while processing the file: {filename}. \n Please check the following error: {e}')
-                    _error_files += 1
+
+    # if feeded with a single csv file 
+    # TODO: DRY principle!!!
+    if os.path.isfile(input) and input.endswith(FILE_TYPE):
+        logger.info(
+            'File recognized. \n Proceeding to reorder columns of it...')
+        out_filename = os.path.join(output, os.path.basename(input))
+        try:
+            df_reordered = map_columns(
+                        columns=ref_columns, filename=input)
+            df_reordered.to_csv(out_filename, index=False)
+            logger.info(f'File reordered successfully: {out_filename}')
+            _files_to_process += 1
+        except Exception as e:
+            logger.error(
+                f'An error has been detected while processing the file: {filename}. \n Please check the following error: {e}')
+            _error_files += 1
+    
+    # else, treat it as a folder 
+    else:
+        for _, dirs, files in os.walk(input):
+            for each in files:
+                if each.endswith(FILE_TYPE):
+                    _files_to_process += 1
+                    filename = os.path.join(input, each)
+                    out_filename = os.path.join(output, each)
+                    try:
+                        df_reordered = map_columns(
+                            columns=ref_columns, filename=filename)
+                        df_reordered.to_csv(out_filename, index=False)
+                        logger.info(f'File reordered successfully: {out_filename}')
+                    except Exception as e:
+                        logger.error(
+                            f'An error has been detected while processing the file: {filename}. \n Please check the following error: {e}')
+                        _error_files += 1
+
     _reordered_files = _files_to_process - _error_files
     _percentage_success = (_reordered_files / _files_to_process) * 100
     logger.info(
         f'Total files reordered:  {_reordered_files}/{_files_to_process} => {_percentage_success} % success!')
 
 
 @click.command(name='rename', short_help='Renames all the files based on standard.')
@@ -137,21 +157,26 @@
     file.
     """
     start_time = time()
     logger.info(
         '-------------------------- RENAMING FILE(S) --------------------------')
     logger.info('Input: %s', input)
     logger.info('Output path: %s', output)
-    if os.path.isfile(input):
+
+    # if feeded with a single csv file 
+    # TODO: refine to follow DRY principle
+    if os.path.isfile(input) and input.endswith(FILE_TYPE):
         logger.info('File recognized. \n Proceeding to rename it...')
         _result = file_rename(filepath=input, output=output)
         if _result is False:
             logger.error('An error occurred during the process of renaming '
                          'the file: %s. Please check the logs.', input)
         logger.info('Total execution time: %f seconds', time() - start_time)
+
+    # else, treat it as a folder 
     elif os.path.isdir(input):
         logger.info('Path recognized.')
         logger.info('Proceeding to rename all files within it...')
         num_files = 0
         num_errors = 0
         error_files = list()
         empty_files = list()
@@ -224,14 +249,16 @@
     """
     if not os.path.exists(output):
         os.makedirs(output)
 
     _files_to_process = 0
     _error_files = 0
 
+    # if feeded with a single csv file 
+    # TODO: refine to follow DRY principle
     if os.path.isfile(input) and input.endswith(FILE_TYPE):
         logger.info(
             'File recognized. \n Proceeding to estimate timestamp of it...')
         out_filename = os.path.join(output, os.path.basename(input))
         try:
             df_timestamp_changed = change_timestamp(
                 filename=input
@@ -239,14 +266,16 @@
             df_timestamp_changed.to_csv(out_filename, index=False)
             logger.info(f'Change timestamp successfully: {out_filename}')
             _files_to_process += 1
         except Exception as e:
             logger.error(
                 f'An error has been detected while processing the file: {filename}. \n Please check the following error: {e}')
             _error_files += 1
+
+    # else, treat it as a folder 
     else:
         # Here, we roughly estimate the StartTimestamp of each file by creating a temporary output folder
         _tmp_intermediate_dir = tempfile.TemporaryDirectory()
         _intermediate_input = _tmp_intermediate_dir.name
         # input -> _tmp_intermediate_dir -> output
         dir_time_estimate(input, _intermediate_input)
         files = [each for each in os.listdir(_intermediate_input) if each.endswith(
@@ -261,21 +290,24 @@
                 )
                 df_timestamp_changed.to_csv(out_filename, index=False)
                 logger.info(f'Change timestamp successfully: {out_filename}')
             except Exception as e:
                 logger.error(
                     f'An error has been detected while processing the file: {filename}. \n Please check the following error: {e}')
                 _error_files += 1
+
+        # clean up temporary directory
+        logger.debug(
+            f'Cleaning up temporary directory: {_tmp_intermediate_dir.name}...')    
+        _tmp_intermediate_dir.cleanup()
+
     _reordered_files = _files_to_process - _error_files
     _percentage_success = (_reordered_files / _files_to_process) * 100
     logger.info(
         f'Total files reordered successfully:  {_reordered_files}/{_files_to_process} => {_percentage_success} % success!')
-    logger.debug(
-        f'Cleaning up temporary directory: {_tmp_intermediate_dir.name}...')
-    _tmp_intermediate_dir.cleanup()
 
 
 @click.command(name='sub-rename', short_help='Updates the subject name based trial level.')
 @click.option('--ref-file', '-f', required=True, help='Reference file that contains the names of subjects and timestamp start and end.')
 @click.option('--input', '-i', required=True, help='Input directory.')
 @click.option('--output', '-o', help='Output directory.')
 def sub_rename(input, output, ref_file):
```

### Comparing `nhp-prep-0.3.2/app/column_mapper.py` & `nhp-prep-0.3.3/app/column_mapper.py`

 * *Files identical despite different names*

### Comparing `nhp-prep-0.3.2/app/config/columns__std_format.csv` & `nhp-prep-0.3.3/app/config/columns__std_format.csv`

 * *Files identical despite different names*

### Comparing `nhp-prep-0.3.2/app/config/logs.yaml` & `nhp-prep-0.3.3/app/config/logs.yaml`

 * *Files identical despite different names*

### Comparing `nhp-prep-0.3.2/app/rename_files.py` & `nhp-prep-0.3.3/app/rename_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 DATE_ENDING_CHAR = 'h'
 EXP_COL = 'Exp'
 SUB_COL = 'Sub'
 RESEARCHER_COL = 'Researcher'
 NAME_COL = 'Name'
 EXP_NAME_END = 'data.csv'
 EXP_START_TS = 'ExpStartTimestamp'
-STD_FILENAME_PATTERN = r'^\d{4}-\d{2}-\d{2}_\d{4}h_([a-zA-Z]+(?:_[a-zA-Z]+)*)_[a-zA-Z]+_[a-zA-Z]{2,6}_data\.csv$'
+
+# to fully comply the naming patterns of existing csv files
+# see ./README.md:115
+STD_FILENAME_PATTERN = r'^\d{4}-\d{2}-\d{2}_\d{4}h_(.*?_)+data.csv$'
 
 
 def find_epoch(file: str):
     """Method that finds the EPOCH
     timestamp within the file.
 
     Args:
```

### Comparing `nhp-prep-0.3.2/app/subject_changer.py` & `nhp-prep-0.3.3/app/subject_changer.py`

 * *Files identical despite different names*

### Comparing `nhp-prep-0.3.2/app/timestamp_estimator.py` & `nhp-prep-0.3.3/app/timestamp_estimator.py`

 * *Files identical despite different names*

### Comparing `nhp-prep-0.3.2/app/util/rough_estimate_std_files.py` & `nhp-prep-0.3.3/app/util/rough_estimate_std_files.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 MS_SEPARATOR = ","
 COLON = ":"
 DOUBLE_ZERO = "00"
 
 TRIAL_START_COL = "TrialStartTimestamp"
 EXP_START_TS = 'ExpStartTimestamp'
 HHMMSS_FORMAT = '%H:%M:%S'
-STD_FILENAME_PATTERN = r'^\d{4}-\d{2}-\d{2}_\d{4}h_([a-zA-Z]+(?:_[a-zA-Z]+)*)_[a-zA-Z]+_[a-zA-Z]{2,6}_data\.csv$'
+
+# to fully comply the naming patterns of existing csv files
+# see ./README.md:115
+STD_FILENAME_PATTERN = r'^\d{4}-\d{2}-\d{2}_\d{4}h_(.*?_)+data.csv$'
 
 
 def estimate_time(filepath, filename, output_path):
     file_data = pd.read_csv(filepath)
     # parse the file name for the month, day, year and start time
     full_time_str = filename.split(HOUR_ENDING)[0]
     _date_str = full_time_str.split(SEPARATOR_TAG)[0]
```

### Comparing `nhp-prep-0.3.2/nhp_prep.egg-info/PKG-INFO` & `nhp-prep-0.3.3/nhp_prep.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhp-prep
-Version: 0.3.2
+Version: 0.3.3
 Summary: Pre-processing data tool for NHP Lab @ CMU
 Home-page: https://caoslab.psy.cmu.edu:32443/monkeylab/preprocessing-scripts
 Author: Hugo Angulo, Zijun Zhao
 Author-email: hugoanda@andrew.cmu.edu, zijunzha@andrew.cmu.edu
 License: MIT
 Keywords: nhp-prep,caoslab,cmu,pre-processing
 Classifier: Development Status :: 5 - Production/Stable
@@ -69,29 +69,23 @@
 ```
 nhp-prep reorder-columns -i <directory_with_files_to_reorder_columns_OR_unique_CSV_file> -o <output_directory> -r <file_with_reference_columns>
 ```
 
 2. Rename the files to follow current standard (`rename`)
 
 ```
-nhp-prep rename -i <directory_files_to_rename_OR_uniques_CSV_file> -o <output_directory>
+nhp-prep rename -i <directory_files_to_rename> -o <output_directory>
 ```
 
 The current format for the file is: `YYYY-MM-DD_HHmmh_<experiment_name>_<Subject_name>_<Researcher_name_or_initials>_data.csv`
 
 3. Timestamp estimation trials from historical data files based on column <X> (`timestamp-estimate`)
 
 ```
-nhp-prep --timestamp-estimate -i <input_file>
-```
-
-Alternatively, you can pass the directory of the files to estimate the timestamp of each trial:
-
-```
-nhp-prep timestamp-estimate -i <directory_with_files_OR_unique_CSV_file>
+nhp-prep timestamp-estimate -i <directory_with_files_OR_unique_CSV_file> -o <output_directory>
 ```
 
 ##### **Since v0.3.0**
 
 Since the previous 3 steps are common across the different datasets collected, the dev team decided to merge them into one single command (`preparation-steps`):
 
 ```
```

### Comparing `nhp-prep-0.3.2/setup.py` & `nhp-prep-0.3.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 setup(
     name='nhp-prep',
-    version='0.3.2',
+    version='0.3.3',
     author='Hugo Angulo, Zijun Zhao',
     author_email='hugoanda@andrew.cmu.edu, zijunzha@andrew.cmu.edu',
     license='MIT',
     description='Pre-processing data tool for NHP Lab @ CMU',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://caoslab.psy.cmu.edu:32443/monkeylab/preprocessing-scripts',
```

