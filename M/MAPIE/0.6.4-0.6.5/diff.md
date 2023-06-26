# Comparing `tmp/MAPIE-0.6.4.tar.gz` & `tmp/MAPIE-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MAPIE-0.6.4.tar", last modified: Wed Apr  5 09:21:05 2023, max compression
+gzip compressed data, was "MAPIE-0.6.5.tar", last modified: Mon Jun 26 18:12:11 2023, max compression
```

## Comparing `MAPIE-0.6.4.tar` & `MAPIE-0.6.5.tar`

### file list

```diff
@@ -1,77 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:21:05.692098 MAPIE-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-05 09:20:57.000000 MAPIE-0.6.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-05 09:20:57.000000 MAPIE-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-05 09:20:57.000000 MAPIE-0.6.4/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:21:05.684098 MAPIE-0.6.4/MAPIE.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-04-05 09:21:05.000000 MAPIE-0.6.4/MAPIE.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-05 09:21:05.000000 MAPIE-0.6.4/MAPIE.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 09:21:05.000000 MAPIE-0.6.4/MAPIE.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 09:21:05.000000 MAPIE-0.6.4/MAPIE.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-05 09:21:05.000000 MAPIE-0.6.4/MAPIE.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-05 09:21:05.000000 MAPIE-0.6.4/MAPIE.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-04-05 09:21:05.692098 MAPIE-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-04-05 09:20:57.000000 MAPIE-0.6.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:21:05.684098 MAPIE-0.6.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:21:05.684098 MAPIE-0.6.4/examples/classification/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:21:05.684098 MAPIE-0.6.4/examples/classification/1-quickstart/
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-04-05 09:20:57.000000 MAPIE-0.6.4/examples/classification/1-quickstart/plot_comp_methods_on_2d_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:21:05.684098 MAPIE-0.6.4/examples/classification/3-scientific-articles/
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-05 09:20:57.000000 MAPIE-0.6.4/examples/classification/3-scientific-articles/plot_sadinle2019_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:21:05.684098 MAPIE-0.6.4/examples/classification/4-tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-04-05 09:20:57.000000 MAPIE-0.6.4/examples/classification/4-tutorials/plot_crossconformal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10647 2023-04-05 09:20:57.000000 MAPIE-0.6.4/examples/classification/4-tutorials/plot_main-tutorial-classification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:21:05.684098 MAPIE-0.6.4/examples/multilabel_classification/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:21:05.688098 MAPIE-0.6.4/examples/multilabel_classification/1-quickstart/
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-04-05 09:20:57.000000 MAPIE-0.6.4/examples/multilabel_classification/1-quickstart/plot_tutorial_multilabel_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:21:05.684098 MAPIE-0.6.4/examples/regression/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:21:05.688098 MAPIE-0.6.4/examples/regression/1-quickstart/
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-04-05 09:20:57.000000 MAPIE-0.6.4/examples/regression/1-quickstart/plot_compare_conformity_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-04-05 09:20:57.000000 MAPIE-0.6.4/examples/regression/1-quickstart/plot_heteroscedastic_1d_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-04-05 09:20:57.000000 MAPIE-0.6.4/examples/regression/1-quickstart/plot_homoscedastic_1d_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-04-05 09:20:57.000000 MAPIE-0.6.4/examples/regression/1-quickstart/plot_prefit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-04-05 09:20:57.000000 MAPIE-0.6.4/examples/regression/1-quickstart/plot_timeseries_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-05 09:20:57.000000 MAPIE-0.6.4/examples/regression/1-quickstart/plot_toy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:21:05.688098 MAPIE-0.6.4/examples/regression/2-advanced-analysis/
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-05 09:20:57.000000 MAPIE-0.6.4/examples/regression/2-advanced-analysis/plot_both_uncertainties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-04-05 09:20:57.000000 MAPIE-0.6.4/examples/regression/2-advanced-analysis/plot_nested-cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-04-05 09:20:57.000000 MAPIE-0.6.4/examples/regression/2-advanced-analysis/plot_timeseries_enbpi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:21:05.688098 MAPIE-0.6.4/examples/regression/3-scientific-articles/
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-04-05 09:20:57.000000 MAPIE-0.6.4/examples/regression/3-scientific-articles/plot_barber2020_simulations.py
--rw-r--r--   0 runner    (1001) docker     (123)    15254 2023-04-05 09:20:57.000000 MAPIE-0.6.4/examples/regression/3-scientific-articles/plot_kim2020_simulations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:21:05.688098 MAPIE-0.6.4/examples/regression/4-tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    15900 2023-04-05 09:20:57.000000 MAPIE-0.6.4/examples/regression/4-tutorials/plot_cqr_tutorial.py
--rw-r--r--   0 runner    (1001) docker     (123)    28652 2023-04-05 09:20:57.000000 MAPIE-0.6.4/examples/regression/4-tutorials/plot_main-tutorial-regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    12576 2023-04-05 09:20:57.000000 MAPIE-0.6.4/examples/regression/4-tutorials/plot_ts-tutorial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:21:05.688098 MAPIE-0.6.4/mapie/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/_machine_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/aggregation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18625 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    48330 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/conformity_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     9578 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    26078 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/multi_label_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    25974 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/quantile_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    25765 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/subsample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:21:05.692098 MAPIE-0.6.4/mapie/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/tests/test_aggregations_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    41471 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/tests/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/tests/test_conformity_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    17616 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/tests/test_multi_label_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    22146 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/tests/test_quantile_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    17456 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/tests/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/tests/test_subsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/tests/test_time_series_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/time_series_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    30456 2023-04-05 09:20:57.000000 MAPIE-0.6.4/mapie/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 09:21:05.692098 MAPIE-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-05 09:20:57.000000 MAPIE-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:11.984788 MAPIE-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-26 18:12:02.000000 MAPIE-0.6.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-26 18:12:02.000000 MAPIE-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-26 18:12:02.000000 MAPIE-0.6.5/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:11.980788 MAPIE-0.6.5/MAPIE.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-06-26 18:12:11.000000 MAPIE-0.6.5/MAPIE.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-26 18:12:11.000000 MAPIE-0.6.5/MAPIE.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 18:12:11.000000 MAPIE-0.6.5/MAPIE.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 18:12:11.000000 MAPIE-0.6.5/MAPIE.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 18:12:11.000000 MAPIE-0.6.5/MAPIE.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 18:12:11.000000 MAPIE-0.6.5/MAPIE.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-06-26 18:12:11.984788 MAPIE-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-06-26 18:12:02.000000 MAPIE-0.6.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:11.980788 MAPIE-0.6.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:11.980788 MAPIE-0.6.5/examples/classification/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:11.980788 MAPIE-0.6.5/examples/classification/1-quickstart/
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-06-26 18:12:02.000000 MAPIE-0.6.5/examples/classification/1-quickstart/plot_comp_methods_on_2d_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:11.980788 MAPIE-0.6.5/examples/classification/3-scientific-articles/
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-26 18:12:02.000000 MAPIE-0.6.5/examples/classification/3-scientific-articles/plot_sadinle2019_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:11.980788 MAPIE-0.6.5/examples/classification/4-tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-06-26 18:12:02.000000 MAPIE-0.6.5/examples/classification/4-tutorials/plot_crossconformal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10647 2023-06-26 18:12:02.000000 MAPIE-0.6.5/examples/classification/4-tutorials/plot_main-tutorial-classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:11.980788 MAPIE-0.6.5/examples/multilabel_classification/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:11.980788 MAPIE-0.6.5/examples/multilabel_classification/1-quickstart/
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-06-26 18:12:02.000000 MAPIE-0.6.5/examples/multilabel_classification/1-quickstart/plot_tutorial_multilabel_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:11.980788 MAPIE-0.6.5/examples/regression/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:11.980788 MAPIE-0.6.5/examples/regression/1-quickstart/
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-26 18:12:02.000000 MAPIE-0.6.5/examples/regression/1-quickstart/plot_compare_conformity_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-26 18:12:02.000000 MAPIE-0.6.5/examples/regression/1-quickstart/plot_heteroscedastic_1d_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-26 18:12:02.000000 MAPIE-0.6.5/examples/regression/1-quickstart/plot_homoscedastic_1d_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-26 18:12:02.000000 MAPIE-0.6.5/examples/regression/1-quickstart/plot_prefit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2023-06-26 18:12:02.000000 MAPIE-0.6.5/examples/regression/1-quickstart/plot_timeseries_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-26 18:12:02.000000 MAPIE-0.6.5/examples/regression/1-quickstart/plot_toy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:11.980788 MAPIE-0.6.5/examples/regression/2-advanced-analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-06-26 18:12:02.000000 MAPIE-0.6.5/examples/regression/2-advanced-analysis/plot_both_uncertainties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-06-26 18:12:02.000000 MAPIE-0.6.5/examples/regression/2-advanced-analysis/plot_nested-cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-06-26 18:12:02.000000 MAPIE-0.6.5/examples/regression/2-advanced-analysis/plot_timeseries_enbpi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:11.980788 MAPIE-0.6.5/examples/regression/3-scientific-articles/
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-26 18:12:02.000000 MAPIE-0.6.5/examples/regression/3-scientific-articles/plot_barber2020_simulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15254 2023-06-26 18:12:02.000000 MAPIE-0.6.5/examples/regression/3-scientific-articles/plot_kim2020_simulations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:11.980788 MAPIE-0.6.5/examples/regression/4-tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    15863 2023-06-26 18:12:02.000000 MAPIE-0.6.5/examples/regression/4-tutorials/plot_cqr_tutorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28615 2023-06-26 18:12:02.000000 MAPIE-0.6.5/examples/regression/4-tutorials/plot_main-tutorial-regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12564 2023-06-26 18:12:02.000000 MAPIE-0.6.5/examples/regression/4-tutorials/plot_ts-tutorial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:11.984788 MAPIE-0.6.5/mapie/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/_machine_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/aggregation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19295 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52453 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/classification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:11.984788 MAPIE-0.6.5/mapie/conformity_scores/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/conformity_scores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/conformity_scores/conformity_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/conformity_scores/residual_conformity_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23666 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26078 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/multi_label_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/quantile_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:11.984788 MAPIE-0.6.5/mapie/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25833 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/regression/quantile_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/regression/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/regression/time_series_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/subsample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:11.984788 MAPIE-0.6.5/mapie/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/tests/test_aggregations_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52313 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/tests/test_conformity_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21012 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17480 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/tests/test_multi_label_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23171 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/tests/test_quantile_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19760 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/tests/test_subsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/tests/test_time_series_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/time_series_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35518 2023-06-26 18:12:02.000000 MAPIE-0.6.5/mapie/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 18:12:11.984788 MAPIE-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-26 18:12:02.000000 MAPIE-0.6.5/setup.py
```

### Comparing `MAPIE-0.6.4/AUTHORS.rst` & `MAPIE-0.6.5/AUTHORS.rst`

 * *Files 10% similar despite different names*

```diff
@@ -26,9 +26,10 @@
 * Abdou Akim Goumbala <aagoumbala@quantmetry.com>
 * Adirtha Borgohain <adirthaborgohain@gmail.com>
 * Thomas Morzadec <tmorzadec@quantmetry.com>
 * Julien Roussel <jroussel@quantmetry.com>
 * Arnaud Capitaine <arnaud.gc.capitaine@gmail.com>
 * Tarik Tazi <ttazi@quantmetry.com>
 * Daniel Herbst <daniel.herbst@tum.de>
+* Candice Moyet <cmoyet@quantmetry.com>
 
 To be continued ...
```

### Comparing `MAPIE-0.6.4/LICENSE` & `MAPIE-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/MAPIE.egg-info/PKG-INFO` & `MAPIE-0.6.5/MAPIE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: MAPIE
-Version: 0.6.4
+Version: 0.6.5
 Summary: A scikit-learn-compatible module for estimating prediction intervals.
 Home-page: https://github.com/scikit-learn-contrib/MAPIE
 Download-URL: https://pypi.org/project/MAPIE/#files
-Maintainer: V. Taquet, V. Blot, T. Morzadec, G. Martinon
-Maintainer-email: vtaquet@quantmetry.com, vblot@quantmetry.com, tmorzadec@quantmetry.com, gmartinon@quantmetry.com
+Maintainer: T. Cordier, V. Blot, L. Lacombe
+Maintainer-email: tcordier@quantmetry.com, vblot@quantmetry.com, llacombe@quantmetry.com
 License: new BSD
 Project-URL: Bug Tracker, https://github.com/scikit-learn-contrib/MAPIE/issues
 Project-URL: Documentation, https://mapie.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/scikit-learn-contrib/MAPIE
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
```

### Comparing `MAPIE-0.6.4/MAPIE.egg-info/SOURCES.txt` & `MAPIE-0.6.5/MAPIE.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -32,22 +32,27 @@
 mapie/_compatibility.py
 mapie/_machine_precision.py
 mapie/_typing.py
 mapie/_version.py
 mapie/aggregation_functions.py
 mapie/calibration.py
 mapie/classification.py
-mapie/conformity_scores.py
 mapie/metrics.py
 mapie/multi_label_classification.py
 mapie/quantile_regression.py
-mapie/regression.py
 mapie/subsample.py
 mapie/time_series_regression.py
 mapie/utils.py
+mapie/conformity_scores/__init__.py
+mapie/conformity_scores/conformity_scores.py
+mapie/conformity_scores/residual_conformity_scores.py
+mapie/regression/__init__.py
+mapie/regression/quantile_regression.py
+mapie/regression/regression.py
+mapie/regression/time_series_regression.py
 mapie/tests/__init__.py
 mapie/tests/test_aggregations_functions.py
 mapie/tests/test_calibration.py
 mapie/tests/test_classification.py
 mapie/tests/test_common.py
 mapie/tests/test_conformity_scores.py
 mapie/tests/test_metrics.py
```

### Comparing `MAPIE-0.6.4/PKG-INFO` & `MAPIE-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: MAPIE
-Version: 0.6.4
+Version: 0.6.5
 Summary: A scikit-learn-compatible module for estimating prediction intervals.
 Home-page: https://github.com/scikit-learn-contrib/MAPIE
 Download-URL: https://pypi.org/project/MAPIE/#files
-Maintainer: V. Taquet, V. Blot, T. Morzadec, G. Martinon
-Maintainer-email: vtaquet@quantmetry.com, vblot@quantmetry.com, tmorzadec@quantmetry.com, gmartinon@quantmetry.com
+Maintainer: T. Cordier, V. Blot, L. Lacombe
+Maintainer-email: tcordier@quantmetry.com, vblot@quantmetry.com, llacombe@quantmetry.com
 License: new BSD
 Project-URL: Bug Tracker, https://github.com/scikit-learn-contrib/MAPIE/issues
 Project-URL: Documentation, https://mapie.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/scikit-learn-contrib/MAPIE
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
```

### Comparing `MAPIE-0.6.4/README.rst` & `MAPIE-0.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/examples/classification/1-quickstart/plot_comp_methods_on_2d_dataset.py` & `MAPIE-0.6.5/examples/classification/1-quickstart/plot_comp_methods_on_2d_dataset.py`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/examples/classification/3-scientific-articles/plot_sadinle2019_example.py` & `MAPIE-0.6.5/examples/classification/3-scientific-articles/plot_sadinle2019_example.py`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/examples/classification/4-tutorials/plot_crossconformal.py` & `MAPIE-0.6.5/examples/classification/4-tutorials/plot_crossconformal.py`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/examples/classification/4-tutorials/plot_main-tutorial-classification.py` & `MAPIE-0.6.5/examples/classification/4-tutorials/plot_main-tutorial-classification.py`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/examples/multilabel_classification/1-quickstart/plot_tutorial_multilabel_classification.py` & `MAPIE-0.6.5/examples/multilabel_classification/1-quickstart/plot_tutorial_multilabel_classification.py`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/examples/regression/1-quickstart/plot_compare_conformity_scores.py` & `MAPIE-0.6.5/examples/regression/1-quickstart/plot_compare_conformity_scores.py`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/examples/regression/1-quickstart/plot_heteroscedastic_1d_data.py` & `MAPIE-0.6.5/examples/regression/1-quickstart/plot_heteroscedastic_1d_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 import scipy
 from matplotlib import pyplot as plt
 from sklearn.linear_model import LinearRegression, QuantileRegressor
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import PolynomialFeatures
 
 from mapie._typing import NDArray
-from mapie.quantile_regression import MapieQuantileRegressor
-from mapie.regression import MapieRegressor
+from mapie.regression import MapieQuantileRegressor, MapieRegressor
 from mapie.subsample import Subsample
 
 random_state = 42
 
 
 def f(x: NDArray) -> NDArray:
     """Polynomial function used to generate one-dimensional data"""
```

### Comparing `MAPIE-0.6.4/examples/regression/1-quickstart/plot_homoscedastic_1d_data.py` & `MAPIE-0.6.5/examples/regression/1-quickstart/plot_homoscedastic_1d_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 import scipy
 from matplotlib import pyplot as plt
 from sklearn.linear_model import LinearRegression, QuantileRegressor
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import PolynomialFeatures
 
 from mapie._typing import NDArray
-from mapie.quantile_regression import MapieQuantileRegressor
-from mapie.regression import MapieRegressor
+from mapie.regression import MapieQuantileRegressor, MapieRegressor
 from mapie.subsample import Subsample
 
 random_state = 42
 
 
 def f(x: NDArray) -> NDArray:
     """Polynomial function used to generate one-dimensional data"""
```

### Comparing `MAPIE-0.6.4/examples/regression/1-quickstart/plot_prefit.py` & `MAPIE-0.6.5/examples/regression/1-quickstart/plot_prefit.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 from lightgbm import LGBMRegressor
 from matplotlib import pyplot as plt
 from sklearn.model_selection import train_test_split
 from sklearn.neural_network import MLPRegressor
 
 from mapie._typing import NDArray
 from mapie.metrics import regression_coverage_score
-from mapie.quantile_regression import MapieQuantileRegressor
-from mapie.regression import MapieRegressor
+from mapie.regression import MapieQuantileRegressor, MapieRegressor
 
 warnings.filterwarnings("ignore")
 
 alpha = 0.1
 
 ##############################################################################
 # 1. Generate dataset
```

### Comparing `MAPIE-0.6.4/examples/regression/1-quickstart/plot_timeseries_example.py` & `MAPIE-0.6.5/examples/regression/1-quickstart/plot_timeseries_example.py`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/examples/regression/1-quickstart/plot_toy_model.py` & `MAPIE-0.6.5/examples/regression/1-quickstart/plot_toy_model.py`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/examples/regression/2-advanced-analysis/plot_both_uncertainties.py` & `MAPIE-0.6.5/examples/regression/2-advanced-analysis/plot_both_uncertainties.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from sklearn.linear_model import LinearRegression, QuantileRegressor
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import PolynomialFeatures
 
 from mapie._typing import NDArray
-from mapie.quantile_regression import MapieQuantileRegressor
-from mapie.regression import MapieRegressor
+from mapie.regression import MapieQuantileRegressor, MapieRegressor
 from mapie.subsample import Subsample
 
 F = TypeVar("F", bound=Callable[..., Any])
 random_state = 42
 
 
 # Functions for generating our dataset
```

### Comparing `MAPIE-0.6.4/examples/regression/2-advanced-analysis/plot_nested-cv.py` & `MAPIE-0.6.5/examples/regression/2-advanced-analysis/plot_nested-cv.py`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/examples/regression/2-advanced-analysis/plot_timeseries_enbpi.py` & `MAPIE-0.6.5/examples/regression/2-advanced-analysis/plot_timeseries_enbpi.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from sklearn.ensemble import RandomForestRegressor
 from sklearn.model_selection import RandomizedSearchCV, TimeSeriesSplit
 
 from mapie._typing import NDArray
 from mapie.metrics import (regression_coverage_score,
                            regression_mean_width_score)
 from mapie.subsample import BlockBootstrap
-from mapie.time_series_regression import MapieTimeSeriesRegressor
+from mapie.regression import MapieTimeSeriesRegressor
 
 # Load input data and feature engineering
 url_file = (
     "https://raw.githubusercontent.com/scikit-learn-contrib/MAPIE/"
     + "master/examples/data/demand_temperature.csv"
 )
 demand_df = pd.read_csv(url_file, parse_dates=True, index_col=0)
```

### Comparing `MAPIE-0.6.4/examples/regression/3-scientific-articles/plot_barber2020_simulations.py` & `MAPIE-0.6.5/examples/regression/3-scientific-articles/plot_barber2020_simulations.py`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/examples/regression/3-scientific-articles/plot_kim2020_simulations.py` & `MAPIE-0.6.5/examples/regression/3-scientific-articles/plot_kim2020_simulations.py`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/examples/regression/4-tutorials/plot_cqr_tutorial.py` & `MAPIE-0.6.5/examples/regression/4-tutorials/plot_cqr_tutorial.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,15 @@
 from matplotlib.ticker import FormatStrFormatter
 from scipy.stats import randint, uniform
 from sklearn.datasets import fetch_california_housing
 from sklearn.model_selection import KFold, RandomizedSearchCV, train_test_split
 
 from mapie.metrics import (regression_coverage_score,
                            regression_mean_width_score)
-from mapie.quantile_regression import MapieQuantileRegressor
-from mapie.regression import MapieRegressor
+from mapie.regression import MapieQuantileRegressor, MapieRegressor
 from mapie.subsample import Subsample
 
 random_state = 23
 rng = np.random.default_rng(random_state)
 round_to = 3
 
 warnings.filterwarnings("ignore")
```

### Comparing `MAPIE-0.6.4/examples/regression/4-tutorials/plot_main-tutorial-regression.py` & `MAPIE-0.6.5/examples/regression/4-tutorials/plot_main-tutorial-regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,16 +36,15 @@
 import numpy as np
 import pandas as pd
 from sklearn.linear_model import LinearRegression, QuantileRegressor
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import PolynomialFeatures
 
 from mapie.metrics import regression_coverage_score
-from mapie.quantile_regression import MapieQuantileRegressor
-from mapie.regression import MapieRegressor
+from mapie.regression import MapieQuantileRegressor, MapieRegressor
 from mapie.subsample import Subsample
 
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
 warnings.filterwarnings("ignore")
 
 
 ##############################################################################
```

### Comparing `MAPIE-0.6.4/examples/regression/4-tutorials/plot_ts-tutorial.py` & `MAPIE-0.6.5/examples/regression/4-tutorials/plot_ts-tutorial.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 from scipy.stats import randint
 from sklearn.ensemble import RandomForestRegressor
 from sklearn.model_selection import RandomizedSearchCV, TimeSeriesSplit
 
 from mapie.metrics import (regression_coverage_score,
                            regression_mean_width_score)
 from mapie.subsample import BlockBootstrap
-from mapie.time_series_regression import MapieTimeSeriesRegressor
+from mapie.regression import MapieTimeSeriesRegressor
 
 warnings.simplefilter("ignore")
 
 
 ##############################################################################
 # 1. Load input data and dataset preparation
 # ------------------------------------------
