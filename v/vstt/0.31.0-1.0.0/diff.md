# Comparing `tmp/vstt-0.31.0.tar.gz` & `tmp/vstt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstt-0.31.0.tar", last modified: Mon Jun 26 09:46:55 2023, max compression
+gzip compressed data, was "vstt-1.0.0.tar", last modified: Mon Jun 26 11:18:07 2023, max compression
```

## Comparing `vstt-0.31.0.tar` & `vstt-1.0.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:46:55.424498 vstt-0.31.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-26 09:46:46.000000 vstt-0.31.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-26 09:46:55.424498 vstt-0.31.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-26 09:46:46.000000 vstt-0.31.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-26 09:46:46.000000 vstt-0.31.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 09:46:55.424498 vstt-0.31.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:46:55.420498 vstt-0.31.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:46:55.420498 vstt-0.31.0/src/vstt/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/display_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/joystick_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/meta_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/results_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    16330 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/trials_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/update.py
--rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/vis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-26 09:46:46.000000 vstt-0.31.0/src/vstt/vtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:46:55.420498 vstt-0.31.0/src/vstt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-26 09:46:55.000000 vstt-0.31.0/src/vstt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-26 09:46:55.000000 vstt-0.31.0/src/vstt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:46:55.000000 vstt-0.31.0/src/vstt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 09:46:55.000000 vstt-0.31.0/src/vstt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-26 09:46:55.000000 vstt-0.31.0/src/vstt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 09:46:55.000000 vstt-0.31.0/src/vstt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:46:55.424498 vstt-0.31.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_display_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_joystick_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_meta_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_results_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_trials_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_vis.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-26 09:46:46.000000 vstt-0.31.0/tests/test_vstt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:18:07.963566 vstt-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-26 11:17:58.000000 vstt-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-26 11:18:07.963566 vstt-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-26 11:17:58.000000 vstt-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-26 11:17:58.000000 vstt-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 11:18:07.963566 vstt-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:18:07.959566 vstt-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:18:07.959566 vstt-1.0.0/src/vstt/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-26 11:17:58.000000 vstt-1.0.0/src/vstt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-26 11:17:58.000000 vstt-1.0.0/src/vstt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-26 11:17:58.000000 vstt-1.0.0/src/vstt/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-26 11:17:58.000000 vstt-1.0.0/src/vstt/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-26 11:17:58.000000 vstt-1.0.0/src/vstt/display_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-26 11:17:58.000000 vstt-1.0.0/src/vstt/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-26 11:17:58.000000 vstt-1.0.0/src/vstt/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-26 11:17:58.000000 vstt-1.0.0/src/vstt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-26 11:17:58.000000 vstt-1.0.0/src/vstt/joystick_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-26 11:17:58.000000 vstt-1.0.0/src/vstt/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-26 11:17:58.000000 vstt-1.0.0/src/vstt/meta_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-26 11:17:58.000000 vstt-1.0.0/src/vstt/results_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-06-26 11:17:58.000000 vstt-1.0.0/src/vstt/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17359 2023-06-26 11:17:58.000000 vstt-1.0.0/src/vstt/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-26 11:17:58.000000 vstt-1.0.0/src/vstt/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-26 11:17:58.000000 vstt-1.0.0/src/vstt/trials_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-26 11:17:58.000000 vstt-1.0.0/src/vstt/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-06-26 11:17:58.000000 vstt-1.0.0/src/vstt/vis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-26 11:17:58.000000 vstt-1.0.0/src/vstt/vtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:18:07.963566 vstt-1.0.0/src/vstt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-26 11:18:07.000000 vstt-1.0.0/src/vstt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-26 11:18:07.000000 vstt-1.0.0/src/vstt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 11:18:07.000000 vstt-1.0.0/src/vstt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 11:18:07.000000 vstt-1.0.0/src/vstt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-26 11:18:07.000000 vstt-1.0.0/src/vstt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 11:18:07.000000 vstt-1.0.0/src/vstt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:18:07.963566 vstt-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-26 11:17:58.000000 vstt-1.0.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-26 11:17:58.000000 vstt-1.0.0/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-26 11:17:58.000000 vstt-1.0.0/tests/test_display_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-06-26 11:17:58.000000 vstt-1.0.0/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-26 11:17:58.000000 vstt-1.0.0/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-26 11:17:58.000000 vstt-1.0.0/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-26 11:17:58.000000 vstt-1.0.0/tests/test_joystick_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-26 11:17:58.000000 vstt-1.0.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-26 11:17:58.000000 vstt-1.0.0/tests/test_meta_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-26 11:17:58.000000 vstt-1.0.0/tests/test_results_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-26 11:17:58.000000 vstt-1.0.0/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-06-26 11:17:58.000000 vstt-1.0.0/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-06-26 11:17:58.000000 vstt-1.0.0/tests/test_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-26 11:17:58.000000 vstt-1.0.0/tests/test_trials_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-26 11:17:58.000000 vstt-1.0.0/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-06-26 11:17:58.000000 vstt-1.0.0/tests/test_vis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-26 11:17:58.000000 vstt-1.0.0/tests/test_vstt.py
```

### Comparing `vstt-0.31.0/LICENSE` & `vstt-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/PKG-INFO` & `vstt-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstt
-Version: 0.31.0
+Version: 1.0.0
 Summary: Visuomotor Serial Targeting Task (VSTT)
 Author-email: Liam Keegan <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Project-URL: Github, https://github.com/ssciwr/vstt
 Project-URL: Issues, https://github.com/ssciwr/vstt/issues
 Project-URL: Documentation, https://vstt.readthedocs.io/
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `vstt-0.31.0/README.md` & `vstt-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/pyproject.toml` & `vstt-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/src/vstt/__main__.py` & `vstt-1.0.0/src/vstt/__main__.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/src/vstt/common.py` & `vstt-1.0.0/src/vstt/common.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/src/vstt/display.py` & `vstt-1.0.0/src/vstt/display.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/src/vstt/display_widget.py` & `vstt-1.0.0/src/vstt/display_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/src/vstt/experiment.py` & `vstt-1.0.0/src/vstt/experiment.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/src/vstt/geom.py` & `vstt-1.0.0/src/vstt/geom.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/src/vstt/gui.py` & `vstt-1.0.0/src/vstt/gui.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/src/vstt/joystick_wrapper.py` & `vstt-1.0.0/src/vstt/joystick_wrapper.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/src/vstt/meta.py` & `vstt-1.0.0/src/vstt/meta.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/src/vstt/meta_widget.py` & `vstt-1.0.0/src/vstt/meta_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/src/vstt/results_widget.py` & `vstt-1.0.0/src/vstt/results_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/src/vstt/stats.py` & `vstt-1.0.0/src/vstt/stats.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/src/vstt/task.py` & `vstt-1.0.0/src/vstt/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import numpy as np
+import vstt.vtypes
 from psychopy.clock import Clock
 from psychopy.data import TrialHandlerExt
 from psychopy.event import Mouse
 from psychopy.hardware.keyboard import Keyboard
 from psychopy.sound import Sound
 from psychopy.visual.basevisual import BaseVisualStim
 from psychopy.visual.elementarray import ElementArrayStim
@@ -56,33 +57,33 @@
         self.to_target_success: List[bool] = []
         self.to_center_success: List[bool] = []
 
 
 class TrialManager:
     """Stores the drawable elements and other objects needed during a trial"""
 
-    def __init__(self, win: Window, trial: Dict[str, Any], rng: np.random.Generator):
-        self.data = TrialData(trial, rng)
+    def __init__(self, win: Window, trial: vstt.vtypes.Trial):
         self.targets = vis.make_targets(
             win,
             trial["num_targets"],
             trial["target_distance"],
             trial["target_size"],
             trial["add_central_target"],
             trial["central_target_size"],
         )
-        self.target_labels = vis.make_target_labels(
-            win,
-            trial["num_targets"],
-            trial["target_distance"],
-            trial["target_size"],
-            trial["target_labels"],
-        )
         self.drawables: List[Union[BaseVisualStim, ElementArrayStim]] = [self.targets]
+        self.target_labels = None
         if trial["show_target_labels"]:
+            self.target_labels = vis.make_target_labels(
+                win,
+                trial["num_targets"],
+                trial["target_distance"],
+                trial["target_size"],
+                trial["target_labels"],
+            )
             self.drawables.extend(self.target_labels)
         self.cursor = vis.make_cursor(win, trial["cursor_size"])
         self.cursor.setPos(np.array([0.0, 0.0]))
         if trial["show_cursor"]:
             self.drawables.append(self.cursor)
         self.point_rotator = PointRotator(trial["cursor_rotation_degrees"])
         self.joystick_point_updater = JoystickPointUpdater(
@@ -126,14 +127,18 @@
         self.experiment = experiment
         if win is None:
             win = Window(fullscr=True, units="height")
             self.close_window_when_done = True
         self.win = win
         if not experiment.trial_list:
             return
+        self.trial_managers = {
+            condition_index: TrialManager(self.win, trial)
+            for condition_index, trial in enumerate(experiment.trial_list)
+        }
         self.trial_handler = experiment.create_trialhandler()
         self.mouse = Mouse(visible=False, win=win)
         self.kb = Keyboard()
         self.js = joystick_wrapper.get_joystick()
         self.rng = np.random.default_rng()
 
     def run(self) -> bool:
@@ -160,30 +165,35 @@
         condition_trial_indices: List[List[int]] = [
             [] for _ in self.trial_handler.trialList
         ]
         current_condition_index = -1
         current_condition_first_trial_index = 0
         current_condition_clock = Clock()
         current_condition_max_time = 0.0
+        self.mouse.setPos((0.0, 0.0))
+        current_cursor_pos = (0.0, 0.0)
         for trial in self.trial_handler:
             if self.trial_handler.thisIndex != current_condition_index:
                 # starting a new set of conditions
                 current_condition_clock.reset()
                 current_condition_max_time = trial["condition_timeout"]
                 current_condition_index = self.trial_handler.thisIndex
                 current_condition_first_trial_index = self.trial_handler.thisTrialN
+                trial_manager = self.trial_managers[current_condition_index]
             condition_trial_indices[self.trial_handler.thisIndex].append(
                 self.trial_handler.thisTrialN
             )
             if (
                 current_condition_max_time == 0.0
                 or current_condition_clock.getTime() < current_condition_max_time
             ):
                 # only do the trial if there is still time left for this condition
-                self._do_trial(trial)
+                current_cursor_pos = self._do_trial(
+                    trial, trial_manager, current_cursor_pos
+                )
             is_final_trial_of_block = (
                 len(condition_trial_indices[self.trial_handler.thisIndex])
                 == trial["weight"]
             )
             if is_final_trial_of_block and trial["post_block_delay"] > 0:
                 vis.display_results(
                     trial["post_block_delay"],
@@ -203,114 +213,132 @@
             display_time_seconds=self.experiment.metadata["display_duration"],
             enter_to_skip_delay=self.experiment.metadata["enter_to_skip_delay"],
             show_delay_countdown=self.experiment.metadata["show_delay_countdown"],
             metadata=self.experiment.metadata,
             win=self.win,
         )
 
-    def _do_trial(self, trial: Dict[str, Any]) -> None:
+    def _do_trial(
+        self,
+        trial: Dict[str, Any],
+        trial_manager: TrialManager,
+        initial_cursor_pos: Tuple[float, float],
+    ) -> Tuple[float, float]:
         if trial["use_joystick"] and self.js is None:
             raise RuntimeError("Use joystick option is enabled, but no joystick found.")
-        tm = TrialManager(self.win, trial, self.rng)
-        self.mouse.setPos(tm.cursor.pos)
+        trial_manager.cursor.setPos(initial_cursor_pos)
+        trial_data = TrialData(trial, self.rng)
         self.win.recordFrameIntervals = True
-        tm.clock.reset()
-        vis.update_target_colors(tm.targets, trial["show_inactive_targets"], None)
-        if trial["show_target_labels"]:
+        trial_manager.clock.reset()
+        vis.update_target_colors(
+            trial_manager.targets, trial["show_inactive_targets"], None
+        )
+        if trial["show_target_labels"] and trial_manager.target_labels is not None:
             vis.update_target_label_colors(
-                tm.target_labels, trial["show_inactive_targets"], None
+                trial_manager.target_labels, trial["show_inactive_targets"], None
             )
-        for index in tm.data.target_indices:
-            self._do_target(trial, index, tm)
+        for index in trial_data.target_indices:
+            self._do_target(trial, index, trial_manager, trial_data)
         self.win.recordFrameIntervals = False
         if trial["automove_cursor_to_center"]:
-            tm.data.to_center_success = [True] * trial["num_targets"]
-        add_trial_data_to_trial_handler(tm.data, self.trial_handler)
+            trial_data.to_center_success = [True] * trial["num_targets"]
+        add_trial_data_to_trial_handler(trial_data, self.trial_handler)
         if trial["post_trial_delay"] > 0:
             vis.display_results(
                 trial["post_trial_delay"],
                 trial["enter_to_skip_delay"],
                 trial["show_delay_countdown"],
                 self.trial_handler if trial["post_trial_display_results"] else None,
                 self.experiment.display_options,
                 self.trial_handler.thisTrialN,
                 False,
                 self.win,
             )
+        return trial_manager.cursor.pos
 
-    def _do_target(self, trial: Dict[str, Any], index: int, tm: TrialManager) -> None:
+    def _do_target(
+        self, trial: Dict[str, Any], index: int, tm: TrialManager, trial_data: TrialData
+    ) -> None:
         minimum_window_for_flip = 1.0 / 60.0
         mouse_pos = tm.cursor.pos
         stop_waiting_time = 0.0
         stop_target_time = 0.0
         if trial["fixed_target_intervals"]:
-            num_completed_targets = len(tm.data.to_target_timestamps)
+            num_completed_targets = len(trial_data.to_target_timestamps)
             stop_waiting_time = (num_completed_targets + 1) * trial["target_duration"]
             stop_target_time = stop_waiting_time + trial["target_duration"]
         for target_index in _get_target_indices(index, trial):
             t0 = tm.clock.getTime()
             is_central_target = target_index == trial["num_targets"]
             mouse_times = []
             mouse_positions = []
+            # current target is not yet displayed
             if not is_central_target:
                 if trial["automove_cursor_to_center"]:
                     mouse_pos = np.array([0.0, 0.0])
                     self.mouse.setPos(mouse_pos)
                     tm.cursor.setPos(mouse_pos)
                 tm.cursor_path_add_vertex(mouse_pos, clear_existing=True)
-                if not trial["fixed_target_intervals"]:
-                    stop_waiting_time = t0 + trial["inter_target_duration"]
-                if stop_waiting_time > t0:
-                    if trial["hide_target_when_reached"]:
-                        vis.update_target_colors(
-                            tm.targets, trial["show_inactive_targets"], None
+            if not trial["fixed_target_intervals"]:
+                if is_central_target:
+                    pre_target_delay = trial["pre_central_target_delay"]
+                else:
+                    pre_target_delay = trial["pre_target_delay"]
+                stop_waiting_time = t0 + pre_target_delay
+            if stop_waiting_time > t0:
+                if trial["hide_target_when_reached"]:
+                    vis.update_target_colors(
+                        tm.targets, trial["show_inactive_targets"], None
+                    )
+                    if trial["show_target_labels"] and tm.target_labels is not None:
+                        vis.update_target_label_colors(
+                            tm.target_labels, trial["show_inactive_targets"], None
                         )
-                        if trial["show_target_labels"]:
-                            vis.update_target_label_colors(
-                                tm.target_labels, trial["show_inactive_targets"], None
+                # ensure we get at least a single flip
+                should_continue_waiting = True
+                while should_continue_waiting:
+                    if trial["freeze_cursor_between_targets"]:
+                        self.mouse.setPos(mouse_pos)
+                    vis.draw_and_flip(self.win, tm.drawables, self.kb)
+                    if not trial["freeze_cursor_between_targets"]:
+                        if trial["use_joystick"]:
+                            mouse_pos = tm.joystick_point_updater(
+                                mouse_pos, (self.js.getX(), self.js.getY())  # type: ignore
                             )
-                    # ensure we get at least a single flip
-                    should_continue_waiting = True
-                    while should_continue_waiting:
-                        if trial["freeze_cursor_between_targets"]:
-                            self.mouse.setPos(mouse_pos)
-                        vis.draw_and_flip(self.win, tm.drawables, self.kb)
-                        if not trial["freeze_cursor_between_targets"]:
-                            if trial["use_joystick"]:
-                                mouse_pos = tm.joystick_point_updater(
-                                    mouse_pos, (self.js.getX(), self.js.getY())  # type: ignore
-                                )
-                            else:
-                                mouse_pos = tm.point_rotator(self.mouse.getPos())
-                        mouse_times.append(tm.clock.getTime())
-                        mouse_positions.append(mouse_pos)
-                        if trial["show_cursor"]:
-                            tm.cursor.setPos(mouse_pos)
-                        if trial["show_cursor_path"]:
-                            tm.cursor_path_add_vertex(mouse_pos)
-                        should_continue_waiting = (
-                            tm.clock.getTime() + minimum_window_for_flip
-                            < stop_waiting_time
-                        )
+                        else:
+                            mouse_pos = tm.point_rotator(self.mouse.getPos())
+                    mouse_times.append(tm.clock.getTime())
+                    mouse_positions.append(mouse_pos)
+                    if trial["show_cursor"]:
+                        tm.cursor.setPos(mouse_pos)
+                    if trial["show_cursor_path"]:
+                        tm.cursor_path_add_vertex(mouse_pos)
+                    should_continue_waiting = (
+                        tm.clock.getTime() + minimum_window_for_flip < stop_waiting_time
+                    )
             # display current target
             t0 = tm.clock.getTime()
             vis.update_target_colors(
                 tm.targets, trial["show_inactive_targets"], target_index
             )
-            if trial["show_target_labels"]:
+            if trial["show_target_labels"] and tm.target_labels is not None:
                 vis.update_target_label_colors(
                     tm.target_labels, trial["show_inactive_targets"], target_index
                 )
             if trial["play_sound"]:
                 Sound("A", secs=0.3, blockSize=1024, stereo=True).play()
             if is_central_target:
-                tm.data.to_center_num_timestamps_before_visible.append(len(mouse_times))
+                trial_data.to_center_num_timestamps_before_visible.append(
+                    len(mouse_times)
+                )
             else:
-                tm.data.target_pos.append(tm.targets.xys[target_index])
-                tm.data.to_target_num_timestamps_before_visible.append(len(mouse_times))
+                trial_data.target_pos.append(tm.targets.xys[target_index])
+                trial_data.to_target_num_timestamps_before_visible.append(
+                    len(mouse_times)
+                )
             target_size = trial["target_size"]
             if is_central_target:
                 target_size = trial["central_target_size"]
             if not trial["fixed_target_intervals"]:
                 if is_central_target:
                     stop_target_time = t0 + trial["central_target_duration"]
                 else:
@@ -347,21 +375,21 @@
                     and tm.clock.getTime() + minimum_window_for_flip < stop_target_time
                 )
             success = (
                 dist_correct <= target_size
                 and tm.clock.getTime() + minimum_window_for_flip < stop_target_time
             )
             if is_central_target:
-                tm.data.to_center_success.append(success)
+                trial_data.to_center_success.append(success)
             else:
-                tm.data.to_target_success.append(success)
+                trial_data.to_target_success.append(success)
             if is_central_target:
-                tm.data.to_center_timestamps.append(np.array(mouse_times))
-                tm.data.to_center_mouse_positions.append(np.array(mouse_positions))
+                trial_data.to_center_timestamps.append(np.array(mouse_times))
+                trial_data.to_center_mouse_positions.append(np.array(mouse_positions))
             else:
-                tm.data.to_target_timestamps.append(np.array(mouse_times))
-                tm.data.to_target_mouse_positions.append(np.array(mouse_positions))
+                trial_data.to_target_timestamps.append(np.array(mouse_times))
+                trial_data.to_target_mouse_positions.append(np.array(mouse_positions))
 
     def _clean_up_and_return(self, return_value: bool) -> bool:
         if self.win is not None and self.close_window_when_done:
             self.win.close()
         return return_value
```

