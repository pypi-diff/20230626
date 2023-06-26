# Comparing `tmp/vstt-0.30.0.tar.gz` & `tmp/vstt-0.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstt-0.30.0.tar", last modified: Fri Jun  9 13:19:24 2023, max compression
+gzip compressed data, was "vstt-0.31.0.tar", last modified: Mon Jun 26 09:46:55 2023, max compression
```

## Comparing `vstt-0.30.0.tar` & `vstt-0.31.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:19:24.887920 vstt-0.30.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-09 13:19:15.000000 vstt-0.30.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-09 13:19:24.887920 vstt-0.30.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-09 13:19:15.000000 vstt-0.30.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-09 13:19:15.000000 vstt-0.30.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 13:19:24.887920 vstt-0.30.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:19:24.883920 vstt-0.30.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:19:24.887920 vstt-0.30.0/src/vstt/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/display_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/joystick_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/meta_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/results_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    16330 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/trials_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/update.py
--rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/vis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/vtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:19:24.887920 vstt-0.30.0/src/vstt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-09 13:19:24.000000 vstt-0.30.0/src/vstt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-09 13:19:24.000000 vstt-0.30.0/src/vstt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:19:24.000000 vstt-0.30.0/src/vstt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-09 13:19:24.000000 vstt-0.30.0/src/vstt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-09 13:19:24.000000 vstt-0.30.0/src/vstt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 13:19:24.000000 vstt-0.30.0/src/vstt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:19:24.887920 vstt-0.30.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_display_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_joystick_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_meta_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_results_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_trials_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_vis.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_vstt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:46:55.424498 vstt-0.31.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-26 09:46:46.000000 vstt-0.31.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-26 09:46:55.424498 vstt-0.31.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-26 09:46:46.000000 vstt-0.31.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-26 09:46:46.000000 vstt-0.31.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 09:46:55.424498 vstt-0.31.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:46:55.420498 vstt-0.31.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:46:55.420498 vstt-0.31.0/src/vstt/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/display_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/joystick_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/meta_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/results_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16330 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/trials_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/vis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/vtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:46:55.420498 vstt-0.31.0/src/vstt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-26 09:46:55.000000 vstt-0.31.0/src/vstt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-26 09:46:55.000000 vstt-0.31.0/src/vstt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:46:55.000000 vstt-0.31.0/src/vstt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 09:46:55.000000 vstt-0.31.0/src/vstt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-26 09:46:55.000000 vstt-0.31.0/src/vstt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 09:46:55.000000 vstt-0.31.0/src/vstt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:46:55.424498 vstt-0.31.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_display_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_joystick_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_meta_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_results_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_trials_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_vis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_vstt.py
```

### Comparing `vstt-0.30.0/LICENSE` & `vstt-0.31.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/PKG-INFO` & `vstt-0.31.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstt
-Version: 0.30.0
+Version: 0.31.0
 Summary: Visuomotor Serial Targeting Task (VSTT)
 Author-email: Liam Keegan <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Project-URL: Github, https://github.com/ssciwr/vstt
 Project-URL: Issues, https://github.com/ssciwr/vstt/issues
 Project-URL: Documentation, https://vstt.readthedocs.io/
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `vstt-0.30.0/README.md` & `vstt-0.31.0/README.md`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/pyproject.toml` & `vstt-0.31.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/src/vstt/__main__.py` & `vstt-0.31.0/src/vstt/__main__.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/src/vstt/common.py` & `vstt-0.31.0/src/vstt/common.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/src/vstt/display.py` & `vstt-0.31.0/src/vstt/display.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/src/vstt/display_widget.py` & `vstt-0.31.0/src/vstt/display_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/src/vstt/experiment.py` & `vstt-0.31.0/src/vstt/experiment.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/src/vstt/geom.py` & `vstt-0.31.0/src/vstt/geom.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/src/vstt/gui.py` & `vstt-0.31.0/src/vstt/gui.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/src/vstt/joystick_wrapper.py` & `vstt-0.31.0/src/vstt/joystick_wrapper.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/src/vstt/meta.py` & `vstt-0.31.0/src/vstt/meta.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/src/vstt/meta_widget.py` & `vstt-0.31.0/src/vstt/meta_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/src/vstt/results_widget.py` & `vstt-0.31.0/src/vstt/results_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/src/vstt/stats.py` & `vstt-0.31.0/src/vstt/stats.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/src/vstt/task.py` & `vstt-0.31.0/src/vstt/task.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/src/vstt/trial.py` & `vstt-0.31.0/src/vstt/trial.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,54 +30,54 @@
     return {
         "weight": 1,
         "condition_timeout": 0.0,
         "num_targets": 8,
         "target_order": "clockwise",
         "target_indices": "0 1 2 3 4 5 6 7",
         "add_central_target": True,
-        "show_target_labels": False,
         "hide_target_when_reached": True,
+        "show_target_labels": False,
         "target_labels": "0 1 2 3 4 5 6 7",
         "fixed_target_intervals": False,
         "target_duration": 5.0,
         "central_target_duration": 5.0,
-        "inter_target_duration": 1.0,
+        "inter_target_duration": 0.0,
         "target_distance": 0.4,
         "target_size": 0.04,
         "central_target_size": 0.02,
         "show_inactive_targets": True,
         "ignore_incorrect_targets": True,
         "play_sound": True,
         "use_joystick": False,
         "joystick_max_speed": 0.02,
         "show_cursor": True,
         "cursor_size": 0.02,
         "show_cursor_path": True,
-        "automove_cursor_to_center": True,
-        "freeze_cursor_between_targets": True,
+        "automove_cursor_to_center": False,
+        "freeze_cursor_between_targets": False,
         "cursor_rotation_degrees": 0.0,
         "post_trial_delay": 0.0,
         "post_trial_display_results": False,
-        "post_block_delay": 5.0,
+        "post_block_delay": 10.0,
         "post_block_display_results": True,
         "show_delay_countdown": True,
         "enter_to_skip_delay": True,
     }
 
 
 def trial_labels() -> Dict:
     return {
         "weight": "Repetitions",
         "condition_timeout": "Maximum time, 0=unlimited (secs)",
         "num_targets": "Number of targets",
         "target_order": "Target order",
         "target_indices": "Target indices",
         "add_central_target": "Add a central target",
-        "show_target_labels": "Display target labels",
         "hide_target_when_reached": "Hide target when reached",
+        "show_target_labels": "Display target labels",
         "target_labels": "Target labels",
         "fixed_target_intervals": "Fixed target display intervals",
         "target_duration": "Target display duration (secs)",
         "central_target_duration": "Central target display duration (secs)",
         "inter_target_duration": "Delay between targets (secs)",
         "target_distance": "Distance to targets (screen height fraction)",
         "target_size": "Target size (screen height fraction)",
@@ -92,15 +92,15 @@
         "show_cursor_path": "Show cursor path",
         "automove_cursor_to_center": "Automatically move cursor to center",
         "freeze_cursor_between_targets": "Freeze cursor until target is displayed",
         "cursor_rotation_degrees": "Cursor rotation (degrees)",
         "post_trial_delay": "Delay between trials (secs)",
         "post_trial_display_results": "Display results after each trial",
         "post_block_delay": "Delay after last trial (secs)",
-        "post_block_display_results": "Display results after this block",
+        "post_block_display_results": "Display combined results after last trial",
         "show_delay_countdown": "Display a countdown during delays",
         "enter_to_skip_delay": "Skip delay by pressing enter key",
     }
 
 
 def get_trial_from_user(
     initial_trial: Optional[Trial] = None,
@@ -111,15 +111,15 @@
         trial = default_trial()
     order_of_targets = [trial["target_order"]]
     for target_order in ["clockwise", "anti-clockwise", "random", "fixed"]:
         if target_order != order_of_targets[0]:
             order_of_targets.append(target_order)
     trial["target_order"] = order_of_targets
     dialog = DlgFromDict(
-        trial, title="Trial settings", labels=trial_labels(), sortKeys=False
+        trial, title="Trial conditions", labels=trial_labels(), sortKeys=False
     )
     if not dialog.OK:
         return None
     return import_and_validate_trial(trial)
 
 
 def import_and_validate_trial(trial_or_dict: Mapping[str, Any]) -> Trial:
```

### Comparing `vstt-0.30.0/src/vstt/trials_widget.py` & `vstt-0.31.0/src/vstt/trials_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/src/vstt/update.py` & `vstt-0.31.0/src/vstt/update.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/src/vstt/vis.py` & `vstt-0.31.0/src/vstt/vis.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/src/vstt/vtypes.py` & `vstt-0.31.0/src/vstt/vtypes.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 class Trial(TypedDict):
     weight: int
     condition_timeout: float
     num_targets: int
     target_order: Union[str, List]
     target_indices: str
     add_central_target: bool
-    show_target_labels: bool
     hide_target_when_reached: bool
+    show_target_labels: bool
     target_labels: str
     fixed_target_intervals: bool
     target_duration: float
     central_target_duration: float
     inter_target_duration: float
     target_distance: float
     target_size: float
```

### Comparing `vstt-0.30.0/src/vstt.egg-info/PKG-INFO` & `vstt-0.31.0/src/vstt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstt
-Version: 0.30.0
+Version: 0.31.0
 Summary: Visuomotor Serial Targeting Task (VSTT)
 Author-email: Liam Keegan <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Project-URL: Github, https://github.com/ssciwr/vstt
 Project-URL: Issues, https://github.com/ssciwr/vstt/issues
 Project-URL: Documentation, https://vstt.readthedocs.io/
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `vstt-0.30.0/src/vstt.egg-info/SOURCES.txt` & `vstt-0.31.0/src/vstt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/tests/test_display.py` & `vstt-0.31.0/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/tests/test_display_widget.py` & `vstt-0.31.0/tests/test_display_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/tests/test_experiment.py` & `vstt-0.31.0/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/tests/test_geom.py` & `vstt-0.31.0/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/tests/test_gui.py` & `vstt-0.31.0/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/tests/test_joystick_wrapper.py` & `vstt-0.31.0/tests/test_joystick_wrapper.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/tests/test_meta.py` & `vstt-0.31.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/tests/test_meta_widget.py` & `vstt-0.31.0/tests/test_meta_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/tests/test_results_widget.py` & `vstt-0.31.0/tests/test_results_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/tests/test_stats.py` & `vstt-0.31.0/tests/test_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             df.loc[df.condition_index == i]["i_target"].unique(),
             list(range(targets[i])),
         )
 
 
 def test_stats_df(experiment_with_results: Experiment) -> None:
     df = vstt.stats.stats_dataframe(experiment_with_results.trial_handler_with_results)
-    assert np.alltrue(np.isnan(df.loc[df.condition_index == 1]["to_center_time"]))
+    assert np.all(np.isnan(df.loc[df.condition_index == 1]["to_center_time"]))
     for destination, stat_label_units in vstt.stats.list_dest_stat_label_units():
         for stat, label, unit in stat_label_units:
             assert stat in df.columns
 
 
 def test_distance() -> None:
     assert np.allclose(vstt.stats._distance(np.array([[0, 0]])), [0])
```

### Comparing `vstt-0.30.0/tests/test_task.py` & `vstt-0.31.0/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/tests/test_trial.py` & `vstt-0.31.0/tests/test_trial.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/tests/test_trials_widget.py` & `vstt-0.31.0/tests/test_trials_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/tests/test_update.py` & `vstt-0.31.0/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `vstt-0.30.0/tests/test_vis.py` & `vstt-0.31.0/tests/test_vis.py`

 * *Files identical despite different names*