```

### Comparing `MAPIE-0.6.4/mapie/_compatibility.py` & `MAPIE-0.6.5/mapie/_compatibility.py`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/mapie/aggregation_functions.py` & `MAPIE-0.6.5/mapie/aggregation_functions.py`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/mapie/calibration.py` & `MAPIE-0.6.5/mapie/calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from sklearn.isotonic import IsotonicRegression
 from sklearn.utils import check_random_state
 from sklearn.utils.multiclass import type_of_target
 from sklearn.utils.validation import (_check_y, _num_samples, check_is_fitted,
                                       indexable)
 
 from ._typing import ArrayLike, NDArray
-from .utils import (check_cv, check_estimator_classification,
+from .utils import (check_estimator_classification,
                     check_estimator_fit_predict, check_n_features_in,
                     check_null_weight, fit_estimator, get_calib_set)
 
 
 class MapieCalibrator(BaseEstimator, ClassifierMixin):
     """
     Calibration for multi-class problems.
@@ -116,28 +116,60 @@
     named_calibrators = {
         "sigmoid": _SigmoidCalibration(),
         "isotonic": IsotonicRegression(out_of_bounds="clip")
     }
 
     valid_methods = ["top_label"]
 
+    valid_cv = ["prefit", "split"]
+
     valid_inputs = ["multiclass", "binary"]
 
     def __init__(
         self,
         estimator: Optional[ClassifierMixin] = None,
         method: str = "top_label",
         calibrator: Optional[Union[str, RegressorMixin]] = None,
         cv: Optional[str] = "split",
     ) -> None:
         self.estimator = estimator
         self.method = method
         self.calibrator = calibrator
         self.cv = cv
 
+    def _check_cv(
+        self,
+        cv: Optional[str],
+    ) -> str:
+        """
+        Check if cross-validator is ``"prefit"`` or ``"split"``.
+        Else raise error.
+
+        Parameters
+        ----------
+        cv : str
+            Cross-validator to check.
+
+        Returns
+        -------
+        str
+            'prefit' or 'split'.
+
+        Raises
+        ------
+        ValueError
+            If the cross-validator is not valid.
+        """
+        if cv in self.valid_cv:
+            return cv
+        raise ValueError(
+            "Invalid cv argument. "
+            f"Allowed values are {self.valid_cv}."
+        )
+
     def _check_calibrator(
         self,
         calibrator: Optional[Union[str, RegressorMixin]],
     ) -> RegressorMixin:
         """
         Check the input that has been provided for calibrator and
         check that the calibrator is a valid estimator to calibrate.
@@ -437,15 +469,15 @@
 
         Returns
         -------
         MapieCalibrator
             The model itself.
         """
         self._check_method()
-        cv = check_cv(self.cv)
+        cv = self._check_cv(self.cv)
         X, y = indexable(X, y)
         y = _check_y(y)
         self._check_type_of_target(y)
         estimator = check_estimator_classification(X, y, cv, self.estimator)
         calibrator = self._check_calibrator(self.calibrator)
         sample_weight, X, y = check_null_weight(sample_weight, X, y)
         self.n_features_in_ = check_n_features_in(X, cv, estimator)
```

### Comparing `MAPIE-0.6.4/mapie/classification.py` & `MAPIE-0.6.5/mapie/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 
 import warnings
 from typing import Any, Iterable, List, Optional, Tuple, Union, cast
 
 import numpy as np
 from joblib import Parallel, delayed
 from sklearn.base import BaseEstimator, ClassifierMixin, clone
-from sklearn.model_selection import BaseCrossValidator, train_test_split
+from sklearn.model_selection import BaseCrossValidator, ShuffleSplit
 from sklearn.preprocessing import LabelEncoder, label_binarize
 from sklearn.utils import _safe_indexing, check_random_state
-from sklearn.utils.multiclass import (
-    check_classification_targets, type_of_target
-)
+from sklearn.utils.multiclass import (check_classification_targets,
+                                      type_of_target)
 from sklearn.utils.validation import (_check_y, _num_samples, check_is_fitted,
                                       indexable)
 
 from ._machine_precision import EPSILON
 from ._typing import ArrayLike, NDArray
 from .metrics import classification_mean_width_score
 from .utils import (check_alpha, check_alpha_and_n_samples, check_cv,
@@ -53,43 +52,58 @@
         - "cumulated_score", based on the sum of the softmax outputs of the
           labels until the true label is reached, on the calibration set.
           See [2] for more details.
 
         - "raps", Regularized Adaptive Prediction Sets method. It uses the
           same technique as cumulated_score method but with a penalty term
           to reduce the size of prediction sets. See [3] for more
-          details. For now, this method only works with "prefit" strategy.
+          details. For now, this method only works with "prefit" and "split"
+          strategies.
 
         - "top_k", based on the sorted index of the probability of the true
           label in the softmax outputs, on the calibration set. In case two
           probabilities are equal, both are taken, thus, the size of some
           prediction sets may be different from the others. See [3] for
           more details.
 
         By default "score".
 
     cv: Optional[str]
-        The cross-validation strategy for computing scores :
+        The cross-validation strategy for computing scores.
+        It directly drives the distinction between jackknife and cv variants.
+        Choose among:
 
         - ``None``, to use the default 5-fold cross-validation
         - integer, to specify the number of folds.
           If equal to -1, equivalent to
           ``sklearn.model_selection.LeaveOneOut()``.
         - CV splitter: any ``sklearn.model_selection.BaseCrossValidator``
           Main variants are:
           - ``sklearn.model_selection.LeaveOneOut`` (jackknife),
           - ``sklearn.model_selection.KFold`` (cross-validation)
+        - ``"split"``, does not involve cross-validation but a division
+          of the data into training and calibration subsets. The splitter
+          used is the following: ``sklearn.model_selection.ShuffleSplit``.
         - ``"prefit"``, assumes that ``estimator`` has been fitted already.
           All data provided in the ``fit`` method is then used
           to calibrate the predictions through the score computation.
           At prediction time, quantiles of these scores are used to estimate
           prediction sets.
 
         By default ``None``.
 
+    test_size: Optional[Union[int, float]]
+        If float, should be between 0.0 and 1.0 and represent the proportion
+        of the dataset to include in the test split. If int, represents the
+        absolute number of test samples. If None, it will be set to 0.1.
+
+        If cv is not ``"split"``, ``test_size`` is ignored.
+
+        By default ``None``.
+
     n_jobs: Optional[int]
         Number of jobs for parallel processing using joblib
         via the "locky" backend.
         At this moment, parallel processing is disabled.
         If ``-1`` all CPUs are used.
         If ``1`` is given, no parallel computing code is used at all,
         which is useful for debugging.
@@ -100,15 +114,15 @@
         By default ``None``.
 
     random_state: Optional[Union[int, RandomState]]
         Pseudo random number generator state used for random uniform sampling
         for evaluation quantiles and prediction sets in cumulated_score.
         Pass an int for reproducible output across multiple function calls.
 
-        By default ```1``.
+        By default ``None``.
 
     verbose : int, optional
         The verbosity level, used with joblib for multiprocessing.
         At this moment, parallel processing is disabled.
         The frequency of the messages increases with the verbosity level.
         If it more than ``10``, all iterations are reported.
         Above ``50``, the output is sent to stdout.
@@ -165,14 +179,15 @@
      [False  True False]
      [False  True  True]
      [False  True  True]
      [False False  True]
      [False False  True]]
     """
 
+    raps_valid_cv_ = ["prefit", "split"]
     valid_methods_ = ["naive", "score", "cumulated_score", "top_k", "raps"]
     fit_attributes = [
         "single_estimator_",
         "estimators_",
         "k_",
         "n_features_in_",
         "conformity_scores_",
@@ -181,21 +196,23 @@
     ]
 
     def __init__(
         self,
         estimator: Optional[ClassifierMixin] = None,
         method: str = "score",
         cv: Optional[Union[int, str, BaseCrossValidator]] = None,
+        test_size: Optional[Union[int, float]] = None,
         n_jobs: Optional[int] = None,
         random_state: Optional[Union[int, np.random.RandomState]] = None,
         verbose: int = 0
     ) -> None:
         self.estimator = estimator
         self.method = method
         self.cv = cv
+        self.test_size = test_size
         self.n_jobs = n_jobs
         self.random_state = random_state
         self.verbose = verbose
 
     def _check_parameters(self) -> None:
         """
         Perform several checks on input parameters.
@@ -204,16 +221,15 @@
         ------
         ValueError
             If parameters are not valid.
         """
         if self.method not in self.valid_methods_:
             raise ValueError(
                 "Invalid method. "
-                "Allowed values are 'score', 'cumulated_score', "
-                "'raps', 'naive' or 'top_k'"
+                f"Allowed values are {self.valid_methods_}."
             )
         check_n_jobs(self.n_jobs)
         check_verbose(self.verbose)
         check_random_state(self.random_state)
         self._check_raps()
 
     def _check_raps(self):
@@ -222,16 +238,22 @@
         the cross validation strategy is "prefit".
 
         Raises
         ------
         ValueError
             If method is "raps" and cv is not "prefit".
         """
-        if (self.method == "raps") and (self.cv != "prefit"):
-            raise ValueError("RAPS method can only be used with cv='prefit'")
+        if (self.method == "raps") and (
+            (self.cv not in self.raps_valid_cv_)
+            or isinstance(self.cv, ShuffleSplit)
+        ):
+            raise ValueError(
+                "RAPS method can only be used "
+                f"with cv in {self.raps_valid_cv_}."
+            )
 
     def _check_include_last_label(
         self,
         include_last_label: Optional[Union[bool, str]]
     ) -> Optional[Union[bool, str]]:
         """
         Check if include_last_label is a boolean or a string.
@@ -325,18 +347,19 @@
         y_pred_proba_cumsum : NDArray of shape (n_samples, n_classes)
             Cumsumed probabilities in the original order.
 
         threshold : NDArray of shape (n_alpha,) or shape (n_samples_train,)
             Threshold to compare with y_proba_last_cumsum, can be either:
 
             - the quantiles associated with alpha values when
-              ``cv`` == "prefit" or ``agg_scores`` is "mean"
+              ``cv`` == "prefit", ``cv`` == "split"
+              or ``agg_scores`` is "mean"
             - the conformity score from training samples otherwise
               (i.e., when ``cv`` is a CV splitter and
-              ``agg_scores`` is "crossval)
+              ``agg_scores`` is "crossval")
 
         include_last_label : Union[bool, str]
             Whether or not include the last label. If 'randomized',
             the last label is included.
 
         Returns
         -------
@@ -402,18 +425,19 @@
         y_pred_proba_last : NDArray of shape (n_samples, 1, threshold)
             Last included probability.
 
         threshold : NDArray of shape (n_alpha,) or shape (n_samples_train,)
             Threshold to compare with y_proba_last_cumsum, can be either:
 
             - the quantiles associated with alpha values when
-              ``cv`` == "prefit" or ``agg_scores`` is "mean"
+              ``cv`` == "prefit", ``cv`` == "split" or
+              ``agg_scores`` is "mean"
             - the conformity score from training samples otherwise
               (i.e., when ``cv`` is a CV splitter and
-              ``agg_scores`` is "crossval)
+              ``agg_scores`` is "crossval")
 
         lambda_star: Union[NDArray, float, None] of shape (n_alpha):
             Optimal value of the regulizer lambda.
 
         k_star: Union[NDArray, None] of shape (n_alpha):
             Optimal value of the regulizer k.
 
@@ -884,14 +908,68 @@
             lambda_star, best_sizes = self._update_size_and_lambda(
                 best_sizes, alpha_np, y_ps, lambda_, lambda_star
             )
         if len(lambda_star) == 1:
             lambda_star = lambda_star[0]
         return lambda_star
 
+    def _get_classes_info(
+            self, estimator: ClassifierMixin, y: NDArray
+    ) -> Tuple[int, NDArray]:
+        """
+        Compute the number of classes and the classes values
+        according to either the pre-trained model or to the
+        values in y.
+
+        Parameters
+        ----------
+        estimator : ClassifierMixin
+            Estimator pre-fitted or not.
+        y : NDArray
+            Values to predict.
+
+        Returns
+        -------
+        Tuple[int, NDArray]
+            The number of unique classes and their unique
+            values.
+
+        Raises
+        ------
+        ValueError
+            If `cv="prefit"` and that classes in `y` are not included into
+            `estimator.classes_`.
+
+        Warning
+            If number of calibration labels is lower than number of labels
+            for training (in prefit setting)
+        """
+        n_unique_y_labels = len(np.unique(y))
+        if self.cv == "prefit":
+            classes = estimator.classes_
+            n_classes = len(np.unique(classes))
+            if not set(np.unique(y)).issubset(classes):
+                raise ValueError(
+                    "Values in y do not matched values in estimator.classes_."
+                    + " Check that you are not adding any new label"
+                )
+            if n_classes > n_unique_y_labels:
+                warnings.warn(
+                    "WARNING: your calibration dataset has less labels"
+                    + " than your training dataset (training"
+                    + f" has {n_classes} unique labels while"
+                    + f" calibration have {n_unique_y_labels} unique labels"
+                )
+
+        else:
+            n_classes = n_unique_y_labels
+            classes = np.unique(y)
+
+        return n_classes, classes
+
     def fit(
         self,
         X: ArrayLike,
         y: ArrayLike,
         sample_weight: Optional[ArrayLike] = None,
         size_raps: Optional[float] = .2,
     ) -> MapieClassifier:
@@ -925,66 +1003,71 @@
         Returns
         -------
         MapieClassifier
             The model itself.
         """
         # Checks
         self._check_parameters()
-        cv = check_cv(self.cv)
+        cv = check_cv(
+            self.cv, test_size=self.test_size, random_state=self.random_state
+        )
         X, y = indexable(X, y)
         y = _check_y(y)
 
         sample_weight = cast(Optional[NDArray], sample_weight)
         sample_weight, X, y = check_null_weight(sample_weight, X, y)
 
         y = cast(NDArray, y)
-        enc = LabelEncoder()
-        y_enc = enc.fit_transform(y)
-        self.label_encoder_ = enc
 
         estimator = check_estimator_classification(
             X,
-            y_enc,
+            y,
             cv,
             self.estimator
         )
         self.n_features_in_ = check_n_features_in(X, cv, estimator)
 
         n_samples = _num_samples(y)
-        self.n_classes_ = len(np.unique(y))
-        self.classes_ = np.unique(y)
+
+        self.n_classes_, self.classes_ = self._get_classes_info(
+            estimator, y
+        )
+        enc = LabelEncoder()
+        enc.fit(self.classes_)
+        y_enc = enc.transform(y)
+
+        self.label_encoder_ = enc
         check_classification_targets(y)
         self._target_type = type_of_target(y)
 
         # Initialization
         self.estimators_: List[ClassifierMixin] = []
         self.k_ = np.empty_like(y, dtype=int)
         self.n_samples_ = _num_samples(X)
 
         if self._target_type == "multiclass":
             if self.method == "raps":
-                X, self.X_raps, y_enc, self.y_raps = train_test_split(
-                    X,
-                    y_enc,
-                    test_size=size_raps,
-                    random_state=self.random_state
+                raps_split = ShuffleSplit(
+                    1, test_size=size_raps, random_state=self.random_state
                 )
+                train_raps_index, val_raps_index = next(raps_split.split(X))
+                X, self.X_raps, y_enc, self.y_raps =\
+                    _safe_indexing(X, train_raps_index),\
+                    _safe_indexing(X, val_raps_index),\
+                    _safe_indexing(y_enc, train_raps_index),\
+                    _safe_indexing(y_enc, val_raps_index)
                 self.y_raps_no_enc = self.label_encoder_.inverse_transform(
                     self.y_raps
                 )
                 y = self.label_encoder_.inverse_transform(y_enc)
                 y_enc = cast(NDArray, y_enc)
                 n_samples = _num_samples(y_enc)
-                self.y_pred_proba_raps = estimator.predict_proba(
-                    self.X_raps
-                )
-                self.position_raps = self._get_true_label_position(
-                    self.y_pred_proba_raps,
-                    self.y_raps
-                )
+                if sample_weight is not None:
+                    sample_weight = sample_weight[train_raps_index]
+                    sample_weight = cast(NDArray, sample_weight)
 
             # Work
             if cv == "prefit":
                 self.single_estimator_ = estimator
                 y_pred_proba = self.single_estimator_.predict_proba(X)
                 y_pred_proba = self._check_proba_normalized(y_pred_proba)
 
@@ -1022,14 +1105,33 @@
                 val_ids = np.concatenate(cast(List[NDArray], val_ids_list))
                 val_indices = np.concatenate(
                     cast(List[NDArray], val_indices_list)
                 )
                 self.k_[val_indices] = val_ids
                 y_pred_proba[val_indices] = predictions
 
+                if isinstance(cv, ShuffleSplit):
+                    # Should delete values indices that
+                    # are not used during calibration
+                    self.k_ = self.k_[val_indices]
+                    y_pred_proba = y_pred_proba[val_indices]
+                    y_enc = y_enc[val_indices]
+                    y = cast(NDArray, y)[val_indices]
+
+            # RAPS: compute y_pred and position on the RAPS validation dataset
+            if self.method == "raps":
+                self.y_pred_proba_raps = self.single_estimator_.predict_proba(
+                    self.X_raps
+                )
+                self.position_raps = self._get_true_label_position(
+                    self.y_pred_proba_raps,
+                    self.y_raps
+                )
+
+            # Conformity scores
             if self.method == "naive":
                 self.conformity_scores_ = np.empty(
                     y_pred_proba.shape,
                     dtype="float"
                 )
             elif self.method == "score":
                 self.conformity_scores_ = np.take_along_axis(
@@ -1048,25 +1150,27 @@
                 random_state = check_random_state(self.random_state)
                 u = random_state.uniform(size=len(y_pred_proba)).reshape(-1, 1)
                 self.conformity_scores_ -= u * y_proba_true
             elif self.method == "top_k":
                 # Here we reorder the labels by decreasing probability
                 # and get the position of each label from decreasing
                 # probability
-
                 self.conformity_scores_ = self._get_true_label_position(
                     y_pred_proba,
                     y_enc
                 )
-
             else:
                 raise ValueError(
                     "Invalid method. "
-                    "Allowed values are 'score' or 'cumulated_score'."
+                    f"Allowed values are {self.valid_methods_}."
                 )
+
+            if isinstance(cv, ShuffleSplit):
+                self.single_estimator_ = self.estimators_[0]
+
         else:
             warnings.warn(
                 "WARNING: your target is not of type multiclass."
                 + " Still fitting the model but not conformal prediction"
                 + " algorithm will be run."
             )
             if cv == "prefit":
@@ -1150,15 +1254,17 @@
 
         - Tuple[NDArray, NDArray] of shapes
         (n_samples,) and (n_samples, n_classes, n_alpha) if alpha is not None.
         """
         if self.method == "top_k":
             agg_scores = "mean"
         # Checks
-        cv = check_cv(self.cv)
+        cv = check_cv(
+            self.cv, test_size=self.test_size, random_state=self.random_state
+        )
         include_last_label = self._check_include_last_label(include_last_label)
         alpha = cast(Optional[NDArray], check_alpha(alpha))
         check_is_fitted(self, self.fit_attributes)
         lambda_star, k_star = None, None
         # Estimate prediction sets
         y_pred = self.single_estimator_.predict(X)
 
@@ -1332,10 +1438,10 @@
                 y_pred_proba[:, :, np.newaxis]
                 - y_pred_proba_last,
                 -EPSILON
             )
         else:
             raise ValueError(
                 "Invalid method. "
-                "Allowed values are 'score' or 'cumulated_score'."
+                f"Allowed values are {self.valid_methods_}."
             )
         return y_pred, prediction_sets
