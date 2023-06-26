# Comparing `tmp/pollination-handlers-0.9.5.tar.gz` & `tmp/pollination-handlers-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-handlers-0.9.5.tar", last modified: Fri Mar 24 15:39:48 2023, max compression
+gzip compressed data, was "dist/pollination-handlers-0.9.6.tar", last modified: Fri Apr 14 14:17:18 2023, max compression
```

## Comparing `pollination-handlers-0.9.5.tar` & `pollination-handlers-0.9.6.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:39:48.000000 pollination-handlers-0.9.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:39:48.000000 pollination-handlers-0.9.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:39:48.000000 pollination-handlers-0.9.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-24 15:39:48.000000 pollination-handlers-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:39:48.000000 pollination-handlers-0.9.5/pollination_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:39:48.000000 pollination-handlers-0.9.5/pollination_handlers/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/inputs/bool_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/inputs/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/inputs/ddy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/inputs/emissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/inputs/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/inputs/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/inputs/north.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/inputs/pit.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/inputs/runperiod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/inputs/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/inputs/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/inputs/wea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:39:48.000000 pollination-handlers-0.9.5/pollination_handlers/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/outputs/comfort.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/outputs/daylight.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/outputs/eui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/outputs/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/pollination_handlers/outputs/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:39:48.000000 pollination-handlers-0.9.5/pollination_handlers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-24 15:39:48.000000 pollination-handlers-0.9.5/pollination_handlers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-03-24 15:39:48.000000 pollination-handlers-0.9.5/pollination_handlers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 15:39:48.000000 pollination-handlers-0.9.5/pollination_handlers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-24 15:39:48.000000 pollination-handlers-0.9.5/pollination_handlers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-24 15:39:48.000000 pollination-handlers-0.9.5/pollination_handlers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-24 15:39:48.000000 pollination-handlers-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:39:48.000000 pollination-handlers-0.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:39:48.000000 pollination-handlers-0.9.5/tests/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:39:48.000000 pollination-handlers-0.9.5/tests/assets/annual_dl_results/
--rw-r--r--   0 runner    (1001) docker     (123)   197920 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/assets/annual_dl_results/TestRoom_1.ill
--rw-r--r--   0 runner    (1001) docker     (123)   197908 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/assets/annual_dl_results/TestRoom_2.ill
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/assets/annual_dl_results/grids_info.json
--rw-r--r--   0 runner    (1001) docker     (123)    30306 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/assets/annual_dl_results/sun-up-hours.txt
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/assets/credit_summary.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:39:48.000000 pollination-handlers-0.9.5/tests/assets/df_results/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/assets/df_results/df_results.res
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/assets/df_results/grids_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/assets/eui.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 15:39:48.000000 pollination-handlers-0.9.5/tests/assets/hours_results/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/assets/hours_results/TestRoom_1.res
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/assets/hours_results/grids_info.json
--rw-r--r--   0 runner    (1001) docker     (123)    28793 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/assets/in.ddy
--rw-r--r--   0 runner    (1001) docker     (123)  1629361 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/assets/in.epw
--rw-r--r--   0 runner    (1001) docker     (123)   149364 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/assets/in.wea
--rw-r--r--   0 runner    (1001) docker     (123)    90398 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/assets/model_complete_simple.dfjson
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/assets/simulation_par_simple.json
--rw-r--r--   0 runner    (1001) docker     (123)   184350 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/assets/two_rooms.hbjson
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/input_data_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/input_ddy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/input_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/input_north_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/input_runperiod_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/input_schedule_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/input_simulation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/input_wea_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/output_daylight_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-24 15:38:28.000000 pollination-handlers-0.9.5/tests/output_eui_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:17:18.000000 pollination-handlers-0.9.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:17:18.000000 pollination-handlers-0.9.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:17:18.000000 pollination-handlers-0.9.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-14 14:17:18.000000 pollination-handlers-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:17:18.000000 pollination-handlers-0.9.6/pollination_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:17:18.000000 pollination-handlers-0.9.6/pollination_handlers/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/inputs/bool_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/inputs/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/inputs/ddy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/inputs/emissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/inputs/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/inputs/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/inputs/north.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/inputs/pit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/inputs/runperiod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/inputs/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/inputs/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/inputs/wea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:17:18.000000 pollination-handlers-0.9.6/pollination_handlers/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/outputs/comfort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/outputs/daylight.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/outputs/eui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/outputs/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/pollination_handlers/outputs/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:17:18.000000 pollination-handlers-0.9.6/pollination_handlers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-14 14:17:18.000000 pollination-handlers-0.9.6/pollination_handlers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-14 14:17:18.000000 pollination-handlers-0.9.6/pollination_handlers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:17:18.000000 pollination-handlers-0.9.6/pollination_handlers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 14:17:18.000000 pollination-handlers-0.9.6/pollination_handlers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-14 14:17:18.000000 pollination-handlers-0.9.6/pollination_handlers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 14:17:18.000000 pollination-handlers-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:17:18.000000 pollination-handlers-0.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:17:18.000000 pollination-handlers-0.9.6/tests/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:17:18.000000 pollination-handlers-0.9.6/tests/assets/annual_dl_results/
+-rw-r--r--   0 runner    (1001) docker     (123)   197920 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/assets/annual_dl_results/TestRoom_1.ill
+-rw-r--r--   0 runner    (1001) docker     (123)   197908 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/assets/annual_dl_results/TestRoom_2.ill
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/assets/annual_dl_results/grids_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30306 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/assets/annual_dl_results/sun-up-hours.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/assets/credit_summary.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:17:18.000000 pollination-handlers-0.9.6/tests/assets/df_results/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/assets/df_results/df_results.res
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/assets/df_results/grids_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/assets/eui.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:17:18.000000 pollination-handlers-0.9.6/tests/assets/hours_results/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/assets/hours_results/TestRoom_1.res
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/assets/hours_results/grids_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28793 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/assets/in.ddy
+-rw-r--r--   0 runner    (1001) docker     (123)  1629361 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/assets/in.epw
+-rw-r--r--   0 runner    (1001) docker     (123)   149364 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/assets/in.wea
+-rw-r--r--   0 runner    (1001) docker     (123)    90398 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/assets/model_complete_simple.dfjson
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/assets/simulation_par_simple.json
+-rw-r--r--   0 runner    (1001) docker     (123)   184350 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/assets/two_rooms.hbjson
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/input_data_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/input_ddy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/input_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/input_north_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/input_runperiod_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/input_schedule_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/input_simulation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/input_wea_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/output_daylight_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-14 14:16:06.000000 pollination-handlers-0.9.6/tests/output_eui_test.py
```

### Comparing `pollination-handlers-0.9.5/.github/workflows/ci.yaml` & `pollination-handlers-0.9.6/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/.gitignore` & `pollination-handlers-0.9.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/LICENSE` & `pollination-handlers-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/PKG-INFO` & `pollination-handlers-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-handlers
-Version: 0.9.5
+Version: 0.9.6
 Summary: Handlers to process Pollination recipes inputs and outputs.
 Home-page: https://github.com/pollination/handlers-python
 Author: Pollination
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pollination-handlers-0.9.5/pollination_handlers/inputs/bool_options.py` & `pollination-handlers-0.9.6/pollination_handlers/inputs/bool_options.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/pollination_handlers/inputs/data.py` & `pollination-handlers-0.9.6/pollination_handlers/inputs/data.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/pollination_handlers/inputs/ddy.py` & `pollination-handlers-0.9.6/pollination_handlers/inputs/ddy.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/pollination_handlers/inputs/emissions.py` & `pollination-handlers-0.9.6/pollination_handlers/inputs/emissions.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/pollination_handlers/inputs/helper.py` & `pollination-handlers-0.9.6/pollination_handlers/inputs/helper.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/pollination_handlers/inputs/model.py` & `pollination-handlers-0.9.6/pollination_handlers/inputs/model.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/pollination_handlers/inputs/north.py` & `pollination-handlers-0.9.6/pollination_handlers/inputs/north.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/pollination_handlers/inputs/pit.py` & `pollination-handlers-0.9.6/pollination_handlers/inputs/pit.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/pollination_handlers/inputs/runperiod.py` & `pollination-handlers-0.9.6/pollination_handlers/inputs/runperiod.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/pollination_handlers/inputs/schedule.py` & `pollination-handlers-0.9.6/pollination_handlers/inputs/schedule.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/pollination_handlers/inputs/simulation.py` & `pollination-handlers-0.9.6/pollination_handlers/inputs/simulation.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/pollination_handlers/inputs/wea.py` & `pollination-handlers-0.9.6/pollination_handlers/inputs/wea.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/pollination_handlers/outputs/comfort.py` & `pollination-handlers-0.9.6/pollination_handlers/outputs/comfort.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/pollination_handlers/outputs/daylight.py` & `pollination-handlers-0.9.6/pollination_handlers/outputs/daylight.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Handlers for daylight simulation."""
 import os
 import json
 
+from ladybug.datacollection import HourlyContinuousCollection
 from .helper import read_sensor_grid_result, read_grid_results
 
 
 def read_df_from_folder(result_folder):
     """Read daylight factor values from a folder with radiance .res result files."""
     return read_sensor_grid_result(result_folder, 'res', 'full_id')
 
@@ -101,7 +102,45 @@
         raise ValueError('Invalid file path: %s' % eui_json)
     with open(eui_json) as json_file:
         data = json.load(json_file)
     results = []
     for key in sorted(data.keys()):
         results.append('{}: {}'.format(key, data[key]))
     return results
+
+
+def read_leed_datacollection_from_folder(result_folder):
+    """Read LEED Daylight Option I datacollections """
+    # check that the required files are present
+    if not os.path.isdir(result_folder):
+        raise ValueError('Invalid result folder: %s' % result_folder)
+    grid_json = os.path.join(result_folder, 'grids_info.json')
+    if not os.path.isfile(grid_json):
+        raise ValueError('Result folder contains no grids_info.json.')
+
+    # load the list of grids and gather all of the results
+    with open(grid_json) as json_file:
+        grid_list = json.load(json_file)
+    results = []
+    for grid in grid_list:
+        grid_id = grid['full_id']
+        result_file = os.path.join(result_folder, '{}.{}'.format(grid_id, 'json'))
+        with open(result_file) as json_file:
+            data = json.load(json_file)
+            datacollection = HourlyContinuousCollection.from_dict(data)
+            results.append(datacollection)
+
+    return results
+
+
+def read_leed_shade_transmittance_schedule(shd_json):
+    """Read LEED Daylight Option I shade transmittance schedule."""
+    if not os.path.isfile(shd_json):
+        raise ValueError('Invalid file path: %s' % shd_json)
+    results = []
+    with open(shd_json) as json_file:
+        data = json.load(json_file)
+        for data_dict in data.values():
+            datacollection = HourlyContinuousCollection.from_dict(data_dict)
+            results.append(datacollection)
+
+    return results
```

### Comparing `pollination-handlers-0.9.5/pollination_handlers/outputs/eui.py` & `pollination-handlers-0.9.6/pollination_handlers/outputs/eui.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/pollination_handlers/outputs/helper.py` & `pollination-handlers-0.9.6/pollination_handlers/outputs/helper.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/pollination_handlers/outputs/summary.py` & `pollination-handlers-0.9.6/pollination_handlers/outputs/summary.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/pollination_handlers.egg-info/PKG-INFO` & `pollination-handlers-0.9.6/pollination_handlers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-handlers
-Version: 0.9.5
+Version: 0.9.6
 Summary: Handlers to process Pollination recipes inputs and outputs.
 Home-page: https://github.com/pollination/handlers-python
 Author: Pollination
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pollination-handlers-0.9.5/pollination_handlers.egg-info/SOURCES.txt` & `pollination-handlers-0.9.6/pollination_handlers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/setup.py` & `pollination-handlers-0.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/tests/assets/annual_dl_results/TestRoom_1.ill` & `pollination-handlers-0.9.6/tests/assets/annual_dl_results/TestRoom_1.ill`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/tests/assets/annual_dl_results/TestRoom_2.ill` & `pollination-handlers-0.9.6/tests/assets/annual_dl_results/TestRoom_2.ill`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/tests/assets/annual_dl_results/sun-up-hours.txt` & `pollination-handlers-0.9.6/tests/assets/annual_dl_results/sun-up-hours.txt`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/tests/assets/hours_results/TestRoom_1.res` & `pollination-handlers-0.9.6/tests/assets/hours_results/TestRoom_1.res`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/tests/assets/in.ddy` & `pollination-handlers-0.9.6/tests/assets/in.ddy`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/tests/assets/in.epw` & `pollination-handlers-0.9.6/tests/assets/in.epw`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/tests/assets/in.wea` & `pollination-handlers-0.9.6/tests/assets/in.wea`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/tests/assets/model_complete_simple.dfjson` & `pollination-handlers-0.9.6/tests/assets/model_complete_simple.dfjson`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/tests/assets/simulation_par_simple.json` & `pollination-handlers-0.9.6/tests/assets/simulation_par_simple.json`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/tests/assets/two_rooms.hbjson` & `pollination-handlers-0.9.6/tests/assets/two_rooms.hbjson`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/tests/input_data_test.py` & `pollination-handlers-0.9.6/tests/input_data_test.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/tests/input_ddy_test.py` & `pollination-handlers-0.9.6/tests/input_ddy_test.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/tests/input_model_test.py` & `pollination-handlers-0.9.6/tests/input_model_test.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/tests/input_schedule_test.py` & `pollination-handlers-0.9.6/tests/input_schedule_test.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/tests/input_simulation_test.py` & `pollination-handlers-0.9.6/tests/input_simulation_test.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/tests/input_wea_test.py` & `pollination-handlers-0.9.6/tests/input_wea_test.py`

 * *Files identical despite different names*

### Comparing `pollination-handlers-0.9.5/tests/output_daylight_test.py` & `pollination-handlers-0.9.6/tests/output_daylight_test.py`

 * *Files identical despite different names*