### Comparing `vstt-0.31.0/src/vstt/trial.py` & `vstt-1.0.0/src/vstt/trial.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,16 @@
         "add_central_target": True,
         "hide_target_when_reached": True,
         "show_target_labels": False,
         "target_labels": "0 1 2 3 4 5 6 7",
         "fixed_target_intervals": False,
         "target_duration": 5.0,
         "central_target_duration": 5.0,
-        "inter_target_duration": 0.0,
+        "pre_target_delay": 0.0,
+        "pre_central_target_delay": 0.0,
         "target_distance": 0.4,
         "target_size": 0.04,
         "central_target_size": 0.02,
         "show_inactive_targets": True,
         "ignore_incorrect_targets": True,
         "play_sound": True,
         "use_joystick": False,
@@ -74,15 +75,16 @@
         "add_central_target": "Add a central target",
         "hide_target_when_reached": "Hide target when reached",
         "show_target_labels": "Display target labels",
         "target_labels": "Target labels",
         "fixed_target_intervals": "Fixed target display intervals",
         "target_duration": "Target display duration (secs)",
         "central_target_duration": "Central target display duration (secs)",
-        "inter_target_duration": "Delay between targets (secs)",
+        "pre_target_delay": "Delay before outer target display (secs)",
+        "pre_central_target_delay": "Delay before central target display (secs)",
         "target_distance": "Distance to targets (screen height fraction)",
         "target_size": "Target size (screen height fraction)",
         "central_target_size": "Central target size (screen height fraction)",
         "show_inactive_targets": "Show inactive targets",
         "ignore_incorrect_targets": "Ignore cursor hitting incorrect target",
         "play_sound": "Play a sound on target display",
         "use_joystick": "Control the cursor using a joystick",