```

### Comparing `MAPIE-0.6.4/mapie/multi_label_classification.py` & `MAPIE-0.6.5/mapie/multi_label_classification.py`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/mapie/quantile_regression.py` & `MAPIE-0.6.5/mapie/regression/quantile_regression.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,89 +8,97 @@
 from sklearn.linear_model import QuantileRegressor
 from sklearn.model_selection import train_test_split
 from sklearn.pipeline import Pipeline
 from sklearn.utils import check_random_state
 from sklearn.utils.validation import (_check_y, _num_samples, check_is_fitted,
                                       indexable)
 
-from ._compatibility import np_quantile
-from ._typing import ArrayLike, NDArray
+from mapie._compatibility import np_quantile
+from mapie._typing import ArrayLike, NDArray
+from mapie.utils import (check_alpha_and_n_samples,
+                         check_defined_variables_predict_cqr,
+                         check_estimator_fit_predict, check_lower_upper_bounds,
+                         check_null_weight, fit_estimator)
+
 from .regression import MapieRegressor
-from .utils import (check_alpha_and_n_samples,
-                    check_defined_variables_predict_cqr,
-                    check_estimator_fit_predict, check_lower_upper_bounds,
-                    check_null_weight, fit_estimator)
 
 
 class MapieQuantileRegressor(MapieRegressor):
     """
     This class implements the conformalized quantile regression strategy
     as proposed by Romano et al. (2019) to make conformal predictions.
-    The only valid ``method`` is "quantile" and the only valid default
-    ``cv`` is "split".
+    The only valid ``method`` is ``"quantile"`` and the only valid
+    ``cv`` is ``"split"``.
 
     Parameters
     ----------
     estimator : Optional[RegressorMixin]
         Any regressor with scikit-learn API
-        (i.e. with fit and predict methods), by default ``None``.
+        (i.e. with ``fit`` and ``predict`` methods).
         If ``None``, estimator defaults to a ``QuantileRegressor`` instance.
 
+        By default ``"None"``.
+
     method: str
         Method to choose for prediction, in this case, the only valid method
-        is the "quantile" method.
+        is the ``"quantile"`` method.
+
+        By default ``"quantile"``.
 
     cv: Optional[str]
-        By default the value is set to None. In theory a split method is
-        implemented as it is needed to provided both a training and calibration
-        set.
+        The cross-validation strategy for computing conformity scores.
+        In theory a split method is implemented as it is needed to provide
+        both a training and calibration set.
+
+        By default ``None``.
 
     alpha: float
-        Between 0 and 1.0, represents the risk level of the confidence
-        interval.
+        Between ``0.0`` and ``1.0``, represents the risk level of the
+        confidence interval.
         Lower ``alpha`` produce larger (more conservative) prediction
         intervals.
         ``alpha`` is the complement of the target coverage level.
 
-        By default 0.1.
+        By default ``0.1``.
 
     Attributes
     ----------
-    valid_methods: List[str]
+    valid_methods_: List[str]
         List of all valid methods.
 
     single_estimator_: RegressorMixin
         Estimator fitted on the whole training set.
 
-    estimators_ : List[RegressorMixin]
+    estimators_: List[RegressorMixin]
         - [0]: Estimator with quantile value of alpha/2
         - [1]: Estimator with quantile value of 1 - alpha/2
         - [2]: Estimator with quantile value of 0.5
 
-    conformity_scores_ : NDArray of shape (n_samples_train, 3)
-        Conformity scores between ``y_calib`` and ``y_pred``:
-            - [:, 0]: for y_calib coming from prediction estimator with
-            quantile of alpha/2
-            - [:, 1]: for y_calib coming from prediction estimator with
-            quantile of 1 - alpha/2
-            - [:, 2]: maximum of those first two scores
+    conformity_scores_: NDArray of shape (n_samples_train, 3)
+        Conformity scores between ``y_calib`` and ``y_pred``.
+
+        - [:, 0]: for ``y_calib`` coming from prediction estimator
+          with quantile of alpha/2
+        - [:, 1]: for ``y_calib`` coming from prediction estimator
+          with quantile of 1 - alpha/2
+        - [:, 2]: maximum of those first two scores
 
     n_calib_samples: int
         Number of samples in the calibration dataset.
 
     References
     ----------
     Yaniv Romano, Evan Patterson and Emmanuel J. Candès.
     "Conformalized Quantile Regression"
     Advances in neural information processing systems 32 (2019).
 
     Examples
     --------
     >>> import numpy as np
-    >>> from mapie.quantile_regression import MapieQuantileRegressor
+    >>> from mapie.regression import MapieQuantileRegressor
     >>> X_train = np.array([[0], [1], [2], [3], [4], [5]])
     >>> y_train = np.array([5, 7.5, 9.5, 10.5, 12.5, 15])
     >>> X_calib = np.array([[0], [1], [2], [3], [4], [5], [6], [7], [8], [9]])
     >>> y_calib = np.array([5, 7, 9, 4, 8, 1, 5, 7.5, 9.5, 12])
     >>> mapie_reg = MapieQuantileRegressor().fit(
     ...     X_train,
     ...     y_train,
@@ -161,46 +169,48 @@
         """
         Perform several checks on the alpha value and changes it from
         a float to an ArrayLike.
 
         Parameters
         ----------
         alpha : float
-            Can only be a float value between 0 and 1.0.
+            Can only be a float value between ``0.0`` and ``1.0``.
             Represent the risk level of the confidence interval.
             Lower alpha produce larger (more conservative) prediction
             intervals. Alpha is the complement of the target coverage level.
-            By default 0.1
+
+            By default ``0.1``.
 
         Returns
         -------
         ArrayLike
             An ArrayLike of three values:
 
             - [0]: alpha value of alpha/2
             - [1]: alpha value of of 1 - alpha/2
             - [2]: alpha value of 0.5
 
         Raises
         ------
         ValueError
             If alpha is not a float.
+
         ValueError
-            If the value of alpha is not between 0 and 1.0.
+            If the value of ``alpha`` is not between ``0.0`` and ``1.0``.
         """
         if self.cv == "prefit":
             warnings.warn(
                 "WARNING: The alpha that is set needs to be the same"
                 + " as the alpha of your prefitted model in the following"
                 " order [alpha/2, 1 - alpha/2, 0.5]"
             )
         if isinstance(alpha, float):
             if np.any(np.logical_or(alpha <= 0, alpha >= 1.0)):
                 raise ValueError(
-                    "Invalid alpha. Allowed values are between 0 and 1.0."
+                    "Invalid alpha. Allowed values are between 0.0 and 1.0."
                 )
             else:
                 alpha_np = np.array([alpha / 2, 1 - alpha / 2, 0.5])
         else:
             raise ValueError(
                 "Invalid alpha. Allowed values are float."
             )
@@ -210,17 +220,17 @@
         self,
         estimator: Optional[Union[RegressorMixin, Pipeline]] = None,
     ) -> Union[RegressorMixin, Pipeline]:
         """
         Perform several checks on the estimator to check if it has
         all the required specifications to be used with this methodology.
         The estimators that can be used in MapieQuantileRegressor need to
-        have a ``fit`` and ``predict``attribute, but also need to allow
+        have a ``fit`` and ``predict`` attribute, but also need to allow
         a quantile loss and therefore also setting a quantile value.
-        Note that there is a TypedDict to check which methods allow for
+        Note that there is a ``TypedDict`` to check which methods allow for
         quantile regression.
 
         Parameters
         ----------
         estimator : Optional[RegressorMixin], optional
             Estimator to check, by default ``None``.
 
@@ -229,26 +239,30 @@
         RegressorMixin
             The estimator itself or a default ``QuantileRegressor`` instance
             with ``solver`` set to "highs".
 
         Raises
         ------
         ValueError
-            If the estimator fit or predict methods.
+            If the estimator implements ``fit`` or ``predict`` methods.
+
         ValueError
             We check if it's a known estimator that does quantile regression
             according to the dictionnary set quantile_estimator_params.
             This dictionnary will need to be updated with the latest new
             available estimators.
+
         ValueError
-            The estimator does not have the "loss_name" in its parameters and
-            therefore can not be used as an estimator.
+            The estimator does not have the ``"loss_name"`` in its parameters
+            and therefore can not be used as an estimator.
+
         ValueError
-            There is no quantile "loss_name" and therefore this estimator
+            There is no quantile ``"loss_name"`` and therefore this estimator
             can not be used as a ``MapieQuantileRegressor``.
+
         ValueError
             The parameter to set the alpha value does not exist in this
             estimator and therefore we cannot use it.
         """
         if estimator is None:
             return QuantileRegressor(
                 solver="highs-ds",
@@ -290,41 +304,41 @@
                             + " estimator does not exist."
                         )
                 else:
                     raise ValueError(
                         "The base model does not seem to be accepted"
                         + " by MapieQuantileRegressor. \n"
                         "Give a base model among: \n"
-                        "``quantile_estimator_params.keys()``"
+                        f"{self.quantile_estimator_params.keys()} "
                         "Or, add your base model to"
                         + " ``quantile_estimator_params``."
                     )
 
     def _check_cv(
         self,
         cv: Optional[str] = None
     ) -> str:
         """
-        Check if cv argument is None, "split" or "prefit".
+        Check if cv argument is ``None``, ``"split"`` or ``"prefit"``.
 
         Parameters
         ----------
         cv : Optional[str], optional
            cv to check, by default ``None``.
 
         Returns
         -------
         str
-            cv itself or a default "split".
+            cv itself or a default ``"split"``.
 
         Raises
         ------
         ValueError
-            Raises an error if the cv is anything else but the method "split"
-            or "prefit.
+            Raises an error if the cv is anything else but the method
+            ``"split"`` or ``"prefit"``.
             Only the split method has been implemented.
         """
         if cv is None:
             return "split"
         if cv in ("split", "prefit"):
             return cv
         else:
@@ -344,15 +358,15 @@
         shuffle: Optional[bool] = True,
         stratify: Optional[ArrayLike] = None,
     ) -> Tuple[
         ArrayLike, ArrayLike, ArrayLike, ArrayLike, Optional[ArrayLike]
     ]:
         """
         Check if a calibration set has already been defined, if not, then
-        we define one using the `train_test_split` method.
+        we define one using the ``train_test_split`` method.
 
         Parameters
         ----------
         Same definition of parameters as for the ``fit`` method.
 
         Returns
         -------
@@ -363,15 +377,14 @@
                 y_train
             - [2]: ArrayLike of shape (n_samples_*calib_size, n_features)
                 X_calib
             - [3]: ArrayLike of shape (n_samples_*calib_size,)
                 y_calib
             - [4]: ArrayLike of shape (n_samples_,)
                 sample_weight_train
-
         """
         if X_calib is None or y_calib is None:
             if sample_weight is None:
                 X_train, X_calib, y_train, y_calib = train_test_split(
                         X,
                         y,
                         test_size=calib_size,
@@ -413,112 +426,117 @@
         estimators.
 
         Parameters
         ----------
         estimator : List[Union[RegressorMixin, Pipeline]]
             List of three prefitted estimators that should have
             pre-defined quantile levels of alpha/2, 1 - alpha/2 and 0.5.
-        X : ArrayLike of shape (n_samples, n_features)
-            Training data.
-        y : ArrayLike of shape (n_samples,)
-            Training labels.
-        X_calib : Optional[ArrayLike] of shape (n_calib_samples, n_features)
-            Calibration data.
-        y_calib : Optional[ArrayLike] of shape (n_calib_samples,)
-            Calibration labels.
 
         Raises
         ------
         ValueError
             If a non-iterable variable is provided for estimator.
+
         ValueError
             If less or more than three models are defined.
-        Warning
-            If X and y are defined, then warning that they are not used.
-        ValueError
-            If the calibration set is not defined.
+
         Warning
             If the alpha is defined, warns the user that it must be set
             accordingly with the prefit estimators.
         """
         if isinstance(estimator, Iterable) is False:
             raise ValueError(
                 "Estimator for prefit must be an iterable object."
             )
         if len(estimator) == 3:
             for est in estimator:
                 check_estimator_fit_predict(est)
                 check_is_fitted(est)
         else:
             raise ValueError(
-                    "You need to have provided 3 different estimators, they"
-                    " need to be preset with alpha values in the following"
-                    " order [alpha/2, 1 - alpha/2, 0.5]."
-                    )
+                "You need to have provided 3 different estimators, they"
+                " need to be preset with alpha values in the following"
+                " order [alpha/2, 1 - alpha/2, 0.5]."
+            )
 
     def fit(
         self,
         X: ArrayLike,
         y: ArrayLike,
         sample_weight: Optional[ArrayLike] = None,
         X_calib: Optional[ArrayLike] = None,
         y_calib: Optional[ArrayLike] = None,
         calib_size: Optional[float] = 0.3,
-        random_state: Optional[Union[int, np.random.RandomState, None]] = None,
+        random_state: Optional[Union[int, np.random.RandomState]] = None,
         shuffle: Optional[bool] = True,
         stratify: Optional[ArrayLike] = None,
     ) -> MapieQuantileRegressor:
         """
         Fit estimator and compute residuals used for prediction intervals.
         All the clones of the estimators for different quantile values are
         stored in order alpha/2, 1 - alpha/2, 0.5 in the ``estimators_``
         attribute. Residuals for the first two estimators and the maximum
         of residuals among these residuals are stored in the
         ``conformity_scores_`` attribute.
 
         Parameters
         ----------
-        X : ArrayLike of shape (n_samples, n_features)
+        X: ArrayLike of shape (n_samples, n_features)
             Training data.
-        y : ArrayLike of shape (n_samples,)
+
+        y: ArrayLike of shape (n_samples,)
             Training labels.
-        sample_weight : Optional[ArrayLike] of shape (n_samples,)
+
+        sample_weight: Optional[ArrayLike] of shape (n_samples,)
             Sample weights for fitting the out-of-fold models.
-            If None, then samples are equally weighted.
+            If ``None``, then samples are equally weighted.
             If some weights are null,
             their corresponding observations are removed
             before the fitting process and hence have no residuals.
             If weights are non-uniform, residuals are still uniformly weighted.
             Note that the sample weight defined are only for the training, not
             for the calibration procedure.
+
             By default ``None``.
-        X_calib : Optional[ArrayLike] of shape (n_calib_samples, n_features)
+
+        X_calib: Optional[ArrayLike] of shape (n_calib_samples, n_features)
             Calibration data.
-        y_calib : Optional[ArrayLike] of shape (n_calib_samples,)
+
+        y_calib: Optional[ArrayLike] of shape (n_calib_samples,)
             Calibration labels.
-        calib_size : Optional[float]
-            If X_calib and y_calib are not defined, then the calibration
-            dataset is created with the split defined by calib_size.
-        random_state : int, RandomState instance or None, default=None
+
+        calib_size: Optional[float]
+            If ``X_calib`` and ``y_calib`` are not defined,
+            then the calibration dataset is created with the split
+            defined by ``calib_size``.
+
+        random_state: Optional[Union[int, np.random.RandomState]], default=None
             For the ``sklearn.model_selection.train_test_split`` documentation.
             Controls the shuffling applied to the data before applying the
             split.
             Pass an int for reproducible output across multiple function calls.
             See :term:`Glossary <random_state>`.
-        shuffle : bool, default=True
+
+            By default ``None``.
+
+        shuffle: bool, default=True
             For the ``sklearn.model_selection.train_test_split`` documentation.
             Whether or not to shuffle the data before splitting.
-            If shuffle=False
-            then stratify must be None.
-        stratify : array-like, default=None
+            If ``shuffle=False`` then stratify must be None.
+
+            By default ``True``.
+
+        stratify: array-like, default=None
             For the ``sklearn.model_selection.train_test_split`` documentation.
-            If not None, data is split in a stratified fashion, using this as
-            the class labels.
+            If not ``None``, data is split in a stratified fashion, using this
+            as the class labels.
             Read more in the :ref:`User Guide <stratification>`.
 
+            By default ``None``.
+
         Returns
         -------
         MapieQuantileRegressor
              The model itself.
         """
         self.cv = self._check_cv(cast(str, self.cv))
 
@@ -623,38 +641,38 @@
         are central to the computation.
         Prediction Intervals for a given ``alpha`` are deduced from the
         quantile regression at the alpha values: alpha/2, 1 - (alpha/2)
         while adding a constant based uppon their residuals.
 
         Parameters
         ----------
-        X : ArrayLike of shape (n_samples, n_features)
+        X: ArrayLike of shape (n_samples, n_features)
             Test data.
-        ensemble : bool
+
+        ensemble: bool
             Ensemble has not been defined in predict and therefore should
             will not have any effects in this method.
-        alpha : Optional[Union[float, Iterable[float]]]
+
+        alpha: Optional[Union[float, Iterable[float]]]
             For ``MapieQuantileRegresor`` the alpha has to be defined
             directly in initial arguments of the class.
-        symmetry : Optional[bool], optional
+
+        symmetry: Optional[bool]
             Deciding factor to whether to find the quantile value for
             each residuals separatly or to use the maximum of the two
             combined.
 
         Returns
         -------
         Union[NDArray, Tuple[NDArray, NDArray]]
-
-        - NDArray of shape (n_samples,) if alpha is None.
-
-        - Tuple[NDArray, NDArray] of shapes
-        (n_samples,) and (n_samples, 2, n_alpha) if alpha is not None.
-
-            - [:, 0, :]: Lower bound of the prediction interval.
-            - [:, 1, :]: Upper bound of the prediction interval.
+            - NDArray of shape (n_samples,) if ``alpha`` is ``None``.
+            - Tuple[NDArray, NDArray] of shapes (n_samples,) and
+              (n_samples, 2, n_alpha) if ``alpha`` is not ``None``.
+                - [:, 0, :]: Lower bound of the prediction interval.
+                - [:, 1, :]: Upper bound of the prediction interval.
         """
         check_is_fitted(self, self.fit_attributes)
         check_defined_variables_predict_cqr(ensemble, alpha)
         alpha = self.alpha if symmetry else self.alpha/2
         check_alpha_and_n_samples(alpha, self.n_calib_samples)
 
         n = self.n_calib_samples
```

### Comparing `MAPIE-0.6.4/mapie/regression.py` & `MAPIE-0.6.5/mapie/regression/regression.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,348 +2,402 @@
 
 from typing import Iterable, List, Optional, Tuple, Union, cast
 
 import numpy as np
 from joblib import Parallel, delayed
 from sklearn.base import BaseEstimator, RegressorMixin, clone
 from sklearn.linear_model import LinearRegression
-from sklearn.model_selection import BaseCrossValidator
+from sklearn.model_selection import BaseCrossValidator, ShuffleSplit
 from sklearn.pipeline import Pipeline
-from sklearn.utils import _safe_indexing
+from sklearn.utils import _safe_indexing, check_random_state
 from sklearn.utils.validation import (_check_y, _num_samples, check_is_fitted,
                                       indexable)
 
-from ._compatibility import np_nanquantile
-from ._typing import ArrayLike, NDArray
-from .aggregation_functions import aggregate_all, phi2D
-from .conformity_scores import ConformityScore
-from .utils import (check_alpha, check_alpha_and_n_samples,
-                    check_conformity_score, check_cv,
-                    check_estimator_fit_predict, check_n_features_in,
-                    check_n_jobs, check_nan_in_aposteriori_prediction,
-                    check_null_weight, check_verbose, fit_estimator)
+from mapie._compatibility import np_nanquantile
+from mapie._typing import ArrayLike, NDArray
+from mapie.aggregation_functions import aggregate_all, phi2D
+from mapie.conformity_scores import ConformityScore
+from mapie.utils import (check_alpha, check_alpha_and_n_samples,
+                         check_conformity_score, check_cv,
+                         check_estimator_fit_predict, check_n_features_in,
+                         check_n_jobs, check_nan_in_aposteriori_prediction,
+                         check_null_weight, check_verbose, fit_estimator)
 
 
 class MapieRegressor(BaseEstimator, RegressorMixin):
     """
     Prediction interval with out-of-fold conformity scores.
 
     This class implements the jackknife+ strategy and its variations
     for estimating prediction intervals on single-output data. The
     idea is to evaluate out-of-fold conformity scores (signed residuals,
     absolute residuals, residuals normalized by the predicted mean...)
     on hold-out validation sets and to deduce valid confidence intervals
-    with strong theoretical
-    guarantees.
+    with strong theoretical guarantees.
 
     Parameters
     ----------
-    estimator : Optional[RegressorMixin]
+    estimator: Optional[RegressorMixin]
         Any regressor with scikit-learn API
-        (i.e. with fit and predict methods), by default ``None``.
+        (i.e. with ``fit`` and ``predict`` methods).
         If ``None``, estimator defaults to a ``LinearRegression`` instance.
 
-    method: str, optional
+        By default ``None``.
+
+    method: str
         Method to choose for prediction interval estimates.
         Choose among:
 
-        - "naive", based on training set conformity scores,
-        - "base", based on validation sets conformity scores,
-        - "plus", based on validation conformity scores and
+        - ``"naive"``, based on training set conformity scores,
+        - ``"base"``, based on validation sets conformity scores,
+        - ``"plus"``, based on validation conformity scores and
           testing predictions,
-        - "minmax", based on validation conformity scores and
+        - ``"minmax"``, based on validation conformity scores and
           testing predictions (min/max among cross-validation clones).
 
-        By default "plus".
+        By default ``"plus"``.
 
     cv: Optional[Union[int, str, BaseCrossValidator]]
         The cross-validation strategy for computing conformity scores.
         It directly drives the distinction between jackknife and cv variants.
         Choose among:
 
         - ``None``, to use the default 5-fold cross-validation
         - integer, to specify the number of folds.
-          If equal to -1, equivalent to
+          If equal to ``-1``, equivalent to
           ``sklearn.model_selection.LeaveOneOut()``.
         - CV splitter: any ``sklearn.model_selection.BaseCrossValidator``
           Main variants are:
-          - ``sklearn.model_selection.LeaveOneOut`` (jackknife),
-          - ``sklearn.model_selection.KFold`` (cross-validation),
-          - ``subsample.Subsample`` object (bootstrap).
+            - ``sklearn.model_selection.LeaveOneOut`` (jackknife),
+            - ``sklearn.model_selection.KFold`` (cross-validation),
+            - ``subsample.Subsample`` object (bootstrap).
+        - ``"split"``, does not involve cross-validation but a division
+          of the data into training and calibration subsets. The splitter
+          used is the following: ``sklearn.model_selection.ShuffleSplit``.
         - ``"prefit"``, assumes that ``estimator`` has been fitted already,
           and the ``method`` parameter is ignored.
           All data provided in the ``fit`` method is then used
           for computing conformity scores only.
           At prediction time, quantiles of these conformity scores are used
           to provide a prediction interval with fixed width.
           The user has to take care manually that data for model fitting and
           conformity scores estimate are disjoint.
 
         By default ``None``.
 
+    test_size: Optional[Union[int, float]]
+        If ``float``, should be between ``0.0`` and ``1.0`` and represent the
+        proportion of the dataset to include in the test split. If ``int``,
+        represents the absolute number of test samples. If ``None``,
+        it will be set to ``0.1``.
+
+        If cv is not ``"split"``, ``test_size`` is ignored.
+
+        By default ``None``.
+
     n_jobs: Optional[int]
         Number of jobs for parallel processing using joblib
         via the "locky" backend.
         If ``-1`` all CPUs are used.
         If ``1`` is given, no parallel computing code is used at all,
         which is useful for debugging.
-        For n_jobs below ``-1``, ``(n_cpus + 1 - n_jobs)`` are used.
-        None is a marker for `unset` that will be interpreted as ``n_jobs=1``
-        (sequential execution).
+        For ``n_jobs`` below ``-1``, ``(n_cpus + 1 - n_jobs)`` are used.
+        ``None`` is a marker for `unset` that will be interpreted as
+        ``n_jobs=1`` (sequential execution).
 
         By default ``None``.
 
-    agg_function : str
+    agg_function: Optional[str]
         Determines how to aggregate predictions from perturbed models, both at
         training and prediction time.
 
-        If ``None``, it is ignored except if cv class is ``Subsample``,
+        If ``None``, it is ignored except if ``cv`` class is ``Subsample``,
         in which case an error is raised.
-        If "mean" or "median", returns the mean or median of the predictions
-        computed from the out-of-folds models.
+        If ``"mean"`` or ``"median"``, returns the mean or median of the
+        predictions computed from the out-of-folds models.
         Note: if you plan to set the ``ensemble`` argument to ``True`` in the
         ``predict`` method, you have to specify an aggregation function.
         Otherwise an error would be raised.
 
         The Jackknife+ interval can be interpreted as an interval around the
         median prediction, and is guaranteed to lie inside the interval,
         unlike the single estimator predictions.
 
-        When the cross-validation strategy is Subsample (i.e. for the
+        When the cross-validation strategy is ``Subsample`` (i.e. for the
         Jackknife+-after-Bootstrap method), this function is also used to
         aggregate the training set in-sample predictions.
 
-        If cv is ``"prefit"``, ``agg_function`` is ignored.
+        If ``cv`` is ``"prefit"`` or ``"split"``, ``agg_function`` is ignored.
 
-        By default "mean".
+        By default ``"mean"``.
 
-    verbose : int, optional
+    verbose: int
         The verbosity level, used with joblib for multiprocessing.
         The frequency of the messages increases with the verbosity level.
         If it more than ``10``, all iterations are reported.
         Above ``50``, the output is sent to stdout.
 
         By default ``0``.
 
-    conformity_score : Optional[ConformityScore]
+    conformity_score: Optional[ConformityScore]
         ConformityScore instance.
         It defines the link between the observed values, the predicted ones
-        and the conformity scores. For instance, the default None value
+        and the conformity scores. For instance, the default ``None`` value
         correspondonds to a conformity score which assumes
         y_obs = y_pred + conformity_score.
 
         - ``None``, to use the default ``AbsoluteConformityScore`` conformity
           score
         - ConformityScore: any ``ConformityScore`` class
 
         By default ``None``.
 
+    random_state: Optional[Union[int, RandomState]]
+        Pseudo random number generator state used for random sampling.
+        Pass an int for reproducible output across multiple function calls.
+
+        By default ``None``.
+
     Attributes
     ----------
-    valid_methods: List[str]
+    valid_methods_: List[str]
         List of all valid methods.
 
-    single_estimator_ : sklearn.RegressorMixin
+    single_estimator_: sklearn.RegressorMixin
         Estimator fitted on the whole training set.
 
-    estimators_ : list
+    estimators_: list
         List of out-of-folds estimators.
 
-    conformity_scores_ : ArrayLike of shape (n_samples_train,)
+    conformity_scores_: ArrayLike of shape (n_samples_train,)
         Conformity scores between ``y_train`` and ``y_pred``.
 
-    k_ : ArrayLike
-        - Array of nans, of shape (len(y), 1) if cv is ``"prefit"``
+    k_: ArrayLike
+        - Array of nans, of shape (len(y), 1) if ``cv`` is ``"prefit"``
           (defined but not used)
         - Dummy array of folds containing each training sample, otherwise.
           Of shape (n_samples_train, cv.get_n_splits(X_train, y_train)).
 
     n_features_in_: int
-        Number of features passed to the fit method.
+        Number of features passed to the ``fit`` method.
 
     References
     ----------
     Rina Foygel Barber, Emmanuel J. Candès,
     Aaditya Ramdas, and Ryan J. Tibshirani.
     "Predictive inference with the jackknife+."
-    Ann. Statist., 49(1):486–507, February 2021.
+    Ann. Statist., 49(1):486-507, February 2021.
 
     Byol Kim, Chen Xu, and Rina Foygel Barber.
     "Predictive Inference Is Free with the Jackknife+-after-Bootstrap."
     34th Conference on Neural Information Processing Systems (NeurIPS 2020).
 
     Examples
     --------
     >>> import numpy as np
     >>> from mapie.regression import MapieRegressor
     >>> from sklearn.linear_model import LinearRegression
     >>> X_toy = np.array([[0], [1], [2], [3], [4], [5]])
     >>> y_toy = np.array([5, 7.5, 9.5, 10.5, 12.5, 15])
-    >>> mapie_reg = MapieRegressor(LinearRegression()).fit(X_toy, y_toy)
+    >>> clf = LinearRegression().fit(X_toy, y_toy)
+    >>> mapie_reg = MapieRegressor(estimator=clf, cv="prefit")
+    >>> mapie_reg = mapie_reg.fit(X_toy, y_toy)
     >>> y_pred, y_pis = mapie_reg.predict(X_toy, alpha=0.5)
     >>> print(y_pis[:, :, 0])
-    [[ 4.7972973   5.8       ]
-     [ 6.69767442  7.65540541]
-     [ 8.59883721  9.58108108]
-     [10.5        11.40116279]
-     [12.4        13.30232558]
-     [14.25       15.20348837]]
+    [[ 4.95714286  5.61428571]
+     [ 6.84285714  7.5       ]
+     [ 8.72857143  9.38571429]
+     [10.61428571 11.27142857]
+     [12.5        13.15714286]
+     [14.38571429 15.04285714]]
     >>> print(y_pred)
     [ 5.28571429  7.17142857  9.05714286 10.94285714 12.82857143 14.71428571]
     """
 
-    cv_need_agg_function = ["Subsample"]
+    cv_need_agg_function_ = ["Subsample"]
+    no_agg_cv_ = ["prefit", "split"]
     valid_methods_ = ["naive", "base", "plus", "minmax"]
-    plus_like_method = ["plus"]
+    no_agg_methods_ = ["naive", "base"]
     valid_agg_functions_ = [None, "median", "mean"]
+    ensemble_agg_functions_ = ["median", "mean"]
     fit_attributes = [
         "single_estimator_",
         "estimators_",
         "k_",
         "conformity_scores_",
         "conformity_score_function_",
         "n_features_in_",
     ]
 
     def __init__(
         self,
         estimator: Optional[RegressorMixin] = None,
         method: str = "plus",
         cv: Optional[Union[int, str, BaseCrossValidator]] = None,
+        test_size: Optional[Union[int, float]] = None,
         n_jobs: Optional[int] = None,
         agg_function: Optional[str] = "mean",
         verbose: int = 0,
         conformity_score: Optional[ConformityScore] = None,
+        random_state: Optional[Union[int, np.random.RandomState]] = None,
     ) -> None:
         self.estimator = estimator
         self.method = method
         self.cv = cv
+        self.test_size = test_size
         self.n_jobs = n_jobs
         self.agg_function = agg_function
         self.verbose = verbose
         self.conformity_score = conformity_score
+        self.random_state = random_state
 
     def _check_parameters(self) -> None:
         """
         Perform several checks on input parameters.
 
         Raises
         ------
         ValueError
             If parameters are not valid.
         """
-        if self.method not in self.valid_methods_:
+        self._check_method(self.method)
+        check_n_jobs(self.n_jobs)
+        check_verbose(self.verbose)
+        check_random_state(self.random_state)
+
+    def _check_method(
+        self, method: str
+    ) -> str:
+        """
+        Check if ``method`` is correct.
+
+        Parameters
+        ----------
+        method: str
+            Method's name to check.
+
+        Returns
+        -------
+        str
+            ``method`` itself.
+
+        Raises
+        ------
+        ValueError
+            If ``method`` is not in ``self.valid_methods_``.
+        """
+        if method not in self.valid_methods_:
             raise ValueError(
                 f"Invalid method. Allowed values are {self.valid_methods_}."
             )
-
-        check_n_jobs(self.n_jobs)
-        check_verbose(self.verbose)
+        else:
+            return method
 
     def _check_agg_function(
         self, agg_function: Optional[str] = None
     ) -> Optional[str]:
         """
         Check if ``agg_function`` is correct, and consistent with other
         arguments.
 
         Parameters
         ----------
-        agg_function : Optional[str], optional
+        agg_function: Optional[str]
             Aggregation function's name to check, by default ``None``.
 
         Returns
         -------
         str
             ``agg_function`` itself or ``"mean"``.
 
         Raises
         ------
         ValueError
             If ``agg_function`` is not in [``None``, ``"mean"``, ``"median"``],
-            or is ``None`` while cv class is in ``cv_need_agg_function``.
+            or is ``None`` while cv class is in ``cv_need_agg_function_``.
         """
         if agg_function not in self.valid_agg_functions_:
             raise ValueError(
                 "Invalid aggregation function "
-                "Allowed values are None, 'mean', 'median'."
+                f"Allowed values are '{self.valid_agg_functions_}'."
             )
-
-        if (agg_function is None) and (
-            type(self.cv).__name__ in self.cv_need_agg_function
+        elif (agg_function is None) and (
+            type(self.cv).__name__ in self.cv_need_agg_function_
         ):
             raise ValueError(
                 "You need to specify an aggregation function when "
-                f"cv's type is in {self.cv_need_agg_function}."
+                f"cv's type is in {self.cv_need_agg_function_}."
             )
-        if (agg_function is not None) or (self.cv == "prefit"):
+        elif (agg_function is not None) or (self.cv in self.no_agg_cv_):
             return agg_function
-        return "mean"
+        else:
+            return "mean"
 
     def _check_estimator(
         self, estimator: Optional[RegressorMixin] = None
     ) -> RegressorMixin:
         """
         Check if estimator is ``None``,
         and returns a ``LinearRegression`` instance if necessary.
         If the ``cv`` attribute is ``"prefit"``,
         check if estimator is indeed already fitted.
 
         Parameters
         ----------
-        estimator : Optional[RegressorMixin], optional
+        estimator: Optional[RegressorMixin]
             Estimator to check, by default ``None``.
 
         Returns
         -------
         RegressorMixin
             The estimator itself or a default ``LinearRegression`` instance.
 
         Raises
         ------
         ValueError
             If the estimator is not ``None``
-            and has no fit nor predict methods.
+            and has no ``fit`` nor ``predict`` methods.
 
         NotFittedError
-            If the estimator is not fitted and ``cv`` attribute is "prefit".
+            If the estimator is not fitted
+            and ``cv`` attribute is ``"prefit"``.
         """
         if estimator is None:
             return LinearRegression()
-        check_estimator_fit_predict(estimator)
-        if self.cv == "prefit":
-            if isinstance(self.estimator, Pipeline):
-                check_is_fitted(self.estimator[-1])
-            else:
-                check_is_fitted(self.estimator)
-        return estimator
+        else:
+            check_estimator_fit_predict(estimator)
+            if self.cv == "prefit":
+                if isinstance(estimator, Pipeline):
+                    check_is_fitted(estimator[-1])
+                else:
+                    check_is_fitted(estimator)
+            return estimator
 
     def _check_ensemble(
-        self,
-        ensemble: bool,
+        self, ensemble: bool,
     ) -> None:
         """
-        Check if ``ensemble`` is False if ``self.agg_function`` is ``None``.
-        Else raise error.
+        Check if ``ensemble`` is ``False`` and if ``self.agg_function``
+        is ``None``. Else raise error.
 
         Parameters
         ----------
-        ensemble : bool
+        ensemble: bool
             ``ensemble`` argument to check the coherennce with
             ``self.agg_function``.
 
         Raises
         ------
         ValueError
-            If ``ensemble`` is True and ``self.agg_function`` is None.
+            If ``ensemble`` is ``True`` and ``self.agg_function`` is ``None``.
         """
         if ensemble and (self.agg_function is None):
             raise ValueError(
                 "If ensemble is True, the aggregation function has to be "
-                "'mean' or 'median'."
+                f"in '{self.ensemble_agg_functions_}'."
             )
 
     def _fit_and_predict_oof_model(
         self,
         estimator: RegressorMixin,
         X: ArrayLike,
         y: ArrayLike,
@@ -353,31 +407,31 @@
     ) -> Tuple[RegressorMixin, NDArray, ArrayLike]:
         """
         Fit a single out-of-fold model on a given training set and
         perform predictions on a test set.
 
         Parameters
         ----------
-        estimator : RegressorMixin
+        estimator: RegressorMixin
             Estimator to train.
 
-        X : ArrayLike of shape (n_samples, n_features)
+        X: ArrayLike of shape (n_samples, n_features)
             Input data.
 
-        y : ArrayLike of shape (n_samples,)
+        y: ArrayLike of shape (n_samples,)
             Input labels.
 
-        train_index : ArrayLike of shape (n_samples_train)
+        train_index: ArrayLike of shape (n_samples_train)
             Training data indices.
 
-        val_index : ArrayLike of shape (n_samples_val)
+        val_index: ArrayLike of shape (n_samples_val)
             Validation data indices.
 
-        sample_weight : Optional[ArrayLike] of shape (n_samples,)
-            Sample weights. If None, then samples are equally weighted.
+        sample_weight: Optional[ArrayLike] of shape (n_samples,)
+            Sample weights. If ``None``, then samples are equally weighted.
             By default ``None``.
 
         Returns
         -------
         Tuple[RegressorMixin, NDArray, ArrayLike]
 
         - [0]: RegressorMixin, fitted estimator
@@ -398,78 +452,85 @@
             )
         if _num_samples(X_val) > 0:
             y_pred = estimator.predict(X_val)
         else:
             y_pred = np.array([])
         return estimator, y_pred, val_index
 
-    def _aggregate_with_mask(self, x: NDArray, k: NDArray) -> NDArray:
+    def _aggregate_with_mask(
+        self,
+        x: NDArray,
+        k: NDArray
+    ) -> NDArray:
         """
         Take the array of predictions, made by the refitted estimators,
         on the testing set, and the 1-or-nan array indicating for each training
         sample which one to integrate, and aggregate to produce phi-{t}(x_t)
         for each training sample x_t.
 
-
         Parameters:
         -----------
-        x : ArrayLike of shape (n_samples_test, n_estimators)
+        x: ArrayLike of shape (n_samples_test, n_estimators)
             Array of predictions, made by the refitted estimators,
             for each sample of the testing set.
 
-        k : ArrayLike of shape (n_samples_training, n_estimators)
+        k: ArrayLike of shape (n_samples_training, n_estimators)
             1-or-nan array: indicates whether to integrate the prediction
             of a given estimator into the aggregation, for each training
             sample.
 
         Returns:
         --------
         ArrayLike of shape (n_samples_test,)
-            Array of aggregated predictions for each testing  sample.
+            Array of aggregated predictions for each testing sample.
         """
-        if self.cv == "prefit":
+        if self.method in self.no_agg_methods_ \
+                or self.cv in self.no_agg_cv_:
             raise ValueError(
-                "There should not be aggregation of predictions if cv is "
-                "'prefit'"
+                "There should not be aggregation of predictions "
+                f"if cv is in '{self.no_agg_cv_}' "
+                f"or if method is in '{self.no_agg_methods_}'."
             )
-        if self.agg_function == "median":
+        elif self.agg_function == "median":
             return phi2D(A=x, B=k, fun=lambda x: np.nanmedian(x, axis=1))
-
         # To aggregate with mean() the aggregation coud be done
         # with phi2D(A=x, B=k, fun=lambda x: np.nanmean(x, axis=1).
         # However, phi2D contains a np.apply_along_axis loop which
         # is much slower than the matrices multiplication that can
         # be used to compute the means.
-        if self.agg_function in ["mean", None]:
+        elif self.agg_function in ["mean", None]:
             K = np.nan_to_num(k, nan=0.0)
             return np.matmul(x, (K / (K.sum(axis=1, keepdims=True))).T)
-        raise ValueError("The value of self.agg_function is not correct")
+        else:
+            raise ValueError("The value of self.agg_function is not correct")
 
-    def _pred_multi(self, X: ArrayLike) -> NDArray:
+    def _pred_multi(
+        self,
+        X: ArrayLike
+    ) -> NDArray:
         """
         Return a prediction per train sample for each test sample, by
-        aggregation with matrix  ``k_``.
+        aggregation with matrix ``k_``.
 
         Parameters
         ----------
-            X: NDArray of shape (n_samples_test, n_features)
-                Input data
+        X: NDArray of shape (n_samples_test, n_features)
+            Input data
 
         Returns
         -------
-            NDArray of shape (n_samples_test, n_samples_train)
+        NDArray of shape (n_samples_test, n_samples_train)
         """
         y_pred_multi = np.column_stack(
             [e.predict(X) for e in self.estimators_]
         )
         # At this point, y_pred_multi is of shape
         # (n_samples_test, n_estimators_). The method
         # ``_aggregate_with_mask`` fits it to the right size
         # thanks to the shape of k_.
-
         y_pred_multi = self._aggregate_with_mask(y_pred_multi, self.k_)
         return y_pred_multi
 
     def fit(
         self,
         X: ArrayLike,
         y: ArrayLike,
@@ -482,23 +543,23 @@
         Fit all cross-validated estimator clones
         and rearrange them into a list, the ``estimators_`` attribute.
         Out-of-fold conformity scores are stored under
         the ``conformity_scores_`` attribute.
 
         Parameters
         ----------
-        X : ArrayLike of shape (n_samples, n_features)
+        X: ArrayLike of shape (n_samples, n_features)
             Training data.
 
-        y : ArrayLike of shape (n_samples,)
+        y: ArrayLike of shape (n_samples,)
             Training labels.
 
-        sample_weight : Optional[ArrayLike] of shape (n_samples,)
+        sample_weight: Optional[ArrayLike] of shape (n_samples,)
             Sample weights for fitting the out-of-fold models.
-            If None, then samples are equally weighted.
+            If ``None``, then samples are equally weighted.
             If some weights are null,
             their corresponding observations are removed
             before the fitting process and hence have no conformity scores.
             If weights are non-uniform,
             conformity scores are still uniformly weighted.
 
             By default ``None``.
@@ -506,15 +567,17 @@
         Returns
         -------
         MapieRegressor
             The model itself.
         """
         # Checks
         self._check_parameters()
-        cv = check_cv(self.cv)
+        cv = check_cv(
+            self.cv, test_size=self.test_size, random_state=self.random_state
+        )
         estimator = self._check_estimator(self.estimator)
         agg_function = self._check_agg_function(self.agg_function)
         X, y = indexable(X, y)
         y = _check_y(y)
         sample_weight = cast(Optional[NDArray], sample_weight)
         self.n_features_in_ = check_n_features_in(X, cv, estimator)
         sample_weight, X, y = check_null_weight(sample_weight, X, y)
@@ -538,23 +601,18 @@
             cv = cast(BaseCrossValidator, cv)
             self.k_ = np.full(
                 shape=(n_samples, cv.get_n_splits(X, y)),
                 fill_value=np.nan,
                 dtype=float,
             )
 
-            pred_matrix = np.full(
-                shape=(n_samples, cv.get_n_splits(X, y)),
-                fill_value=np.nan,
-                dtype=float,
-            )
-
             self.single_estimator_ = fit_estimator(
                 clone(estimator), X, y, sample_weight
             )
+
             if self.method == "naive":
                 y_pred = self.single_estimator_.predict(X)
             else:
                 outputs = Parallel(n_jobs=self.n_jobs, verbose=self.verbose)(
                     delayed(self._fit_and_predict_oof_model)(
                         clone(estimator),
                         X,
@@ -565,121 +623,130 @@
                     )
                     for train_index, val_index in cv.split(X)
                 )
                 self.estimators_, predictions, val_indices = map(
                     list, zip(*outputs)
                 )
 
+                pred_matrix = np.full(
+                    shape=(n_samples, cv.get_n_splits(X, y)),
+                    fill_value=np.nan,
+                    dtype=float,
+                )
                 for i, val_ind in enumerate(val_indices):
                     pred_matrix[val_ind, i] = np.array(
                         predictions[i], dtype=float
                     )
                     self.k_[val_ind, i] = 1
                 check_nan_in_aposteriori_prediction(pred_matrix)
 
                 y_pred = aggregate_all(agg_function, pred_matrix)
 
         self.conformity_scores_ = (
             self.conformity_score_function_.get_conformity_scores(y, y_pred)
         )
 
+        if isinstance(cv, ShuffleSplit):
+            self.single_estimator_ = self.estimators_[0]
+
         return self
 
     def predict(
         self,
         X: ArrayLike,
         ensemble: bool = False,
         alpha: Optional[Union[float, Iterable[float]]] = None,
     ) -> Union[NDArray, Tuple[NDArray, NDArray]]:
         """
         Predict target on new samples with confidence intervals.
         Conformity scores from the training set and predictions
         from the model clones are central to the computation.
         Prediction Intervals for a given ``alpha`` are deduced from either
 
-        - quantiles of conformity scores (naive and base methods),
-        - quantiles of (predictions +/- conformity scores) (plus method),
+        - quantiles of conformity scores (``naive`` and ``base`` methods),
+        - quantiles of (predictions +/- conformity scores) (``plus`` method),
         - quantiles of (max/min(predictions) +/- conformity scores)
-          (minmax method).
+          (``minmax`` method).
 
         Parameters
         ----------
-        X : ArrayLike of shape (n_samples, n_features)
+        X: ArrayLike of shape (n_samples, n_features)
             Test data.
 
         ensemble: bool
             Boolean determining whether the predictions are ensembled or not.
-            If False, predictions are those of the model trained on the whole
-            training set.
-            If True, predictions from perturbed models are aggregated by
+            If ``False``, predictions are those of the model trained on the
+            whole training set.
+            If ``True``, predictions from perturbed models are aggregated by
             the aggregation function specified in the ``agg_function``
             attribute.
 
-            If cv is ``"prefit"``, ``ensemble`` is ignored.
+            If ``cv`` is ``"prefit"`` or ``"split"``, ``ensemble`` is ignored.
 
             By default ``False``.
 
         alpha: Optional[Union[float, Iterable[float]]]
             Can be a float, a list of floats, or a ``ArrayLike`` of floats.
-            Between 0 and 1, represents the uncertainty of the confidence
-            interval.
+            Between ``0`` and ``1``, represents the uncertainty of the
+            confidence interval.
             Lower ``alpha`` produce larger (more conservative) prediction
             intervals.
             ``alpha`` is the complement of the target coverage level.
 
             By default ``None``.
 
         Returns
         -------
         Union[NDArray, Tuple[NDArray, NDArray]]
-
-        - NDArray of shape (n_samples,) if alpha is None.
-
-        - Tuple[NDArray, NDArray] of shapes
-        (n_samples,) and (n_samples, 2, n_alpha) if alpha is not None.
-
-            - [:, 0, :]: Lower bound of the prediction interval.
-            - [:, 1, :]: Upper bound of the prediction interval.
-
+            - NDArray of shape (n_samples,) if ``alpha`` is ``None``.
+            - Tuple[NDArray, NDArray] of shapes (n_samples,) and
+              (n_samples, 2, n_alpha) if ``alpha`` is not ``None``.
+                - [:, 0, :]: Lower bound of the prediction interval.
+                - [:, 1, :]: Upper bound of the prediction interval.
         """
         # Checks
         check_is_fitted(self, self.fit_attributes)
         self._check_ensemble(ensemble)
         alpha = cast(Optional[NDArray], check_alpha(alpha))
+
         y_pred = self.single_estimator_.predict(X)
         n = len(self.conformity_scores_)
 
         if alpha is None:
             return np.array(y_pred)
 
         alpha_np = cast(NDArray, alpha)
         check_alpha_and_n_samples(alpha_np, n)
-        if self.method in ["naive", "base"] or self.cv == "prefit":
+
+        if self.method in self.no_agg_methods_ \
+                or self.cv in self.no_agg_cv_:
             y_pred_multi_low = y_pred[:, np.newaxis]
             y_pred_multi_up = y_pred[:, np.newaxis]
         else:
             y_pred_multi = self._pred_multi(X)
 
             if self.method == "minmax":
                 y_pred_multi_low = np.min(y_pred_multi, axis=1, keepdims=True)
                 y_pred_multi_up = np.max(y_pred_multi, axis=1, keepdims=True)
             else:
                 y_pred_multi_low = y_pred_multi
                 y_pred_multi_up = y_pred_multi
+
             if ensemble:
                 y_pred = aggregate_all(self.agg_function, y_pred_multi)
 
         # compute distributions of lower and upper bounds
         if self.conformity_score_function_.sym:
             conformity_scores_low = -self.conformity_scores_
             conformity_scores_up = self.conformity_scores_
         else:
             conformity_scores_low = self.conformity_scores_
             conformity_scores_up = self.conformity_scores_
             alpha_np = alpha_np / 2
+
         lower_bounds = (
             self.conformity_score_function_.get_estimation_distribution(
                 y_pred_multi_low, conformity_scores_low
             )
         )
         upper_bounds = (
             self.conformity_score_function_.get_estimation_distribution(
@@ -694,21 +761,21 @@
                     lower_bounds.astype(float),
                     _alpha,
                     axis=1,
                     method="lower",
                 )
                 for _alpha in alpha_np
             ]
-        ).data
+        )
         y_pred_up = np.column_stack(
             [
                 np_nanquantile(
                     upper_bounds.astype(float),
                     1 - _alpha,
                     axis=1,
                     method="higher",
                 )
                 for _alpha in alpha_np
             ]
-        ).data
+        )
 
         return y_pred, np.stack([y_pred_low, y_pred_up], axis=1)