@@ -125,15 +127,16 @@
 def import_and_validate_trial(trial_or_dict: Mapping[str, Any]) -> Trial:
     trial = import_typed_dict(trial_or_dict, default_trial())
     # make any negative time durations zero
     for duration in [
         "condition_timeout",
         "target_duration",
         "central_target_duration",
-        "inter_target_duration",
+        "pre_target_delay",
+        "pre_central_target_delay",
         "post_trial_delay",
         "post_block_delay",
     ]:
         if trial[duration] < 0.0:  # type: ignore
             trial[duration] = 0.0  # type: ignore
     # convert string of target indices to a numpy array of ints
     target_indices = np.fromstring(trial["target_indices"], dtype="int", sep=" ")
```

### Comparing `vstt-0.31.0/src/vstt/trials_widget.py` & `vstt-1.0.0/src/vstt/trials_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/src/vstt/update.py` & `vstt-1.0.0/src/vstt/update.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/src/vstt/vis.py` & `vstt-1.0.0/src/vstt/vis.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/src/vstt/vtypes.py` & `vstt-1.0.0/src/vstt/vtypes.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     add_central_target: bool
     hide_target_when_reached: bool
     show_target_labels: bool
     target_labels: str
     fixed_target_intervals: bool
     target_duration: float
     central_target_duration: float