```

### Comparing `MAPIE-0.6.4/mapie/subsample.py` & `MAPIE-0.6.5/mapie/subsample.py`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/mapie/tests/test_aggregations_functions.py` & `MAPIE-0.6.5/mapie/tests/test_aggregations_functions.py`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/mapie/tests/test_calibration.py` & `MAPIE-0.6.5/mapie/tests/test_calibration.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,41 +26,73 @@
 
 ESTIMATORS = [
     LogisticRegression(),
     RandomForestClassifier(random_state=random_state),
 ]
 
 results = {
-    "y_score": [
-        [np.nan, 0.33333333, np.nan],
-        [0.66666667, np.nan, np.nan],
-        [np.nan, 0.33333333, np.nan],
-        [np.nan, 0.33333333, np.nan],
-        [np.nan, 0.33333333, np.nan],
-        [np.nan, np.nan, 0.35635314],
-        [np.nan, np.nan, 0.18501723],
-    ],
-    "top_label_ece": 0.3881,
+    "split": {
+        "y_score": [
+            [np.nan, 0.33333333, np.nan],
+            [0.66666667, np.nan, np.nan],
+            [np.nan, 0.33333333, np.nan],
+            [np.nan, 0.33333333, np.nan],
+            [np.nan, 0.33333333, np.nan],
+            [np.nan, np.nan, 0.35635314],
+            [np.nan, np.nan, 0.18501723],
+        ],
+        "top_label_ece": 0.3881,
+    },
+    "prefit": {
+        "y_score": [
+            [np.nan, np.nan, 0.85714286],
+            [0.83333333, np.nan, np.nan],
+            [np.nan, 0.83333333, np.nan],
+            [np.nan, np.nan, 0.85714286],
+            [np.nan, np.nan, 0.85714286],
+            [np.nan, np.nan, 0.85714286],
+            [0.83333333, np.nan, np.nan]
+        ],
+        "top_label_ece": 0.31349206349206343
+    }
 }
 
 results_binary = {
-    "y_score": [
-        [0.76226014, np.nan],
-        [0.39557708, np.nan],
-        [np.nan, 0.66666667],
-        [0.75506701, np.nan],
-        [np.nan, 0.66666667],
-        [0.81175724, np.nan],
-        [0.77294068, np.nan],
-        [0.62599563, np.nan],
-        [np.nan, 0.66666667],
-        [np.nan, 0.66666667],
-    ],
-    "top_label_ece": 0.30562,
-    "ece": 0.56657,
+    "split": {
+        "y_score": [
+            [0.76226014, np.nan],
+            [0.39557708, np.nan],
+            [np.nan, 0.66666667],
+            [0.75506701, np.nan],
+            [np.nan, 0.66666667],
+            [0.81175724, np.nan],
+            [0.77294068, np.nan],
+            [0.62599563, np.nan],
+            [np.nan, 0.66666667],
+            [np.nan, 0.66666667],
+        ],
+        "top_label_ece": 0.30562,
+        "ece": 0.56657,
+    },
+    "prefit": {
+        "y_score": [
+            [0.85714286, np.nan],
+            [np.nan, 0.85714286],
+            [np.nan, 0.85714286],
+            [0.85714286, np.nan],
+            [np.nan, 0.85714286],
+            [0.85714286, np.nan],
+            [0.85714286, np.nan],
+            [0.85714286, np.nan],
+            [np.nan, 0.85714286],
+            [np.nan, 0.85714286]
+        ],
+        "top_label_ece": 0.1428571428571429,
+        "ece": 0.3571428571428571
+    },
 }
 
 
 X, y = make_classification(
     n_samples=20,
     n_classes=3,
     n_informative=4,
@@ -153,21 +185,38 @@
         ValueError,
         match=r".*Invalid method, allowed method are*",
     ):
         mapie_cal = MapieCalibrator(method="no_method")
         mapie_cal.fit(X, y)
 
 
-def test_prefit() -> None:
+def test_prefit_cv_argument() -> None:
     """Test that prefit method works"""
     est = RandomForestClassifier().fit(X, y)
     mapie_cal = MapieCalibrator(estimator=est, cv="prefit")
     mapie_cal.fit(X, y)
 
 
+def test_split_cv_argument() -> None:
+    """Test that split method works"""
+    mapie_cal = MapieCalibrator(cv="split")
+    mapie_cal.fit(X, y)
+
+
+@pytest.mark.parametrize("cv", ["noprefit", "nosplit"])
+def test_invalid_cv_argument(cv: str) -> None:
+    """Test that other cv method does not work"""
+    with pytest.raises(
+        ValueError,
+        match=r".*Invalid cv argument*",
+    ):
+        mapie_cal = MapieCalibrator(cv=cv)
+        mapie_cal.fit(X, y)
+
+
 def test_prefit_split_same_results() -> None:
     """Test that prefit and split method return the same result"""
     est = RandomForestClassifier(
         random_state=random_state
     ).fit(X_train, y_train)
     mapie_cal_prefit = MapieCalibrator(estimator=est, cv="prefit")
     mapie_cal_prefit.fit(X_calib, y_calib)
@@ -246,67 +295,69 @@
     np.testing.assert_allclose(y_pred_calib_set, y_pred_calibrated_test_set)
     np.testing.assert_allclose(
         y_pred_calib_set,
         y_pred_calib_set_through_predict
     )
 
 
-def test_correct_results() -> None:
+@pytest.mark.parametrize("cv", MapieCalibrator.valid_cv)
+def test_correct_results(cv: str) -> None:
     """
     Test that the y_score and top label score from the test dataset result
     in the correct scores (in a multi-class setting).
     """
-    mapie_cal = MapieCalibrator(cv="split")
+    mapie_cal = MapieCalibrator(cv=cv)
     mapie_cal.fit(
         X=X_,
         y=y_,
         random_state=random_state
     )
     pred_ = mapie_cal.predict_proba(X_test)
     top_label_ece_ = top_label_ece(y_test, pred_)
     np.testing.assert_array_almost_equal(
-        results["y_score"], pred_  # type:ignore
+        results[cv]["y_score"], pred_  # type:ignore
     )
     np.testing.assert_allclose(  # type:ignore
-        results["top_label_ece"],
+        results[cv]["top_label_ece"],
         top_label_ece_,
         rtol=1e-2
     )
 
 
-def test_correct_results_binary() -> None:
+@pytest.mark.parametrize("cv", MapieCalibrator.valid_cv)
+def test_correct_results_binary(cv: str) -> None:
     """
     Test that the y_score and top label score from the test dataset result
     in the correct scores (in a binary setting).
     """
     X_binary, y_binary = make_classification(
         n_samples=10,
         n_classes=2,
         n_informative=4,
         random_state=random_state
     )
-    mapie_cal = MapieCalibrator()
+    mapie_cal = MapieCalibrator(cv=cv)
     mapie_cal.fit(
         X=X_binary,
         y=y_binary,
         random_state=random_state
     )
     pred_ = mapie_cal.predict_proba(X_binary)
     top_label_ece_ = top_label_ece(y_binary, pred_)
     ece = expected_calibration_error(y_binary, pred_)
     np.testing.assert_array_almost_equal(
-        results_binary["y_score"], pred_  # type:ignore
+        results_binary[cv]["y_score"], pred_  # type:ignore
     )
     np.testing.assert_allclose(  # type:ignore
-        results_binary["top_label_ece"],
+        results_binary[cv]["top_label_ece"],
         top_label_ece_,
         rtol=1e-2
     )
     np.testing.assert_allclose(  # type:ignore
-        results_binary["ece"],
+        results_binary[cv]["ece"],
         ece,
         rtol=1e-2
     )
 
 
 def test_different_binary_y_combinations() -> None:
     """
```

### Comparing `MAPIE-0.6.4/mapie/tests/test_classification.py` & `MAPIE-0.6.5/mapie/tests/test_classification.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
 from typing import Any, Dict, Iterable, List, Optional, Union, cast
+from copy import deepcopy
 
 import numpy as np
 import pandas as pd
 import pytest
 from sklearn.base import ClassifierMixin
 from sklearn.compose import ColumnTransformer
 from sklearn.datasets import make_classification
 from sklearn.dummy import DummyClassifier
 from sklearn.impute import SimpleImputer
 from sklearn.linear_model import LogisticRegression
-from sklearn.model_selection import KFold, LeaveOneOut
+from sklearn.model_selection import KFold, LeaveOneOut, ShuffleSplit
 from sklearn.pipeline import Pipeline, make_pipeline
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.utils.estimator_checks import check_estimator
 from sklearn.utils.validation import check_is_fitted
 from typing_extensions import TypedDict
 
 from mapie._typing import ArrayLike, NDArray
@@ -72,14 +73,15 @@
 ]
 
 Params = TypedDict(
     "Params",
     {
         "method": str,
         "cv": Optional[Union[int, str]],
+        "test_size": Optional[Union[int, float]],
         "random_state": Optional[int]
     }
 )
 ParamsPredict = TypedDict(
     "ParamsPredict",
     {
         "include_last_label": Union[bool, str],
@@ -88,205 +90,325 @@
 )
 
 STRATEGIES = {
     "score": (
         Params(
             method="score",
             cv="prefit",
+            test_size=None,
+            random_state=42
+        ),
+        ParamsPredict(
+            include_last_label=False,
+            agg_scores="mean"
+        )
+    ),
+    "score_split": (
+        Params(
+            method="score",
+            cv="split",
+            test_size=0.5,
             random_state=42
         ),
         ParamsPredict(
             include_last_label=False,
             agg_scores="mean"
         )
     ),
     "score_cv_mean": (
         Params(
             method="score",
             cv=3,
+            test_size=None,
             random_state=42
         ),
         ParamsPredict(
             include_last_label=False,
             agg_scores="mean"
         )
     ),
     "score_cv_crossval": (
         Params(
             method="score",
             cv=3,
+            test_size=None,
             random_state=42
         ),
         ParamsPredict(
             include_last_label=False,
             agg_scores="crossval"
         )
     ),
     "cumulated_score_include": (
         Params(
             method="cumulated_score",
             cv="prefit",
+            test_size=None,
             random_state=42
         ),
         ParamsPredict(
             include_last_label=True,
             agg_scores="mean"
         )
     ),
     "cumulated_score_not_include": (
         Params(
             method="cumulated_score",
             cv="prefit",
+            test_size=None,
             random_state=42
         ),
         ParamsPredict(
             include_last_label=False,
             agg_scores="mean"
         )
     ),
     "cumulated_score_randomized": (
         Params(
             method="cumulated_score",
             cv="prefit",
+            test_size=None,
+            random_state=42
+        ),
+        ParamsPredict(
+            include_last_label="randomized",
+            agg_scores="mean"
+        )
+    ),
+    "cumulated_score_include_split": (
+        Params(
+            method="cumulated_score",
+            cv="split",
+            test_size=0.5,
+            random_state=42
+        ),
+        ParamsPredict(
+            include_last_label=True,
+            agg_scores="mean"
+        )
+    ),
+    "cumulated_score_not_include_split": (
+        Params(
+            method="cumulated_score",
+            cv="split",
+            test_size=0.5,
+            random_state=42
+        ),
+        ParamsPredict(
+            include_last_label=False,
+            agg_scores="mean"
+        )
+    ),
+    "cumulated_score_randomized_split": (
+        Params(
+            method="cumulated_score",
+            cv="split",
+            test_size=0.5,
             random_state=42
         ),
         ParamsPredict(
             include_last_label="randomized",
             agg_scores="mean"
         )
     ),
     "cumulated_score_include_cv_mean": (
         Params(
             method="cumulated_score",
             cv=3,
+            test_size=None,
             random_state=42
         ),
         ParamsPredict(
             include_last_label=True,
             agg_scores="mean"
         )
     ),
     "cumulated_score_not_include_cv_mean": (
         Params(
             method="cumulated_score",
             cv=3,
+            test_size=None,
             random_state=42
         ),
         ParamsPredict(
             include_last_label=False,
             agg_scores="mean"
         )
     ),
     "cumulated_score_randomized_cv_mean": (
         Params(
             method="cumulated_score",
             cv=3,
+            test_size=None,
             random_state=42
         ),
         ParamsPredict(
             include_last_label="randomized",
             agg_scores="mean"
         )
     ),
     "cumulated_score_include_cv_crossval": (
         Params(
             method="cumulated_score",
             cv=3,
+            test_size=None,
             random_state=42
         ),
         ParamsPredict(
             include_last_label=True,
             agg_scores="crossval"
         )
     ),
     "cumulated_score_not_include_cv_crossval": (
         Params(
             method="cumulated_score",
             cv=3,
+            test_size=None,
             random_state=42
         ),
         ParamsPredict(
             include_last_label=False,
             agg_scores="crossval"
         )
     ),
     "cumulated_score_randomized_cv_crossval": (
         Params(
             method="cumulated_score",
             cv=3,
+            test_size=None,
             random_state=42
         ),
         ParamsPredict(
             include_last_label="randomized",
             agg_scores="crossval"
         )
     ),
     "naive": (
         Params(
             method="naive",
             cv="prefit",
+            test_size=None,
+            random_state=42
+        ),
+        ParamsPredict(
+            include_last_label=True,
+            agg_scores="mean"
+        )
+    ),
+    "naive_split": (
+        Params(
+            method="naive",
+            cv="split",
+            test_size=0.5,
             random_state=42
         ),
         ParamsPredict(
             include_last_label=True,
             agg_scores="mean"
         )
     ),
     "top_k": (
         Params(
             method="top_k",
             cv="prefit",
+            test_size=None,
+            random_state=42
+        ),
+        ParamsPredict(
+            include_last_label=True,
+            agg_scores="mean"
+        )
+    ),
+    "top_k_split": (
+        Params(
+            method="top_k",
+            cv="split",
+            test_size=0.5,
             random_state=42
         ),
         ParamsPredict(
             include_last_label=True,
             agg_scores="mean"
         )
     ),
     "raps": (
         Params(
             method="raps",
             cv="prefit",
+            test_size=None,
+            random_state=42
+        ),
+        ParamsPredict(
+            include_last_label=True,
+            agg_scores="mean"
+        )
+    ),
+    "raps_split": (
+        Params(
+            method="raps",
+            cv="split",
+            test_size=0.5,
             random_state=42
         ),
         ParamsPredict(
             include_last_label=True,
             agg_scores="mean"
         )
     ),
     "raps_randomized": (
         Params(
             method="raps",
             cv="prefit",
+            test_size=None,
+            random_state=42
+        ),
+        ParamsPredict(
+            include_last_label="randomized",
+            agg_scores="mean"
+        )
+    ),
+    "raps_randomized_split": (
+        Params(
+            method="raps",
+            cv="split",
+            test_size=0.5,
             random_state=42
         ),
         ParamsPredict(
             include_last_label="randomized",
             agg_scores="mean"
         )
     ),
 }
 
 COVERAGES = {
-    "score": 6 / 9,
-    "score_cv_mean": 1,
-    "score_cv_crossval": 1,
-    "cumulated_score_include": 1,
-    "cumulated_score_not_include": 5 / 9,
-    "cumulated_score_randomized": 6 / 9,
-    "cumulated_score_include_cv_mean": 1,
-    "cumulated_score_not_include_cv_mean": 5 / 9,
-    "cumulated_score_randomized_cv_mean": 5 / 9,
-    "cumulated_score_include_cv_crossval": 2 / 9,
-    "cumulated_score_not_include_cv_crossval": 0,
-    "cumulated_score_randomized_cv_crossval": 4 / 9,
-    "naive": 5 / 9,
-    "top_k": 1,
-    "raps": 1,
-    "raps_randomized": 8/9
+    "score": 6/9,
+    "score_split": 8/9,
+    "score_cv_mean": 1.0,
+    "score_cv_crossval": 1.0,
+    "cumulated_score_include": 1.0,
+    "cumulated_score_not_include": 5/9,
+    "cumulated_score_randomized": 6/9,
+    "cumulated_score_include_split": 8/9,
+    "cumulated_score_not_include_split": 5/9,
+    "cumulated_score_randomized_split": 7/9,
+    "cumulated_score_include_cv_mean": 1.0,
+    "cumulated_score_not_include_cv_mean": 5/9,
+    "cumulated_score_randomized_cv_mean": 8/9,
+    "cumulated_score_include_cv_crossval": 4/9,
+    "cumulated_score_not_include_cv_crossval": 1/9,
+    "cumulated_score_randomized_cv_crossval": 7/9,
+    "naive": 5/9,
+    "naive_split": 5/9,
+    "top_k": 1.0,
+    "top_k_split": 1.0,
+    "raps": 1.0,
+    "raps_split": 7/9,
+    "raps_randomized": 8/9,
+    "raps_randomized_split": 1.0
 }
 
 X_toy = np.arange(9).reshape(-1, 1)
 y_toy = np.array([0, 0, 1, 0, 1, 1, 2, 1, 2])
 y_toy_string = np.array(["0", "0", "1", "0", "1", "1", "2", "1", "2"])
 
 y_toy_mapie = {
@@ -295,181 +417,269 @@
         [True, False, False],
         [True, False, False],
         [False, True, False],
         [False, True, False],
         [False, True, False],
         [False, True, False],
         [False, True, True],
+        [False, False, True]
+    ],
+    "score_split": [
+        [True, True, False],
+        [True, True, False],
+        [True, True, False],
+        [True, True, False],
+        [True, True, False],
+        [False, True, True],
+        [False, False, True],
+        [False, False, True],
         [False, False, True],
     ],
     "score_cv_mean": [
         [True, False, False],
         [True, False, False],
         [True, True, False],
         [True, True, False],
         [False, True, False],
-        [False, True, False],
         [False, True, True],
         [False, True, True],
         [False, True, True],
+        [False, True, True]
     ],
     "score_cv_crossval": [
         [True, False, False],
         [True, False, False],
         [True, True, False],
         [True, True, False],
         [False, True, False],
         [False, True, False],
         [False, True, True],
         [False, True, True],
-        [False, True, True],
+        [False, True, True]
     ],
     "cumulated_score_include": [
         [True, False, False],
         [True, False, False],
         [True, True, False],
         [True, True, False],
         [False, True, False],
         [False, True, False],
         [False, True, True],
         [False, True, True],
-        [False, False, True],
+        [False, False, True]
     ],
     "cumulated_score_not_include": [
         [True, False, False],
         [True, False, False],
         [True, False, False],
         [False, True, False],
         [False, True, False],
         [False, True, False],
         [False, True, False],
         [False, False, True],
-        [False, False, True],
+        [False, False, True]
     ],
     "cumulated_score_randomized": [
         [True, False, False],
         [True, False, False],
         [True, False, False],
         [False, True, False],
         [False, True, False],
         [False, True, False],
         [False, True, False],
         [False, True, True],
+        [False, False, True]
+    ],
+    "cumulated_score_include_split": [
+        [True, True, False],
+        [True, True, False],
+        [True, True, False],
+        [True, True, False],
+        [True, True, True],
+        [True, True, True],
+        [False, True, True],
         [False, False, True],
+        [False, False, True]
+    ],
+    "cumulated_score_not_include_split": [
+        [False, True, False],
+        [False, True, False],
+        [False, True, False],
+        [False, True, False],
+        [True, True, False],
+        [False, True, True],
+        [False, False, True],
+        [False, False, True],
+        [False, False, True]
+    ],
+    "cumulated_score_randomized_split": [
+        [False, True, False],
+        [True, True, False],
+        [True, True, False],
+        [True, True, False],
+        [True, True, False],
+        [False, True, True],
+        [False, False, True],
+        [False, False, True],
+        [False, False, True]
     ],
     "cumulated_score_include_cv_mean": [
         [True, False, False],
-        [True, False, False],
         [True, True, False],
         [True, True, False],
         [True, True, False],
-        [False, True, False],
+        [True, True, False],
         [False, True, True],
         [False, True, True],
         [False, True, True],
+        [False, True, True]
     ],
     "cumulated_score_not_include_cv_mean": [
         [True, False, False],
         [True, False, False],
         [True, False, False],
         [False, True, False],
         [False, True, False],
         [False, True, False],
         [False, True, False],
-        [False, True, False],
-        [False, True, False],
+        [False, False, True],
+        [False, False, True]
     ],
     "cumulated_score_randomized_cv_mean": [
         [True, False, False],
-        [True, False, False],
-        [True, False, False],
-        [False, True, False],
-        [False, True, False],
+        [True, True, False],
+        [True, True, False],
+        [True, True, False],
+        [True, True, False],
         [False, True, False],
         [False, True, False],
         [False, True, True],
-        [False, True, False],
+        [False, True, True]
     ],
     "cumulated_score_include_cv_crossval": [
         [False, False, False],
-        [False, False, False],
         [True, False, False],
         [False, False, False],
         [False, True, False],
+        [True, True, False],
         [False, True, False],
         [False, True, False],
-        [False, False, False],
-        [False, False, False],
+        [False, True, False],
+        [False, False, False]
     ],
     "cumulated_score_not_include_cv_crossval": [
         [False, False, False],
         [False, False, False],
         [False, False, False],
         [False, False, False],
+        [False, True, False],
         [False, False, False],
         [False, False, False],
         [False, False, False],
-        [False, False, False],
-        [False, False, False],
+        [False, False, False]
     ],
     "cumulated_score_randomized_cv_crossval": [
         [True, False, False],
-        [False, False, False],
+        [True, False, False],
         [True, False, False],
         [False, True, False],
-        [False, True, False],
-        [False, True, False],
+        [True, True, True],
+        [False, True, True],
         [False, True, True],
-        [False, False, True],
         [False, True, False],
+        [False, False, True]
     ],
     "naive": [
         [True, False, False],
         [True, False, False],
         [True, False, False],
         [False, True, False],
         [False, True, False],
         [False, True, False],
         [False, True, False],
         [False, False, True],
+        [False, False, True]
+    ],
+    "naive_split": [
+        [False, True, False],
+        [False, True, False],
+        [False, True, False],
+        [False, True, False],
+        [False, True, False],
+        [False, True, True],
+        [False, False, True],
         [False, False, True],
+        [False, False, True]
     ],
     "top_k": [
         [True, True, False],
         [True, True, False],
         [True, True, False],
         [True, True, False],
         [True, True, False],
         [False, True, True],
         [False, True, True],
         [False, True, True],
+        [False, True, True]
+    ],
+    "top_k_split": [
+        [True, True, False],
+        [True, True, False],
+        [True, True, False],
+        [True, True, False],
+        [True, True, False],
         [False, True, True],
+        [False, True, True],
+        [False, True, True],
+        [False, True, True]
     ],
     "raps": [
         [True, False, False],
         [True, False, False],
         [True, True, False],
         [True, True, False],
         [True, True, False],
         [False, True, True],
         [False, True, True],
         [False, True, True],
-        [False, True, True],
+        [False, True, True]
+    ],
+    "raps_split": [
+        [True, True, False],
+        [True, True, False],
+        [True, True, False],
+        [True, True, False],
+        [True, True, False],
+        [True, True, False],
+        [True, True, False],
+        [True, True, False],
+        [True, True, False]
     ],
     "raps_randomized": [
         [True, False, False],
         [True, False, False],
         [True, True, False],
         [True, True, False],
         [False, True, False],
         [False, True, False],
         [False, True, False],
         [False, True, True],
-        [False, False, True],
+        [False, False, True]
     ],
+    "raps_randomized_split": [
+        [True, True, True],
+        [True, True, True],
+        [True, True, True],
+        [True, True, True],
+        [True, True, True],
+        [True, True, True],
+        [True, True, True],
+        [True, True, True],
+        [True, True, True]
+    ]
 }
 
 REGULARIZATION_PARAMETERS = [
     [.001, [1]],
     [[.01, .2], [1, 3]],
     [.1, [2, 4]]
 ]
@@ -630,17 +840,18 @@
 
 def test_default_parameters() -> None:
     """Test default values of input parameters."""
     mapie_clf = MapieClassifier()
     assert mapie_clf.method == "score"
 
 
-def test_warning_binary_classif() -> None:
+@pytest.mark.parametrize("cv", ["prefit", "split"])
+def test_warning_binary_classif(cv: str) -> None:
     """Test that a warning is raised y is binary."""
-    mapie_clf = MapieClassifier(random_state=42)
+    mapie_clf = MapieClassifier(cv=cv, random_state=42)
     X, y = make_classification(
         n_samples=500,
         n_features=10,
         n_informative=3,
         n_classes=2,
         random_state=1,
     )
@@ -677,15 +888,18 @@
 def test_valid_method(method: str) -> None:
     """Test that valid methods raise no errors."""
     mapie_clf = MapieClassifier(method=method, cv="prefit")
     mapie_clf.fit(X_toy, y_toy)
     check_is_fitted(mapie_clf, mapie_clf.fit_attributes)
 
 
-@pytest.mark.parametrize("cv", [None, -1, 2, KFold(), LeaveOneOut()])
+@pytest.mark.parametrize(
+    "cv", [None, -1, 2, KFold(), LeaveOneOut(),
+           ShuffleSplit(n_splits=1, test_size=0.5), "prefit"]
+)
 def test_valid_cv(cv: Any) -> None:
     """Test that valid cv raises no errors."""
     model = LogisticRegression(multi_class="multinomial")
     model.fit(X_toy, y_toy)
     mapie_clf = MapieClassifier(estimator=model, cv=cv)
     mapie_clf.fit(X_toy, y_toy)
     mapie_clf.predict(X_toy, alpha=0.5)
@@ -775,14 +989,52 @@
         agg_scores=args_predict["agg_scores"]
     )
     n_alpha = len(alpha) if hasattr(alpha, "__len__") else 1
     assert y_pred.shape == (X.shape[0],)
     assert y_ps.shape == (X.shape[0], len(np.unique(y)), n_alpha)
 
 
+@pytest.mark.parametrize(
+    "strategy", ["naive", "top_k", "score", "cumulated_score_include"]
+)
+def test_same_results_prefit_split(strategy: str) -> None:
+    """
+    Test checking that if split and prefit method have exactly
+    the same data split, then we have exactly the same results.
+    """
+    random_state = 1
+    X, y = make_classification(
+        n_samples=500,
+        n_features=10,
+        n_informative=3,
+        n_classes=n_classes,
+        random_state=random_state,
+    )
+    cv = ShuffleSplit(n_splits=1, test_size=0.5, random_state=random_state)
+    train_index, val_index = next(cv.split(X))
+    X_train_, X_calib_ = X[train_index], X[val_index]
+    y_train_, y_calib_ = y[train_index], y[val_index]
+
+    args_init, args_predict = deepcopy(STRATEGIES[strategy + '_split'])
+    args_init["cv"] = cv
+    mapie_reg = MapieClassifier(**args_init)
+    mapie_reg.fit(X, y)
+    y_pred_1, y_pis_1 = mapie_reg.predict(X, alpha=0.1, **args_predict)
+
+    args_init, _ = STRATEGIES[strategy]
+    model = LogisticRegression().fit(X_train_, y_train_)
+    mapie_reg = MapieClassifier(estimator=model, **args_init)
+    mapie_reg.fit(X_calib_, y_calib_)
+    y_pred_2, y_pis_2 = mapie_reg.predict(X, alpha=0.1, **args_predict)
+
+    np.testing.assert_allclose(y_pred_1, y_pred_2)
+    np.testing.assert_allclose(y_pis_1[:, 0, 0], y_pis_2[:, 0, 0])
+    np.testing.assert_allclose(y_pis_1[:, 1, 0], y_pis_2[:, 1, 0])
+
+
 @pytest.mark.parametrize("strategy", [*STRATEGIES])
 @pytest.mark.parametrize("alpha", [0.2, [0.2, 0.3], (0.2, 0.3)])
 def test_same_result_y_numeric_and_string(
     strategy: str, alpha: Any,
 ) -> None:
     """Test that MAPIE outputs the same results if y is
     numeric or string"""
@@ -988,15 +1240,18 @@
     mapie_clf.predict(X_toy, alpha=alpha)
 
 
 @pytest.mark.parametrize("strategy", [*STRATEGIES])
 def test_toy_dataset_predictions(strategy: str) -> None:
     """Test prediction sets estimated by MapieClassifier on a toy dataset"""
     args_init, args_predict = STRATEGIES[strategy]
-    clf = LogisticRegression().fit(X_toy, y_toy)
+    if "split" not in strategy:
+        clf = LogisticRegression().fit(X_toy, y_toy)
+    else:
+        clf = LogisticRegression()
     mapie_clf = MapieClassifier(estimator=clf, **args_init)
     mapie_clf.fit(X_toy, y_toy, size_raps=.5)
     _, y_ps = mapie_clf.predict(
         X_toy,
         alpha=0.5,
         include_last_label=args_predict["include_last_label"],
         agg_scores=args_predict["agg_scores"]
@@ -1203,28 +1458,29 @@
     pipe = make_pipeline(preprocessor, LogisticRegression())
     pipe.fit(X, y)
     mapie = MapieClassifier(estimator=pipe, **STRATEGIES[strategy][0])
     mapie.fit(X, y)
     mapie.predict(X)
 
 
-def test_pred_proba_float64():
+def test_pred_proba_float64() -> None:
     """Check that the method _check_proba_normalized returns float64."""
     y_pred_proba = np.random.random((1000, 10)).astype(np.float32)
     sum_of_rows = y_pred_proba.sum(axis=1)
     normalized_array = y_pred_proba / sum_of_rows[:, np.newaxis]
     mapie = MapieClassifier()
     checked_normalized_array = mapie._check_proba_normalized(normalized_array)
 
     assert checked_normalized_array.dtype == "float64"
 
 
 @pytest.mark.parametrize("cv", ["prefit", None])
-def test_classif_float32(cv):
-    """Check that by returning float64 arrays there are not
+def test_classif_float32(cv) -> None:
+    """
+    Check that by returning float64 arrays there are not
     empty predictions sets with naive method using both
     prefit and cv=5. If the y_pred_proba was still in
     float32, as the quantile=0.90 would have been equal
     to the highest probability, MAPIE would have return
     empty prediction sets"""
     X_cal, y_cal = make_classification(
         n_samples=20,
@@ -1252,48 +1508,51 @@
 
     assert (
         np.repeat([[True, False, False]], 20, axis=0)[:, :, np.newaxis] == yps
     ).all()
 
 
 @pytest.mark.parametrize("k_lambda", REGULARIZATION_PARAMETERS)
-def test_regularize_conf_scores_shape(k_lambda):
-    """Test that the conformity scores have the correct shape.
+def test_regularize_conf_scores_shape(k_lambda) -> None:
+    """
+    Test that the conformity scores have the correct shape.
     """
     lambda_, k = k_lambda[0], k_lambda[1]
     args_init, _ = STRATEGIES["raps"]
     clf = LogisticRegression().fit(X, y)
     mapie_clf = MapieClassifier(estimator=clf, **args_init)
     conf_scores = np.random.rand(100, 1)
     cutoff = np.cumsum(np.ones(conf_scores.shape)) - 1
     reg_conf_scores = mapie_clf._regularize_conformity_score(
         k, lambda_, conf_scores, cutoff
     )
 
     assert reg_conf_scores.shape == (100, 1, len(k))
 
 
-def test_get_true_label_cumsum_proba_shape():
-    """Test that the true label cumsumed probabilities
+def test_get_true_label_cumsum_proba_shape() -> None:
+    """
+    Test that the true label cumsumed probabilities
     have the correct shape.
     """
     clf = LogisticRegression()
     clf.fit(X, y)
     y_pred = clf.predict_proba(X)
     mapie_clf = MapieClassifier(estimator=clf)
     mapie_clf.fit(X, y)
     cumsum_proba, cutoff = mapie_clf._get_true_label_cumsum_proba(
         y, y_pred
     )
     assert cumsum_proba.shape == (len(X), 1)
     assert cutoff.shape == (len(X), )
 
 
-def test_get_true_label_cumsum_proba_result():
-    """Test that the true label cumsumed probabilities
+def test_get_true_label_cumsum_proba_result() -> None:
+    """
+    Test that the true label cumsumed probabilities
     are the expected ones.
     """
     clf = LogisticRegression()
     clf.fit(X_toy, y_toy)
     y_pred = clf.predict_proba(X_toy)
     mapie_clf = MapieClassifier(estimator=clf)
     mapie_clf.fit(X_toy, y_toy)
@@ -1316,15 +1575,16 @@
     )
     np.testing.assert_allclose(cutoff, np.array([1, 1, 2, 2, 1, 1, 2, 2, 1]))
 
 
 @pytest.mark.parametrize("k_lambda", REGULARIZATION_PARAMETERS)
 @pytest.mark.parametrize("strategy", [*STRATEGIES])
 def test_get_last_included_proba_shape(k_lambda, strategy):
-    """Test that the outputs of _get_last_included_proba method
+    """
+    Test that the outputs of _get_last_included_proba method
     have the correct shape.
     """
     lambda_, k = k_lambda[0], k_lambda[1]
     if len(k) == 1:
         thresholds = .2
     else:
         thresholds = np.random.rand(len(k))
@@ -1345,28 +1605,173 @@
 
     assert y_p_p_c.shape == (len(X), len(np.unique(y)), len(thresholds))
     assert y_p_i_l.shape == (len(X), 1, len(thresholds))
     assert y_p_p_i_l.shape == (len(X), 1, len(thresholds))
 
 
 @pytest.mark.parametrize("y_true_proba_place", Y_TRUE_PROBA_PLACE)
-def test_get_true_label_position(y_true_proba_place: List[NDArray]):
-    """Check that the returned true label position the good.
+def test_get_true_label_position(
+    y_true_proba_place: List[NDArray]
+) -> None:
+    """
+    Check that the returned true label position the good.
     """
     y_true = y_true_proba_place[0]
     y_pred_proba = y_true_proba_place[1]
     place = y_true_proba_place[2]
 
     mapie = MapieClassifier()
     found_place = mapie._get_true_label_position(y_pred_proba, y_true)
 
     assert (found_place == place).all()
 
 
 @pytest.mark.parametrize("cv", [5, None])
-def test_error_raps_cv_not_prefit(cv: Union[int, None]):
-    """Test that an error is raised if the method is RAPS
-    and cv is different from prefit.
+def test_error_raps_cv_not_prefit(cv: Union[int, None]) -> None:
+    """
+    Test that an error is raised if the method is RAPS
+    and cv is different from prefit and split.
     """
     mapie = MapieClassifier(method="raps", cv=5)
     with pytest.raises(ValueError, match=r".*RAPS method can only.*"):
         mapie.fit(X_toy, y_toy)
+
+
+def test_not_all_label_in_calib() -> None:
+    """
+    Test that the true label cumsumed probabilities
+    have the correct shape.
+    """
+    clf = LogisticRegression()
+    clf.fit(X, y)
+    indices_remove = np.where(y != 2)
+    X_mapie = X[indices_remove]
+    y_mapie = y[indices_remove]
+    mapie_clf = MapieClassifier(
+        estimator=clf, method="cumulated_score",
+        cv="prefit"
+    )
+    mapie_clf.fit(X_mapie, y_mapie)
+    y_pred, y_pss = mapie_clf.predict(X, alpha=0.5)
+    assert y_pred.shape == (len(X), )
+    assert y_pss.shape == (len(X), len(np.unique(y)), 1)
+
+
+def test_warning_not_all_label_in_calib() -> None:
+    """
+    Test that a warning is raised y is binary.
+    """
+    clf = LogisticRegression()
+    clf.fit(X, y)
+    indices_remove = np.where(y != 2)
+    X_mapie = X[indices_remove]
+    y_mapie = y[indices_remove]
+    mapie_clf = MapieClassifier(
+        estimator=clf, method="cumulated_score",
+        cv="prefit"
+    )
+    with pytest.warns(
+        UserWarning, match=r".*WARNING: your calibration dataset.*"
+    ):
+        mapie_clf.fit(X_mapie, y_mapie)
+
+
+def test_n_classes_prefit() -> None:
+    """
+    Test that the attribute n_classes_ has the correct
+    value with cv="prefit".
+    """
+    clf = LogisticRegression()
+    clf.fit(X, y)
+    indices_remove = np.where(y != 2)
+    X_mapie = X[indices_remove]
+    y_mapie = y[indices_remove]
+    mapie_clf = MapieClassifier(
+        estimator=clf, method="cumulated_score",
+        cv="prefit"
+    )
+    mapie_clf.fit(X_mapie, y_mapie)
+    assert mapie_clf.n_classes_ == len(np.unique(y))
+
+
+def test_classes_prefit() -> None:
+    """
+    Test that the attribute classes_ has the correct
+    value with cv="prefit".
+    """
+    clf = LogisticRegression()
+    clf.fit(X, y)
+    indices_remove = np.where(y != 2)
+    X_mapie = X[indices_remove]
+    y_mapie = y[indices_remove]
+    mapie_clf = MapieClassifier(
+        estimator=clf, method="cumulated_score",
+        cv="prefit"
+    )
+    mapie_clf.fit(X_mapie, y_mapie)
+    assert (mapie_clf.classes_ == np.unique(y)).all()
+
+
+def test_classes_encoder_same_than_model() -> None:
+    """
+    Test that the attribute label encoder has the same
+    classes as the prefit model
+    """
+    clf = LogisticRegression()
+    clf.fit(X, y)
+    indices_remove = np.where(y != 2)
+    X_mapie = X[indices_remove]
+    y_mapie = y[indices_remove]
+    mapie_clf = MapieClassifier(
+        estimator=clf, method="cumulated_score",
+        cv="prefit"
+    )
+    mapie_clf.fit(X_mapie, y_mapie)
+    assert (mapie_clf.label_encoder_.classes_ == np.unique(y)).all()
+
+
+def test_n_classes_cv() -> None:
+    """
+    Test that the attribute n_classes_ has the correct
+    value with cross_validation.
+    """
+    clf = LogisticRegression()
+
+    mapie_clf = MapieClassifier(
+        estimator=clf, method="cumulated_score",
+        cv=5
+    )
+    mapie_clf.fit(X, y)
+    assert mapie_clf.n_classes_ == len(np.unique(y))
+
+
+def test_classes_cv() -> None:
+    """
+    Test that the attribute classes_ has the correct
+    value with cross_validation.
+    """
+    clf = LogisticRegression()
+
+    mapie_clf = MapieClassifier(
+        estimator=clf, method="cumulated_score",
+        cv=5
+    )
+    mapie_clf.fit(X, y)
+    assert (mapie_clf.classes_ == np.unique(y)).all()
+
+
+def test_raise_error_new_class() -> None:
+    """
+    Test that the attribute if there is an unseen
+    classe in `y` then an error is raised.
+    """
+    clf = LogisticRegression()
+    clf.fit(X, y)
+    y[-1] = 10
+    mapie_clf = MapieClassifier(
+        estimator=clf, method="cumulated_score",
+        cv="prefit"
+    )
+    with pytest.raises(
+        ValueError, match=r".*Values in y do not matched values.*"
+    ):
+        mapie_clf.fit(X, y)
```

### Comparing `MAPIE-0.6.4/mapie/tests/test_common.py` & `MAPIE-0.6.5/mapie/tests/test_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 from sklearn.linear_model import LinearRegression, LogisticRegression
 from sklearn.model_selection import KFold
 from sklearn.pipeline import make_pipeline
 from sklearn.utils.estimator_checks import parametrize_with_checks
 from sklearn.utils.validation import check_is_fitted
 
 from mapie.classification import MapieClassifier
-from mapie.quantile_regression import MapieQuantileRegressor
-from mapie.regression import MapieRegressor
+from mapie.regression import MapieQuantileRegressor, MapieRegressor
 
 X_toy = np.arange(18).reshape(-1, 1)
 y_toy = np.array(
     [0, 0, 1, 0, 1, 2, 1, 2, 2, 0, 0, 1, 0, 1, 2, 1, 2, 2]
     )
```

### Comparing `MAPIE-0.6.4/mapie/tests/test_conformity_scores.py` & `MAPIE-0.6.5/mapie/tests/test_conformity_scores.py`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/mapie/tests/test_multi_label_classification.py` & `MAPIE-0.6.5/mapie/tests/test_multi_label_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,28 +114,27 @@
 
 class WrongOutputModel:
 
     def __init__(self):
         pass
 
     def predict_proba(self, *args: Any) -> NDArray:
-        pass
+        """Dummy predict_proba."""
 
     def predict(self, *args: Any) -> NDArray:
-        pass
+        """Dummy predict."""
 
 
 class ArrayOutputModel:
 
     def __init__(self):
         self.trained_ = True
 
     def fit(self, *args: Any) -> None:
         """Dummy fit."""
-        self.trained_ = True
 
     def predict_proba(self, X: NDArray, *args: Any) -> NDArray:
         probas = np.array([[.9, .05, .05]])
         proba_out = np.repeat(probas, len(X), axis=0)
         return proba_out
 
     def predict(self, X: NDArray, *args: Any) -> NDArray:
@@ -429,19 +428,15 @@
     """Test error for wrong method"""
     clf = MultiOutputClassifier(LogisticRegression()).fit(
         X_no_label,
         y_no_label
     )
     mapie_clf = MapieMultiLabelClassifier(clf)
     with pytest.raises(ValueError, match=r".*Invalid y.*"):
-        for i in range(len(X_no_label)):
-            mapie_clf.partial_fit(
-                np.expand_dims(X_no_label[i], axis=0),
-                np.expand_dims(y_no_label[i], axis=0)
-            )
+        mapie_clf.partial_fit(X_no_label, y_no_label)
 
 
 @pytest.mark.parametrize("bound", WRONG_BOUNDS)
 def test_bound_error_in_predict(bound: str) -> None:
     """Test error for wrong method"""
     mapie_clf = MapieMultiLabelClassifier(random_state=42)
     mapie_clf.fit(X_toy, y_toy)
```

### Comparing `MAPIE-0.6.4/mapie/tests/test_quantile_regression.py` & `MAPIE-0.6.5/mapie/tests/test_quantile_regression.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from sklearn.pipeline import Pipeline, make_pipeline
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.utils.validation import check_is_fitted
 from typing_extensions import TypedDict
 
 from mapie._typing import NDArray
 from mapie.metrics import regression_coverage_score
-from mapie.quantile_regression import MapieQuantileRegressor
+from mapie.regression import MapieQuantileRegressor
 
 X_toy = np.array(
     [0, 1, 2, 3, 4, 5, 0, 1, 2, 3, 4, 5, 0, 1, 2, 3, 4,
      5, 0, 1, 2, 3, 4, 5]
 ).reshape(-1, 1)
 y_toy = np.array(
     [5, 7, 9, 11, 13, 15, 5, 7, 9, 11, 13, 15, 5, 7, 9,
@@ -359,15 +359,15 @@
 
 
 @pytest.mark.parametrize("alphas", [1.0, 1.6, 1.95, 5.0, -0.1, -0.001, -10.0])
 def test_wrong_alphas(alphas: float) -> None:
     """Checking for alphas values that are too big according to all value."""
     with pytest.raises(
         ValueError,
-        match=r".*Invalid alpha. Allowed values are between 0 and .*",
+        match=r".*Invalid alpha. Allowed values are between .*",
     ):
         mapie_reg = MapieQuantileRegressor(alpha=alphas)
         mapie_reg.fit(X_train, y_train, X_calib=X_calib, y_calib=y_calib)
 
 
 def test_estimators_quantile_function() -> None:
     """Checking for badly set estimator parameters."""
@@ -728,7 +728,37 @@
     mapie.fit(
         X_train_toy,
         y_train_toy,
         X_calib=X_calib_toy,
         y_calib=y_calib_toy
     )
     mapie.predict(X)
+
+
+def test_deprecated_path_warning() -> None:
+    """
+    Test that a warning is raised if import with deprecated path.
+    """
+    with pytest.warns(
+        FutureWarning,
+        match=r".*WARNING: Deprecated path*"
+    ):
+        from mapie.quantile_regression import MapieQuantileRegressor
+        _ = MapieQuantileRegressor()
+
+
+def test_consistent_class() -> None:
+    """
+    Test that importing a class with a new or obsolete path
+    produces the same results.
+    """
+    from mapie.quantile_regression import MapieQuantileRegressor as C1
+    from mapie.regression import MapieQuantileRegressor as C2
+
+    mapie_c1 = C1(alpha=0.1).fit(X, y, random_state=random_state)
+    mapie_c2 = C2(alpha=0.1).fit(X, y, random_state=random_state)
+
+    y_pred_1, y_pis_1 = mapie_c1.predict(X, alpha=0.1)
+    y_pred_2, y_pis_2 = mapie_c2.predict(X, alpha=0.1)
+    np.testing.assert_allclose(y_pis_1[:, 0, 0], y_pis_2[:, 0, 0])
+    np.testing.assert_allclose(y_pis_1[:, 1, 0], y_pis_2[:, 1, 0])
+    np.testing.assert_allclose(y_pred_1, y_pred_2)
```

### Comparing `MAPIE-0.6.4/mapie/tests/test_regression.py` & `MAPIE-0.6.5/mapie/tests/test_regression.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 import pandas as pd
 import pytest
 from sklearn.compose import ColumnTransformer
 from sklearn.datasets import make_regression
 from sklearn.dummy import DummyRegressor
 from sklearn.impute import SimpleImputer
 from sklearn.linear_model import LinearRegression
-from sklearn.model_selection import KFold, LeaveOneOut, train_test_split
+from sklearn.model_selection import (KFold, LeaveOneOut, ShuffleSplit,
+                                     train_test_split)
 from sklearn.pipeline import Pipeline, make_pipeline
 from sklearn.preprocessing import OneHotEncoder
 from sklearn.utils.validation import check_is_fitted
 from typing_extensions import TypedDict
 
 from mapie._typing import ArrayLike, NDArray
 from mapie.aggregation_functions import aggregate_all
@@ -29,64 +30,109 @@
 y_toy = np.array([5, 7, 9, 11, 13, 15])
 X, y = make_regression(
     n_samples=500, n_features=10, noise=1.0, random_state=1
 )
 k = np.ones(shape=(5, X.shape[1]))
 METHODS = ["naive", "base", "plus", "minmax"]
 
+random_state = 1
+
 Params = TypedDict(
     "Params",
     {
         "method": str,
         "agg_function": str,
         "cv": Optional[Union[int, KFold, Subsample]],
+        "test_size": Optional[Union[int, float]],
+        "random_state": Optional[int],
     },
 )
 STRATEGIES = {
-    "naive": Params(method="naive", agg_function="median", cv=None),
-    "jackknife": Params(method="base", agg_function="mean", cv=-1),
-    "jackknife_plus": Params(method="plus", agg_function="mean", cv=-1),
-    "jackknife_minmax": Params(method="minmax", agg_function="mean", cv=-1),
+    "naive": Params(
+        method="naive",
+        agg_function="median",
+        cv=None,
+        test_size=None,
+        random_state=random_state
+    ),
+    "split": Params(
+        method="base",
+        agg_function="median",
+        cv="split",
+        test_size=0.5,
+        random_state=random_state
+    ),
+    "jackknife": Params(
+        method="base",
+        agg_function="mean",
+        cv=-1,
+        test_size=None,
+        random_state=random_state
+    ),
+    "jackknife_plus": Params(
+        method="plus",
+        agg_function="mean",
+        cv=-1,
+        test_size=None,
+        random_state=random_state
+    ),
+    "jackknife_minmax": Params(
+        method="minmax",
+        agg_function="mean",
+        cv=-1,
+        test_size=None,
+        random_state=random_state
+    ),
     "cv": Params(
         method="base",
         agg_function="mean",
-        cv=KFold(n_splits=3, shuffle=True, random_state=1),
+        cv=KFold(n_splits=3, shuffle=True, random_state=random_state),
+        test_size=None,
+        random_state=random_state
     ),
     "cv_plus": Params(
         method="plus",
         agg_function="mean",
-        cv=KFold(n_splits=3, shuffle=True, random_state=1),
+        cv=KFold(n_splits=3, shuffle=True, random_state=random_state),
+        test_size=None,
+        random_state=random_state
     ),
     "cv_minmax": Params(
         method="minmax",
         agg_function="mean",
-        cv=KFold(n_splits=3, shuffle=True, random_state=1),
+        cv=KFold(n_splits=3, shuffle=True, random_state=random_state),
+        test_size=None,
+        random_state=random_state
     ),
     "jackknife_plus_ab": Params(
         method="plus",
         agg_function="mean",
-        cv=Subsample(n_resamplings=30, random_state=1),
+        cv=Subsample(n_resamplings=30, random_state=random_state),
+        test_size=None,
+        random_state=random_state
     ),
     "jackknife_minmax_ab": Params(
         method="minmax",
         agg_function="mean",
-        cv=Subsample(n_resamplings=30, random_state=1),
+        cv=Subsample(n_resamplings=30, random_state=random_state),
+        test_size=None,
+        random_state=random_state
     ),
     "jackknife_plus_median_ab": Params(
         method="plus",
         agg_function="median",
-        cv=Subsample(
-            n_resamplings=30,
-            random_state=1,
-        ),
+        cv=Subsample(n_resamplings=30, random_state=random_state),
+        test_size=None,
+        random_state=random_state
     ),
 }
 
 WIDTHS = {
     "naive": 3.81,
+    "split": 3.87,
     "jackknife": 3.89,
     "jackknife_plus": 3.90,
     "jackknife_minmax": 3.96,
     "cv": 3.85,
     "cv_plus": 3.90,
     "cv_minmax": 4.04,
     "prefit": 4.81,
@@ -94,14 +140,15 @@
     "jackknife_plus_ab": 3.90,
     "jackknife_minmax_ab": 4.13,
     "jackknife_plus_median_ab": 3.87,
 }
 
 COVERAGES = {
     "naive": 0.952,
+    "split": 0.952,
     "jackknife": 0.952,
     "jackknife_plus": 0.952,
     "jackknife_minmax": 0.952,
     "cv": 0.958,
     "cv_plus": 0.956,
     "cv_minmax": 0.966,
     "prefit": 0.980,
@@ -155,19 +202,25 @@
 @pytest.mark.parametrize("agg_function", [None, "mean", "median"])
 def test_valid_agg_function(agg_function: str) -> None:
     """Test that valid agg_functions raise no errors."""
     mapie_reg = MapieRegressor(agg_function=agg_function)
     mapie_reg.fit(X_toy, y_toy)
 
 
-@pytest.mark.parametrize("cv", [None, -1, 2, KFold(), LeaveOneOut()])
+@pytest.mark.parametrize(
+    "cv", [None, -1, 2, KFold(), LeaveOneOut(),
+           ShuffleSplit(n_splits=1), "prefit", "split"]
+)
 def test_valid_cv(cv: Any) -> None:
     """Test that valid cv raise no errors."""
-    mapie = MapieRegressor(cv=cv)
-    mapie.fit(X_toy, y_toy)
+    model = LinearRegression()
+    model.fit(X_toy, y_toy)
+    mapie_reg = MapieRegressor(estimator=model, cv=cv)
+    mapie_reg.fit(X_toy, y_toy)
+    mapie_reg.predict(X_toy, alpha=0.5)
 
 
 @pytest.mark.parametrize("cv", [100, 200, 300])
 def test_too_large_cv(cv: Any) -> None:
     """Test that too large cv raise sklearn errors."""
     mapie_reg = MapieRegressor(cv=cv)
     with pytest.raises(
@@ -189,14 +242,41 @@
     mapie_reg.fit(X, y)
     y_pred, y_pis = mapie_reg.predict(X, alpha=alpha)
     n_alpha = len(alpha) if hasattr(alpha, "__len__") else 1
     assert y_pred.shape == (X.shape[0],)
     assert y_pis.shape == (X.shape[0], 2, n_alpha)
 
 
+def test_same_results_prefit_split() -> None:
+    """
+    Test checking that if split and prefit method have exactly
+    the same data split, then we have exactly the same results.
+    """
+    X, y = make_regression(
+        n_samples=500, n_features=10, noise=1.0, random_state=1
+    )
+    cv = ShuffleSplit(n_splits=1, test_size=0.1, random_state=random_state)
+    train_index, val_index = list(cv.split(X))[0]
+    X_train, X_calib = X[train_index], X[val_index]
+    y_train, y_calib = y[train_index], y[val_index]
+
+    mapie_reg = MapieRegressor(cv=cv)
+    mapie_reg.fit(X, y)
+    y_pred_1, y_pis_1 = mapie_reg.predict(X, alpha=0.1)
+
+    model = LinearRegression().fit(X_train, y_train)
+    mapie_reg = MapieRegressor(estimator=model, cv="prefit")
+    mapie_reg.fit(X_calib, y_calib)
+    y_pred_2, y_pis_2 = mapie_reg.predict(X, alpha=0.1)
+
+    np.testing.assert_allclose(y_pred_1, y_pred_2)
+    np.testing.assert_allclose(y_pis_1[:, 0, 0], y_pis_2[:, 0, 0])
+    np.testing.assert_allclose(y_pis_1[:, 1, 0], y_pis_2[:, 1, 0])
+
+
 @pytest.mark.parametrize("strategy", [*STRATEGIES])
 def test_results_for_same_alpha(strategy: str) -> None:
     """
     Test that predictions and intervals
     are similar with two equal values of alpha.
     """
     mapie_reg = MapieRegressor(**STRATEGIES[strategy])
@@ -481,17 +561,17 @@
     mapie.predict(X)
 
 
 @pytest.mark.parametrize("strategy", [*STRATEGIES])
 @pytest.mark.parametrize(
     "conformity_score", [AbsoluteConformityScore(), GammaConformityScore()]
 )
-def test_gammaconformityscore(
+def test_conformity_score(
     strategy: str, conformity_score: ConformityScore
 ) -> None:
-    """Test that GammaConformityScore with MAPIE raises no error."""
+    """Test that any conformity score function with MAPIE raises no error."""
     mapie_reg = MapieRegressor(
         conformity_score=conformity_score,
         **STRATEGIES[strategy]
     )
     mapie_reg.fit(X, y + 1e3)
-    _, y_pis = mapie_reg.predict(X, alpha=0.05)
+    mapie_reg.predict(X, alpha=0.05)
```

### Comparing `MAPIE-0.6.4/mapie/tests/test_subsample.py` & `MAPIE-0.6.5/mapie/tests/test_subsample.py`

 * *Files identical despite different names*

### Comparing `MAPIE-0.6.4/mapie/tests/test_time_series_regression.py` & `MAPIE-0.6.5/mapie/tests/test_time_series_regression.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,20 +9,23 @@
 from sklearn.model_selection import KFold, LeaveOneOut, train_test_split
 from sklearn.utils.estimator_checks import check_estimator
 from typing_extensions import TypedDict
 
 from mapie._typing import NDArray
 from mapie.aggregation_functions import aggregate_all
 from mapie.metrics import regression_coverage_score
+from mapie.regression import MapieTimeSeriesRegressor
 from mapie.subsample import BlockBootstrap
-from mapie.time_series_regression import MapieTimeSeriesRegressor
 
+random_state = 1
 X_toy = np.array(range(5)).reshape(-1, 1)
 y_toy = (5.0 + 2.0 * X_toy ** 1.1).flatten()
-X, y = make_regression(n_samples=500, n_features=10, noise=1.0, random_state=1)
+X, y = make_regression(
+    n_samples=500, n_features=10, noise=1.0, random_state=random_state
+)
 k = np.ones(shape=(5, X.shape[1]))
 METHODS = ["enbpi"]
 UPDATE_DATA = ([6], 17.5)
 CONFORMITY_SCORES = [14.189 - 14.038, 17.5 - 18.665]
 
 Params = TypedDict(
     "Params",
@@ -32,37 +35,41 @@
         "cv": Optional[Union[int, KFold, BlockBootstrap]],
     },
 )
 STRATEGIES = {
     "jackknife_enbpi_mean_ab_wopt": Params(
         method="enbpi",
         agg_function="mean",
-        cv=BlockBootstrap(n_resamplings=30, n_blocks=5, random_state=1),
+        cv=BlockBootstrap(
+            n_resamplings=30, n_blocks=5, random_state=random_state
+        ),
     ),
     "jackknife_enbpi_median_ab_wopt": Params(
         method="enbpi",
         agg_function="median",
         cv=BlockBootstrap(
             n_resamplings=30,
             n_blocks=5,
-            random_state=1,
+            random_state=random_state,
         ),
     ),
     "jackknife_enbpi_mean_ab": Params(
         method="enbpi",
         agg_function="mean",
-        cv=BlockBootstrap(n_resamplings=30, n_blocks=5, random_state=1),
+        cv=BlockBootstrap(
+            n_resamplings=30, n_blocks=5, random_state=random_state
+        ),
     ),
     "jackknife_enbpi_median_ab": Params(
         method="enbpi",
         agg_function="median",
         cv=BlockBootstrap(
             n_resamplings=30,
             n_blocks=5,
-            random_state=1,
+            random_state=random_state,
         ),
     ),
 }
 
 WIDTHS = {
     "jackknife_enbpi_mean_ab_wopt": 3.76,
     "jackknife_enbpi_median_ab_wopt": 3.76,
@@ -248,18 +255,18 @@
     np.testing.assert_allclose(width_mean, WIDTHS[strategy], rtol=1e-2)
     np.testing.assert_allclose(coverage, COVERAGES[strategy], rtol=1e-2)
 
 
 def test_results_prefit() -> None:
     """Test prefit results on a standard train/validation/test split."""
     X_train_val, X_test, y_train_val, y_test = train_test_split(
-        X, y, test_size=1 / 10, random_state=1
+        X, y, test_size=1 / 10, random_state=random_state
     )
     X_train, X_val, y_train, y_val = train_test_split(
-        X_train_val, y_train_val, test_size=1 / 9, random_state=1
+        X_train_val, y_train_val, test_size=1 / 9, random_state=random_state
     )
     estimator = LinearRegression().fit(X_train, y_train)
     mapie_ts_reg = MapieTimeSeriesRegressor(estimator=estimator, cv="prefit")
     mapie_ts_reg.fit(X_val, y_val)
     _, y_pis = mapie_ts_reg.predict(X_test, alpha=0.05)
     width_mean = (y_pis[:, 1, 0] - y_pis[:, 0, 0]).mean()
     coverage = regression_coverage_score(
@@ -267,15 +274,18 @@
     )
     np.testing.assert_allclose(width_mean, WIDTHS["prefit"], rtol=1e-2)
     np.testing.assert_allclose(coverage, COVERAGES["prefit"], rtol=1e-2)
 
 
 def test_not_enough_resamplings() -> None:
     """Test that a warning is raised if at least one residual is nan."""
-    with pytest.warns(UserWarning, match=r"WARNING: at least one point of*"):
+    with pytest.warns(
+        UserWarning,
+        match=r"WARNING: at least one point of*"
+    ):
         mapie_ts_reg = MapieTimeSeriesRegressor(
             cv=BlockBootstrap(n_resamplings=1, n_blocks=1), agg_function="mean"
         )
         mapie_ts_reg.fit(X, y)
 
 
 def test_no_agg_fx_specified_with_subsample() -> None:
@@ -349,7 +359,37 @@
 def test_MapieTimeSeriesRegressor_beta_optimize_eeror() -> None:
     """Test ``beta_optimize`` raised error."""
     mapie_ts_reg = MapieTimeSeriesRegressor(cv=-1)
     with pytest.raises(ValueError, match=r".*Lower and upper bounds arrays*"):
         mapie_ts_reg._beta_optimize(
             alpha=0.1, upper_bounds=X, lower_bounds=X_toy
         )
+
+
+def test_deprecated_path_warning() -> None:
+    """
+    Test that a warning is raised if import with deprecated path.
+    """
+    with pytest.warns(
+        FutureWarning,
+        match=r".*WARNING: Deprecated path*"
+    ):
+        from mapie.time_series_regression import MapieTimeSeriesRegressor
+        _ = MapieTimeSeriesRegressor()
+
+
+def test_consistent_class() -> None:
+    """
+    Test that importing a class with a new or obsolete path
+    produces the same results.
+    """
+    from mapie.regression import MapieTimeSeriesRegressor as C2
+    from mapie.time_series_regression import MapieTimeSeriesRegressor as C1
+
+    mapie_c1 = C1(random_state=random_state).fit(X, y)
+    mapie_c2 = C2(random_state=random_state).fit(X, y)
+
+    y_pred_1, y_pis_1 = mapie_c1.predict(X, alpha=0.1)
+    y_pred_2, y_pis_2 = mapie_c2.predict(X, alpha=0.1)
+    np.testing.assert_allclose(y_pis_1[:, 0, 0], y_pis_2[:, 0, 0])
+    np.testing.assert_allclose(y_pis_1[:, 1, 0], y_pis_2[:, 1, 0])
+    np.testing.assert_allclose(y_pred_1, y_pred_2)
```

### Comparing `MAPIE-0.6.4/mapie/tests/test_utils.py` & `MAPIE-0.6.5/mapie/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pytest
 from numpy.random import RandomState
 from sklearn.datasets import make_regression
 from sklearn.linear_model import LinearRegression
 from sklearn.utils.validation import check_is_fitted
 
 from mapie._typing import ArrayLike, NDArray
-from mapie.quantile_regression import MapieQuantileRegressor
+from mapie.regression import MapieQuantileRegressor
 from mapie.utils import (check_alpha, check_alpha_and_n_samples,
                          check_binary_zero_one, check_lower_upper_bounds,
                          check_n_features_in, check_n_jobs, check_null_weight,
                          check_number_bins, check_split_strategy,
                          check_verbose, compute_quantiles, fit_estimator,
                          get_binning_groups)
```

### Comparing `MAPIE-0.6.4/mapie/time_series_regression.py` & `MAPIE-0.6.5/mapie/regression/time_series_regression.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,54 +3,62 @@
 from typing import Iterable, Optional, Tuple, Union, cast
 
 import numpy as np
 from sklearn.base import RegressorMixin
 from sklearn.model_selection import BaseCrossValidator
 from sklearn.utils.validation import check_is_fitted
 
-from ._compatibility import np_nanquantile
-from ._typing import ArrayLike, NDArray
-from .aggregation_functions import aggregate_all
+from mapie._compatibility import np_nanquantile
+from mapie._typing import ArrayLike, NDArray
+from mapie.aggregation_functions import aggregate_all
 from .regression import MapieRegressor
-from .utils import check_alpha, check_alpha_and_n_samples
+from mapie.utils import check_alpha, check_alpha_and_n_samples
 
 
 class MapieTimeSeriesRegressor(MapieRegressor):
     """
     Prediction intervals with out-of-fold residuals for time series.
 
     This class implements the EnbPI strategy for estimating
     prediction intervals on single-output time series. The only valid
-    ``method`` is 'enbpi'.
+    ``method`` is ``"enbpi"``.
 
     Actually, EnbPI only corresponds to ``MapieTimeSeriesRegressor`` if the
     ``cv`` argument is of type ``BlockBootstrap``.
 
     References
     ----------
     Chen Xu, and Yao Xie.
     "Conformal prediction for dynamic time-series."
     https://arxiv.org/abs/2010.09107
     """
 
-    cv_need_agg_function = MapieRegressor.cv_need_agg_function \
+    cv_need_agg_function_ = MapieRegressor.cv_need_agg_function_ \
         + ["BlockBootstrap"]
     valid_methods_ = ["enbpi"]
-    plus_like_method = MapieRegressor.plus_like_method + ["enbpi"]
 
     def __init__(
         self,
         estimator: Optional[RegressorMixin] = None,
         method: str = "enbpi",
         cv: Optional[Union[int, str, BaseCrossValidator]] = None,
         n_jobs: Optional[int] = None,
         agg_function: Optional[str] = "mean",
         verbose: int = 0,
+        random_state: Optional[Union[int, np.random.RandomState]] = None,
     ) -> None:
-        super().__init__(estimator, method, cv, n_jobs, agg_function, verbose)
+        super().__init__(
+            estimator=estimator,
+            method=method,
+            cv=cv,
+            n_jobs=n_jobs,
+            agg_function=agg_function,
+            verbose=verbose,
+            random_state=random_state
+        )
 
     def _relative_conformity_scores(
         self,
         X: ArrayLike,
         y: ArrayLike,
     ) -> NDArray:
         """
@@ -143,14 +151,33 @@
         sample_weight: Optional[ArrayLike] = None,
     ) -> MapieTimeSeriesRegressor:
         """
         Compared to the method ``fit`` of ``MapieRegressor``, the ``fit``
         method of ``MapieTimeSeriesRegressor`` computes the
         ``conformity_scores_`` with relative values.
 
+        Parameters
+        ----------
+        X: ArrayLike of shape (n_samples, n_features)
+            Training data.
+
+        y: ArrayLike of shape (n_samples,)
+            Training labels.
+
+        sample_weight: Optional[ArrayLike] of shape (n_samples,)
+            Sample weights for fitting the out-of-fold models.
+            If ``None``, then samples are equally weighted.
+            If some weights are null,
+            their corresponding observations are removed
+            before the fitting process and hence have no conformity scores.
+            If weights are non-uniform,
+            conformity scores are still uniformly weighted.
+
+            By default ``None``.
+
         Returns
         -------
         MapieTimeSeriesRegressor
             The model itself.
         """
         self = super().fit(X=X, y=y, sample_weight=sample_weight)
         self.conformity_scores_ = self._relative_conformity_scores(X, y)
@@ -164,29 +191,30 @@
         """
         Update the ``conformity_scores_`` attribute when new data with known
         labels are available.
         Note: Don't use ``partial_fit`` with samples of the training set.
 
         Parameters
         ----------
-        X : ArrayLike of shape (n_samples_test, n_features)
+        X: ArrayLike of shape (n_samples_test, n_features)
             Input data.
 
-        y : ArrayLike of shape (n_samples_test,)
+        y: ArrayLike of shape (n_samples_test,)
             Input labels.
 
         Returns
         -------
         MapieTimeSeriesRegressor
             The model itself.
 
         Raises
         ------
         ValueError
-            If the length of y is greater than the length of the training set.
+            If the length of ``y`` is greater than
+            the length of the training set.
         """
         check_is_fitted(self, self.fit_attributes)
         X = cast(NDArray, X)
         y = cast(NDArray, y)
         n = len(self.conformity_scores_)
         if len(X) > n:
             raise ValueError(
@@ -210,17 +238,50 @@
         optimize_beta: bool = True,
     ) -> Union[NDArray, Tuple[NDArray, NDArray]]:
         """
         Correspond to 'Conformal prediction for dynamic time-series'.
 
         Parameters
         ----------
+        X: ArrayLike of shape (n_samples, n_features)
+            Test data.
+
+        ensemble: bool
+            Boolean determining whether the predictions are ensembled or not.
+            If ``False``, predictions are those of the model trained on the
+            whole training set.
+            If ``True``, predictions from perturbed models are aggregated by
+            the aggregation function specified in the ``agg_function``
+            attribute.
+
+            If ``cv`` is ``"prefit"`` or ``"split"``, ``ensemble`` is ignored.
+
+            By default ``False``.
+
+        alpha: Optional[Union[float, Iterable[float]]]
+            Can be a float, a list of floats, or a ``ArrayLike`` of floats.
+            Between ``0`` and ``1``, represents the uncertainty of the
+            confidence interval.
+            Lower ``alpha`` produce larger (more conservative) prediction
+            intervals.
+            ``alpha`` is the complement of the target coverage level.
+
+            By default ``None``.
+
         optimize_beta: bool
             Whether to optimize the PIs' width or not.
 
+        Returns
+        -------
+        Union[NDArray, Tuple[NDArray, NDArray]]
+            - NDArray of shape (n_samples,) if ``alpha`` is ``None``.
+            - Tuple[NDArray, NDArray] of shapes (n_samples,) and
+              (n_samples, 2, n_alpha) if ``alpha`` is not ``None``.
+                - [:, 0, :]: Lower bound of the prediction interval.
+                - [:, 1, :]: Upper bound of the prediction interval.
         """
         # Checks
         check_is_fitted(self, self.fit_attributes)
         self._check_ensemble(ensemble)
         alpha = cast(Optional[NDArray], check_alpha(alpha))
         y_pred = self.single_estimator_.predict(X)
         n = len(self.conformity_scores_)
@@ -251,15 +312,16 @@
             1 - alpha_np + betas_0[0, :],
             axis=0,
             method="higher",
         ).T
         self.lower_quantiles_ = lower_quantiles
         self.higher_quantiles_ = higher_quantiles
 
-        if self.cv == "prefit":
+        if self.method in self.no_agg_methods_ \
+                or self.cv in self.no_agg_cv_:
             y_pred_low = y_pred[:, np.newaxis] + lower_quantiles
             y_pred_up = y_pred[:, np.newaxis] + higher_quantiles
         else:
             y_pred_multi = self._pred_multi(X)
             pred = aggregate_all(self.agg_function, y_pred_multi)
             lower_bounds, upper_bounds = pred, pred
```

### Comparing `MAPIE-0.6.4/mapie/utils.py` & `MAPIE-0.6.5/mapie/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from inspect import signature
 from typing import Any, Iterable, Optional, Tuple, Union, cast
 
 import numpy as np
 from sklearn.base import ClassifierMixin, RegressorMixin
 from sklearn.linear_model import LogisticRegression
 from sklearn.model_selection import (BaseCrossValidator, KFold, LeaveOneOut,
+                                     BaseShuffleSplit, ShuffleSplit,
                                      train_test_split)
 from sklearn.pipeline import Pipeline
 from sklearn.utils import _safe_indexing
 from sklearn.utils.multiclass import type_of_target
 from sklearn.utils.validation import (_check_sample_weight, _num_features,
                                       check_is_fitted, column_or_1d)
 
@@ -24,30 +25,30 @@
     sample_weight: Optional[ArrayLike], X: ArrayLike, y: ArrayLike
 ) -> Tuple[Optional[NDArray], ArrayLike, ArrayLike]:
     """
     Check sample weights and remove samples with null sample weights.
 
     Parameters
     ----------
-    sample_weight : Optional[ArrayLike] of shape (n_samples,)
+    sample_weight: Optional[ArrayLike] of shape (n_samples,)
         Sample weights.
-    X : ArrayLike of shape (n_samples, n_features)
+    X: ArrayLike of shape (n_samples, n_features)
         Training samples.
-    y : ArrayLike of shape (n_samples,)
+    y: ArrayLike of shape (n_samples,)
         Training labels.
 
     Returns
     -------
-    sample_weight : Optional[NDArray] of shape (n_samples,)
+    sample_weight: Optional[NDArray] of shape (n_samples,)
         Non-null sample weights.
 
-    X : ArrayLike of shape (n_samples, n_features)
+    X: ArrayLike of shape (n_samples, n_features)
         Training samples with non-null weights.
 
-    y : ArrayLike of shape (n_samples,)
+    y: ArrayLike of shape (n_samples,)
         Training labels with non-null weights.
 
     Examples
     --------
     >>> import numpy as np
     >>> from mapie.utils import check_null_weight
     >>> X = np.array([[0], [1], [2], [3], [4], [5]])
@@ -85,21 +86,21 @@
     Fit an estimator on training data by distinguishing two cases:
     - the estimator supports sample weights and sample weights are provided.
     - the estimator does not support samples weights or
       samples weights are not provided.
 
     Parameters
     ----------
-    estimator : Union[RegressorMixin, ClassifierMixin]
+    estimator: Union[RegressorMixin, ClassifierMixin]
         Estimator to train.
 
-    X : ArrayLike of shape (n_samples, n_features)
+    X: ArrayLike of shape (n_samples, n_features)
         Input data.
 
-    y : ArrayLike of shape (n_samples,)
+    y: ArrayLike of shape (n_samples,)
         Input labels.
 
     sample_weight : Optional[ArrayLike] of shape (n_samples,)
         Sample weights. If None, then samples are equally weighted.
         By default None.
 
     Returns
@@ -124,68 +125,99 @@
         estimator.fit(X, y, sample_weight=sample_weight)
     else:
         estimator.fit(X, y)
     return estimator
 
 
 def check_cv(
-    cv: Optional[Union[int, str, BaseCrossValidator]] = None
+    cv: Optional[Union[int, str, BaseCrossValidator]] = None,
+    test_size: Optional[Union[int, float]] = None,
+    random_state: Optional[Union[int, np.random.RandomState]] = None,
 ) -> Union[str, BaseCrossValidator]:
     """
     Check if cross-validator is
-    ``None``, ``int``, ``"prefit"`` or ``BaseCrossValidator``.
+    ``None``, ``int``, ``"prefit"``, ``"split"``or ``BaseCrossValidator``.
     Return a ``LeaveOneOut`` instance if integer equal to -1.
     Return a ``KFold`` instance if integer superior or equal to 2.
     Return a ``KFold`` instance if ``None``.
     Else raise error.
 
     Parameters
     ----------
-    cv : Optional[Union[int, str, BaseCrossValidator]], optional
+    cv: Optional[Union[int, str, BaseCrossValidator]], optional
         Cross-validator to check, by default ``None``.
 
+    test_size: Optional[Union[int, float]]
+        If float, should be between 0.0 and 1.0 and represent the proportion
+        of the dataset to include in the test split. If int, represents the
+        absolute number of test samples. If None, it will be set to 0.1.
+
+        If cv is not ``"split"``, ``test_size`` is ignored.
+
+        By default ``None``.
+
+    random_state: Optional[Union[int, np.random.RandomState]], optional
+        Pseudo random number generator state used for random uniform sampling
+        for evaluation quantiles and prediction sets in cumulated_score.
+        Pass an int for reproducible output across multiple function calls.
+        By default ```None``.
+
     Returns
     -------
     Optional[Union[float, str]]
         'prefit' or None.
 
     Raises
     ------
     ValueError
         If the cross-validator is not valid.
     """
     if cv is None:
-        return KFold(n_splits=5)
-    if isinstance(cv, int):
+        return KFold(
+            n_splits=5, shuffle=True, random_state=random_state
+        )
+    elif isinstance(cv, int):
         if cv == -1:
             return LeaveOneOut()
-        if cv >= 2:
-            return KFold(n_splits=cv)
-    if (
-        isinstance(cv, BaseCrossValidator)
-        or (cv == "prefit")
-        or (cv == "split")
-    ):
+        elif cv >= 2:
+            return KFold(
+                n_splits=cv, shuffle=True, random_state=random_state
+            )
+        else:
+            raise ValueError(
+                "Invalid cv argument. "
+                "Allowed integer values are -1 or int >= 2."
+            )
+    elif isinstance(cv, BaseCrossValidator):
         return cv
-    raise ValueError(
-        "Invalid cv argument. "
-        "Allowed values are None, -1, int >= 2, 'prefit', "
-        "or a BaseCrossValidator object (Kfold, LeaveOneOut)."
-    )
+    elif isinstance(cv, BaseShuffleSplit):
+        return cv
+    elif cv == "prefit":
+        return cv
+    elif cv == "split":
+        return ShuffleSplit(
+            n_splits=1, test_size=test_size, random_state=random_state
+        )
+    else:
+        raise ValueError(
+            "Invalid cv argument. "
+            "Allowed values are None, -1, int >= 2, 'prefit', 'split', "
+            "or a BaseCrossValidator object (Kfold, LeaveOneOut)."
+        )
 
 
 def check_alpha(
     alpha: Optional[Union[float, Iterable[float]]] = None
 ) -> Optional[ArrayLike]:
     """
     Check alpha and prepare it as a ArrayLike.
 
     Parameters
     ----------
-    alpha : Union[float, Iterable[float]]
+    alpha: Union[float, Iterable[float]]
         Can be a float, a list of floats, or a ArrayLike of floats.
         Between 0 and 1, represent the uncertainty of the confidence interval.
         Lower alpha produce larger (more conservative) prediction intervals.
         alpha is the complement of the target coverage level.
         Only used at prediction time. By default 0.1.
 
     Returns
@@ -238,22 +270,22 @@
     In general it is simply the number of columns in the data.
     If ``cv=="prefit"`` however,
     it can be deduced from the estimator's ``n_features_in_`` attribute.
     These two values absolutely must coincide.
 
     Parameters
     ----------
-    cv : Optional[Union[float, str]]
+    cv: Optional[Union[float, str]]
         The cross-validation strategy for computing scores,
         by default ``None``.
 
-    X : ArrayLike of shape (n_samples, n_features)
+    X: ArrayLike of shape (n_samples, n_features)
         Data passed into the ``fit`` method.
 
-    estimator : RegressorMixin
+    estimator: RegressorMixin
         Backend estimator of MAPIE.
 
     Returns
     -------
     int
         Expected number of training features.
 
@@ -294,18 +326,18 @@
 ) -> None:
     """
     Check if the quantile can be computed based
     on the number of samples and the alpha value.
 
     Parameters
     ----------
-    alphas : Iterable[float]
+    alphas: Iterable[float]
         Iterable of floats.
 
-    n : int
+    n: int
         number of samples.
 
     Raises
     ------
     ValueError
         If the number of samples of the score is too low,
         1/alpha (or 1/(1 - alpha)) must be lower than the number of samples.
@@ -388,15 +420,15 @@
 def check_nan_in_aposteriori_prediction(X: ArrayLike) -> None:
     """
     Check that all the points are used at least once, otherwise this means
     you have set the number of subsamples too low.
 
     Parameters
     ----------
-    X : Array of shape (size of training set, number of estimators) whose rows
+    X: Array of shape (size of training set, number of estimators) whose rows
     are the predictions by each estimator of each training sample.
 
     Raises
     ------
     Warning
         If the aggregated predictions of any training sample would be nan.
     Examples
@@ -428,20 +460,20 @@
     """
     Check if the lower or upper bounds are consistent.
     If check for MapieQuantileRegressor's outputs, then also check
     initial quantile predictions.
 
     Parameters
     ----------
-    y_preds : NDArray of shape (n_samples, 3) or (n_samples,)
+    y_preds: NDArray of shape (n_samples, 3) or (n_samples,)
         All the predictions at quantile:
         alpha/2, (1 - alpha/2), 0.5 or only the predictions
-    y_pred_low : NDArray of shape (n_samples,)
+    y_pred_low: NDArray of shape (n_samples,)
         Final lower bound prediction
-    y_pred_up : NDArray of shape (n_samples,)
+    y_pred_up: NDArray of shape (n_samples,)
         Final upper bound prediction
 
     Raises
     ------
     Warning
         If y_preds, y_pred_low and y_pred_up are ill sorted
         at anay rank.
@@ -507,20 +539,18 @@
 
 
 def check_conformity_score(
     conformity_score: Optional[ConformityScore],
 ) -> ConformityScore:
     """
     Check parameter ``conformity_score``.
-
     Raises
     ------
     ValueError
         If parameter is not valid.
-
     Examples
     --------
     >>> from mapie.utils import check_conformity_score
     >>> try:
     ...     check_conformity_score(1)
     ... except Exception as exception:
     ...     print(exception)
@@ -545,18 +575,18 @@
 ) -> None:
     """
     Check that the parameters defined for the predict method
     of ``MapieQuantileRegressor`` are correct.
 
     Parameters
     ----------
-    ensemble : bool
+    ensemble: bool
         Ensemble has not been defined in predict and therefore should
         will not have any effects in this method.
-    alpha : Optional[Union[float, Iterable[float]]]
+    alpha: Optional[Union[float, Iterable[float]]]
         For ``MapieQuantileRegresor`` the alpha has to be defined
         directly in initial arguments of the class.
 
     Raises
     ------
     Warning
         If the ensemble value is defined in the predict function
@@ -592,15 +622,15 @@
     estimator: Union[RegressorMixin, ClassifierMixin]
 ) -> None:
     """
     Check that the estimator has a fit and precict method.
 
     Parameters
     ----------
-    estimator : Union[RegressorMixin, ClassifierMixin]
+    estimator: Union[RegressorMixin, ClassifierMixin]
         Estimator to train.
 
     Raises
     ------
     ValueError
         If the estimator does not have a fit or predict attribute.
     """
@@ -613,17 +643,17 @@
 
 def check_alpha_and_last_axis(vector: NDArray, alpha_np: NDArray):
     """Check when the dimension of vector is 3 that its last axis
     size is the same than the number of alphas.
 
     Parameters
     ----------
-    vector : NDArray of shape (n_samples, 1, n_alphas)
+    vector: NDArray of shape (n_samples, 1, n_alphas)
         Vector on which compute the quantile.
-    alpha_np : NDArray of shape (n_alphas, )
+    alpha_np: NDArray of shape (n_alphas, )
         Confidence levels.
 
 
     Raises
     ------
     ValueError
         Error is the last axis dimension is different from the
@@ -639,19 +669,19 @@
 
 
 def compute_quantiles(vector: NDArray, alpha: NDArray) -> NDArray:
     """Compute the desired quantiles of a vector.
 
     Parameters
     ----------
-    vector : NDArray of shape Union[(n_samples, 1), (n_samples, 1, n_alphas)]
+    vector: NDArray of shape Union[(n_samples, 1), (n_samples, 1, n_alphas)]
         Vector on which compute the quantile. If the vector has 3 dimensions,
         then each 1-alpha quantile will be computed on its corresping matrix
         selected on the last axis of the matrix.
-    alpha : NDArray for shape (n_alphas, )
+    alpha: NDArray for shape (n_alphas, )
         Risk levels.
 
     Returns
     -------
     NDArray of shape (n_alphas, )
         Quantiles of the vector.
     """
@@ -752,33 +782,33 @@
     return (
         X_train, y_train, X_calib, y_calib,
         sample_weight_train, sample_weight_calib
     )
 
 
 def check_estimator_classification(
-        X: ArrayLike,
-        y: ArrayLike,
-        cv: Union[str, BaseCrossValidator],
-        estimator: Optional[ClassifierMixin],
+    X: ArrayLike,
+    y: ArrayLike,
+    cv: Union[str, BaseCrossValidator],
+    estimator: Optional[ClassifierMixin],
 ) -> ClassifierMixin:
     """
     Check if estimator is ``None``,
     and returns a ``LogisticRegression`` instance if necessary.
     If the ``cv`` attribute is ``"prefit"``,
     check if estimator is indeed already fitted.
     Parameters
     ----------
-    X : ArrayLike of shape (n_samples, n_features)
+    X: ArrayLike of shape (n_samples, n_features)
         Training data.
-    y : ArrayLike of shape (n_samples,)
+    y: ArrayLike of shape (n_samples,)
         Training labels.
-    cv : Union[str, BaseCrossValidator]
+    cv: Union[str, BaseCrossValidator]
         Cross validation parameter.
-    estimator : Optional[ClassifierMixin]
+    estimator: Optional[ClassifierMixin]
         Estimator to check.
     Returns
     -------
     ClassifierMixin
         The estimator itself or a default ``LogisticRegression`` instance.
     Raises
     ------
@@ -859,21 +889,21 @@
     num_bins: int,
     strategy: str,
 ) -> Union[NDArray, NDArray, NDArray, NDArray]:
     """
     For each bins, calculate the accuracy, average confidence and size.
     Parameters
     ----------
-    y_true : NDArray of shape (n_samples,)
+    y_true: NDArray of shape (n_samples,)
         The "true" values, target for the calibrator.
-    y_score : NDArray of shape (n_samples,)
+    y_score: NDArray of shape (n_samples,)
         The scores given from the calibrator.
-    num_bins : int
+    num_bins: int
         Number of bins to make the split in the y_score.
-    strategy : str
+    strategy: str
         The way of splitting the predictions into different bins.
     Returns
     -------
     Union[NDArray, NDArray, NDArray, NDArray]
     - [0]: NDArray of shape (num_bins,)
     An array of all the splitting points for a new bin.
     - [1]: NDArray of shape (num_bins,)
@@ -907,15 +937,15 @@
     strategy: Optional[str]
 ) -> str:
     """
     Checks that the split strategy provided is valid
     and defults None split strategy to "uniform".
     Parameters
     ----------
-    strategy : Optional[str]
+    strategy: Optional[str]
         Can be a string or None.
 
     Returns
     -------
     str
         The spitting strategy that will be adopted, needs to be a string.
 
@@ -937,15 +967,15 @@
     num_bins: int
 ) -> int:
     """
     Checks that the bin specified is a number.
 
     Parameters
     ----------
-    num_bins : int
+    num_bins: int
         An integer that determines the number of bins to create
         on an array.
 
     Raises
     ------
     ValueError
         When num_bins is not an integer is raises an error.
@@ -973,15 +1003,15 @@
 ) -> NDArray:
     """
     Checks if the array is binary and changes a non binary array
     to a zero, one array.
 
     Parameters
     ----------
-    y_true : ArrayLike of shape (n_samples,)
+    y_true: ArrayLike of shape (n_samples,)
         Could be any array, but in this case is the true values
         as binary input.
 
     Returns
     -------
     NDArray of shape (n_samples,)
         An array of zero, one values.
@@ -1016,17 +1046,17 @@
     """
     Fix shape of y_proba of validation set if number of classes
     of the training set used for cross-validation is different than
     number of classes of the original dataset y.
 
     Parameters
     ----------
-    n_classes_training : NDArray
+    n_classes_training: NDArray
         Classes of the training set.
-    y_proba : NDArray
+    y_proba: NDArray
         Probabilities of the validation set.
 
     Returns
     -------
     NDArray
         Probabilities with the right number of classes.
     """
@@ -1037,7 +1067,141 @@
     np.put_along_axis(
         y_pred_full,
         y_index,
         y_proba,
         axis=1
     )
     return y_pred_full
+
+
+def check_array_shape_classification(
+    y_true: NDArray,
+    y_pred_set: NDArray
+) -> NDArray:
+    """
+    Fix shape of y_pred_set (to 3d array of shape (n_obs, n_class, n_alpha)).
+
+    Parameters
+    ----------
+    y_true: ArrayLike
+        True labels.
+    y_pred_set: ArrayLike
+        Prediction sets given by booleans of labels.
+
+    Returns
+    -------
+    NDArray
+        Fixed y_pred_set.
+
+    Raises
+    ------
+    ValueError
+        If y_true and y_pred_set doesn't have the same number of samples
+        and if y_pred_sets is an array of shape greater than 3 or lower than 2.
+    """
+    if y_true.shape[0] != y_pred_set.shape[0]:
+        raise ValueError(
+            f"shape mismatch between y_true {y_true.shape} \
+                and y_pred_set {y_pred_set.shape}"
+        )
+    if len(y_pred_set.shape) != 3:
+        if len(y_pred_set.shape) != 2:
+            raise ValueError(
+                "y_pred_set should be a 3D array of shape \
+                (n_obs, n_classes, n_alpha)"
+            )
+        else:
+            y_pred_set = np.expand_dims(y_pred_set, axis=2)
+    return y_pred_set
+
+
+def check_array_shape_regression(
+    y_true: NDArray,
+    y_intervals: NDArray
+) -> NDArray:
+    """
+    Fix shape of y_intervals (to 3d array of shape (n_obs, 2, n_alpha)).
+
+    Parameters
+    ----------
+    y_true: NDArray
+        True labels.
+    y_intervals: NDArray
+        Lower and upper bound of prediction intervals
+        with different alpha risks.
+
+    Returns
+    -------
+    NDArray
+        Fixed y_intervals.
+
+    Raises
+    ------
+    ValueError
+        If y_true and y_intervals doesn't have the same number of samples
+        and if y_intervals is an array of shape greater than 3 or lower than 2.
+    """
+    if len(y_intervals.shape) != 3:
+        if len(y_intervals.shape) != 2:
+            raise ValueError(
+                "y_intervals should be a 3D array of shape (n_obs, 2, n_alpha)"
+            )
+        else:
+            y_intervals = np.expand_dims(y_intervals, axis=2)
+    if y_true.shape[0] != y_intervals.shape[0]:
+        raise ValueError(
+            f"shape mismatch between y_true {y_true.shape} \
+                and y_intervals {y_intervals.shape}"
+        )
+    return y_intervals
+
+
+def check_nb_intervals_sizes(widths: NDArray, num_bins: int) -> None:
+    """
+    Checks that the number of bins is less than the number of different
+    interval widths.
+
+    Parameters
+    ----------
+    widths: NDArray (n_samples, n_alpha)
+        Widths of the prediction intervals.
+    num_bins: int
+        Number of bins.
+
+    Raises
+    ------
+    ValueError
+        If the number of bins is greater than the number of different widths.
+    """
+    for alpha in range(widths.shape[1]):
+        nb_widths = len(np.unique(widths[:, alpha].round(5)))
+        if nb_widths <= num_bins:
+            raise ValueError(
+                "The number of bins should be lower or equal to the number of \
+                different interval widths."
+            )
+
+
+def check_nb_sets_sizes(sizes: NDArray, num_bins: int) -> None:
+    """
+    Checks that the number of bins is less than the number of different
+    set sizes.
+
+    Parameters
+    ----------
+    sizes: NDArrat of shape (n_samples, n_alpha)
+        Sizes of the prediction sets.
+    num_bins: int
+        Number of bins.
+
+    Raises
+    ------
+    ValueError
+        If the number of bins is greater than the number of different sizes.
+    """
+    for alpha in range(sizes.shape[1]):
+        nb_sizes = len(np.unique(sizes[:, alpha]))
+        if nb_sizes <= num_bins:
+            raise ValueError(
+                "The number of bins should be less than the number of \
+                different set sizes."
+            )
```

### Comparing `MAPIE-0.6.4/setup.py` & `MAPIE-0.6.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import codecs
 
 from setuptools import find_packages, setup
 
 DISTNAME = "MAPIE"
-VERSION = "0.6.4"
+VERSION = "0.6.5"
 DESCRIPTION = (
     "A scikit-learn-compatible module "
     "for estimating prediction intervals."
 )
 with codecs.open("README.rst", encoding="utf-8-sig") as f:
     LONG_DESCRIPTION = f.read()
 LONG_DESCRIPTION_CONTENT_TYPE = "text/x-rst"
@@ -15,20 +15,19 @@
 DOWNLOAD_URL = "https://pypi.org/project/MAPIE/#files"
 PROJECT_URLS = {
     "Bug Tracker": "https://github.com/scikit-learn-contrib/MAPIE/issues",
     "Documentation": "https://mapie.readthedocs.io/en/latest/",
     "Source Code": "https://github.com/scikit-learn-contrib/MAPIE"
 }
 LICENSE = "new BSD"
-MAINTAINER = "V. Taquet, V. Blot, T. Morzadec, G. Martinon"
+MAINTAINER = "T. Cordier, V. Blot, L. Lacombe"
 MAINTAINER_EMAIL = (
-    "vtaquet@quantmetry.com, "
+    "tcordier@quantmetry.com, "
     "vblot@quantmetry.com, "
-    "tmorzadec@quantmetry.com, "
-    "gmartinon@quantmetry.com"
+    "llacombe@quantmetry.com"
 )
 PYTHON_REQUIRES = ">=3.7"
 PACKAGES = find_packages()
 INSTALL_REQUIRES = ["scikit-learn", "numpy>=1.21", "packaging"]
 CLASSIFIERS = [
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
```