-    inter_target_duration: float
+    pre_target_delay: float
+    pre_central_target_delay: float
     target_distance: float
     target_size: float
     central_target_size: float
     show_inactive_targets: bool
     ignore_incorrect_targets: bool
     play_sound: bool
     use_joystick: bool
```

### Comparing `vstt-0.31.0/src/vstt.egg-info/PKG-INFO` & `vstt-1.0.0/src/vstt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstt
-Version: 0.31.0
+Version: 1.0.0
 Summary: Visuomotor Serial Targeting Task (VSTT)
 Author-email: Liam Keegan <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Project-URL: Github, https://github.com/ssciwr/vstt
 Project-URL: Issues, https://github.com/ssciwr/vstt/issues
 Project-URL: Documentation, https://vstt.readthedocs.io/
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `vstt-0.31.0/src/vstt.egg-info/SOURCES.txt` & `vstt-1.0.0/src/vstt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/tests/test_display.py` & `vstt-1.0.0/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/tests/test_display_widget.py` & `vstt-1.0.0/tests/test_display_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/tests/test_experiment.py` & `vstt-1.0.0/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/tests/test_geom.py` & `vstt-1.0.0/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/tests/test_gui.py` & `vstt-1.0.0/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/tests/test_joystick_wrapper.py` & `vstt-1.0.0/tests/test_joystick_wrapper.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/tests/test_meta.py` & `vstt-1.0.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/tests/test_meta_widget.py` & `vstt-1.0.0/tests/test_meta_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/tests/test_results_widget.py` & `vstt-1.0.0/tests/test_results_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/tests/test_stats.py` & `vstt-1.0.0/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/tests/test_task.py` & `vstt-1.0.0/tests/test_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,16 @@
     experiment = Experiment()
     experiment.metadata["display_duration"] = 0.0
     trial1 = vstt.trial.default_trial()
     trial1["weight"] = 100
     trial1["condition_timeout"] = 4.0
     trial1["num_targets"] = 1
     trial1["target_duration"] = 2.1
-    trial1["inter_target_duration"] = 0.0
+    trial1["pre_target_delay"] = 0.0
+    trial1["pre_central_target_delay"] = 0.0
     trial1["add_central_target"] = False
     trial1["automove_cursor_to_center"] = False
     trial1["freeze_cursor_between_targets"] = False
     trial1["post_block_delay"] = 0.0
     trial1["play_sound"] = False
     # then a second copy but with 3 targets, each for 0.4 seconds, and a 1-second condition timeout -> single trial
     trial2 = deepcopy(trial1)
```

### Comparing `vstt-0.31.0/tests/test_trial.py` & `vstt-1.0.0/tests/test_trial.py`

 * *Files 16% similar despite different names*

```diff
@@ -54,15 +54,16 @@
         "add_central_target": True,
         "show_target_labels": False,
         "hide_target_when_reached": True,
         "target_labels": "0 1 2 3 4 5",
         "fixed_target_intervals": False,
         "target_duration": 3,
         "central_target_duration": 3,
-        "inter_target_duration": 0,
+        "pre_target_delay": 0,
+        "pre_central_target_delay": 0,
         "target_distance": 0.3,
         "target_size": 0.03,
         "central_target_size": 0.01,
         "show_inactive_targets": False,
         "ignore_incorrect_targets": True,
         "play_sound": True,
         "use_joystick": True,
@@ -108,33 +109,37 @@
 
 
 def test_validate_trial_durations() -> None:
     trial = vstt.trial.default_trial()
     # positive durations are not modified
     trial["target_duration"] = 1
     trial["central_target_duration"] = 1
-    trial["inter_target_duration"] = 0.1
+    trial["pre_target_delay"] = 0.1
+    trial["pre_central_target_delay"] = 0.087
     trial["post_trial_delay"] = 0.2
     trial["post_block_delay"] = 0.7
     vtrial = vstt.trial.import_and_validate_trial(trial)
     assert vtrial["target_duration"] == 1
     assert vtrial["central_target_duration"] == 1
-    assert vtrial["inter_target_duration"] == 0.1
+    assert vtrial["pre_target_delay"] == 0.1
+    assert vtrial["pre_central_target_delay"] == 0.087
     assert vtrial["post_trial_delay"] == 0.2
     assert vtrial["post_block_delay"] == 0.7
     # negative durations are cast to zero
     trial["target_duration"] = -1
     trial["central_target_duration"] = -0.8
-    trial["inter_target_duration"] = -0.1
+    trial["pre_target_delay"] = -0.1
+    trial["pre_central_target_delay"] = -0.087
     trial["post_trial_delay"] = -0.2
     trial["post_block_delay"] = -0.7
     vtrial = vstt.trial.import_and_validate_trial(trial)
     assert vtrial["target_duration"] == 0
     assert vtrial["central_target_duration"] == 0
-    assert vtrial["inter_target_duration"] == 0
+    assert vtrial["pre_target_delay"] == 0
+    assert vtrial["pre_central_target_delay"] == 0
     assert vtrial["post_trial_delay"] == 0
     assert vtrial["post_block_delay"] == 0
 
 
 def test_validate_trial_target_order() -> None:
     trial = vstt.trial.default_trial()
     assert isinstance(trial["target_indices"], str)
```

### Comparing `vstt-0.31.0/tests/test_trials_widget.py` & `vstt-1.0.0/tests/test_trials_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/tests/test_update.py` & `vstt-1.0.0/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `vstt-0.31.0/tests/test_vis.py` & `vstt-1.0.0/tests/test_vis.py`

 * *Files identical despite different names*

