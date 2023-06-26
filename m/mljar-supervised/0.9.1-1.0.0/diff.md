# Comparing `tmp/mljar-supervised-0.9.1.tar.gz` & `tmp/mljar-supervised-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mljar-supervised-0.9.1.tar", last modified: Tue Mar  2 09:49:51 2021, max compression
+gzip compressed data, was "mljar-supervised-1.0.0.tar", last modified: Mon Jun 26 13:38:22 2023, max compression
```

## Comparing `mljar-supervised-0.9.1.tar` & `mljar-supervised-1.0.0.tar`

### file list

```diff
@@ -1,99 +1,113 @@
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2021-03-02 09:49:51.000000 mljar-supervised-0.9.1/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2021-03-02 09:49:51.000000 mljar-supervised-0.9.1/setup.cfg
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       48 2020-09-29 10:18:51.000000 mljar-supervised-0.9.1/requirements_dev.txt
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2021-03-02 09:49:51.000000 mljar-supervised-0.9.1/supervised/
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2021-03-02 09:49:51.000000 mljar-supervised-0.9.1/supervised/preprocessing/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2390 2020-07-23 07:30:13.000000 mljar-supervised-0.9.1/supervised/preprocessing/text_transformer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3664 2020-12-18 12:36:02.000000 mljar-supervised-0.9.1/supervised/preprocessing/scale.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3861 2021-02-27 15:01:21.000000 mljar-supervised-0.9.1/supervised/preprocessing/kmeans_transformer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4660 2020-12-03 12:30:01.000000 mljar-supervised-0.9.1/supervised/preprocessing/preprocessing_categorical.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3760 2020-12-03 12:30:01.000000 mljar-supervised-0.9.1/supervised/preprocessing/preprocessing_missing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    10323 2021-02-27 15:01:21.000000 mljar-supervised-0.9.1/supervised/preprocessing/goldenfeatures_transformer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3563 2020-07-23 07:30:13.000000 mljar-supervised-0.9.1/supervised/preprocessing/datetime_transformer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    12529 2021-01-15 11:19:26.000000 mljar-supervised-0.9.1/supervised/preprocessing/eda.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1174 2021-01-21 11:57:08.000000 mljar-supervised-0.9.1/supervised/preprocessing/exclude_missing_target.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2018-11-05 13:11:46.000000 mljar-supervised-0.9.1/supervised/preprocessing/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1794 2020-12-03 12:30:01.000000 mljar-supervised-0.9.1/supervised/preprocessing/label_encoder.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1603 2020-12-03 12:30:01.000000 mljar-supervised-0.9.1/supervised/preprocessing/loo_encoder.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3835 2021-01-15 11:19:26.000000 mljar-supervised-0.9.1/supervised/preprocessing/preprocessing_utils.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    26350 2021-02-27 15:01:21.000000 mljar-supervised-0.9.1/supervised/preprocessing/preprocessing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2111 2020-07-13 11:15:38.000000 mljar-supervised-0.9.1/supervised/preprocessing/label_binarizer.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      889 2020-12-03 12:30:01.000000 mljar-supervised-0.9.1/supervised/preprocessing/encoding_selector.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2021-03-02 09:49:51.000000 mljar-supervised-0.9.1/supervised/algorithms/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4550 2021-02-27 15:01:20.000000 mljar-supervised-0.9.1/supervised/algorithms/nn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5221 2021-02-27 15:01:20.000000 mljar-supervised-0.9.1/supervised/algorithms/random_forest.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3487 2021-02-27 15:01:20.000000 mljar-supervised-0.9.1/supervised/algorithms/knn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    10001 2021-02-27 15:01:20.000000 mljar-supervised-0.9.1/supervised/algorithms/catboost.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8558 2021-02-27 15:01:20.000000 mljar-supervised-0.9.1/supervised/algorithms/lightgbm.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2118 2020-10-01 13:32:59.000000 mljar-supervised-0.9.1/supervised/algorithms/registry.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      911 2021-02-27 15:01:20.000000 mljar-supervised-0.9.1/supervised/algorithms/factory.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     9812 2021-02-27 15:01:20.000000 mljar-supervised-0.9.1/supervised/algorithms/xgboost.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4985 2021-02-27 15:01:20.000000 mljar-supervised-0.9.1/supervised/algorithms/extra_trees.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2020-04-07 04:28:59.000000 mljar-supervised-0.9.1/supervised/algorithms/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5018 2021-02-27 15:01:20.000000 mljar-supervised-0.9.1/supervised/algorithms/sklearn.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8094 2021-02-27 15:01:20.000000 mljar-supervised-0.9.1/supervised/algorithms/decision_tree.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2526 2021-02-27 15:01:20.000000 mljar-supervised-0.9.1/supervised/algorithms/baseline.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4125 2021-02-27 15:01:20.000000 mljar-supervised-0.9.1/supervised/algorithms/algorithm.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5974 2021-02-27 15:01:20.000000 mljar-supervised-0.9.1/supervised/algorithms/linear.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    18305 2021-02-27 15:01:20.000000 mljar-supervised-0.9.1/supervised/automl.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2021-03-02 09:49:51.000000 mljar-supervised-0.9.1/supervised/utils/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1052 2020-12-08 11:05:15.000000 mljar-supervised-0.9.1/supervised/utils/common.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      287 2020-09-09 10:59:43.000000 mljar-supervised-0.9.1/supervised/utils/config.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    12103 2020-11-24 10:51:52.000000 mljar-supervised-0.9.1/supervised/utils/shap.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1922 2021-02-27 15:01:21.000000 mljar-supervised-0.9.1/supervised/utils/leaderboard_plots.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      464 2020-10-02 12:50:04.000000 mljar-supervised-0.9.1/supervised/utils/subsample.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3194 2021-02-27 15:01:21.000000 mljar-supervised-0.9.1/supervised/utils/importance.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1482 2021-02-27 15:01:21.000000 mljar-supervised-0.9.1/supervised/utils/data_validation.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      173 2019-03-12 11:52:37.000000 mljar-supervised-0.9.1/supervised/utils/constants.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      184 2019-03-12 11:52:37.000000 mljar-supervised-0.9.1/supervised/utils/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     4772 2021-02-27 15:01:21.000000 mljar-supervised-0.9.1/supervised/utils/learning_curves.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3230 2021-02-27 15:01:21.000000 mljar-supervised-0.9.1/supervised/utils/metric.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    28873 2021-02-27 15:01:21.000000 mljar-supervised-0.9.1/supervised/utils/additional_metrics.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      546 2021-02-27 15:01:21.000000 mljar-supervised-0.9.1/supervised/exceptions.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2021-03-02 09:49:51.000000 mljar-supervised-0.9.1/supervised/tuner/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8735 2021-02-27 15:01:21.000000 mljar-supervised-0.9.1/supervised/tuner/time_controller.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2585 2021-01-12 12:02:31.000000 mljar-supervised-0.9.1/supervised/tuner/data_info.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    36480 2021-02-27 15:01:21.000000 mljar-supervised-0.9.1/supervised/tuner/mljar_tuner.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     6391 2021-02-27 15:01:21.000000 mljar-supervised-0.9.1/supervised/tuner/preprocessing_tuner.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      564 2020-04-14 18:32:55.000000 mljar-supervised-0.9.1/supervised/tuner/random_parameters.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2019-03-13 13:58:54.000000 mljar-supervised-0.9.1/supervised/tuner/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     2213 2021-02-27 15:01:21.000000 mljar-supervised-0.9.1/supervised/tuner/hill_climbing.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    78548 2021-03-02 09:47:58.000000 mljar-supervised-0.9.1/supervised/base_automl.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2021-03-02 09:49:51.000000 mljar-supervised-0.9.1/supervised/callbacks/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      607 2020-04-07 04:28:59.000000 mljar-supervised-0.9.1/supervised/callbacks/max_iters_constraint.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1027 2020-05-21 12:38:18.000000 mljar-supervised-0.9.1/supervised/callbacks/callback_list.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      932 2020-06-02 10:49:03.000000 mljar-supervised-0.9.1/supervised/callbacks/terminate_on_nan.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1700 2020-12-10 13:06:16.000000 mljar-supervised-0.9.1/supervised/callbacks/learner_time_constraint.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     8528 2021-02-27 15:01:20.000000 mljar-supervised-0.9.1/supervised/callbacks/early_stopping.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3352 2021-02-27 15:01:20.000000 mljar-supervised-0.9.1/supervised/callbacks/total_time_constraint.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      592 2019-03-21 16:28:03.000000 mljar-supervised-0.9.1/supervised/callbacks/callback.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2019-03-12 11:52:37.000000 mljar-supervised-0.9.1/supervised/callbacks/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1868 2020-06-02 10:49:03.000000 mljar-supervised-0.9.1/supervised/callbacks/metric_logger.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2021-03-02 09:49:51.000000 mljar-supervised-0.9.1/supervised/validation/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3726 2021-02-27 15:01:21.000000 mljar-supervised-0.9.1/supervised/validation/validator_split.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1187 2019-03-12 11:52:37.000000 mljar-supervised-0.9.1/supervised/validation/validator_with_dataset.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1412 2020-12-08 11:05:15.000000 mljar-supervised-0.9.1/supervised/validation/validation_step.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     5105 2021-01-21 11:57:08.000000 mljar-supervised-0.9.1/supervised/validation/validator_kfold.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2018-11-05 13:12:27.000000 mljar-supervised-0.9.1/supervised/validation/__init__.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2021-03-02 09:49:51.000000 mljar-supervised-0.9.1/supervised/validation/disabled_t_ests/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1505 2019-03-12 11:52:37.000000 mljar-supervised-0.9.1/supervised/validation/disabled_t_ests/test_validator_with_dataset.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1211 2019-03-12 11:52:37.000000 mljar-supervised-0.9.1/supervised/validation/disabled_t_ests/test_validation_step.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1632 2020-04-07 04:28:59.000000 mljar-supervised-0.9.1/supervised/validation/disabled_t_ests/test_validator_split.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      409 2019-03-12 11:52:37.000000 mljar-supervised-0.9.1/supervised/validation/disabled_t_ests/run.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2019-03-12 11:52:37.000000 mljar-supervised-0.9.1/supervised/validation/disabled_t_ests/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      264 2020-12-08 11:05:15.000000 mljar-supervised-0.9.1/supervised/validation/validator_base.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    19648 2021-02-27 15:01:21.000000 mljar-supervised-0.9.1/supervised/model_framework.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       60 2021-03-02 09:48:43.000000 mljar-supervised-0.9.1/supervised/__init__.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    17351 2021-02-27 15:01:21.000000 mljar-supervised-0.9.1/supervised/ensemble.py
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    14017 2021-03-02 09:49:18.000000 mljar-supervised-0.9.1/README.md
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    16941 2021-03-02 09:49:51.000000 mljar-supervised-0.9.1/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       47 2020-05-04 15:21:30.000000 mljar-supervised-0.9.1/MANIFEST.in
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      278 2021-02-27 15:01:20.000000 mljar-supervised-0.9.1/requirements.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1062 2018-11-05 13:05:32.000000 mljar-supervised-0.9.1/LICENSE
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     1127 2021-03-02 09:49:08.000000 mljar-supervised-0.9.1/setup.py
-drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2021-03-02 09:49:51.000000 mljar-supervised-0.9.1/mljar_supervised.egg-info/
--rw-rw-r--   0 piotr     (1000) piotr     (1000)    16941 2021-03-02 09:49:51.000000 mljar-supervised-0.9.1/mljar_supervised.egg-info/PKG-INFO
--rw-rw-r--   0 piotr     (1000) piotr     (1000)      278 2021-03-02 09:49:51.000000 mljar-supervised-0.9.1/mljar_supervised.egg-info/requires.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)     3155 2021-03-02 09:49:51.000000 mljar-supervised-0.9.1/mljar_supervised.egg-info/SOURCES.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2021-03-02 09:49:51.000000 mljar-supervised-0.9.1/mljar_supervised.egg-info/dependency_links.txt
--rw-rw-r--   0 piotr     (1000) piotr     (1000)       11 2021-03-02 09:49:51.000000 mljar-supervised-0.9.1/mljar_supervised.egg-info/top_level.txt
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1073 2022-03-28 10:53:20.000000 mljar-supervised-1.0.0/LICENSE
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       47 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/MANIFEST.in
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26713 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    22164 2023-06-26 11:22:02.000000 mljar-supervised-1.0.0/README.md
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.905047 mljar-supervised-1.0.0/mljar_supervised.egg-info/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26713 2023-06-26 13:38:22.000000 mljar-supervised-1.0.0/mljar_supervised.egg-info/PKG-INFO
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3461 2023-06-26 13:38:22.000000 mljar-supervised-1.0.0/mljar_supervised.egg-info/SOURCES.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        1 2023-06-26 13:38:22.000000 mljar-supervised-1.0.0/mljar_supervised.egg-info/dependency_links.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      310 2023-06-26 13:38:22.000000 mljar-supervised-1.0.0/mljar_supervised.egg-info/requires.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       11 2023-06-26 13:38:22.000000 mljar-supervised-1.0.0/mljar_supervised.egg-info/top_level.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      309 2023-06-26 11:10:20.000000 mljar-supervised-1.0.0/requirements.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       48 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/requirements_dev.txt
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       38 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/setup.cfg
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1213 2023-06-26 13:37:16.000000 mljar-supervised-1.0.0/setup.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.905047 mljar-supervised-1.0.0/supervised/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)       60 2023-06-26 13:37:44.000000 mljar-supervised-1.0.0/supervised/__init__.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.905047 mljar-supervised-1.0.0/supervised/algorithms/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/algorithms/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4172 2021-09-02 10:34:57.000000 mljar-supervised-1.0.0/supervised/algorithms/algorithm.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2524 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/baseline.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    14472 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/catboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9168 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/decision_tree.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5170 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/extra_trees.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      911 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/algorithms/factory.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3550 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/knn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12114 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/lightgbm.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5972 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/linear.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4792 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/nn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5406 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/random_forest.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2349 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/registry.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6108 2023-06-26 08:29:57.000000 mljar-supervised-1.0.0/supervised/algorithms/sklearn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12628 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/algorithms/xgboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26161 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/automl.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)   100170 2023-06-26 11:40:41.000000 mljar-supervised-1.0.0/supervised/base_automl.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/supervised/callbacks/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/callbacks/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      592 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/callbacks/callback.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1027 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/callbacks/callback_list.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     9058 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/callbacks/early_stopping.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1700 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/callbacks/learner_time_constraint.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      607 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/callbacks/max_iters_constraint.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1867 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/callbacks/metric_logger.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      932 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/callbacks/terminate_on_nan.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3351 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/callbacks/total_time_constraint.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    23009 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/ensemble.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      546 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/exceptions.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/supervised/fairness/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2023-06-26 08:29:57.000000 mljar-supervised-1.0.0/supervised/fairness/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26295 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/fairness/metrics.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    15058 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/fairness/optimization.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4049 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/fairness/plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3863 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/fairness/report.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      701 2023-06-26 08:29:57.000000 mljar-supervised-1.0.0/supervised/fairness/utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    29363 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/model_framework.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/supervised/preprocessing/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/preprocessing/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3563 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/preprocessing/datetime_transformer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12634 2023-06-26 11:40:03.000000 mljar-supervised-1.0.0/supervised/preprocessing/eda.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      889 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/preprocessing/encoding_selector.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1509 2023-06-26 08:29:57.000000 mljar-supervised-1.0.0/supervised/preprocessing/exclude_missing_target.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    10747 2023-06-26 11:40:03.000000 mljar-supervised-1.0.0/supervised/preprocessing/goldenfeatures_transformer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3866 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/preprocessing/kmeans_transformer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2458 2023-06-26 11:40:07.000000 mljar-supervised-1.0.0/supervised/preprocessing/label_binarizer.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1804 2022-12-30 13:35:06.000000 mljar-supervised-1.0.0/supervised/preprocessing/label_encoder.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1613 2023-06-26 08:29:57.000000 mljar-supervised-1.0.0/supervised/preprocessing/loo_encoder.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    26512 2023-06-26 11:40:03.000000 mljar-supervised-1.0.0/supervised/preprocessing/preprocessing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4658 2023-06-26 11:40:03.000000 mljar-supervised-1.0.0/supervised/preprocessing/preprocessing_categorical.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3759 2023-06-26 11:40:03.000000 mljar-supervised-1.0.0/supervised/preprocessing/preprocessing_missing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4038 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/preprocessing/preprocessing_utils.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3664 2023-06-26 11:40:03.000000 mljar-supervised-1.0.0/supervised/preprocessing/scale.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2603 2021-09-30 14:10:40.000000 mljar-supervised-1.0.0/supervised/preprocessing/text_transformer.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/supervised/tuner/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/tuner/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2584 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/tuner/data_info.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2409 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/tuner/hill_climbing.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    58739 2023-06-26 11:40:41.000000 mljar-supervised-1.0.0/supervised/tuner/mljar_tuner.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/supervised/tuner/optuna/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/tuner/optuna/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5634 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/tuner/optuna/catboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2635 2022-12-30 13:09:00.000000 mljar-supervised-1.0.0/supervised/tuner/optuna/extra_trees.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2054 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/tuner/optuna/knn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5999 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/tuner/optuna/lightgbm.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2260 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/tuner/optuna/nn.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     2637 2022-12-30 13:09:15.000000 mljar-supervised-1.0.0/supervised/tuner/optuna/random_forest.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    11488 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/tuner/optuna/tuner.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4824 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/tuner/optuna/xgboost.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     6389 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/tuner/preprocessing_tuner.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      564 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/tuner/random_parameters.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     8974 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/tuner/time_controller.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/supervised/utils/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      184 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/utils/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    37134 2023-06-26 11:40:41.000000 mljar-supervised-1.0.0/supervised/utils/additional_metrics.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     7895 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/utils/additional_plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5409 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/utils/automl_plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1052 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/utils/common.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      524 2021-09-17 07:39:41.000000 mljar-supervised-1.0.0/supervised/utils/config.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      173 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/utils/constants.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1481 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/utils/data_validation.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     3204 2021-09-02 10:34:57.000000 mljar-supervised-1.0.0/supervised/utils/importance.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4949 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/utils/leaderboard_plots.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4880 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/utils/learning_curves.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    13752 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/utils/metric.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)    12099 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/utils/shap.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      463 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/utils/subsample.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      628 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/utils/utils.py
+drwxrwxr-x   0 piotr     (1000) piotr     (1000)        0 2023-06-26 13:38:22.909047 mljar-supervised-1.0.0/supervised/validation/
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)        0 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/validation/__init__.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     1211 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/validation/validation_step.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)      264 2021-09-02 08:06:45.000000 mljar-supervised-1.0.0/supervised/validation/validator_base.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4267 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/validation/validator_custom.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     5611 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/validation/validator_kfold.py
+-rw-rw-r--   0 piotr     (1000) piotr     (1000)     4788 2023-06-26 11:40:40.000000 mljar-supervised-1.0.0/supervised/validation/validator_split.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mljar-supervised-0.9.1/supervised/preprocessing/text_transformer.py` & `mljar-supervised-1.0.0/supervised/preprocessing/text_transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import pandas as pd
+import warnings
 import datetime
 import json
 from sklearn.feature_extraction.text import TfidfVectorizer
 
 
 class TextTransformer(object):
     def __init__(self):
@@ -19,29 +20,32 @@
             stop_words="english",
             lowercase=True,
             max_features=self._max_features,
         )
 
         x = X[column][~pd.isnull(X[column])]
         self._vectorizer.fit(x)
-        for f in self._vectorizer.get_feature_names():
+        for f in list(self._vectorizer.get_feature_names_out()):
             new_col = self._old_column + "_" + f
             self._new_columns += [new_col]
 
     def transform(self, X):
+        with warnings.catch_warnings():
+            warnings.simplefilter(
+                action="ignore", category=pd.errors.PerformanceWarning
+            )
+            ii = ~pd.isnull(X[self._old_column])
+            x = X[self._old_column][ii]
+            vect = self._vectorizer.transform(x)
 
-        ii = ~pd.isnull(X[self._old_column])
-        x = X[self._old_column][ii]
-        vect = self._vectorizer.transform(x)
+            for f in self._new_columns:
+                X[f] = 0.0
 
-        for f in self._new_columns:
-            X[f] = 0.0
-
-        X.loc[ii, self._new_columns] = vect.toarray()
-        X.drop(self._old_column, axis=1, inplace=True)
+            X.loc[ii, self._new_columns] = vect.toarray()
+            X.drop(self._old_column, axis=1, inplace=True)
         return X
 
     def to_json(self):
         for k in self._vectorizer.vocabulary_.keys():
             self._vectorizer.vocabulary_[k] = int(self._vectorizer.vocabulary_[k])
 
         data_json = {
```

### Comparing `mljar-supervised-0.9.1/supervised/preprocessing/scale.py` & `mljar-supervised-1.0.0/supervised/preprocessing/scale.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,62 @@
 import pandas as pd
 import numpy as np
 
 from sklearn import preprocessing
 
 
 class Scale(object):
-
     SCALE_NORMAL = "scale_normal"
     SCALE_LOG_AND_NORMAL = "scale_log_and_normal"
 
     def __init__(self, columns=[], scale_method=SCALE_NORMAL):
         self.scale_method = scale_method
         self.columns = columns
         self.scale = preprocessing.StandardScaler(
             copy=True, with_mean=True, with_std=True
         )
         self.X_min_values = None  # it is used in SCALE_LOG_AND_NORMAL
 
     def fit(self, X):
-
         if len(self.columns):
             for c in self.columns:
                 X[c] = X[c].astype(float)
 
             if self.scale_method == self.SCALE_NORMAL:
                 self.scale.fit(X[self.columns])
             elif self.scale_method == self.SCALE_LOG_AND_NORMAL:
-                self.X_min_values = np.min(X[self.columns])
+                self.X_min_values = np.min(X[self.columns], axis=0)
                 self.scale.fit(np.log(X[self.columns] - self.X_min_values + 1))
 
     def transform(self, X):
-
         if len(self.columns):
             X.loc[:, self.columns] = X.loc[:, self.columns].astype(float)
             if self.scale_method == self.SCALE_NORMAL:
                 X.loc[:, self.columns] = self.scale.transform(X[self.columns])
             elif self.scale_method == self.SCALE_LOG_AND_NORMAL:
-
                 X[self.columns] = np.log(
                     np.clip(
                         X[self.columns] - self.X_min_values + 1, a_min=1, a_max=None
                     )
                 )
                 X.loc[:, self.columns] = self.scale.transform(X[self.columns])
         return X
 
     def inverse_transform(self, X):
-
         if len(self.columns):
-
             if self.scale_method == self.SCALE_NORMAL:
                 X.loc[:, self.columns] = self.scale.inverse_transform(X[self.columns])
             elif self.scale_method == self.SCALE_LOG_AND_NORMAL:
-
                 X[self.columns] = self.scale.inverse_transform(X[self.columns])
                 X[self.columns] = np.exp(X[self.columns])
 
                 X.loc[:, self.columns] += self.X_min_values - 1
         return X
 
     def to_json(self):
-
         if len(self.columns) == 0:
             return None
         data_json = {
             "scale": list(self.scale.scale_),
             "mean": list(self.scale.mean_),
             "var": list(self.scale.var_),
             "n_samples_seen": int(self.scale.n_samples_seen_),
```

### Comparing `mljar-supervised-0.9.1/supervised/preprocessing/kmeans_transformer.py` & `mljar-supervised-1.0.0/supervised/preprocessing/kmeans_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,17 @@
         X = self._scale.fit_transform(X)
 
         # Kmeans
         self._kmeans = kmeans = MiniBatchKMeans(n_clusters=n_clusters, init="k-means++")
         self._kmeans.fit(X)
         self._create_new_features_names()
 
-        print(
-            f"Created {len(self._new_features)} KMeans Features in {np.round(time.time() - start_time,2)} seconds."
-        )
+        # print(
+        #    f"Created {len(self._new_features)} KMeans Features in {np.round(time.time() - start_time,2)} seconds."
+        # )
 
     def _create_new_features_names(self):
         n_clusters = self._kmeans.cluster_centers_.shape[0]
         self._new_features = [f"Dist_Cluster_{i}" for i in range(n_clusters)]
         self._new_features += ["Cluster"]
 
     def transform(self, X):
```

### Comparing `mljar-supervised-0.9.1/supervised/preprocessing/preprocessing_categorical.py` & `mljar-supervised-1.0.0/supervised/preprocessing/preprocessing_categorical.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from supervised.preprocessing.preprocessing_utils import PreprocessingUtils
 from supervised.preprocessing.label_encoder import LabelEncoder
 from supervised.preprocessing.label_binarizer import LabelBinarizer
 from supervised.preprocessing.loo_encoder import LooEncoder
 
 
 class PreprocessingCategorical(object):
-
     CONVERT_ONE_HOT = "categorical_to_onehot"
     CONVERT_INTEGER = "categorical_to_int"
     CONVERT_LOO = "categorical_to_loo"
 
     FEW_CATEGORIES = "few_categories"
     MANY_CATEGORIES = "many_categories"
 
@@ -32,15 +31,14 @@
             self._enc = LooEncoder(cols=self._columns)
             self._enc.fit(X, y)
         else:
             self._fit_categorical_convert(X)
 
     def _fit_categorical_convert(self, X):
         for column in self._columns:
-
             if PreprocessingUtils.get_type(X[column]) != PreprocessingUtils.CATEGORICAL:
                 # no need to convert, already a number
                 continue
             # limit categories - it is needed when doing one hot encoding
             # this code is also used in predict.py file
             # and transform_utils.py
             # TODO it needs refactoring !!!
```

### Comparing `mljar-supervised-0.9.1/supervised/preprocessing/preprocessing_missing.py` & `mljar-supervised-1.0.0/supervised/preprocessing/preprocessing_missing.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import numpy as np
 import pandas as pd
 
 from supervised.preprocessing.preprocessing_utils import PreprocessingUtils
 
 
 class PreprocessingMissingValues(object):
-
     FILL_NA_MIN = "na_fill_min_1"
     FILL_NA_MEAN = "na_fill_mean"
     FILL_NA_MEDIAN = "na_fill_median"
     FILL_DATETIME = "na_fill_datetime"
 
     NA_EXCLUDE = "na_exclude"
     MISSING_VALUE = "_missing_value_"
```

### Comparing `mljar-supervised-0.9.1/supervised/preprocessing/goldenfeatures_transformer.py` & `mljar-supervised-1.0.0/supervised/preprocessing/goldenfeatures_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import numpy as np
 import pandas as pd
 import datetime
 import json
 import time
 import itertools
-from multiprocessing import Pool
+from joblib import Parallel, delayed
 from sklearn.model_selection import train_test_split
 from sklearn.tree import DecisionTreeClassifier, DecisionTreeRegressor
 from sklearn.metrics import log_loss, mean_squared_error
 from supervised.algorithms.registry import (
     BINARY_CLASSIFICATION,
     MULTICLASS_CLASSIFICATION,
     REGRESSION,
@@ -100,18 +100,20 @@
         multiply_score = None
         print(str(e))
 
     return (diff_score, ratio_1_score, ratio_2_score, sum_score, multiply_score)
 
 
 class GoldenFeaturesTransformer(object):
-    def __init__(self, results_path=None, ml_task=None):
+    def __init__(self, results_path=None, ml_task=None, features_count=None, n_jobs=-1):
         self._new_features = []
         self._new_columns = []
         self._ml_task = ml_task
+        self._features_count = features_count
+        self._n_jobs = n_jobs
         self._scorer = None
         if self._ml_task == BINARY_CLASSIFICATION:
             self._scorer = get_binary_score
         elif self._ml_task == MULTICLASS_CLASSIFICATION:
             self._scorer = get_multiclass_score
         else:
             self._scorer = get_regression_score
@@ -149,16 +151,18 @@
         X_train, X_test, y_train, y_test = self._subsample(X, y)
 
         for i in range(len(items)):
             items[i] += (X_train, y_train, X_test, y_test, self._scorer)
 
         scores = []
         # parallel version
-        with Pool() as p:
-            scores = p.map(get_score, items)
+        scores = Parallel(n_jobs=self._n_jobs, backend="loky")(
+            delayed(get_score)(i) for i in items
+        )
+
         # single process version
         # for item in items:
         #    scores += [get_score(item)]
 
         if not scores:
             self._error = f"Golden Features not created. Empty scores. Input data shape: {X.shape}, {y.shape}"
             self.save()
@@ -180,14 +184,22 @@
         df = pd.DataFrame(
             result, columns=["feature1", "feature2", "operation", "score"]
         )
         df.sort_values(by="score", inplace=True)
 
         new_cols_cnt = np.min([100, np.max([10, int(0.1 * X.shape[1])])])
 
+        if (
+            self._features_count is not None
+            and self._features_count > 0
+            and self._features_count < df.shape[0]
+        ):
+            new_cols_cnt = self._features_count
+
+        print(self._features_count, new_cols_cnt)
         self._new_features = json.loads(df.head(new_cols_cnt).to_json(orient="records"))
 
         for new_feature in self._new_features:
             new_col = "_".join(
                 [
                     new_feature["feature1"],
                     new_feature["operation"],
@@ -247,15 +259,14 @@
         self._result_path = os.path.join(results_path, self._result_file)
 
     def save(self):
         with open(self._result_path, "w") as fout:
             fout.write(json.dumps(self.to_json(), indent=4))
 
     def _subsample(self, X, y):
-
         MAX_SIZE = 10000
         TRAIN_SIZE = 2500
 
         shuffle = True
         stratify = None
 
         if X.shape[0] > MAX_SIZE:
```

### Comparing `mljar-supervised-0.9.1/supervised/preprocessing/datetime_transformer.py` & `mljar-supervised-1.0.0/supervised/preprocessing/datetime_transformer.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-0.9.1/supervised/preprocessing/eda.py` & `mljar-supervised-1.0.0/supervised/preprocessing/eda.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,41 +24,40 @@
 MAXCOL = 25
 
 import string
 import base64
 
 
 class EDA:
-    """ Creates plots for Automated Exploratory Data Analysis. """
+    """Creates plots for Automated Exploratory Data Analysis."""
 
     @staticmethod
     def prepare(column):
-        """ Prepare the column to be used as file name. """
+        """Prepare the column to be used as file name."""
         valid_chars = "-_.() %s%s" % (string.ascii_letters, string.digits)
         valid_chars = frozenset(valid_chars)
         col = "".join(c for c in column if c in valid_chars)
         if not len(col):
             col = base64.urlsafe_b64encode(column.encode("utf-8"))
             col = col.decode("utf-8")
         return col.replace(" ", "_")
 
     @staticmethod
     def plot_fname(column):
-        """ Returns file name for the plot based on the column name. """
+        """Returns file name for the plot based on the column name."""
         return EDA.prepare(column) + ".png"
 
     @staticmethod
     def plot_path(eda_path, column):
-        """ Returns full path for the plot based on the column name. """
+        """Returns full path for the plot based on the column name."""
         fname = os.path.join(eda_path, EDA.plot_fname(column))
         return fname
 
     @staticmethod
     def compute(X, y, eda_path):
-
         # Check for empty dataframes in params
         if X.empty:
             raise ValueError("X is empty")
         if y.empty:
             raise ValueError("y is empty")
         try:
             # check if exists
@@ -69,20 +68,19 @@
             else:
                 # need to create directory for EDA analysis
                 os.mkdir(eda_path)
 
             inform = defaultdict(list)
 
             if isinstance(y, pd.Series):
-
                 plt.figure(figsize=(5, 5))
                 if PreprocessingUtils.get_type(y) in ("categorical"):
-                    sns.countplot(y, color=BLUE)
+                    sns.countplot(data=y, color=BLUE)
                 else:
-                    sns.distplot(y, color=BLUE)
+                    sns.displot(data=y, color=BLUE)
                 plt.title("Target class distribution")
                 plt.tight_layout(pad=2.0)
                 plt.savefig(EDA.plot_path(eda_path, "target"))
                 plt.close("all")
 
                 inform["missing"].append(pd.isnull(y).sum() / y.shape[0])
                 inform["unique"].append(y.nunique())
@@ -90,32 +88,31 @@
                 inform["plot"].append(f"![]({EDA.plot_fname('target')})")
                 inform["feature"].append("target")
                 inform["desc"].append(y.describe().to_dict())
             for col in X.columns:
                 inform["feature_type"].append(PreprocessingUtils.get_type(X[col]))
 
                 if PreprocessingUtils.get_type(X[col]) in ("categorical"):
-
                     plt.figure(figsize=(5, 5))
                     chart = sns.countplot(
-                        X[col], order=X[col].value_counts().iloc[:10].index, color=BLUE
+                        x=X[col],
+                        order=X[col].value_counts().iloc[:10].index,
+                        color=BLUE,
                     )
                     chart.set_xticklabels(chart.get_xticklabels(), rotation=90)
                     plt.title(f"{col} class distribution")
                     plt.tight_layout(pad=2.0)
 
                 elif PreprocessingUtils.get_type(X[col]) in ("continous", "discrete"):
-
                     plt.figure(figsize=(5, 5))
-                    sns.distplot(X[col], color=BLUE)
+                    sns.displot(data=X[col], color=BLUE)
                     plt.title(f"{col} value distribution")
                     plt.tight_layout(pad=2.0)
 
                 elif PreprocessingUtils.get_type(X[col]) in ("text"):
-
                     plt.figure(figsize=(10, 10), dpi=70)
                     word_string = " ".join(X[col].str.lower())
                     wordcloud = WordCloud(
                         width=500,
                         height=500,
                         stopwords=STOPWORDS,
                         background_color="white",
@@ -123,15 +120,14 @@
                         max_font_size=None,
                     ).generate(word_string)
 
                     plt.imshow(wordcloud, aspect="auto", interpolation="nearest")
                     plt.axis("off")
 
                 elif PreprocessingUtils.get_type(X[col]) in ("datetime"):
-
                     plt.figure(figsize=(5, 5))
                     pd.to_datetime(X[col]).plot(grid="True", color=BLUE)
                     plt.tight_layout(pad=2.0)
 
                 plt.savefig(EDA.plot_path(eda_path, col))
                 plt.close("all")
 
@@ -140,20 +136,18 @@
                 inform["plot"].append(f"![]({EDA.plot_fname(col)})")
                 inform["feature"].append(str(col))
                 inform["desc"].append(X[col].describe().to_dict())
 
             df = pd.DataFrame(inform)
 
             with open(os.path.join(eda_path, "README.md"), "w") as fout:
-
                 fout.write("# Exploratory Data Analysis\n")
                 fout.write("\n\n[<< Go back](../README.md)\n")
 
                 for i, row in df.iterrows():
-
                     fout.write(f"## Feature : {row['feature']}\n")
                     fout.write(f"- **Feature type** : {row['feature_type']}\n")
                     fout.write(f"- **Missing** : {row['missing']}%\n")
                     fout.write(f"- **Unique** : {row['unique']}\n")
 
                     for key in row["desc"].keys():
                         if key in ("25%", "50%", "75%"):
@@ -170,15 +164,14 @@
 
             fout.close()
         except Exception as e:
             logger.error(f"There was an issue when running EDA. {str(e)}")
 
     @staticmethod
     def extensive_eda(X, y, save_path):
-
         # Check for empty dataframes in params
         if not isinstance(X, pd.DataFrame):
             raise ValueError("X should be a dataframe")
         if X.shape[0] != len(y):
             raise ValueError("X and y should have the same number of samples")
 
         if X.shape[1] > MAXCOL:
@@ -191,25 +184,21 @@
             if not os.path.exists(save_path):
                 os.mkdir(save_path)
         else:
             raise ValueError("Please provide a valid path to save the Extensive EDA")
 
         plt.style.use("ggplot")
         try:
-
             if PreprocessingUtils.get_type(y) in ("categorical", "discrete"):
-
                 for col in X.columns:
-
                     if PreprocessingUtils.get_type(X[col]) == "continous":
-
                         plt.figure(figsize=(5, 5))
                         for i in np.unique(y):
                             sns.kdeplot(
-                                X.iloc[np.where(y == i)[0]][col],
+                                x=X.iloc[np.where(y == i)[0]][col],
                                 label=f"class {i}",
                                 shade=True,
                             )
                         plt.legend()
                         plt.gca().set_title(
                             f"Distribution of {col} for each class",
                             fontsize=11,
@@ -218,15 +207,14 @@
                         )
                         plt.savefig(EDA.plot_path(save_path, col + "_target"))
 
                     elif PreprocessingUtils.get_type(X[col]) in (
                         "categorical",
                         "discrete",
                     ):
-
                         if X[col].nunique() > 7:
                             warnings.warn("Considering 7 the most frequent values")
 
                         values = X[col].value_counts().index[:7]
                         plt.figure(figsize=(5, 5))
                         sns.countplot(
                             x=X[X[col].isin(values)][col], hue=y[X[col].isin(values)]
@@ -237,17 +225,15 @@
                             weight="bold",
                             alpha=0.75,
                         )
                         plt.savefig(EDA.plot_path(save_path, col + "_target"))
 
             elif PreprocessingUtils.get_type(y) == "continous":
                 for col in X.columns:
-
                     if PreprocessingUtils.get_type(X[col]) == "continous":
-
                         plt.figure(figsize=(5, 5))
                         plt.scatter(X[col].values, y)
                         plt.gca().set_xlabel(f"{col}")
                         plt.gca().set_ylabel("target")
                         plt.gca().set_title(
                             f"Scatter plot of {col} vs target",
                             fontsize=11,
@@ -263,28 +249,29 @@
                     ):
                         if X[col].nunique() > 7:
                             warnings.warn("Considering 7 the most frequent values")
 
                         plt.figure(figsize=(5, 5))
                         for i in X[col].value_counts().index[:7]:
                             sns.kdeplot(
-                                y[X[X[col] == i].index], shade=True, label=f"{col}_{i}"
+                                x=y[X[X[col] == i].index],
+                                shade=True,
+                                label=f"{col}_{i}",
                             )
                         plt.gca().set_title(
                             f"Distribution of target for each {col}",
                             fontsize=11,
                             weight="bold",
                             alpha=0.75,
                         )
                         plt.legend()
 
                         plt.savefig(EDA.plot_path(save_path, col + "_target"))
 
                     elif PreprocessingUtils.get_type(X[col]) == "datetime":
-
                         plt.figure(figsize=(5, 5))
                         plt.plot(X[col], y)
                         plt.gca().set_xticklabels(X[col].dt.date, rotation="45")
                         plt.gca().set_title(
                             f"Distribution of target over time",
                             fontsize=11,
                             weight="bold",
@@ -295,25 +282,22 @@
             cols = [
                 col
                 for col in X.columns
                 if PreprocessingUtils.get_type(X[col]) == "continous"
             ][:COLS]
 
             if len(cols) > 0:
-
                 plt.figure(figsize=(10, 10))
                 sns.heatmap(X[cols].corr())
                 plt.gca().set_title("Heatmap", fontsize=11, weight="bold", alpha=0.75)
 
             plt.savefig(os.path.join(save_path, "heatmap"))
 
             with open(os.path.join(save_path, "Extensive_EDA.md"), "w") as fout:
-
                 for col in X.columns:
-
                     fout.write(f"## Bivariate analysis of {col} feature with target\n")
                     fout.write("\n![]({})\n".format(EDA.plot_fname(col + "_target")))
                     fout.write("\n")
                     fout.write(
                         "------------------------------------------------------\n"
                     )
```

### Comparing `mljar-supervised-0.9.1/supervised/preprocessing/exclude_missing_target.py` & `mljar-supervised-1.0.0/supervised/preprocessing/exclude_missing_target.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 
 logger = logging.getLogger(__name__)
 logger.setLevel(LOG_LEVEL)
 
 
 class ExcludeRowsMissingTarget(object):
     @staticmethod
-    def transform(X=None, y=None, sample_weight=None, warn=False):
+    def transform(
+        X=None, y=None, sample_weight=None, sensitive_features=None, warn=False
+    ):
         if y is None:
-            return X, y, sample_weight
+            return X, y, sample_weight, sensitive_features
         y_missing = pd.isnull(y)
         if np.sum(np.array(y_missing)) == 0:
-            return X, y, sample_weight
+            return X, y, sample_weight, sensitive_features
         logger.debug("Exclude rows with missing target values")
         if warn:
             warnings.warn(
                 "There are samples with missing target values in the data which will be excluded for further analysis"
             )
         y = y.drop(y.index[y_missing])
         y.reset_index(drop=True, inplace=True)
@@ -31,8 +33,14 @@
             X = X.drop(X.index[y_missing])
             X.reset_index(drop=True, inplace=True)
 
         if sample_weight is not None:
             sample_weight = sample_weight.drop(sample_weight.index[y_missing])
             sample_weight.reset_index(drop=True, inplace=True)
 
-        return X, y, sample_weight
+        if sensitive_features is not None:
+            sensitive_features = sensitive_features.drop(
+                sensitive_features.index[y_missing]
+            )
+            sensitive_features.reset_index(drop=True, inplace=True)
+
+        return X, y, sample_weight, sensitive_features
```

### Comparing `mljar-supervised-0.9.1/supervised/preprocessing/label_encoder.py` & `mljar-supervised-1.0.0/supervised/preprocessing/label_encoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,9 +46,9 @@
         for i, cl in enumerate(self.lbl.classes_):
             data_json[str(cl)] = i
         return data_json
 
     def from_json(self, data_json):
         keys = np.array(list(data_json.keys()))
         if len(keys) == 2 and "False" in keys and "True" in keys:
-            keys = [False, True]
+            keys = np.array([False, True])
         self.lbl.classes_ = keys
```

### Comparing `mljar-supervised-0.9.1/supervised/preprocessing/loo_encoder.py` & `mljar-supervised-1.0.0/supervised/preprocessing/loo_encoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         return self.enc.transform(X)
 
     def to_json(self):
         data_json = {
             "cols": self.enc.cols,
             "dim": self.enc._dim,
             "mean": float(self.enc._mean),
-            "feature_names": self.enc.feature_names,
+            "feature_names": self.enc.get_feature_names_out(),
             "mapping": {},
         }
         for k, v in self.enc.mapping.items():
             data_json["mapping"][k] = v.to_json()
         return data_json
 
     def from_json(self, data_json):
```

### Comparing `mljar-supervised-0.9.1/supervised/preprocessing/preprocessing_utils.py` & `mljar-supervised-1.0.0/supervised/preprocessing/preprocessing_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,18 @@
         data_type = PreprocessingUtils.CATEGORICAL
         if col_type.startswith("float"):
             data_type = PreprocessingUtils.CONTINOUS
         elif col_type.startswith("int") or col_type.startswith("uint"):
             data_type = PreprocessingUtils.DISCRETE
         elif col_type.startswith("datetime"):
             data_type = PreprocessingUtils.DATETIME
+        elif col_type.startswith("category"):
+            # do not check the additional condition for text feature
+            # treat it as categorical
+            return PreprocessingUtils.CATEGORICAL
 
         if data_type == PreprocessingUtils.CATEGORICAL:
             # check maybe this categorical is a text
             # it is a text, if:
             # has more than 200 unique values
             # more than half of rows is unique
             unique_cnt = len(np.unique(x[~pd.isnull(x)]))
```

### Comparing `mljar-supervised-0.9.1/supervised/preprocessing/preprocessing.py` & `mljar-supervised-1.0.0/supervised/preprocessing/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
         if y_train is not None:
             # target preprocessing
             # this must be used first, maybe we will drop some rows because of missing target values
             target_preprocessing = self._params.get("target_preprocessing")
             logger.debug("target_preprocessing params: {}".format(target_preprocessing))
 
-            X_train, y_train, sample_weight = ExcludeRowsMissingTarget.transform(
+            X_train, y_train, sample_weight, _ = ExcludeRowsMissingTarget.transform(
                 X_train, y_train, sample_weight
             )
 
             if PreprocessingCategorical.CONVERT_INTEGER in target_preprocessing:
                 logger.debug("Convert target to integer")
                 self._categorical_y = LabelEncoder(try_to_fit_numeric=True)
                 self._categorical_y.fit(y_train)
@@ -181,15 +181,19 @@
             self._missing_values += [missing]
 
         # golden features
         golden_columns = []
         if "golden_features" in self._params:
             results_path = self._params["golden_features"]["results_path"]
             ml_task = self._params["golden_features"]["ml_task"]
-            self._golden_features = GoldenFeaturesTransformer(results_path, ml_task)
+            features_count = self._params["golden_features"].get("features_count")
+            n_jobs = self._params["golden_features"].get("n_jobs", -1)
+            self._golden_features = GoldenFeaturesTransformer(
+                results_path, ml_task, features_count, n_jobs
+            )
             self._golden_features.fit(X_train[numeric_cols], y_train)
             X_train = self._golden_features.transform(X_train)
             golden_columns = self._golden_features._new_columns
 
         kmeans_columns = []
         if "kmeans_features" in self._params:
             results_path = self._params["kmeans_features"]["results_path"]
@@ -222,15 +226,14 @@
                 lambda k: "datetime_transform" in columns_preprocessing[k],
                 columns_preprocessing,
             )
         )
 
         new_datetime_columns = []
         for col in cols_to_process:
-
             t = DateTimeTransformer()
             t.fit(X_train, col)
             X_train = t.transform(X_train)
             self._datetime_transforms += [t]
             new_datetime_columns += t._new_columns
 
         # SCALE
@@ -314,14 +317,15 @@
             target_preprocessing = self._params.get("target_preprocessing")
             logger.debug("target_preprocessing -> {}".format(target_preprocessing))
 
             (
                 X_validation,
                 y_validation,
                 sample_weight_validation,
+                _,
             ) = ExcludeRowsMissingTarget.transform(
                 X_validation, y_validation, sample_weight_validation
             )
 
             if PreprocessingCategorical.CONVERT_INTEGER in target_preprocessing:
                 if y_validation is not None and self._categorical_y is not None:
                     y_validation = pd.Series(
@@ -430,17 +434,15 @@
             y = pd.DataFrame({"target": y})
             y = self._scale_y.inverse_transform(y)
             y = y["target"]
         return y
 
     def inverse_categorical_target(self, y):
         if self._categorical_y is not None:
-            y = self._categorical_y.inverse_transform(
-                pd.DataFrame({"target": np.array(y)})
-            )
+            y = self._categorical_y.inverse_transform(y)
             y = y.astype(str)
         return y
 
     def get_target_class_names(self):
         pos_label, neg_label = "1", "0"
         if self._categorical_y is not None:
             if self._params["ml_task"] == BINARY_CLASSIFICATION:
@@ -589,15 +591,14 @@
             preprocessing_params["drop_features"] = self._drop_features
 
         preprocessing_params["params"] = self._params
 
         return preprocessing_params
 
     def from_json(self, data_json, results_path):
-
         self._params = data_json.get("params", self._params)
 
         if "remove_columns" in data_json:
             self._remove_columns = data_json.get("remove_columns", [])
         if "missing_values" in data_json:
             self._missing_values = []
             for mv_data in data_json["missing_values"]:
```

### Comparing `mljar-supervised-0.9.1/supervised/preprocessing/label_binarizer.py` & `mljar-supervised-1.0.0/supervised/preprocessing/label_binarizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -45,22 +45,34 @@
                 old_col[X[new_col] == 1] = unique_value
 
         X[self._old_column] = old_col
         X.drop(self._new_columns, axis=1, inplace=True)
         return X
 
     def to_json(self):
-        self._uniq_values = [
-            i if type(i) != np.bool_ else bool(i) for i in list(self._uniq_values)
-        ]
+        self._uniq_values = [str(i) for i in list(self._uniq_values)]
         data_json = {
             "new_columns": list(self._new_columns),
             "unique_values": self._uniq_values,
             "old_column": self._old_column,
         }
 
+        if (
+            "True" in self._uniq_values
+            and "False" in self._uniq_values
+            and len(self._uniq_values) == 2
+        ):
+            self._uniq_values = [False, True]
+
         return data_json
 
     def from_json(self, data_json):
         self._new_columns = data_json.get("new_columns", None)
         self._uniq_values = data_json.get("unique_values", None)
         self._old_column = data_json.get("old_column", None)
+
+        if (
+            "True" in self._uniq_values
+            and "False" in self._uniq_values
+            and len(self._uniq_values) == 2
+        ):
+            self._uniq_values = [False, True]
```

### Comparing `mljar-supervised-0.9.1/supervised/preprocessing/encoding_selector.py` & `mljar-supervised-1.0.0/supervised/preprocessing/encoding_selector.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-0.9.1/supervised/algorithms/nn.py` & `mljar-supervised-1.0.0/supervised/algorithms/nn.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import logging
-import copy
 import numpy as np
 import pandas as pd
-import os
-import json
+import warnings
+import logging
 
 from supervised.algorithms.algorithm import BaseAlgorithm
 from supervised.algorithms.sklearn import SklearnAlgorithm
 from supervised.algorithms.registry import AlgorithmsRegistry
 from supervised.algorithms.registry import (
     BINARY_CLASSIFICATION,
     MULTICLASS_CLASSIFICATION,
@@ -42,61 +40,64 @@
         sample_weight=None,
         X_validation=None,
         y_validation=None,
         sample_weight_validation=None,
         log_to_file=None,
         max_time=None,
     ):
-        self.model.fit(X, y)
+        with warnings.catch_warnings():
+            warnings.simplefilter(action="ignore")
+            # filter
+            # X does not have valid feature names, but MLPClassifier was fitted with feature names
+            self.model.fit(X, y)
 
         if log_to_file is not None:
             loss_curve = self.model.loss_curve_
             result = pd.DataFrame(
                 {
                     "iteration": range(len(loss_curve)),
                     "train": loss_curve,
                     "validation": None,
                 }
             )
             result.to_csv(log_to_file, index=False, header=False)
 
 
 class MLPAlgorithm(NNFit):
-
     algorithm_name = "Neural Network"
     algorithm_short_name = "Neural Network"
 
     def __init__(self, params):
         super(MLPAlgorithm, self).__init__(params)
         logger.debug("MLPAlgorithm.__init__")
         self.max_iters = 1
         self.library_version = sklearn.__version__
         h1 = params.get("dense_1_size", 32)
         h2 = params.get("dense_2_size", 16)
         learning_rate = params.get("learning_rate", 0.05)
-        momentum = params.get("momentum", 0.9)
-        early_stopping = True
+
         max_iter = 500
         self.model = MLPClassifier(
             hidden_layer_sizes=(h1, h2),
             activation="relu",
             solver="adam",
-            learning_rate="constant",
+            learning_rate=params.get("learning_rate_type", "constant"),
             learning_rate_init=learning_rate,
-            momentum=momentum,
-            early_stopping=early_stopping,
+            alpha=params.get("alpha", 0.0001),
+            early_stopping=True,
+            n_iter_no_change=50,
             max_iter=max_iter,
+            random_state=params.get("seed", 123),
         )
 
     def get_metric_name(self):
         return "logloss"
 
 
 class MLPRegressorAlgorithm(NNFit):
-
     algorithm_name = "Neural Network"
     algorithm_short_name = "Neural Network"
 
     def __init__(self, params):
         super(MLPRegressorAlgorithm, self).__init__(params)
         logger.debug("MLPRegressorAlgorithm.__init__")
         self.max_iters = 1
```

### Comparing `mljar-supervised-0.9.1/supervised/algorithms/random_forest.py` & `mljar-supervised-1.0.0/supervised/algorithms/random_forest.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from supervised.utils.config import LOG_LEVEL
 
 logger = logging.getLogger(__name__)
 logger.setLevel(LOG_LEVEL)
 
 
 class RandomForestAlgorithm(SklearnTreesEnsembleClassifierAlgorithm):
-
     algorithm_name = "Random Forest"
     algorithm_short_name = "Random Forest"
 
     def __init__(self, params):
         super(RandomForestAlgorithm, self).__init__(params)
         logger.debug("RandomForestAlgorithm.__init__")
 
@@ -36,28 +35,26 @@
         self.early_stopping_rounds = additional.get("early_stopping_rounds", 50)
         self.model = RandomForestClassifier(
             n_estimators=self.trees_in_step,
             criterion=params.get("criterion", "gini"),
             max_features=params.get("max_features", 0.8),
             max_depth=params.get("max_depth", 6),
             min_samples_split=params.get("min_samples_split", 4),
+            min_samples_leaf=params.get("min_samples_leaf", 1),
             warm_start=True,
             n_jobs=params.get("n_jobs", -1),
             random_state=params.get("seed", 1),
         )
+        self.max_steps = self.params.get("max_steps", self.max_steps)
 
     def file_extension(self):
         return "random_forest"
 
-    def get_metric_name(self):
-        return "logloss"
-
 
 class RandomForestRegressorAlgorithm(SklearnTreesEnsembleRegressorAlgorithm):
-
     algorithm_name = "Random Forest"
     algorithm_short_name = "Random Forest"
 
     def __init__(self, params):
         super(RandomForestRegressorAlgorithm, self).__init__(params)
         logger.debug("RandomForestRegressorAlgorithm.__init__")
 
@@ -65,29 +62,28 @@
         self.trees_in_step = regression_additional.get("trees_in_step", 5)
         self.max_steps = regression_additional.get("max_steps", 3)
         self.early_stopping_rounds = regression_additional.get(
             "early_stopping_rounds", 50
         )
         self.model = RandomForestRegressor(
             n_estimators=self.trees_in_step,
-            criterion=params.get("criterion", "mse"),
+            criterion=params.get("criterion", "squared_error"),
             max_features=params.get("max_features", 0.8),
             max_depth=params.get("max_depth", 6),
             min_samples_split=params.get("min_samples_split", 4),
+            min_samples_leaf=params.get("min_samples_leaf", 1),
             warm_start=True,
             n_jobs=params.get("n_jobs", -1),
             random_state=params.get("seed", 1),
         )
+        self.max_steps = self.params.get("max_steps", self.max_steps)
 
     def file_extension(self):
         return "random_forest"
 
-    def get_metric_name(self):
-        return "rmse"
-
 
 # For binary classification target should be 0, 1. There should be no NaNs in target.
 rf_params = {
     "criterion": ["gini", "entropy"],
     "max_features": [0.5, 0.6, 0.7, 0.8, 0.9, 1.0],
     "min_samples_split": [10, 20, 30, 40, 50],
     "max_depth": [3, 4, 5, 6, 7],
@@ -139,23 +135,23 @@
 
 #
 # REGRESSION
 #
 
 regression_rf_params = {
     "criterion": [
-        "mse"
+        "squared_error"
     ],  # remove "mae" because it slows down a lot https://github.com/scikit-learn/scikit-learn/issues/9626
     "max_features": [0.5, 0.6, 0.7, 0.8, 0.9, 1.0],
     "min_samples_split": [10, 20, 30, 40, 50],
     "max_depth": [3, 4, 5, 6, 7],
 }
 
 regression_default_params = {
-    "criterion": "mse",
+    "criterion": "squared_error",
     "max_features": 0.9,
     "min_samples_split": 30,
     "max_depth": 4,
 }
 
 regression_additional = {
     "trees_in_step": 100,
```

### Comparing `mljar-supervised-0.9.1/supervised/algorithms/knn.py` & `mljar-supervised-1.0.0/supervised/algorithms/knn.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 )
 from supervised.utils.config import LOG_LEVEL
 
 logger = logging.getLogger(__name__)
 logger.setLevel(LOG_LEVEL)
 
 
-from dtreeviz.trees import dtreeviz
+KNN_ROWS_LIMIT = 1000
 
 
 class KNNFit(SklearnAlgorithm):
     def file_extension(self):
         return "k_neighbors"
 
     def is_fitted(self):
@@ -41,25 +41,25 @@
         sample_weight=None,
         X_validation=None,
         y_validation=None,
         sample_weight_validation=None,
         log_to_file=None,
         max_time=None,
     ):
-        if X.shape[0] > 1000:
+        rows_limit = self.params.get("rows_limit", KNN_ROWS_LIMIT)
+        if X.shape[0] > rows_limit:
             X1, _, y1, _ = train_test_split(
-                X, y, train_size=1000, stratify=y, random_state=1234
+                X, y, train_size=rows_limit, stratify=y, random_state=1234
             )
             self.model.fit(X1, y1)
         else:
             self.model.fit(X, y)
 
 
 class KNeighborsAlgorithm(KNNFit):
-
     algorithm_name = "k-Nearest Neighbors"
     algorithm_short_name = "Nearest Neighbors"
 
     def __init__(self, params):
         super(KNeighborsAlgorithm, self).__init__(params)
         logger.debug("KNeighborsAlgorithm.__init__")
         self.library_version = sklearn.__version__
@@ -69,15 +69,14 @@
             weights=params.get("weights", "uniform"),
             algorithm="kd_tree",
             n_jobs=params.get("n_jobs", -1),
         )
 
 
 class KNeighborsRegressorAlgorithm(KNNFit):
-
     algorithm_name = "k-Nearest Neighbors"
     algorithm_short_name = "Nearest Neighbors"
 
     def __init__(self, params):
         super(KNeighborsRegressorAlgorithm, self).__init__(params)
         logger.debug("KNeighborsRegressorAlgorithm.__init__")
         self.library_version = sklearn.__version__
```

### Comparing `mljar-supervised-0.9.1/supervised/algorithms/catboost.py` & `mljar-supervised-1.0.0/supervised/algorithms/catboost.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,25 +9,80 @@
 from supervised.algorithms.registry import AlgorithmsRegistry
 from supervised.algorithms.registry import (
     BINARY_CLASSIFICATION,
     MULTICLASS_CLASSIFICATION,
     REGRESSION,
 )
 from supervised.preprocessing.preprocessing_utils import PreprocessingUtils
+from supervised.utils.metric import (
+    CatBoostEvalMetricSpearman,
+    CatBoostEvalMetricPearson,
+    CatBoostEvalMetricAveragePrecision,
+    CatBoostEvalMetricMSE,
+    CatBoostEvalMetricUserDefined,
+)
+
 from supervised.utils.config import LOG_LEVEL
 
 logger = logging.getLogger(__name__)
 logger.setLevel(LOG_LEVEL)
 
 from catboost import CatBoostClassifier, CatBoostRegressor, CatBoost, Pool
 import catboost
 
 
-class CatBoostAlgorithm(BaseAlgorithm):
+def catboost_eval_metric(ml_task, eval_metric):
+    if eval_metric == "user_defined_metric":
+        return eval_metric
+    metric_name_mapping = {
+        BINARY_CLASSIFICATION: {
+            "auc": "AUC",
+            "logloss": "Logloss",
+            "f1": "F1",
+            "average_precision": "average_precision",
+            "accuracy": "Accuracy",
+        },
+        MULTICLASS_CLASSIFICATION: {
+            "logloss": "MultiClass",
+            "f1": "TotalF1:average=Micro",
+            "accuracy": "Accuracy",
+        },
+        REGRESSION: {
+            "rmse": "RMSE",
+            "mse": "mse",
+            "mae": "MAE",
+            "mape": "MAPE",
+            "r2": "R2",
+            "spearman": "spearman",
+            "pearson": "pearson",
+        },
+    }
+    return metric_name_mapping[ml_task][eval_metric]
+
+
+def catboost_objective(ml_task, eval_metric):
+    objective = "RMSE"
+    if ml_task == BINARY_CLASSIFICATION:
+        objective = "Logloss"
+    elif ml_task == MULTICLASS_CLASSIFICATION:
+        objective = "MultiClass"
+    else:  # ml_task == REGRESSION
+        objective = catboost_eval_metric(REGRESSION, eval_metric)
+        if objective in [
+            "mse",
+            "R2",
+            "spearman",
+            "pearson",
+            "user_defined_metric",
+        ]:  # cant optimize them directly
+            objective = "RMSE"
+    return objective
 
+
+class CatBoostAlgorithm(BaseAlgorithm):
     algorithm_name = "CatBoost"
     algorithm_short_name = "CatBoost"
     warmup_iterations = 20
 
     def __init__(self, params):
         super(CatBoostAlgorithm, self).__init__(params)
         self.library_version = catboost.__version__
@@ -44,46 +99,74 @@
             loss_function = self.params.get("loss_function", "Logloss")
         elif self.params["ml_task"] == MULTICLASS_CLASSIFICATION:
             loss_function = self.params.get("loss_function", "MultiClass")
         elif self.params["ml_task"] == REGRESSION:
             loss_function = self.params.get("loss_function", "RMSE")
             Algo = CatBoostRegressor
 
-        self.learner_params = {
+        cat_params = {
+            "iterations": self.params.get("num_boost_round", self.rounds),
             "learning_rate": self.params.get("learning_rate", 0.1),
             "depth": self.params.get("depth", 3),
             "rsm": self.params.get("rsm", 1.0),
-            "random_seed": self.params.get("seed", 1),
+            "l2_leaf_reg": self.params.get("l2_leaf_reg", 3.0),
+            "random_strength": self.params.get("random_strength", 1.0),
             "loss_function": loss_function,
+            "eval_metric": self.params.get("eval_metric", loss_function),
+            # "custom_metric": self.params.get("eval_metric", loss_function),
+            "thread_count": self.params.get("n_jobs", -1),
+            "verbose": False,
+            "allow_writing_files": False,
+            "random_seed": self.params.get("seed", 1),
         }
-        self.model = Algo(
-            iterations=self.rounds,
-            learning_rate=self.learner_params["learning_rate"],
-            depth=self.learner_params["depth"],
-            rsm=self.learner_params["rsm"],
-            loss_function=self.learner_params["loss_function"],
-            thread_count=self.params.get("n_jobs", -1),
-            verbose=False,
-            allow_writing_files=False,
-        )
+
+        for extra_param in [
+            "min_data_in_leaf",
+            "bootstrap_type",
+            "bagging_temperature",
+            "subsample",
+            "border_count",
+        ]:
+            if extra_param in self.params:
+                cat_params[extra_param] = self.params[extra_param]
+
+        self.log_metric_name = cat_params["eval_metric"]
+        if cat_params["eval_metric"] == "spearman":
+            cat_params["eval_metric"] = CatBoostEvalMetricSpearman()
+            self.log_metric_name = "CatBoostEvalMetricSpearman"
+        elif cat_params["eval_metric"] == "pearson":
+            cat_params["eval_metric"] = CatBoostEvalMetricPearson()
+            self.log_metric_name = "CatBoostEvalMetricPearson"
+        elif cat_params["eval_metric"] == "average_precision":
+            cat_params["eval_metric"] = CatBoostEvalMetricAveragePrecision()
+            self.log_metric_name = "CatBoostEvalMetricAveragePrecision"
+        elif cat_params["eval_metric"] == "mse":
+            cat_params["eval_metric"] = CatBoostEvalMetricMSE()
+            self.log_metric_name = "CatBoostEvalMetricMSE"
+        elif cat_params["eval_metric"] == "user_defined_metric":
+            cat_params["eval_metric"] = CatBoostEvalMetricUserDefined()
+            self.log_metric_name = "CatBoostEvalMetricUserDefined"
+
+        self.model = Algo(**cat_params)
         self.cat_features = None
         self.best_ntree_limit = 0
 
         logger.debug("CatBoostAlgorithm.__init__")
 
-    def _assess_iterations(self, X, y, eval_set, max_time=None):
+    def _assess_iterations(self, X, y, sample_weight, eval_set, max_time=None):
         if max_time is None:
             max_time = 3600
         try:
             model = copy.deepcopy(self.model)
             model.set_params(iterations=self.warmup_iterations)
             start_time = time.time()
             model.fit(
                 X,
                 y,
+                sample_weight=sample_weight,
                 cat_features=self.cat_features,
                 init_model=None if self.model.tree_count_ is None else self.model,
                 eval_set=eval_set,
                 early_stopping_rounds=self.early_stopping_rounds,
                 verbose_eval=False,
             )
             elapsed_time = (time.time() - start_time) / float(self.warmup_iterations)
@@ -111,64 +194,87 @@
             return
 
         if self.cat_features is None:
             self.cat_features = []
             for i in range(X.shape[1]):
                 if PreprocessingUtils.is_categorical(X.iloc[:, i]):
                     self.cat_features += [i]
+                    X.iloc[:, i] = X.iloc[:, i].astype(str)
+                    if X_validation is not None:
+                        X_validation.iloc[:, i] = X_validation.iloc[:, i].astype(str)
 
         eval_set = None
         if X_validation is not None and y_validation is not None:
             eval_set = Pool(
                 data=X_validation,
                 label=y_validation,
                 cat_features=self.cat_features,
                 weight=sample_weight_validation,
             )
 
-        # disable for now ...
-        model_init, new_iterations = self._assess_iterations(X, y, eval_set, max_time)
-        self.model.set_params(iterations=new_iterations)
+        if self.params.get("num_boost_round") is None:
+            model_init, new_iterations = self._assess_iterations(
+                X, y, sample_weight, eval_set, max_time
+            )
+            self.model.set_params(iterations=new_iterations)
+        else:
+            model_init = None
+            self.model.set_params(iterations=self.params.get("num_boost_round"))
+            self.early_stopping_rounds = self.params.get("early_stopping_rounds", 50)
+
         self.model.fit(
             X,
             y,
             sample_weight=sample_weight,
             cat_features=self.cat_features,
             init_model=model_init,
             eval_set=eval_set,
             early_stopping_rounds=self.early_stopping_rounds,
             verbose_eval=False,
         )
+
         if self.model.best_iteration_ is not None:
-            self.best_ntree_limit = (
-                self.model.best_iteration_ + model_init.tree_count_ + 1
-            )
+            if model_init is not None:
+                self.best_ntree_limit = (
+                    self.model.best_iteration_ + model_init.tree_count_ + 1
+                )
+            else:
+                self.best_ntree_limit = self.model.best_iteration_ + 1
+
         else:
             # just take all the trees
             # the warm-up trees are already included
             # dont need to add +1
             self.best_ntree_limit = self.model.tree_count_
 
         if log_to_file is not None:
-
-            metric_name = list(self.model.evals_result_["learn"].keys())[0]
-            train_scores = self.model.evals_result_["learn"][metric_name]
-            validation_scores = self.model.evals_result_["validation"][metric_name]
+            train_scores = self.model.evals_result_["learn"].get(self.log_metric_name)
+            validation_scores = self.model.evals_result_["validation"].get(
+                self.log_metric_name
+            )
             if model_init is not None:
-                train_scores = (
-                    model_init.evals_result_["learn"][metric_name] + train_scores
-                )
-                validation_scores = (
-                    model_init.evals_result_["validation"][metric_name]
-                    + validation_scores
-                )
+                if train_scores is not None:
+                    train_scores = (
+                        model_init.evals_result_["learn"].get(self.log_metric_name)
+                        + train_scores
+                    )
+                if validation_scores is not None:
+                    validation_scores = (
+                        model_init.evals_result_["validation"].get(self.log_metric_name)
+                        + validation_scores
+                    )
+            iteration = None
+            if train_scores is not None:
+                iteration = range(len(validation_scores))
+            elif validation_scores is not None:
+                iteration = range(len(validation_scores))
 
             result = pd.DataFrame(
                 {
-                    "iteration": range(len(train_scores)),
+                    "iteration": iteration,
                     "train": train_scores,
                     "validation": validation_scores,
                 }
             )
             result.to_csv(log_to_file, index=False, header=False)
 
     def is_fitted(self):
@@ -195,35 +301,45 @@
         logger.debug("CatBoostLearner load model from %s" % model_file_path)
 
         # waiting for fix https://github.com/catboost/catboost/issues/696
         Algo = CatBoostClassifier
         if self.params["ml_task"] == REGRESSION:
             Algo = CatBoostRegressor
 
+        # loading might throw warnings in the case of custom eval_metric
+        # check https://github.com/catboost/catboost/issues/1169
         self.model = Algo().load_model(model_file_path)
         self.model_file_path = model_file_path
 
     def file_extension(self):
         return "catboost"
 
     def get_metric_name(self):
-        metric = self.params.get("loss_function")
+        metric = self.params.get("eval_metric")
         if metric is None:
             return None
         if metric == "Logloss":
             return "logloss"
+        elif metric == "AUC":
+            return "auc"
         elif metric == "MultiClass":
             return "logloss"
         elif metric == "RMSE":
             return "rmse"
+        elif metric == "MSE":
+            return "mse"
         elif metric == "MAE":
             return "mae"
         elif metric == "MAPE":
             return "mape"
-        return None
+        elif metric in ["F1", "TotalF1:average=Micro"]:
+            return "f1"
+        elif metric == "Accuracy":
+            return "accuracy"
+        return metric
 
 
 classification_params = {
     "learning_rate": [0.025, 0.05, 0.1, 0.2],
     "depth": [4, 5, 6, 7, 8, 9],
     "rsm": [0.7, 0.8, 0.9, 1],  # random subspace method
     "loss_function": ["Logloss"],
```

### Comparing `mljar-supervised-0.9.1/supervised/algorithms/lightgbm.py` & `mljar-supervised-1.0.0/supervised/algorithms/lightgbm.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,22 +10,84 @@
 from supervised.algorithms.algorithm import BaseAlgorithm
 from supervised.algorithms.registry import AlgorithmsRegistry
 from supervised.algorithms.registry import (
     BINARY_CLASSIFICATION,
     MULTICLASS_CLASSIFICATION,
     REGRESSION,
 )
+from supervised.utils.metric import (
+    lightgbm_eval_metric_r2,
+    lightgbm_eval_metric_spearman,
+    lightgbm_eval_metric_pearson,
+    lightgbm_eval_metric_f1,
+    lightgbm_eval_metric_average_precision,
+    lightgbm_eval_metric_accuracy,
+    lightgbm_eval_metric_user_defined,
+)
 from supervised.utils.config import LOG_LEVEL
 
 logger = logging.getLogger(__name__)
 logger.setLevel(LOG_LEVEL)
 
 
-class LightgbmAlgorithm(BaseAlgorithm):
+def lightgbm_objective(ml_task, automl_eval_metric):
+    objective = "regression"
+    if ml_task == BINARY_CLASSIFICATION:
+        objective = "binary"
+    elif ml_task == MULTICLASS_CLASSIFICATION:
+        objective = "multiclass"
+    else:  # ml_task == REGRESSION
+        objective = "regression"
+    return objective
+
+
+def lightgbm_eval_metric(ml_task, automl_eval_metric):
+    if automl_eval_metric == "user_defined_metric":
+        return "custom", automl_eval_metric
+    metric_name_mapping = {
+        BINARY_CLASSIFICATION: {
+            "auc": "auc",
+            "logloss": "binary_logloss",
+            "f1": "custom",
+            "average_precision": "custom",
+            "accuracy": "custom",
+        },
+        MULTICLASS_CLASSIFICATION: {
+            "logloss": "multi_logloss",
+            "f1": "custom",
+            "accuracy": "custom",
+        },
+        REGRESSION: {
+            "rmse": "rmse",
+            "mse": "l2",
+            "mae": "l1",
+            "mape": "mape",
+            "r2": "custom",
+            "spearman": "custom",
+            "pearson": "custom",
+        },
+    }
+
+    metric = metric_name_mapping[ml_task][automl_eval_metric]
+    custom_eval_metric = None
+
+    if automl_eval_metric in [
+        "r2",
+        "spearman",
+        "pearson",
+        "f1",
+        "average_precision",
+        "accuracy",
+    ]:
+        custom_eval_metric = automl_eval_metric
+
+    return metric, custom_eval_metric
 
+
+class LightgbmAlgorithm(BaseAlgorithm):
     algorithm_name = "LightGBM"
     algorithm_short_name = "LightGBM"
 
     def __init__(self, params):
         super(LightgbmAlgorithm, self).__init__(params)
         self.library_version = lgb.__version__
 
@@ -47,26 +109,64 @@
             "learning_rate": self.params.get("learning_rate", 0.1),
             "feature_fraction": self.params.get("feature_fraction", 1.0),
             "bagging_fraction": self.params.get("bagging_fraction", 1.0),
             "min_data_in_leaf": self.params.get("min_data_in_leaf", 20),
             "num_threads": n_jobs,
             "verbose": -1,
             "seed": self.params.get("seed", 1),
+            "extra_trees": self.params.get("extra_trees", False),
         }
+
+        for extra_param in [
+            "lambda_l1",
+            "lambda_l2",
+            "bagging_freq",
+            "feature_pre_filter",
+            "cat_feature",
+            "cat_l2",
+            "cat_smooth",
+            "max_bin",
+        ]:
+            if extra_param in self.params:
+                self.learner_params[extra_param] = self.params[extra_param]
+
+        if "num_boost_round" in self.params:
+            self.rounds = self.params["num_boost_round"]
+        if "early_stopping_rounds" in self.params:
+            self.early_stopping_rounds = self.params["early_stopping_rounds"]
+
         if "num_class" in self.params:  # multiclass classification
             self.learner_params["num_class"] = self.params.get("num_class")
 
+        self.custom_eval_metric = None
+        if self.params.get("custom_eval_metric_name") is not None:
+            if self.params["custom_eval_metric_name"] == "r2":
+                self.custom_eval_metric = lightgbm_eval_metric_r2
+            elif self.params["custom_eval_metric_name"] == "spearman":
+                self.custom_eval_metric = lightgbm_eval_metric_spearman
+            elif self.params["custom_eval_metric_name"] == "pearson":
+                self.custom_eval_metric = lightgbm_eval_metric_pearson
+            elif self.params["custom_eval_metric_name"] == "f1":
+                self.custom_eval_metric = lightgbm_eval_metric_f1
+            elif self.params["custom_eval_metric_name"] == "average_precision":
+                self.custom_eval_metric = lightgbm_eval_metric_average_precision
+            elif self.params["custom_eval_metric_name"] == "accuracy":
+                self.custom_eval_metric = lightgbm_eval_metric_accuracy
+            elif self.params["custom_eval_metric_name"] == "user_defined_metric":
+                self.custom_eval_metric = lightgbm_eval_metric_user_defined
+
         logger.debug("LightgbmLearner __init__")
 
     def file_extension(self):
         return "lightgbm"
 
     def update(self, update_params):
         pass
 
+    """
     def get_boosting_rounds(self, lgb_train, valid_sets, esr, max_time):
         if max_time is None:
             max_time = 3600.0
         start_time = time.time()
         evals_result = {}
         model = lgb.train(
             self.learner_params,
@@ -81,45 +181,48 @@
 
         # 2.0 is just a scaling factor
         # purely heuristic
         iters = int(max_time / time_1_iter * 2.0)
         iters = max(iters, 100)
         iters = min(iters, 10000)
         return iters
+    """
 
     def fit(
         self,
         X,
         y,
         sample_weight=None,
         X_validation=None,
         y_validation=None,
         sample_weight_validation=None,
         log_to_file=None,
         max_time=None,
     ):
         lgb_train = lgb.Dataset(
-            X.to_numpy() if isinstance(X, pd.DataFrame) else X, y, weight=sample_weight
+            X.values if isinstance(X, pd.DataFrame) else X,
+            y,
+            weight=sample_weight,
         )
+        valid_sets = None
         if self.early_stopping_rounds == 0:
             self.model = lgb.train(
                 self.learner_params,
                 lgb_train,
                 num_boost_round=self.rounds,
                 init_model=self.model,
             )
         else:
-            valid_sets = None
             valid_names = None
             esr = None
             if X_validation is not None and y_validation is not None:
                 valid_sets = [
                     lgb_train,
                     lgb.Dataset(
-                        X_validation.to_numpy()
+                        X_validation.values
                         if isinstance(X_validation, pd.DataFrame)
                         else X_validation,
                         y_validation,
                         weight=sample_weight_validation,
                     ),
                 ]
                 valid_names = ["train", "validation"]
@@ -131,19 +234,26 @@
 
             self.model = lgb.train(
                 self.learner_params,
                 lgb_train,
                 num_boost_round=self.rounds,
                 valid_sets=valid_sets,
                 valid_names=valid_names,
-                early_stopping_rounds=esr,
-                evals_result=evals_result,
-                verbose_eval=False,
+                feval=self.custom_eval_metric,
+                callbacks=[
+                    lgb.early_stopping(esr, verbose=False),
+                    lgb.record_evaluation(evals_result),
+                ],
             )
 
+            del lgb_train
+            if valid_sets is not None:
+                del valid_sets[0]
+                del valid_sets
+
             if log_to_file is not None:
                 metric_name = list(evals_result["train"].keys())[0]
                 result = pd.DataFrame(
                     {
                         "iteration": range(len(evals_result["train"][metric_name])),
                         "train": evals_result["train"][metric_name],
                         "validation": evals_result["validation"][metric_name],
@@ -152,15 +262,15 @@
                 result.to_csv(log_to_file, index=False, header=False)
 
     def is_fitted(self):
         return self.model is not None
 
     def predict(self, X):
         self.reload()
-        return self.model.predict(X.to_numpy() if isinstance(X, pd.DataFrame) else X)
+        return self.model.predict(X.values if isinstance(X, pd.DataFrame) else X)
 
     def copy(self):
         with open(os.devnull, "w") as f, contextlib.redirect_stdout(f):
             return copy.deepcopy(self)
 
     def save(self, model_file_path):
         self.model.save_model(model_file_path)
@@ -170,40 +280,38 @@
     def load(self, model_file_path):
         logger.debug("LightgbmAlgorithm load model from %s" % model_file_path)
         self.model_file_path = model_file_path
         self.model = lgb.Booster(model_file=model_file_path)
 
     def get_metric_name(self):
         metric = self.params.get("metric")
+        custom_metric = self.params.get("custom_eval_metric_name")
+
         if metric is None:
             return None
+        if metric == "custom":
+            return custom_metric
         if metric == "binary_logloss":
             return "logloss"
-        elif metric == "auc":
-            return "auc"
         elif metric == "multi_logloss":
             return "logloss"
-        elif metric == "rmse":
-            return "rmse"
-        return None
+        return metric
 
 
 lgbm_bin_params = {
     "objective": ["binary"],
-    "metric": ["binary_logloss", "auc"],
     "num_leaves": [15, 31, 63, 95, 127],
     "learning_rate": [0.05, 0.1, 0.2],
     "feature_fraction": [0.5, 0.8, 0.9, 1.0],
     "bagging_fraction": [0.5, 0.8, 0.9, 1.0],
     "min_data_in_leaf": [5, 10, 15, 20, 30, 50],
 }
 
 classification_bin_default_params = {
     "objective": "binary",
-    "metric": "binary_logloss",
     "num_leaves": 63,
     "learning_rate": 0.05,
     "feature_fraction": 0.9,
     "bagging_fraction": 0.9,
     "min_data_in_leaf": 10,
 }
 
@@ -221,29 +329,26 @@
     "datetime_transform",
     "text_transform",
     "target_as_integer",
 ]
 
 lgbm_multi_params = copy.deepcopy(lgbm_bin_params)
 lgbm_multi_params["objective"] = ["multiclass"]
-lgbm_multi_params["metric"] = ["multi_logloss"]
 
 classification_multi_default_params = {
     "objective": "multiclass",
-    "metric": "multi_logloss",
     "num_leaves": 63,
     "learning_rate": 0.05,
     "feature_fraction": 0.9,
     "bagging_fraction": 0.9,
     "min_data_in_leaf": 10,
 }
 
 lgbr_params = copy.deepcopy(lgbm_bin_params)
 lgbr_params["objective"] = ["regression"]
-lgbr_params["metric"] = ["rmse", "mae", "mape"]
 
 AlgorithmsRegistry.add(
     BINARY_CLASSIFICATION,
     LightgbmAlgorithm,
     lgbm_bin_params,
     required_preprocessing,
     additional,
@@ -266,15 +371,14 @@
     "text_transform",
     "target_scale",
 ]
 
 
 regression_default_params = {
     "objective": "regression",
-    "metric": "rmse",
     "num_leaves": 63,
     "learning_rate": 0.05,
     "feature_fraction": 0.9,
     "bagging_fraction": 0.9,
     "min_data_in_leaf": 10,
 }
```

### Comparing `mljar-supervised-0.9.1/supervised/algorithms/registry.py` & `mljar-supervised-1.0.0/supervised/algorithms/registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # tasks that can be handled by the package
 BINARY_CLASSIFICATION = "binary_classification"
 MULTICLASS_CLASSIFICATION = "multiclass_classification"
 REGRESSION = "regression"
 
 
 class AlgorithmsRegistry:
-
     registry = {
         BINARY_CLASSIFICATION: {},
         MULTICLASS_CLASSIFICATION: {},
         REGRESSION: {},
     }
 
     @staticmethod
@@ -54,14 +53,21 @@
 
     @staticmethod
     def get_max_cols_limit(ml_task, algorithm_name):
         return AlgorithmsRegistry.registry[ml_task][algorithm_name]["additional"][
             "max_cols_limit"
         ]
 
+    @staticmethod
+    def get_eval_metric(algorithm_name, ml_task, automl_eval_metric):
+        if algorithm_name == "Xgboost":
+            return xgboost_eval_metric(ml_task, automl_eval_metric)
+
+        return automl_eval_metric
+
 
 # Import algorithm to be registered
 import supervised.algorithms.random_forest
 import supervised.algorithms.xgboost
 import supervised.algorithms.decision_tree
 import supervised.algorithms.baseline
 import supervised.algorithms.lightgbm
```

### Comparing `mljar-supervised-0.9.1/supervised/algorithms/factory.py` & `mljar-supervised-1.0.0/supervised/algorithms/factory.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-0.9.1/supervised/algorithms/xgboost.py` & `mljar-supervised-1.0.0/supervised/algorithms/xgboost.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 import logging
 import copy
 import numpy as np
 import pandas as pd
 import os
 import time
+from inspect import signature
 import xgboost as xgb
 
 from supervised.algorithms.algorithm import BaseAlgorithm
 from supervised.algorithms.registry import AlgorithmsRegistry
 from supervised.algorithms.registry import (
     BINARY_CLASSIFICATION,
     MULTICLASS_CLASSIFICATION,
     REGRESSION,
 )
+from supervised.utils.metric import (
+    xgboost_eval_metric_r2,
+    xgboost_eval_metric_spearman,
+    xgboost_eval_metric_pearson,
+    xgboost_eval_metric_f1,
+    xgboost_eval_metric_average_precision,
+    xgboost_eval_metric_accuracy,
+    xgboost_eval_metric_mse,
+    xgboost_eval_metric_user_defined,
+)
 from supervised.utils.config import LOG_LEVEL
 
 logger = logging.getLogger(__name__)
 logger.setLevel(LOG_LEVEL)
 
 import tempfile
 
@@ -28,14 +39,34 @@
 
 
 def time_constraint(env):
     # print("time constraint")
     pass
 
 
+def xgboost_eval_metric(ml_task, automl_eval_metric):
+    # the mapping is almost the same
+    eval_metric_name = automl_eval_metric
+    if ml_task == MULTICLASS_CLASSIFICATION:
+        if automl_eval_metric == "logloss":
+            eval_metric_name = "mlogloss"
+    return eval_metric_name
+
+
+def xgboost_objective(ml_task, automl_eval_metric):
+    objective = "reg:squarederror"
+    if ml_task == BINARY_CLASSIFICATION:
+        objective = "binary:logistic"
+    elif ml_task == MULTICLASS_CLASSIFICATION:
+        objective = "multi:softprob"
+    else:  # ml_task == REGRESSION
+        objective = "reg:squarederror"
+    return objective
+
+
 class XgbAlgorithm(BaseAlgorithm):
     """
     This is a wrapper over xgboost algorithm.
     """
 
     algorithm_name = "Extreme Gradient Boosting"
     algorithm_short_name = "Xgboost"
@@ -57,25 +88,53 @@
             "max_depth": self.params.get("max_depth", 1),
             "min_child_weight": self.params.get("min_child_weight", 1),
             "subsample": self.params.get("subsample", 0.8),
             "colsample_bytree": self.params.get("colsample_bytree", 0.8),
             "n_jobs": self.params.get("n_jobs", -1),
             # "silent": self.params.get("silent", 1),
             "seed": self.params.get("seed", 1),
+            "verbosity": 0,
         }
 
+        if "lambda" in self.params:
+            self.learner_params["lambda"] = self.params["lambda"]
+        if "alpha" in self.params:
+            self.learner_params["alpha"] = self.params["alpha"]
+
         # check https://github.com/dmlc/xgboost/issues/5637
         if self.learner_params["seed"] > 2147483647:
             self.learner_params["seed"] = self.learner_params["seed"] % 2147483647
         if "num_class" in self.params:  # multiclass classification
             self.learner_params["num_class"] = self.params.get("num_class")
 
+        if "max_rounds" in self.params:
+            self.boosting_rounds = self.params["max_rounds"]
+
+        self.custom_eval_metric = None
+        if self.params.get("eval_metric", "") == "r2":
+            self.custom_eval_metric = xgboost_eval_metric_r2
+        elif self.params.get("eval_metric", "") == "spearman":
+            self.custom_eval_metric = xgboost_eval_metric_spearman
+        elif self.params.get("eval_metric", "") == "pearson":
+            self.custom_eval_metric = xgboost_eval_metric_pearson
+        elif self.params.get("eval_metric", "") == "f1":
+            self.custom_eval_metric = xgboost_eval_metric_f1
+        elif self.params.get("eval_metric", "") == "average_precision":
+            self.custom_eval_metric = xgboost_eval_metric_average_precision
+        elif self.params.get("eval_metric", "") == "accuracy":
+            self.custom_eval_metric = xgboost_eval_metric_accuracy
+        elif self.params.get("eval_metric", "") == "mse":
+            self.custom_eval_metric = xgboost_eval_metric_mse
+        elif self.params.get("eval_metric", "") == "user_defined_metric":
+            self.custom_eval_metric = xgboost_eval_metric_user_defined
+
         self.best_ntree_limit = 0
         logger.debug("XgbLearner __init__")
 
+    """
     def get_boosting_rounds(self, dtrain, evals, esr, max_time):
         if max_time is None:
             return self.boosting_rounds
 
         start_time = time.time()
         evals_result = {}
         model = xgb.train(
@@ -91,34 +150,35 @@
 
         # 2.0 is just a scaling factor
         # purely heuristic
         iters = int(max_time / time_1_iter * 2.0)
         iters = max(iters, 100)
         iters = min(iters, 10000)
         return iters
+    """
 
     def fit(
         self,
         X,
         y,
         sample_weight=None,
         X_validation=None,
         y_validation=None,
         sample_weight_validation=None,
         log_to_file=None,
         max_time=None,
     ):
         dtrain = xgb.DMatrix(
-            X.to_numpy() if isinstance(X, pd.DataFrame) else X,
+            X.values if isinstance(X, pd.DataFrame) else X,
             label=y,
             missing=np.NaN,
             weight=sample_weight,
         )
         dvalidation = xgb.DMatrix(
-            X_validation.to_numpy()
+            X_validation.values
             if isinstance(X_validation, pd.DataFrame)
             else X_validation,
             label=y_validation,
             missing=np.NaN,
             weight=sample_weight_validation,
         )
         evals_result = {}
@@ -130,38 +190,60 @@
             esr = self.early_stopping_rounds
 
         # disable for now, dont have better idea how to handle time limit ...
         # looks like there is better not to limit the algorithm
         # just wait till they converge ...
         # boosting_rounds = self.get_boosting_rounds(dtrain, evals, esr, max_time)
 
+        if self.custom_eval_metric is not None:
+            del self.learner_params["eval_metric"]
+
         self.model = xgb.train(
             self.learner_params,
             dtrain,
             self.boosting_rounds,
             evals=evals,
             early_stopping_rounds=esr,
             evals_result=evals_result,
-            verbose_eval=False
+            verbose_eval=False,
+            feval=self.custom_eval_metric
             # callbacks=[time_constraint] # callback slows down by factor ~8
         )
 
+        del dtrain
+        del dvalidation
+
         # dump_list = self.model.get_dump()
         # num_trees = len(dump_list)
         # print(self.model.best_ntree_limit, num_trees)
 
         if log_to_file is not None:
-            metric_name = list(evals_result["train"].keys())[0]
+            metric_name = list(evals_result["train"].keys())[-1]
+
             result = pd.DataFrame(
                 {
                     "iteration": range(len(evals_result["train"][metric_name])),
                     "train": evals_result["train"][metric_name],
                     "validation": evals_result["validation"][metric_name],
                 }
             )
+            # it a is custom metric
+            # that is always minimized
+            # we need to revert it
+            if metric_name in [
+                "r2",
+                "spearman",
+                "pearson",
+                "f1",
+                "average_precision",
+                "accuracy",
+            ]:
+                result["train"] *= -1.0
+                result["validation"] *= -1.0
+
             result.to_csv(log_to_file, index=False, header=False)
 
         # save best_ntree_limit because of:
         # https://github.com/dmlc/xgboost/issues/805
         self.best_ntree_limit = self.model.best_ntree_limit
         # fix high memory consumption in xgboost,
         # waiting for release with fix
@@ -181,17 +263,23 @@
     def predict(self, X):
         self.reload()
 
         if self.model is None:
             raise XgbAlgorithmException("Xgboost model is None")
 
         dtrain = xgb.DMatrix(
-            X.to_numpy() if isinstance(X, pd.DataFrame) else X, missing=np.NaN
+            X.values if isinstance(X, pd.DataFrame) else X, missing=np.NaN
         )
-        a = self.model.predict(dtrain, ntree_limit=self.best_ntree_limit)
+        if "iteration_range" in str(signature(self.model.predict)):
+            # the newer version
+            a = self.model.predict(dtrain, iteration_range=(0, self.best_ntree_limit))
+        else:
+            # the older interface
+            a = self.model.predict(dtrain, ntree_limit=self.best_ntree_limit)
+
         return a
 
     def copy(self):
         return copy.deepcopy(self)
 
     def save(self, model_file_path):
         self.model.save_model(model_file_path)
@@ -207,75 +295,60 @@
     def file_extension(self):
         return "xgboost"
 
     def get_metric_name(self):
         metric = self.params.get("eval_metric")
         if metric is None:
             return None
-        if metric == "logloss":
+        if metric == "mlogloss":
             return "logloss"
-        elif metric == "auc":
-            return "auc"
-        elif metric == "mlogloss":
-            return "logloss"
-        elif metric == "rmse":
-            return "rmse"
-        elif metric == "mae":
-            return "mae"
-        elif metric == "mape":
-            return "mape"
-
-        return None
+        return metric
 
 
 # For binary classification target should be 0, 1. There should be no NaNs in target.
 xgb_bin_class_params = {
     "objective": ["binary:logistic"],
-    "eval_metric": ["logloss", "auc"],
     "eta": [0.05, 0.075, 0.1, 0.15],
     "max_depth": [4, 5, 6, 7, 8, 9],
     "min_child_weight": [1, 5, 10, 25, 50],
     "subsample": [0.5, 0.6, 0.7, 0.8, 0.9, 1.0],
     "colsample_bytree": [0.5, 0.6, 0.7, 0.8, 0.9, 1.0],
 }
 
 classification_bin_default_params = {
     "objective": "binary:logistic",
-    "eval_metric": "logloss",
     "eta": 0.075,
     "max_depth": 6,
     "min_child_weight": 1,
     "subsample": 1.0,
     "colsample_bytree": 1.0,
 }
 
 xgb_regression_params = dict(xgb_bin_class_params)
 xgb_regression_params["objective"] = ["reg:squarederror"]
-xgb_regression_params["eval_metric"] = ["rmse", "mae", "mape"]
+# xgb_regression_params["eval_metric"] = ["rmse", "mae", "mape"]
 xgb_regression_params["max_depth"] = [4, 5, 6, 7, 8, 9]
 
 
 xgb_multi_class_params = dict(xgb_bin_class_params)
 xgb_multi_class_params["objective"] = ["multi:softprob"]
-xgb_multi_class_params["eval_metric"] = ["mlogloss"]
+# xgb_multi_class_params["eval_metric"] = ["mlogloss"]
 
 classification_multi_default_params = {
     "objective": "multi:softprob",
-    "eval_metric": "mlogloss",
     "eta": 0.075,
     "max_depth": 6,
     "min_child_weight": 1,
     "subsample": 1.0,
     "colsample_bytree": 1.0,
 }
 
 
 regression_default_params = {
     "objective": "reg:squarederror",
-    "eval_metric": "rmse",
     "eta": 0.075,
     "max_depth": 6,
     "min_child_weight": 1,
     "subsample": 1.0,
     "colsample_bytree": 1.0,
 }
```

### Comparing `mljar-supervised-0.9.1/supervised/algorithms/extra_trees.py` & `mljar-supervised-1.0.0/supervised/algorithms/extra_trees.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from supervised.utils.config import LOG_LEVEL
 
 logger = logging.getLogger(__name__)
 logger.setLevel(LOG_LEVEL)
 
 
 class ExtraTreesAlgorithm(SklearnTreesEnsembleClassifierAlgorithm):
-
     algorithm_name = "Extra Trees Classifier"
     algorithm_short_name = "Extra Trees"
 
     def __init__(self, params):
         super(ExtraTreesAlgorithm, self).__init__(params)
         logger.debug("ExtraTreesAlgorithm.__init__")
 
@@ -35,28 +34,26 @@
         self.early_stopping_rounds = additional.get("early_stopping_rounds", 50)
         self.model = ExtraTreesClassifier(
             n_estimators=self.trees_in_step,
             criterion=params.get("criterion", "gini"),
             max_features=params.get("max_features", 0.8),
             max_depth=params.get("max_depth", 6),
             min_samples_split=params.get("min_samples_split", 4),
+            min_samples_leaf=params.get("min_samples_leaf", 1),
             warm_start=True,
             n_jobs=params.get("n_jobs", -1),
             random_state=params.get("seed", 1),
         )
+        self.max_steps = self.params.get("max_steps", self.max_steps)
 
     def file_extension(self):
         return "extra_trees"
 
-    def get_metric_name(self):
-        return "logloss"
-
 
 class ExtraTreesRegressorAlgorithm(SklearnTreesEnsembleRegressorAlgorithm):
-
     algorithm_name = "Extra Trees Regressor"
     algorithm_short_name = "Extra Trees"
 
     def __init__(self, params):
         super(ExtraTreesRegressorAlgorithm, self).__init__(params)
         logger.debug("ExtraTreesRegressorAlgorithm.__init__")
 
@@ -64,29 +61,28 @@
         self.trees_in_step = regression_additional.get("trees_in_step", 100)
         self.max_steps = regression_additional.get("max_steps", 50)
         self.early_stopping_rounds = regression_additional.get(
             "early_stopping_rounds", 50
         )
         self.model = ExtraTreesRegressor(
             n_estimators=self.trees_in_step,
-            criterion=params.get("criterion", "mse"),
+            criterion=params.get("criterion", "squared_error"),
             max_features=params.get("max_features", 0.6),
             max_depth=params.get("max_depth", 6),
             min_samples_split=params.get("min_samples_split", 30),
+            min_samples_leaf=params.get("min_samples_leaf", 1),
             warm_start=True,
             n_jobs=params.get("n_jobs", -1),
             random_state=params.get("seed", 1),
         )
+        self.max_steps = self.params.get("max_steps", self.max_steps)
 
     def file_extension(self):
         return "extra_trees"
 
-    def get_metric_name(self):
-        return "rmse"
-
 
 # For binary classification target should be 0, 1. There should be no NaNs in target.
 et_params = {
     "criterion": ["gini", "entropy"],
     "max_features": [0.5, 0.6, 0.7, 0.8, 0.9, 1.0],
     "min_samples_split": [10, 20, 30, 40, 50],
     "max_depth": [3, 4, 5, 6, 7],
@@ -135,23 +131,23 @@
 
 #
 # REGRESSION
 #
 
 regression_et_params = {
     "criterion": [
-        "mse"
+        "squared_error"
     ],  # remove "mae" because it slows down a lot https://github.com/scikit-learn/scikit-learn/issues/9626
     "max_features": [0.5, 0.6, 0.7, 0.8, 0.9, 1.0],
     "min_samples_split": [10, 20, 30, 40, 50],
     "max_depth": [3, 4, 5, 6, 7],
 }
 
 regression_default_params = {
-    "criterion": "mse",
+    "criterion": "squared_error",
     "max_features": 0.9,
     "min_samples_split": 30,
     "max_depth": 4,
 }
 
 regression_additional = {
     "trees_in_step": 100,
```

### Comparing `mljar-supervised-0.9.1/supervised/algorithms/sklearn.py` & `mljar-supervised-1.0.0/supervised/algorithms/sklearn.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import copy
 import logging
 import numpy as np
 import pandas as pd
 import time
 import joblib
+import warnings
 
 from supervised.algorithms.algorithm import BaseAlgorithm
 from supervised.algorithms.registry import (
     BINARY_CLASSIFICATION,
     MULTICLASS_CLASSIFICATION,
     REGRESSION,
 )
@@ -28,15 +29,17 @@
         sample_weight=None,
         X_validation=None,
         y_validation=None,
         sample_weight_validation=None,
         log_to_file=None,
         max_time=None,
     ):
-        self.model.fit(X, y, sample_weight=sample_weight)
+        with warnings.catch_warnings():
+            warnings.simplefilter(action="ignore")
+            self.model.fit(X, y, sample_weight=sample_weight)
 
     def copy(self):
         return copy.deepcopy(self)
 
     def save(self, model_file_path):
         logger.debug("SklearnAlgorithm save to {0}".format(model_file_path))
         joblib.dump(self.model, model_file_path, compress=True)
@@ -45,43 +48,52 @@
     def load(self, model_file_path):
         logger.debug("SklearnAlgorithm loading model from {0}".format(model_file_path))
         self.model = joblib.load(model_file_path)
         self.model_file_path = model_file_path
 
     def is_fitted(self):
         return (
-            hasattr(self.model, "n_features_")
-            and self.model.n_features_ is not None
-            and self.model.n_features_ > 0
+            hasattr(self.model, "n_features_in_")
+            and self.model.n_features_in_ is not None
+            and self.model.n_features_in_ > 0
         )
 
     def predict(self, X):
         self.reload()
         if self.params["ml_task"] == BINARY_CLASSIFICATION:
             return self.model.predict_proba(X)[:, 1]
         elif self.params["ml_task"] == MULTICLASS_CLASSIFICATION:
             return self.model.predict_proba(X)
         return self.model.predict(X)
 
 
 from supervised.utils.metric import Metric
 
 
-def predict_proba_function(estimator, X):
+def predict_proba_function_binary(estimator, X):
+    return estimator.predict_proba(X)[:, 1]
+
+
+def predict_proba_function_multiclass(estimator, X):
     return estimator.predict_proba(X)
 
 
 class SklearnTreesEnsembleClassifierAlgorithm(SklearnAlgorithm):
     def __init__(self, params):
         super(SklearnTreesEnsembleClassifierAlgorithm, self).__init__(params)
-        self.log_metric = Metric({"name": "logloss"})
+        self.log_metric = Metric(
+            {"name": self.params.get("eval_metric_name", "logloss")}
+        )
         self.max_iters = (
             1  # max iters is used by model_framework, max_steps is used internally
         )
-        self.predict_function = predict_proba_function
+        if params.get("ml_task") == BINARY_CLASSIFICATION:
+            self.predict_function = predict_proba_function_binary
+        else:
+            self.predict_function = predict_proba_function_multiclass
 
     def fit(
         self,
         X,
         y,
         sample_weight=None,
         X_validation=None,
@@ -96,74 +108,85 @@
         min_val = 10e12
         min_e = 0
 
         p_tr, p_vd = None, None
         result = {"iteration": [], "train": [], "validation": []}
 
         start_time = time.time()
+        with warnings.catch_warnings():
+            warnings.simplefilter(action="ignore")
 
-        for i in range(max_steps):
-
-            self.model.fit(X, np.ravel(y), sample_weight=sample_weight)
-            self.model.n_estimators += self.trees_in_step
+            for i in range(max_steps):
+                self.model.fit(X, np.ravel(y), sample_weight=sample_weight)
+                self.model.n_estimators += self.trees_in_step
+
+                if X_validation is None or y_validation is None:
+                    continue
+                estimators = self.model.estimators_
+
+                stop = False
+                for e in range(n_estimators, len(estimators)):
+                    p = self.predict_function(estimators[e], X)
+                    if p_tr is None:
+                        p_tr = p
+                    else:
+                        p_tr += p
+
+                    p = self.predict_function(estimators[e], X_validation)
+                    if p_vd is None:
+                        p_vd = p
+                    else:
+                        p_vd += p
+
+                    tr = self.log_metric(
+                        y, p_tr / float(e + 1), sample_weight=sample_weight
+                    )
+                    vd = self.log_metric(
+                        y_validation,
+                        p_vd / float(e + 1),
+                        sample_weight=sample_weight_validation,
+                    )
+
+                    if vd < min_val:  # optimize direction
+                        min_val = vd
+                        min_e = e
+
+                    if e - min_e >= self.early_stopping_rounds:
+                        stop = True
+                        break
+
+                    result["iteration"] += [e]
+                    result["train"] += [tr]
+                    result["validation"] += [vd]
+
+                # disable for now ...
+                # if max_time is not None and time.time()-start_time > max_time:
+                #    stop = True
 
-            if X_validation is None or y_validation is None:
-                continue
-            estimators = self.model.estimators_
-
-            stop = False
-            for e in range(n_estimators, len(estimators)):
-                p = self.predict_function(estimators[e], X)
-                if p_tr is None:
-                    p_tr = p
-                else:
-                    p_tr += p
-
-                p = self.predict_function(estimators[e], X_validation)
-                if p_vd is None:
-                    p_vd = p
-                else:
-                    p_vd += p
-
-                tr = self.log_metric(
-                    y, p_tr / float(e + 1), sample_weight=sample_weight
-                )
-                vd = self.log_metric(
-                    y_validation,
-                    p_vd / float(e + 1),
-                    sample_weight=sample_weight_validation,
-                )
-
-                result["iteration"] += [e]
-                result["train"] += [tr]
-                result["validation"] += [vd]
-
-                if vd < min_val:  # optimize direction
-                    min_val = vd
-                    min_e = e
-
-                if e - min_e >= self.early_stopping_rounds:
-                    stop = True
+                if stop:
+                    self.model.estimators_ = estimators[: (min_e + 1)]
                     break
-
-            # disable for now ...
-            # if max_time is not None and time.time()-start_time > max_time:
-            #    stop = True
-
-            if stop:
-                self.model.estimators_ = estimators[: (min_e + 1)]
-                break
-            n_estimators = len(estimators)
+                n_estimators = len(estimators)
 
         if log_to_file is not None:
-            pd.DataFrame(result).to_csv(log_to_file, index=False, header=False)
+            df_result = pd.DataFrame(result)
+            if self.log_metric.is_negative():
+                df_result["train"] *= -1.0
+                df_result["validation"] *= -1.0
+            df_result.to_csv(log_to_file, index=False, header=False)
+
+    def get_metric_name(self):
+        return self.params.get("eval_metric_name", "logloss")
 
 
 def predict_function(estimator, X):
     return estimator.predict(X)
 
 
 class SklearnTreesEnsembleRegressorAlgorithm(SklearnTreesEnsembleClassifierAlgorithm):
     def __init__(self, params):
         super(SklearnTreesEnsembleRegressorAlgorithm, self).__init__(params)
-        self.log_metric = Metric({"name": "rmse"})
+        self.log_metric = Metric({"name": self.params.get("eval_metric_name", "rmse")})
         self.predict_function = predict_function
+
+    def get_metric_name(self):
+        return self.params.get("eval_metric_name", "rmse")
```

### Comparing `mljar-supervised-0.9.1/supervised/algorithms/decision_tree.py` & `mljar-supervised-1.0.0/supervised/algorithms/decision_tree.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import os
 import sklearn
+import warnings
 import numpy as np
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.tree import DecisionTreeRegressor
 
 from supervised.algorithms.algorithm import BaseAlgorithm
 from supervised.algorithms.sklearn import SklearnAlgorithm
 from supervised.algorithms.registry import AlgorithmsRegistry
@@ -15,80 +16,81 @@
 )
 from supervised.utils.config import LOG_LEVEL
 
 logger = logging.getLogger(__name__)
 logger.setLevel(LOG_LEVEL)
 
 from sklearn.tree import _tree
-from dtreeviz.trees import dtreeviz
+from dtreeviz import *
+from supervised.utils.subsample import subsample
+
 
 def get_rules(tree, feature_names, class_names):
     tree_ = tree.tree_
     feature_name = [
         feature_names[i] if i != _tree.TREE_UNDEFINED else "undefined!"
         for i in tree_.feature
     ]
 
     paths = []
     path = []
-    
+
     def recurse(node, path, paths):
-        
         if tree_.feature[node] != _tree.TREE_UNDEFINED:
             name = feature_name[node]
             threshold = tree_.threshold[node]
             p1, p2 = list(path), list(path)
             p1 += [f"({name} <= {np.round(threshold, 3)})"]
             recurse(tree_.children_left[node], p1, paths)
             p2 += [f"({name} > {np.round(threshold, 3)})"]
             recurse(tree_.children_right[node], p2, paths)
         else:
             path += [(tree_.value[node], tree_.n_node_samples[node])]
             paths += [path]
-            
+
     recurse(0, path, paths)
 
     # sort by samples count
     samples_count = [p[-1][1] for p in paths]
     ii = list(np.argsort(samples_count))
     paths = [paths[i] for i in reversed(ii)]
-    
+
     rules = []
     for path in paths:
         rule = "if "
-        
+
         for p in path[:-1]:
             if rule != "if ":
                 rule += " and "
             rule += str(p)
         rule += " then "
         if class_names is None:
-            rule += "response: "+str(np.round(path[-1][0][0][0],3))
+            rule += "response: " + str(np.round(path[-1][0][0][0], 3))
         else:
             classes = path[-1][0][0]
             l = np.argmax(classes)
             rule += f"class: {class_names[l]} (proba: {np.round(100.0*classes[l]/np.sum(classes),2)}%)"
         rule += f" | based on {path[-1][1]:,} samples"
         rules += [rule]
-        
+
     return rules
 
 
 def save_rules(tree, feature_names, class_names, model_file_path, learner_name):
     try:
         rules = get_rules(tree, feature_names, class_names)
         fname = os.path.join(model_file_path, f"{learner_name}_rules.txt")
         with open(fname, "w") as fout:
             for r in rules:
                 fout.write(r + "\n\n")
     except Exception as e:
         logger.info(f"Problem with extracting decision tree rules. {str(e)}")
 
-class DecisionTreeAlgorithm(SklearnAlgorithm):
 
+class DecisionTreeAlgorithm(SklearnAlgorithm):
     algorithm_name = "Decision Tree"
     algorithm_short_name = "Decision Tree"
 
     def __init__(self, params):
         super(DecisionTreeAlgorithm, self).__init__(params)
         logger.debug("DecisionTreeAlgorithm.__init__")
         self.library_version = sklearn.__version__
@@ -127,47 +129,51 @@
             class_names,
             metric_name,
             ml_task,
             explain_level,
         )
         if explain_level == 0:
             return
-        try:
-            if len(class_names) > 10:
-                # dtreeviz does not support more than 10 classes
-                return
-            viz = dtreeviz(
-                self.model,
-                X_train,
-                y_train,
-                target_name="target",
-                feature_names=X_train.columns,
-                class_names=class_names,
-            )
-            tree_file_plot = os.path.join(model_file_path, learner_name + "_tree.svg")
-            viz.save(tree_file_plot)
-        except Exception as e:
-            logger.info(f"Problem when visualizing decision tree. {str(e)}")
-
-        save_rules(self.model, X_train.columns, class_names, model_file_path, learner_name)
+        with warnings.catch_warnings():
+            warnings.simplefilter(action="ignore")
+            try:
+                if len(class_names) > 10:
+                    # dtreeviz does not support more than 10 classes
+                    return
+                viz = dtreeviz(
+                    self.model,
+                    X_train,
+                    y_train,
+                    target_name="target",
+                    feature_names=X_train.columns,
+                    class_names=class_names,
+                )
+                tree_file_plot = os.path.join(
+                    model_file_path, learner_name + "_tree.svg"
+                )
+                viz.save(tree_file_plot)
+            except Exception as e:
+                logger.info(f"Problem when visualizing decision tree. {str(e)}")
 
+            save_rules(
+                self.model, X_train.columns, class_names, model_file_path, learner_name
+            )
 
 
 class DecisionTreeRegressorAlgorithm(SklearnAlgorithm):
-
     algorithm_name = "Decision Tree"
     algorithm_short_name = "Decision Tree"
 
     def __init__(self, params):
         super(DecisionTreeRegressorAlgorithm, self).__init__(params)
         logger.debug("DecisionTreeRegressorAlgorithm.__init__")
         self.library_version = sklearn.__version__
         self.max_iters = additional.get("max_steps", 1)
         self.model = DecisionTreeRegressor(
-            criterion=params.get("criterion", "mse"),
+            criterion=params.get("criterion", "squared_error"),
             max_depth=params.get("max_depth", 3),
             random_state=params.get("seed", 1),
         )
 
     def file_extension(self):
         return "decision_tree"
 
@@ -196,29 +202,46 @@
             class_names,
             metric_name,
             ml_task,
             explain_level,
         )
         if explain_level == 0:
             return
-        try:
-
-            viz = dtreeviz(
-                self.model,
-                X_train,
-                y_train,
-                target_name="target",
-                feature_names=X_train.columns,
-            )
-            tree_file_plot = os.path.join(model_file_path, learner_name + "_tree.svg")
-            viz.save(tree_file_plot)
-        except Exception as e:
-            logger.info(f"Problem when visuzalizin decision tree regressor. {str(e)}")
+        with warnings.catch_warnings():
+            warnings.simplefilter(action="ignore")
+            try:
+                # 250 is hard limit for number of points used in visualization
+                # if too many points are used then final SVG plot is very large (can be > 100MB)
+                if X_train.shape[0] > 250:
+                    x, _, y, _ = subsample(X_train, y_train, REGRESSION, 250)
+                    viz = dtreeviz(
+                        self.model,
+                        x,
+                        y,
+                        target_name="target",
+                        feature_names=x.columns,
+                    )
+                else:
+                    viz = dtreeviz(
+                        self.model,
+                        X_train,
+                        y_train,
+                        target_name="target",
+                        feature_names=X_train.columns,
+                    )
+                tree_file_plot = os.path.join(
+                    model_file_path, learner_name + "_tree.svg"
+                )
+                viz.save(tree_file_plot)
+            except Exception as e:
+                logger.info(
+                    f"Problem when visuzalizin decision tree regressor. {str(e)}"
+                )
 
-        save_rules(self.model, X_train.columns, None, model_file_path, learner_name)
+            save_rules(self.model, X_train.columns, None, model_file_path, learner_name)
 
 
 dt_params = {"criterion": ["gini", "entropy"], "max_depth": [2, 3, 4]}
 
 classification_default_params = {"criterion": "gini", "max_depth": 3}
 
 additional = {
@@ -252,27 +275,27 @@
     required_preprocessing,
     additional,
     classification_default_params,
 )
 
 dt_regression_params = {
     "criterion": [
-        "mse",
+        "squared_error",
         "friedman_mse",
     ],  # remove "mae" because it slows down a lot https://github.com/scikit-learn/scikit-learn/issues/9626
     "max_depth": [2, 3, 4],
 }
 regression_required_preprocessing = [
     "missing_values_inputation",
     "convert_categorical",
     "datetime_transform",
     "text_transform",
 ]
 
-regression_default_params = {"criterion": "mse", "max_depth": 3}
+regression_default_params = {"criterion": "squared_error", "max_depth": 3}
 
 AlgorithmsRegistry.add(
     REGRESSION,
     DecisionTreeRegressorAlgorithm,
     dt_regression_params,
     regression_required_preprocessing,
     additional,
```

### Comparing `mljar-supervised-0.9.1/supervised/algorithms/baseline.py` & `mljar-supervised-1.0.0/supervised/algorithms/baseline.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from supervised.utils.config import LOG_LEVEL
 
 logger = logging.getLogger(__name__)
 logger.setLevel(LOG_LEVEL)
 
 
 class BaselineClassifierAlgorithm(SklearnAlgorithm):
-
     algorithm_name = "Baseline Classifier"
     algorithm_short_name = "Baseline"
 
     def __init__(self, params):
         super(BaselineClassifierAlgorithm, self).__init__(params)
         logger.debug("BaselineClassifierAlgorithm.__init__")
 
@@ -38,15 +37,14 @@
             hasattr(self.model, "n_outputs_")
             and self.model.n_outputs_ is not None
             and self.model.n_outputs_ > 0
         )
 
 
 class BaselineRegressorAlgorithm(SklearnAlgorithm):
-
     algorithm_name = "Baseline Regressor"
     algorithm_short_name = "Baseline"
 
     def __init__(self, params):
         super(BaselineRegressorAlgorithm, self).__init__(params)
         logger.debug("BaselineRegressorAlgorithm.__init__")
```

### Comparing `mljar-supervised-0.9.1/supervised/algorithms/algorithm.py` & `mljar-supervised-1.0.0/supervised/algorithms/algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
                 self,
                 X_validation,
                 y_validation,
                 model_file_path,
                 learner_name,
                 metric_name,
                 ml_task,
+                self.params.get("n_jobs", -1),
             )
         if explain_level > 1:
             PlotSHAP.compute(
                 self,
                 X_train,
                 y_train,
                 X_validation,
```

### Comparing `mljar-supervised-0.9.1/supervised/algorithms/linear.py` & `mljar-supervised-1.0.0/supervised/algorithms/linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from supervised.utils.config import LOG_LEVEL
 
 logger = logging.getLogger(__name__)
 logger.setLevel(LOG_LEVEL)
 
 
 class LinearAlgorithm(SklearnAlgorithm):
-
     algorithm_name = "Logistic Regression"
     algorithm_short_name = "Linear"
 
     def __init__(self, params):
         super(LinearAlgorithm, self).__init__(params)
         logger.debug("LinearAlgorithm.__init__")
         self.max_iters = 1
@@ -102,15 +101,14 @@
             )
             df.to_csv(
                 os.path.join(model_file_path, f"{learner_name}_coefs.csv"), index=True
             )
 
 
 class LinearRegressorAlgorithm(SklearnAlgorithm):
-
     algorithm_name = "Linear Regression"
     algorithm_short_name = "Linear"
 
     def __init__(self, params):
         super(LinearRegressorAlgorithm, self).__init__(params)
         logger.debug("LinearRegressorAlgorithm.__init__")
         self.max_iters = 1
```

### Comparing `mljar-supervised-0.9.1/supervised/automl.py` & `mljar-supervised-1.0.0/supervised/automl.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 import logging
 
-from supervised.base_automl import BaseAutoML
+import warnings
+
+warnings.filterwarnings("ignore", message=".*The 'nopython' keyword.*")
 
+from supervised.base_automl import BaseAutoML
 from supervised.utils.config import LOG_LEVEL
 
+# libraries for type hints
+from typing import Optional, Union, List
+from typing_extensions import (
+    Literal,
+)  # typing_extensions is used for using Literal from python 3.7
+from re import U
+import numpy
+import pandas
+from collections.abc import Iterable
 
 logging.basicConfig(
     format="%(asctime)s %(name)s %(levelname)s %(message)s", level=logging.ERROR
 )
 logger = logging.getLogger(__name__)
 logger.setLevel(LOG_LEVEL)
 
@@ -16,65 +28,95 @@
 
     """
     Automated Machine Learning for supervised tasks (binary classification, multiclass classification, regression).
     """
 
     def __init__(
         self,
-        results_path=None,
-        total_time_limit=60 * 60,
-        mode="Explain",
-        ml_task="auto",
-        model_time_limit=None,
-        algorithms="auto",
-        train_ensemble=True,
-        stack_models="auto",
-        eval_metric="auto",
-        validation_strategy="auto",
-        explain_level="auto",
-        golden_features="auto",
-        features_selection="auto",
-        start_random_models="auto",
-        hill_climbing_steps="auto",
-        top_models_to_improve="auto",
-        boost_on_errors="auto",
-        kmeans_features="auto",
-        mix_encoding="auto",
-        max_single_prediction_time=None,
-        n_jobs=-1,
-        verbose=1,
-        random_state=1234,
+        results_path: Optional[str] = None,
+        total_time_limit: int = 60 * 60,
+        mode: Literal["Explain", "Perform", "Compete", "Optuna"] = "Explain",
+        ml_task: Literal[
+            "auto", "binary_classification", "multiclass_classification", "regression"
+        ] = "auto",
+        model_time_limit: Optional[int] = None,
+        algorithms: Union[
+            Literal["auto"],
+            List[
+                Literal[
+                    "Baseline",
+                    "Linear",
+                    "Decicion Tree",
+                    "Random Forest",
+                    "Extra Trees",
+                    "LightGBM",
+                    "Xgboost",
+                    "CatBoost",
+                    "Neural Network",
+                    "Nearest Neighbors",
+                ]
+            ],
+        ] = "auto",
+        train_ensemble: bool = True,
+        stack_models: Union[Literal["auto"], bool] = "auto",
+        eval_metric: str = "auto",
+        validation_strategy: Union[Literal["auto"], dict] = "auto",
+        explain_level: Union[Literal["auto"], Literal[0, 1, 2]] = "auto",
+        golden_features: Union[Literal["auto"], bool, int] = "auto",
+        features_selection: Union[Literal["auto"], bool] = "auto",
+        start_random_models: Union[Literal["auto"], int] = "auto",
+        hill_climbing_steps: Union[Literal["auto"], int] = "auto",
+        top_models_to_improve: Union[Literal["auto"], int] = "auto",
+        boost_on_errors: Union[Literal["auto"], bool] = "auto",
+        kmeans_features: Union[Literal["auto"], bool] = "auto",
+        mix_encoding: Union[Literal["auto"], bool] = "auto",
+        max_single_prediction_time: Optional[Union[int, float]] = None,
+        optuna_time_budget: Optional[int] = None,
+        optuna_init_params: dict = {},
+        optuna_verbose: bool = True,
+        fairness_metric: str = "auto",
+        fairness_threshold: Union[Literal["auto"], float] = "auto",
+        privileged_groups: Union[Literal["auto"], list] = "auto",
+        underprivileged_groups: Union[Literal["auto"], list] = "auto",
+        n_jobs: int = -1,
+        verbose: int = 1,
+        random_state: int = 1234,
     ):
         """
         Initialize `AutoML` object.
 
         Arguments:
             results_path (str): The path with results. If None, then the name of directory will be generated with the template: AutoML_{number},
                 where the number can be from 1 to 1,000 - depends which direcory name will be available.
                 If the `results_path` will point to directory with AutoML results (`params.json` must be present),
                 then all models will be loaded.
 
             total_time_limit (int): The total time limit in seconds for AutoML training.
                 It is not used when `model_time_limit` is not `None`.
 
-            mode (str): Can be {`Explain`, `Perform`, `Compete`}. This parameter defines the goal of AutoML and how intensive the AutoML search will be.
+            mode (str): Can be {`Explain`, `Perform`, `Compete`, `Optuna`}. This parameter defines the goal of AutoML and how intensive the AutoML search will be.
 
                 - `Explain` : To to be used when the user wants to explain and understand the data.
                     - Uses 75%/25% train/test split.
                     - Uses the following models: `Baseline`, `Linear`, `Decision Tree`, `Random Forest`, `XGBoost`, `Neural Network`, and `Ensemble`.
                     - Has full explanations in reports: learning curves, importance plots, and SHAP plots.
                 - `Perform` : To be used when the user wants to train a model that will be used in real-life use cases.
                     - Uses 5-fold CV (Cross-Validation).
                     - Uses the following models: `Linear`, `Random Forest`, `LightGBM`, `XGBoost`, `CatBoost`, `Neural Network`, and `Ensemble`.
                     - Has learning curves and importance plots in reports.
                 - `Compete` : To be used for machine learning competitions (maximum performance).
-                    - Uses 10-fold CV (Cross-Validation).
-                    - Uses the following models: `Decision Tree`, `Random Forest`, `Extra Trees`, `XGBoost`, `CatBoost`, `Neural Network`,
+                    - Uses 80/20 train/test split, or 5-fold CV, or 10-fold CV (Cross-Validation) - it depends on `total_time_limit`. If not set directly, AutoML will select validation automatically.
+                    - Uses the following models: `Decision Tree`, `Random Forest`, `Extra Trees`, `LightGBM`,  `XGBoost`, `CatBoost`, `Neural Network`,
                         `Nearest Neighbors`, `Ensemble`, and `Stacking`.
                     - It has only learning curves in the reports.
+                - `Optuna` : To be used for creating highly-tuned machine learning models.
+                    - Uses 10-fold CV (Cross-Validation).
+                    - It tunes with Optuna the following algorithms: `Random Forest`, `Extra Trees`, `LightGBM`, `XGBoost`, `CatBoost`, `Neural Network`.
+                    - It applies `Ensemble` and `Stacking` for trained models.
+                    - It has only learning curves in the reports.
 
             ml_task (str): Can be {"auto", "binary_classification", "multiclass_classification", "regression"}.
 
                 - If left `auto` AutoML will try to guess the task based on target values.
                 - If there will be only 2 values in the target, then task will be set to `"binary_classification"`.
                 - If number of values in the target will be between 2 and 20 (included), then task will be set to `"multiclass_classification"`.
                 - In all other casses, the task is set to `"regression"`.
@@ -101,22 +143,19 @@
                 - `Nearest Neighbors`,
 
 
             train_ensemble (boolean): Whether an ensemble gets created at the end of the training.
 
             stack_models (boolean): Whether a models stack gets created at the end of the training. Stack level is 1.
 
-            eval_metric (str): The metric to be optimized.
-                If "auto", then:
-
-                - `logloss` is used for classifications taks.
-                - `rmse` is used for regression taks.
+            eval_metric (str): The metric to be used in early stopping and to compare models.
 
-                Note:
-                    Still not implemented, please left `None`
+                - for binary classification: `logloss`, `auc`, `f1`, `average_precision`, `accuracy` - default is logloss (if left "auto")
+                - for mutliclass classification: `logloss`, `f1`, `accuracy` - default is `logloss` (if left "auto")
+                - for regression: `rmse`, `mse`, `mae`, `r2`, `mape`, `spearman`, `pearson` - default is `rmse` (if left "auto")
 
             validation_strategy (dict): Dictionary with validation type. Right now train/test split and cross-validation are supported.
 
                 Example:
 
                     Cross-validation exmaple:
                     {
@@ -139,21 +178,26 @@
 
                 - if `explain_level` is `0` no explanations are produced.
                 - if `explain_level` is `1` the following explanations are produced: importance plot (with permutation method), for decision trees produce tree plots, for linear models save coefficients.
                 - if `explain_level` is `2` the following explanations are produced: the same as `1` plus SHAP explanations.
 
                 If left `auto` AutoML will produce explanations based on the selected `mode`.
 
-            golden_features (boolean): Whether to use golden features
+            golden_features (boolean or int): Whether to use golden features (and how many should be added)
                 If left `auto` AutoML will use golden features based on the selected `mode`:
 
                 - If `mode` is "Explain", `golden_features` = False.
                 - If `mode` is "Perform", `golden_features` = True.
                 - If `mode` is "Compete", `golden_features` = True.
 
+                If `boolean` value is set then the number of Golden Features is set automatically.
+                It is set to min(100, max(10, 0.1*number_of_input_features)).
+
+                If `int` value is set, the number of Golden Features is set to this value.
+
             features_selection (boolean): Whether to do features_selection
                 If left `auto` AutoML will do feature selection based on the selected `mode`:
 
                 - If `mode` is "Explain", `features_selection` = False.
                 - If `mode` is "Perform", `features_selection` = True.
                 - If `mode` is "Compete", `features_selection` = True.
 
@@ -186,14 +230,66 @@
                 for categoricals with more than 25 categories, and one-hot binary encoding for other categoricals. It is only applied if there are
                 categorical features with cardinality smaller than 25. By default it is available in the `Compete` mode.
 
             max_single_prediction_time (int or float): The limit for prediction time for single sample. Use it if you want to have a model with fast predictions.
                 Ideal for creating ML pipelines used as REST API. Time is in seconds. By default (`max_single_prediction_time=None`) models are not optimized for fast predictions,
                 except the mode `Perform`. For the mode `Perform` the default is `0.5` seconds.
 
+            optuna_time_budget (int): The time in seconds which should be used by Optuna to tune each algorithm. It is time for tuning single algorithm.
+                If you select two algorithms: Xgboost and CatBoost, and set optuna_time_budget=1000, then Xgboost will be tuned for 1000 seconds and CatBoost will be tuned for 1000 seconds.
+                What is more, the tuning is made for each data type, for example for raw data and for data with inserted Golden Features.
+                This parameter is only used when `mode="Optuna"`. If you set `mode="Optuna"` and forget to set this parameter, it will be set to 3600 seconds.
+
+            optuna_init_params (dict): If you have already tuned parameters from Optuna you can reuse them by setting this parameter.
+                This parameter is only used when `mode="Optuna"`. The dict should have structure and params as specified in the MLJAR AutoML .
+
+            optuna_verbose (boolean): If true the Optuna tuning details are displayed. Set to `True` by default.
+
+            fairness_metric (string): Name of fairness metric that will be used for assessing fairness criteria.
+                Available metrics for binary and multiclass classification:
+
+                - `demographic_parity_difference`,
+                - `demographic_parity_ratio` - default metric,
+                - `equalized_odds_difference`,
+                - `equalized_odds_ratio`.
+
+                Metrics for regression:
+
+                - `group_loss_difference`,
+                - `group_loss_ratio` - default metric.
+
+
+            fairness_threshold (float): The treshold value for fairness metric.
+                The direction optimization (below or above threshold) of fairness metric is determined automatically.
+
+                Default values:
+
+                - for `demographic_parity_difference` the metric value should be below 0.1,
+                - for `demographic_parity_ratio` the metric value should be above 0.8,
+                - for `equalized_odds_difference` the metric value should be below 0.1,
+                - for `equalized_odds_ratio` the metric value shoule be above 0.8.
+                - for `group_loss_ratio` the metric value shoule be above 0.8.
+
+                For `group_loss_difference` the default threshold value can't be set because it depends on the dataset.
+                If `group_loss_difference` metric is used and `fairness_threshold` is not specified manually, then an exception will be raised.
+
+            privileged_groups (list): The list of privileged groups.
+
+                By default, list of privileged groups are automatically detected based on fairness metrics.
+                For example, in binary classification task, a privileged group is the one with the highest selection rate.
+
+                Example value: `[{"sex": "Male"}]`
+
+            underprivileged_groups (list): The list of underprivileged groups.
+
+                By default, list of underprivileged groups are automatically detected based on fairness metrics.
+                For example, in binary classification task, an underprivileged group is the one with the lowest selection rate.
+
+                Example value: `[{"sex": "Female"}]`
+
             n_jobs (int): Number of CPU cores to be used. By default is set to `-1` which means using  all processors.
 
             verbose (int): Controls the verbosity when fitting and predicting.
 
                 Note:
                     Still not implemented, please left `1`
 
@@ -237,19 +333,19 @@
             >>> automl.fit(X_train, y_train)
             >>> y_pred = automl.predict(X_test)
             >>> print(f"Accuracy: {accuracy_score(y_test, y_pred):.2f}%")
 
             Regression Example:
 
             >>> import pandas as pd
-            >>> from sklearn.datasets import load_boston
+            >>> from sklearn.datasets import fetch_california_housing
             >>> from sklearn.model_selection import train_test_split
             >>> from sklearn.metrics import mean_squared_error
             >>> from supervised import AutoML
-            >>> housing = load_boston()
+            >>> housing = fetch_california_housing()
             >>> X_train, X_test, y_train, y_test = train_test_split(
             ...       pd.DataFrame(housing.data, columns=housing.feature_names),
             ...       housing.target,
             ...       test_size=0.25,
             ...       random_state=123,
             ... )
             >>> automl = AutoML(mode="Compete")
@@ -288,33 +384,54 @@
         self.start_random_models = start_random_models
         self.hill_climbing_steps = hill_climbing_steps
         self.top_models_to_improve = top_models_to_improve
         self.boost_on_errors = boost_on_errors
         self.kmeans_features = kmeans_features
         self.mix_encoding = mix_encoding
         self.max_single_prediction_time = max_single_prediction_time
+        self.optuna_time_budget = optuna_time_budget
+        self.optuna_init_params = optuna_init_params
+        self.optuna_verbose = optuna_verbose
+        self.fairness_metric = fairness_metric
+        self.fairness_threshold = fairness_threshold
+        self.privileged_groups = privileged_groups
+        self.underprivileged_groups = underprivileged_groups
         self.n_jobs = n_jobs
         self.random_state = random_state
 
-    def fit(self, X, y, sample_weight=None):
+    def fit(
+        self,
+        X: Union[numpy.ndarray, pandas.DataFrame],
+        y: Union[numpy.ndarray, pandas.Series],
+        sample_weight: Optional[Union[numpy.ndarray, pandas.Series]] = None,
+        cv: Optional[Union[Iterable, List]] = None,
+        sensitive_features: Optional[
+            Union[numpy.ndarray, pandas.Series, pandas.DataFrame]
+        ] = None,
+    ):
         """Fit the AutoML model.
 
         Arguments:
             X (numpy.ndarray or pandas.DataFrame): Training data
 
             y (numpy.ndarray or pandas.Series): Training targets
 
             sample_weight (numpy.ndarray or pandas.Series): Training sample weights
 
+            cv (iterable or list): List or iterable with (train, validation) splits representing array of indices.
+                It is used only with custom validation (`validation_strategy={'validation_type': 'custom'}`).
+
+            sensitive_features (numpy.ndarray or pandas.Series or pandas.DataFrame): Sensitive features to learn fair models
+
         Returns:
             AutoML object: Returns `self`
         """
-        return self._fit(X, y, sample_weight)
+        return self._fit(X, y, sample_weight, cv, sensitive_features)
 
-    def predict(self, X):
+    def predict(self, X: Union[List, numpy.ndarray, pandas.DataFrame]) -> numpy.ndarray:
         """
         Computes predictions from AutoML best model.
 
         Arguments:
             X (list or numpy.ndarray or pandas.DataFrame):
                 Input values to make predictions on.
 
@@ -325,15 +442,17 @@
             - One-dimensional array of predictions for regression.
 
         Raises:
             AutoMLException: Model has not yet been fitted.
         """
         return self._predict(X)
 
-    def predict_proba(self, X):
+    def predict_proba(
+        self, X: Union[List, numpy.ndarray, pandas.DataFrame]
+    ) -> numpy.ndarray:
         """
         Computes class probabilities from AutoML best model.
         This method can only be used for classification tasks.
 
         Arguments:
             X (list or numpy.ndarray or pandas.DataFrame):
                 Input values to make predictions on.
@@ -344,15 +463,17 @@
 
         Raises:
             AutoMLException: Model has not yet been fitted.
 
         """
         return self._predict_proba(X)
 
-    def predict_all(self, X):
+    def predict_all(
+        self, X: Union[List, numpy.ndarray, pandas.DataFrame]
+    ) -> pandas.DataFrame:
         """
         Computes both class probabilities and class labels for classification tasks.
         Computes predictions for regression tasks.
 
         Arguments:
             X (list or numpy.ndarray or pandas.DataFrame):
                 Input values to make predictions on.
@@ -365,15 +486,20 @@
 
         Raises:
             AutoMLException: Model has not yet been fitted.
 
         """
         return self._predict_all(X)
 
-    def score(self, X, y=None, sample_weight=None):
+    def score(
+        self,
+        X: Union[numpy.ndarray, pandas.DataFrame],
+        y: Optional[Union[numpy.ndarray, pandas.Series]] = None,
+        sample_weight: Optional[Union[numpy.ndarray, pandas.Series]] = None,
+    ) -> float:
         """Calculates a goodness of `fit` for an AutoML instance.
 
         Arguments:
             X (numpy.ndarray or pandas.DataFrame):
                 Test values to make predictions on.
 
             y (numpy.ndarray or pandas.Series):
@@ -388,30 +514,35 @@
             - For regression tasks: returns the R^2 (coefficient of determination) on the given test data and labels.
         """
         return self._score(X, y, sample_weight)
 
     def report(self, width=900, height=1200):
         return self._report(width, height)
 
-
-    def need_retrain(self, X, y, sample_weight=None, decrease=0.1):
+    def need_retrain(
+        self,
+        X: Union[numpy.ndarray, pandas.DataFrame],
+        y: Union[numpy.ndarray, pandas.Series],
+        sample_weight: Optional[Union[numpy.ndarray, pandas.Series]] = None,
+        decrease: float = 0.1,
+    ) -> bool:
         """Decides about model retraining based on new data.
 
         Arguments:
             X (numpy.ndarray or pandas.DataFrame):
                 New data.
 
             y (numpy.ndarray or pandas.Series):
                 True labels for X.
 
             sample_weight (numpy.ndarray or pandas.Series):
                 Sample weights.
 
             decrease (float): The ratio of change in the performance used as a threshold for retraining decision.
-                By default, it is set to `0.1` which means that if the performance of AutoML will decrease by 10% 
+                By default, it is set to `0.1` which means that if the performance of AutoML will decrease by 10%
                 on new data then there is a need to retrain. This value should be set depending on your project needs.
                 Sometimes, 10% is enough, but for some projects, it can be even lower than 1%.
 
             Returns:
                 boolean: Decides if there is a need to retrain the AutoML.
         """
-        return self._need_retrain(X, y, sample_weight, decrease)
+        return self._need_retrain(X, y, sample_weight, decrease)
```

### Comparing `mljar-supervised-0.9.1/supervised/utils/common.py` & `mljar-supervised-1.0.0/supervised/utils/common.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-0.9.1/supervised/utils/shap.py` & `mljar-supervised-1.0.0/supervised/utils/shap.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 logger.setLevel(LOG_LEVEL)
 import warnings
 
 
 class PlotSHAP:
     @staticmethod
     def is_available(algorithm, X_train, y_train, ml_task):
-
         # https://github.com/mljar/mljar-supervised/issues/112 disable for NN
         # https://github.com/mljar/mljar-supervised/issues/114 disable for CatBoost
         if algorithm.algorithm_short_name in ["Baseline", "Neural Network", "CatBoost"]:
             return False
         if (
             algorithm.algorithm_short_name == "Xgboost"
             and algorithm.learner_params["booster"] == "gblinear"
@@ -50,15 +49,14 @@
                 "Disable SHAP explanations because of small number of samples (< 20)."
             )
             return False
         return True
 
     @staticmethod
     def get_explainer(algorithm, X_train):
-
         explainer = None
         if algorithm.algorithm_short_name in [
             "Xgboost",
             "Decision Tree",
             "Random Forest",
             "LightGBM",
             "Extra Trees",
@@ -337,19 +335,17 @@
         expected_value,
         X_vald,
         y_vald,
         model_file_path,
         learner_name,
         class_names,
     ):
-
         for decision_type in ["worst", "best"]:
             m = 1 if decision_type == "worst" else -1
             for i in range(4):
-
                 fig = plt.gcf()
                 shap.multioutput_decision_plot(
                     list(expected_value),
                     shap_values,
                     row_index=df_preds.lp.iloc[m * i],
                     show=False,
                     legend_labels=class_names,
```

### Comparing `mljar-supervised-0.9.1/supervised/utils/importance.py` & `mljar-supervised-1.0.0/supervised/utils/importance.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         model,
         X_validation,
         y_validation,
         model_file_path,
         learner_name,
         metric_name=None,
         ml_task=None,
+        n_jobs=-1,
     ):
         # for scoring check https://scikit-learn.org/stable/modules/model_evaluation.html#scoring-parameter
         if ml_task == BINARY_CLASSIFICATION:
             scoring = log_loss_scorer
             model.classes_ = np.unique(y_validation)
         elif ml_task == MULTICLASS_CLASSIFICATION:
             scoring = log_loss_scorer
@@ -70,15 +71,15 @@
                     y_vald = y_validation
 
                 importance = permutation_importance(
                     model,
                     X_vald,
                     y_vald,
                     scoring=scoring,
-                    n_jobs=-1,  # all cores
+                    n_jobs=n_jobs,
                     random_state=12,
                     n_repeats=5,  # default
                 )
 
             sorted_idx = importance["importances_mean"].argsort()
 
             # save detailed importance
```

### Comparing `mljar-supervised-0.9.1/supervised/utils/data_validation.py` & `mljar-supervised-1.0.0/supervised/utils/data_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     if not isinstance(value, bool):
         raise ValueError(
             f"'{original_var_name}' must be a boolean, got '{type(value)}'."
         )
 
 
 def check_greater_than_zero_integer_or_float(value, original_var_name):
-
     if not (isinstance(value, int) or isinstance(value, float)):
         raise ValueError(
             f"'{original_var_name}' must be an integer or float, got '{type(value)}'."
         )
 
     if value <= 0:
         raise ValueError(
```

### Comparing `mljar-supervised-0.9.1/supervised/utils/learning_curves.py` & `mljar-supervised-1.0.0/supervised/utils/learning_curves.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import matplotlib.pyplot as plt
 import matplotlib.colors as mcolors
 
 MY_COLORS = list(mcolors.TABLEAU_COLORS.values())
 
 
 class LearningCurves:
-
     output_file_name = "learning_curves.png"
 
     @staticmethod
     def single_iteration(learner_names, model_path):
         for ln in learner_names:
             df = pd.read_csv(
                 os.path.join(model_path, f"{ln}_training.log"),
@@ -84,21 +83,23 @@
                 names=["iteration", "train", "test"],
             )
 
             fold, repeat = learner_name_to_fold_repeat(ln)
             repeat_str = f" Reapeat {repeat+1}," if repeat is not None else ""
             # if trees_in_iteration is not None:
             #    df.iteration = df.iteration * trees_in_iteration
-            plt.plot(
-                df.iteration,
-                df.train,
-                "--",
-                color=colors[fold],
-                label=f"Fold {fold+1},{repeat_str} train",
-            )
+            any_none = np.sum(pd.isnull(df.train))
+            if any_none == 0:
+                plt.plot(
+                    df.iteration,
+                    df.train,
+                    "--",
+                    color=colors[fold],
+                    label=f"Fold {fold+1},{repeat_str} train",
+                )
             any_none = np.sum(pd.isnull(df.test))
             if any_none == 0:
                 plt.plot(
                     df.iteration,
                     df.test,
                     color=colors[fold],
                     label=f"Fold {fold+1},{repeat_str} test",
```

### Comparing `mljar-supervised-0.9.1/supervised/utils/additional_metrics.py` & `mljar-supervised-1.0.0/supervised/utils/additional_metrics.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,23 +31,59 @@
 
 logger = logging.getLogger(__name__)
 from supervised.utils.config import LOG_LEVEL
 
 logger.setLevel(LOG_LEVEL)
 from supervised.utils.learning_curves import LearningCurves
 from supervised.utils.common import construct_learner_name, get_fold_repeat_cnt
+from supervised.utils.additional_plots import AdditionalPlots
 from tabulate import tabulate
 
+from supervised.fairness.metrics import FairnessMetrics
+from supervised.fairness.report import FairnessReport
+
+
+from supervised.fairness.utils import (
+    accuracy,
+    selection_rate,
+    true_positive_rate,
+    false_positive_rate,
+    true_negative_rate,
+    false_negative_rate,
+)
+
 
 class AdditionalMetrics:
     @staticmethod
-    def binary_classification(target, predictions, sample_weight=None):
+    def binary_classification(
+        target,
+        predictions,
+        sample_weight=None,
+        sensitive_features=None,
+        fairness_metric=None,
+        fairness_threshold=None,
+        privileged_groups=[],
+        underprivileged_groups=[],
+        previous_fairness_optimization=None,
+    ):
+        negative_label, positive_label = "0", "1"
+        mapping = None
+        try:
+            pred_col = predictions.columns[0]
+            if "_0_for_" in pred_col and "_1_for_" in pred_col:
+                t = pred_col.split("_0_for_")[1]
+                t = t.split("_1_for_")
+                negative_label, positive_label = t[0], t[1]
+                mapping = {0: negative_label, 1: positive_label}
+        except Exception as e:
+            pass
 
-        predictions = np.array(predictions)
+        predictions = np.array(predictions).flatten()
         sorted_predictions = np.sort(predictions)
+
         STEPS = 100  # can go lower for speed increase ???
         details = {
             "threshold": [],
             "f1": [],
             "accuracy": [],
             "precision": [],
             "recall": [],
@@ -120,43 +156,125 @@
                 "score": np.max(details["mcc"]),
                 "threshold": details["threshold"][np.argmax(details["mcc"])],
             },
         }
 
         threshold = float(max_metrics["accuracy"]["threshold"])
 
+        # updating resopnse variable for accuracy metric
+        response = (predictions > threshold).astype(int)
+
+        # accuracy threshold metrics
+        accuracy_threshold_metrics = {
+            "logloss": {
+                "score": logloss(target, predictions, sample_weight=sample_weight),
+                "threshold": None,
+            },  # there is no threshold for LogLoss
+            "auc": {
+                "score": roc_auc_score(
+                    target, predictions, sample_weight=sample_weight
+                ),
+                "threshold": None,
+            },  # there is no threshold for AUC
+            "f1": {
+                "score": f1_score(target, response, sample_weight=sample_weight),
+                "threshold": threshold,
+            },
+            "accuracy": {
+                "score": accuracy_score(target, response, sample_weight=sample_weight),
+                "threshold": threshold,
+            },
+            "precision": {
+                "score": precision_score(target, response, sample_weight=sample_weight),
+                "threshold": threshold,
+            },
+            "recall": {
+                "score": recall_score(target, response, sample_weight=sample_weight),
+                "threshold": threshold,
+            },
+            "mcc": {
+                "score": matthews_corrcoef(
+                    target, response, sample_weight=sample_weight
+                ),
+                "threshold": threshold,
+            },
+        }
+
         # if sample_weight is not None:
         #    new_max_metrics = {}
         #    for k, v in max_metrics.items():
         #        new_max_metrics["weighted_" + k] = v
         #    max_metrics = new_max_metrics
 
         # confusion matrix
 
         conf_matrix = confusion_matrix(
             target, predictions > threshold, sample_weight=sample_weight
         )
 
         conf_matrix = pd.DataFrame(
             conf_matrix,
-            columns=["Predicted as negative", "Predicted as positive"],
-            index=["Labeled as negative", "Labeled as positive"],
+            columns=[
+                f"Predicted as {negative_label}",
+                f"Predicted as {positive_label}",
+            ],
+            index=[f"Labeled as {negative_label}", f"Labeled as {positive_label}"],
+        )
+
+        predicted_labels = pd.Series((predictions.ravel() > threshold).astype(int))
+        predicted_probas = pd.DataFrame(
+            {"proba_0": 1 - predictions.ravel(), "proba_1": predictions.ravel()}
         )
 
-        return {
+        if mapping is not None:
+            labeled_target = target["target"].map(mapping)
+            predicted_labels = predicted_labels.map(mapping)
+        else:
+            labeled_target = target
+
+        metrics = {
             "metric_details": pd.DataFrame(details),
             "max_metrics": pd.DataFrame(max_metrics),
+            "accuracy_threshold_metrics": pd.DataFrame(accuracy_threshold_metrics),
             "confusion_matrix": conf_matrix,
             "threshold": threshold,
+            "additional_plots": AdditionalPlots.plots_binary(
+                labeled_target, predicted_labels, predicted_probas
+            ),
         }
 
-    @staticmethod
-    def multiclass_classification(target, predictions, sample_weight=None):
+        if sensitive_features is not None:
+            metrics["fairness_metrics"] = FairnessMetrics.binary_classification(
+                target,
+                predicted_labels,
+                sensitive_features,
+                fairness_metric,
+                fairness_threshold,
+                privileged_groups,
+                underprivileged_groups,
+                previous_fairness_optimization,
+            )
+
+        return metrics
+
+    @staticmethod
+    def multiclass_classification(
+        target,
+        predictions,
+        sample_weight=None,
+        sensitive_features=None,
+        fairness_metric=None,
+        fairness_threshold=None,
+        privileged_groups=[],
+        underprivileged_groups=[],
+        previous_fairness_optimization=None,
+    ):
         all_labels = [i[11:] for i in predictions.columns.tolist()[:-1]]
 
+        predicted_probas = predictions[predictions.columns[:-1]]
         ll = logloss(
             target, predictions[predictions.columns[:-1]], sample_weight=sample_weight
         )
 
         if "target" in target.columns.tolist():
             # multiclass coding with integer
             labels = {i: l for i, l in enumerate(all_labels)}
@@ -167,14 +285,15 @@
             t = target[old_columns[0]]
             for l in all_labels:
                 t[target[f"target_{l}"] == 1] = l
 
             target = pd.DataFrame({"target": t})
 
         # Print the confusion matrix
+        predicted_labels = predictions["label"]
         predictions = predictions["label"]
         if not pd.api.types.is_string_dtype(predictions):
             predictions = predictions.astype(str)
 
         if not pd.api.types.is_string_dtype(target):
             target = target.astype(str)
 
@@ -193,57 +312,135 @@
             digits=6,
             labels=all_labels,
             output_dict=True,
             sample_weight=sample_weight,
         )
         max_metrics["logloss"] = ll
 
-        return {
+        metrics = {
             "max_metrics": pd.DataFrame(max_metrics).transpose(),
             "confusion_matrix": conf_matrix,
+            "additional_plots": AdditionalPlots.plots_multiclass(
+                target, predicted_labels, predicted_probas
+            ),
         }
 
-    @staticmethod
-    def regression(target, predictions, sample_weight=None):
+        if sensitive_features is not None:
+            metrics["fairness_metrics"] = FairnessMetrics.multiclass_classification(
+                target,
+                predicted_labels,
+                sensitive_features,
+                fairness_metric,
+                fairness_threshold,
+                privileged_groups,
+                underprivileged_groups,
+                previous_fairness_optimization,
+            )
+        return metrics
+
+    @staticmethod
+    def regression(
+        target,
+        predictions,
+        sample_weight=None,
+        sensitive_features=None,
+        fairness_metric=None,
+        fairness_threshold=None,
+        privileged_groups=[],
+        underprivileged_groups=[],
+        previous_fairness_optimization=None,
+    ):
         regression_metrics = {
             "MAE": mean_absolute_error,
             "MSE": mean_squared_error,
             "RMSE": lambda t, p, sample_weight: np.sqrt(
                 mean_squared_error(t, p, sample_weight=sample_weight)
             ),
             "R2": r2_score,
             "MAPE": mean_absolute_percentage_error,
         }
         max_metrics = {}
         for k, v in regression_metrics.items():
             max_metrics[k] = v(target, predictions, sample_weight=sample_weight)
 
-        return {
+        metrics = {
             "max_metrics": pd.DataFrame(
                 {
                     "Metric": list(max_metrics.keys()),
                     "Score": list(max_metrics.values()),
                 }
-            )
+            ),
+            "additional_plots": AdditionalPlots.plots_regression(target, predictions),
         }
 
-    @staticmethod
-    def compute(target, predictions, sample_weight, ml_task):
+        if sensitive_features is not None:
+            metrics["fairness_metrics"] = FairnessMetrics.regression(
+                target,
+                predictions,
+                sensitive_features,
+                fairness_metric,
+                fairness_threshold,
+                privileged_groups,
+                underprivileged_groups,
+                previous_fairness_optimization,
+            )
+
+        return metrics
+
+    @staticmethod
+    def compute(
+        target,
+        predictions,
+        sample_weight,
+        ml_task,
+        sensitive_features=None,
+        fairness_metric=None,
+        fairness_threshold=None,
+        privileged_groups=[],
+        underprivileged_groups=[],
+        previous_fairness_optimization=None,
+    ):
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             if ml_task == BINARY_CLASSIFICATION:
                 return AdditionalMetrics.binary_classification(
-                    target, predictions, sample_weight
+                    target,
+                    predictions,
+                    sample_weight,
+                    sensitive_features,
+                    fairness_metric,
+                    fairness_threshold,
+                    privileged_groups,
+                    underprivileged_groups,
+                    previous_fairness_optimization,
                 )
             elif ml_task == MULTICLASS_CLASSIFICATION:
                 return AdditionalMetrics.multiclass_classification(
-                    target, predictions, sample_weight
+                    target,
+                    predictions,
+                    sample_weight,
+                    sensitive_features,
+                    fairness_metric,
+                    fairness_threshold,
+                    privileged_groups,
+                    underprivileged_groups,
+                    previous_fairness_optimization,
                 )
             elif ml_task == REGRESSION:
-                return AdditionalMetrics.regression(target, predictions, sample_weight)
+                return AdditionalMetrics.regression(
+                    target,
+                    predictions,
+                    sample_weight,
+                    sensitive_features,
+                    fairness_metric,
+                    fairness_threshold,
+                    privileged_groups,
+                    underprivileged_groups,
+                    previous_fairness_optimization,
+                )
 
     @staticmethod
     def save(additional_metrics, ml_task, model_desc, model_path):
         try:
             fold_cnt, repeat_cnt = get_fold_repeat_cnt(model_path)
             if ml_task == BINARY_CLASSIFICATION:
                 AdditionalMetrics.save_binary_classification(
@@ -254,107 +451,155 @@
                     additional_metrics, model_desc, model_path, fold_cnt, repeat_cnt
                 )
             elif ml_task == REGRESSION:
                 AdditionalMetrics.save_regression(
                     additional_metrics, model_desc, model_path, fold_cnt, repeat_cnt
                 )
         except Exception as e:
-            logger.error(
+            logger.exception(
                 f"Exception while saving additional metrics. {str(e)}\nContinuing ..."
             )
 
     @staticmethod
     def add_learning_curves(fout):
         fout.write("\n\n## Learning curves\n")
         fout.write(f"![Learning curves]({LearningCurves.output_file_name})")
 
     @staticmethod
     def save_binary_classification(
         additional_metrics, model_desc, model_path, fold_cnt, repeat_cnt
     ):
         max_metrics = additional_metrics["max_metrics"].transpose()
+        accuracy_threshold_metrics = additional_metrics[
+            "accuracy_threshold_metrics"
+        ].transpose()
         confusion_matrix = additional_metrics["confusion_matrix"]
         threshold = additional_metrics["threshold"]
 
-        with open(os.path.join(model_path, "README.md"), "w") as fout:
+        fairness_metrics = additional_metrics.get("fairness_metrics")
+
+        with open(os.path.join(model_path, "README.md"), "w", encoding="utf-8") as fout:
             fout.write(model_desc)
             fout.write("\n## Metric details\n{}\n\n".format(max_metrics.to_markdown()))
             fout.write(
+                "\n## Metric details with threshold from accuracy metric\n{}\n\n".format(
+                    accuracy_threshold_metrics.to_markdown()
+                )
+            )
+            fout.write(
                 "\n## Confusion matrix (at threshold={})\n{}".format(
                     np.round(threshold, 6), confusion_matrix.to_markdown()
                 )
             )
+
+            if fairness_metrics is not None:
+                FairnessReport.save_classification(
+                    fairness_metrics, fout, model_path, is_multi=False
+                )
+
             AdditionalMetrics.add_learning_curves(fout)
             AdditionalMetrics.add_tree_viz(fout, model_path, fold_cnt, repeat_cnt)
             AdditionalMetrics.add_linear_coefs(fout, model_path, fold_cnt, repeat_cnt)
             AdditionalMetrics.add_permutation_importance(
                 fout, model_path, fold_cnt, repeat_cnt
             )
+
+            plots = additional_metrics.get("additional_plots")
+            if plots is not None:
+                AdditionalPlots.append(fout, model_path, plots)
+
             AdditionalMetrics.add_shap_importance(
                 fout, model_path, fold_cnt, repeat_cnt
             )
             AdditionalMetrics.add_shap_binary(fout, model_path, fold_cnt, repeat_cnt)
+
             fout.write("\n\n[<< Go back](../README.md)\n")
 
     @staticmethod
     def save_multiclass_classification(
         additional_metrics, model_desc, model_path, fold_cnt, repeat_cnt
     ):
         max_metrics = additional_metrics["max_metrics"].transpose()
         confusion_matrix = additional_metrics["confusion_matrix"]
 
-        with open(os.path.join(model_path, "README.md"), "w") as fout:
+        fairness_metrics = additional_metrics.get("fairness_metrics")
+
+        with open(os.path.join(model_path, "README.md"), "w", encoding="utf-8") as fout:
             fout.write(model_desc)
             fout.write("\n### Metric details\n{}\n\n".format(max_metrics.to_markdown()))
             fout.write(
                 "\n## Confusion matrix\n{}".format(confusion_matrix.to_markdown())
             )
+
+            if fairness_metrics is not None:
+                # we treat multiclass problem as several binary problems
+                FairnessReport.save_classification(
+                    fairness_metrics, fout, model_path, is_multi=True
+                )
+
             AdditionalMetrics.add_learning_curves(fout)
             AdditionalMetrics.add_tree_viz(fout, model_path, fold_cnt, repeat_cnt)
             AdditionalMetrics.add_linear_coefs(fout, model_path, fold_cnt, repeat_cnt)
             AdditionalMetrics.add_permutation_importance(
                 fout, model_path, fold_cnt, repeat_cnt
             )
+
+            plots = additional_metrics.get("additional_plots")
+            if plots is not None:
+                AdditionalPlots.append(fout, model_path, plots)
+
             AdditionalMetrics.add_shap_importance(
                 fout, model_path, fold_cnt, repeat_cnt
             )
             AdditionalMetrics.add_shap_multiclass(
                 fout, model_path, fold_cnt, repeat_cnt
             )
+
             fout.write("\n\n[<< Go back](../README.md)\n")
 
     @staticmethod
     def save_regression(
         additional_metrics, model_desc, model_path, fold_cnt, repeat_cnt
     ):
         max_metrics = additional_metrics["max_metrics"]
-        with open(os.path.join(model_path, "README.md"), "w") as fout:
+        fairness_metrics = additional_metrics.get("fairness_metrics")
+
+        with open(os.path.join(model_path, "README.md"), "w", encoding="utf-8") as fout:
             fout.write(model_desc)
             fout.write(
                 "\n### Metric details:\n{}\n\n".format(
                     tabulate(max_metrics.values, max_metrics.columns, tablefmt="pipe")
                 )
             )
+
+            if fairness_metrics is not None:
+                FairnessReport.regression(fairness_metrics, fout, model_path)
+
             AdditionalMetrics.add_learning_curves(fout)
             AdditionalMetrics.add_tree_viz(fout, model_path, fold_cnt, repeat_cnt)
             AdditionalMetrics.add_linear_coefs(fout, model_path, fold_cnt, repeat_cnt)
             AdditionalMetrics.add_permutation_importance(
                 fout, model_path, fold_cnt, repeat_cnt
             )
+
+            plots = additional_metrics.get("additional_plots")
+            if plots is not None:
+                AdditionalPlots.append(fout, model_path, plots)
+
             AdditionalMetrics.add_shap_importance(
                 fout, model_path, fold_cnt, repeat_cnt
             )
             AdditionalMetrics.add_shap_regression(
                 fout, model_path, fold_cnt, repeat_cnt
             )
+
             fout.write("\n\n[<< Go back](../README.md)\n")
 
     @staticmethod
     def add_linear_coefs(fout, model_path, fold_cnt, repeat_cnt):
-
         coef_files = [f for f in os.listdir(model_path) if "_coefs.csv" in f]
         if not len(coef_files):
             return
 
         # check if multiclass
         df = pd.read_csv(os.path.join(model_path, coef_files[0]), index_col=0)
         if df.shape[0] > 100:
@@ -395,15 +640,14 @@
             df = df.drop("m", axis=1)
 
             fout.write("\n\n## Coefficients\n")
             fout.write(df.to_markdown() + "\n")
 
     @staticmethod
     def add_tree_viz(fout, model_path, fold_cnt, repeat_cnt):
-
         tree_viz = [f for f in os.listdir(model_path) if "_tree.svg" in f]
         if len(tree_viz):
             fout.write("\n\n## Decision Tree \n")
             for repeat in range(repeat_cnt):
                 repeat_str = f", Repeat #{repeat+1}" if repeat_cnt > 1 else ""
                 for fold in range(fold_cnt):
                     learner_name = construct_learner_name(fold, repeat, repeat_cnt)
@@ -416,15 +660,14 @@
                         if os.path.exists(fname):
                             fout.write("\n\n### Rules\n\n")
                             with open(fname, "r") as fin:
                                 fout.write(fin.read() + "\n\n")
                     except Exception as e:
                         logger.info("Problem with adding rules to report. " + str(e))
 
-
     @staticmethod
     def add_permutation_importance(fout, model_path, fold_cnt, repeat_cnt):
         # permutation importance
         imp_data = [
             f
             for f in os.listdir(model_path)
             if "_importance.csv" in f and "shap" not in f
@@ -461,15 +704,14 @@
             ax.set_title("Feature importance")
 
         fig.savefig(os.path.join(model_path, "permutation_importance.png"))
         fout.write("\n\n## Permutation-based Importance\n")
         fout.write(f"![Permutation-based Importance](permutation_importance.png)")
 
         if "random_feature" in df.index.tolist():
-
             df["counter"] = 0
             df = df.fillna(
                 0
             )  # there might be not-used features between different learners
             max_counter = 0.0
             for col in df.columns:
                 if "Learner" not in col:
```

### Comparing `mljar-supervised-0.9.1/supervised/exceptions.py` & `mljar-supervised-1.0.0/supervised/exceptions.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-0.9.1/supervised/tuner/time_controller.py` & `mljar-supervised-1.0.0/supervised/tuner/time_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,16 @@
             pass
         return None
 
     def already_spend(self):
         return np.sum([s["train_time"] for s in self._spend])
 
     def time_should_use(self, fit_level):
+        if self._total_time_limit is None:
+            return 7 * 24 * 3600  # 7 days
 
         ratios = {
             "default_algorithms": 0.3,
             "not_so_random": 0.35,
             "mix_encoding": 0.05,
             "golden_features": 0.05,
             "kmeans_features": 0.05,
@@ -83,15 +85,14 @@
                 "kmeans_features",
                 "insert_random_feature",
                 "features_selection",
                 "stack",
             ]
             or "hill_climbing" in fit_level
         ):
-
             ratio = 0
             for k, v in ratios.items():
                 if k in self._steps:
                     ratio += v
 
             fl = fit_level
             if "hill_climbing" in fit_level:
@@ -130,26 +131,28 @@
                 break
         # if fit_level == "stack":
         #    compound -= 120 # leave time for ensemble
         # maybe not needed
         return compound
 
     def enough_time_for_step(self, fit_level):
-        if fit_level in ["ensemble", "ensemble_stacked"]:
+        if fit_level in ["ensemble", "ensemble_stacked", "fairness"]:
             return True
         total_time_spend = time.time() - self._start_time
         compound = self.compound_time_should_use(fit_level)
         # print("Enough time for step", fit_level, np.round(total_time_spend,2), np.round(compound,2))
         if total_time_spend > compound:
             # dont train more
             return False
 
         return True
 
     def enough_time_for_model(self, model_type):
+        if self._total_time_limit is None:
+            return True
 
         time_left = self._total_time_limit - self.already_spend()
         spend = [s["train_time"] for s in self._spend if s["model_type"] == model_type]
         model_mean_spend = np.mean(spend)
         return model_mean_spend <= time_left
 
     def enough_time(self, model_type, step):
@@ -202,14 +205,16 @@
         # dont need to check ...
         if step == "stack":
             return True
         # check if there is enough time for model to train
         return self.enough_time_for_model(model_type)
 
     def learner_time_limit(self, model_type, fit_level, k_folds):
+        if self._total_time_limit is None:
+            return 7 * 24 * 3600
 
         if self._model_time_limit is not None:
             return self._model_time_limit / k_folds
 
         # just train them ...
         if fit_level == "simple_algorithms":
             return None
@@ -244,15 +249,14 @@
         if self._is_stacking and fit_level == "stack":
             tt = time_left
             tt /= tune_algs_cnt  # give time equally for each algorithm
             tt /= k_folds  # time is per learner (per fold)
             return tt
 
     def log_time(self, model_name, model_type, fit_level, train_time):
-
         self._spend += [
             {
                 "model_name": model_name,
                 "model_type": model_type,
                 "fit_level": fit_level,
                 "train_time": train_time,
             }
```

### Comparing `mljar-supervised-0.9.1/supervised/tuner/data_info.py` & `mljar-supervised-1.0.0/supervised/tuner/data_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     BINARY_CLASSIFICATION,
 )
 
 
 class DataInfo:
     @staticmethod
     def compute(X, y, machinelearning_task):
-
         columns_info = {}
         for col in X.columns:
             columns_info[col] = []
             #
             empty_column = np.sum(pd.isnull(X[col]) == True) == X.shape[0]
             if empty_column:
                 columns_info[col] += ["empty_column"]
```

### Comparing `mljar-supervised-0.9.1/supervised/tuner/mljar_tuner.py` & `mljar-supervised-1.0.0/supervised/tuner/mljar_tuner.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,40 +13,52 @@
 from supervised.tuner.hill_climbing import HillClimbing
 from supervised.algorithms.registry import (
     BINARY_CLASSIFICATION,
     MULTICLASS_CLASSIFICATION,
     REGRESSION,
 )
 
+from supervised.algorithms.xgboost import xgboost_eval_metric
+from supervised.algorithms.lightgbm import lightgbm_eval_metric
+from supervised.algorithms.catboost import catboost_eval_metric
+from supervised.utils.utils import dump_data, load_data
 import logging
 from supervised.utils.config import LOG_LEVEL
 
 logger = logging.getLogger(__name__)
 logger.setLevel(LOG_LEVEL)
 
 
 class MljarTuner:
     def __init__(
         self,
         tuner_params,
         algorithms,
         ml_task,
+        eval_metric,
         validation_strategy,
         explain_level,
         data_info,
         golden_features,
         features_selection,
         train_ensemble,
         stack_models,
         adjust_validation,
         boost_on_errors,
         kmeans_features,
         mix_encoding,
+        optuna_time_budget,
+        optuna_init_params,
+        optuna_verbose,
         n_jobs,
         seed,
+        fairness_metric=None,
+        fairness_threshold=None,
+        privileged_groups=[],
+        underprivileged_groups=[],
     ):
         logger.debug("MljarTuner.__init__")
         self._start_random_models = tuner_params.get("start_random_models", 5)
         self._hill_climbing_steps = tuner_params.get("hill_climbing_steps", 3)
         self._top_models_to_improve = tuner_params.get("top_models_to_improve", 3)
         self._algorithms = algorithms
         self._ml_task = ml_task
@@ -57,15 +69,23 @@
         self._features_selection = features_selection
         self._train_ensemble = train_ensemble
         self._stack_models = stack_models
         self._adjust_validation = adjust_validation
         self._boost_on_errors = boost_on_errors
         self._kmeans_features = kmeans_features
         self._mix_encoding = mix_encoding
+        self._optuna_time_budget = optuna_time_budget
+        self._optuna_init_params = optuna_init_params
+        self._optuna_verbose = optuna_verbose
+        self._eval_metric = eval_metric
         self._n_jobs = n_jobs
+        self._fairness_metric = fairness_metric
+        self._fairness_threshold = fairness_threshold
+        self._privileged_groups = privileged_groups
+        self._underprivileged_groups = underprivileged_groups
         self._seed = seed
         self._unique_params_keys = []
 
     def _apply_categorical_strategies(self):
         if self._data_info is None:
             return []
         if self._data_info.get("columns_info") is None:
@@ -128,21 +148,26 @@
         if continous_cols == 0:
             return False
 
         # all good, can apply golden features
         return True
 
     def steps(self):
-
         all_steps = []
         if self._adjust_validation:
             all_steps += ["adjust_validation"]
 
         all_steps += ["simple_algorithms", "default_algorithms"]
 
+        if self._fairness_metric is not None:
+            all_steps += ["unfairness_mitigation"]
+            # up to 10 steps
+            for i in range(10):
+                all_steps += [f"unfairness_mitigation_update_{i+1}"]
+
         if self._start_random_models > 1:
             all_steps += ["not_so_random"]
 
         categorical_strategies = self._apply_categorical_strategies()
         if PreprocessingTuner.CATEGORICALS_MIX in categorical_strategies:
             all_steps += ["mix_encoding"]
         if PreprocessingTuner.CATEGORICALS_LOO in categorical_strategies:
@@ -152,15 +177,16 @@
         if self._kmeans_features and self._can_apply_kmeans_features():
             all_steps += ["kmeans_features"]
         if self._features_selection:
             all_steps += ["insert_random_feature"]
             all_steps += ["features_selection"]
         for i in range(self._hill_climbing_steps):
             all_steps += [f"hill_climbing_{i+1}"]
-        if self._boost_on_errors:
+        if self._boost_on_errors and self._fairness_metric is None:
+            # we can tun boost on errors only if there is not fairness optimization
             all_steps += ["boost_on_errors"]
         if self._train_ensemble:
             all_steps += ["ensemble"]
         if self._stack_models:
             all_steps += ["stack"]
             if self._train_ensemble:
                 all_steps += ["ensemble_stacked"]
@@ -179,16 +205,18 @@
             models_cnt = len(models)
             if step == "adjust_validation":
                 return self.adjust_validation_params(models_cnt)
             elif step == "simple_algorithms":
                 return self.simple_algorithms_params(models_cnt)
             elif step == "default_algorithms":
                 return self.default_params(models_cnt)
+            elif "fairness" in step:
+                return self.fairness_optimization(models, results_path)
             elif step == "not_so_random":
-                return self.get_not_so_random_params(models_cnt)
+                return self.get_not_so_random_params(models_cnt, models)
             elif step == "mix_encoding":
                 return self.get_mix_categorical_strategy(models, total_time_limit)
             elif step == "loo_encoding":
                 return self.get_loo_categorical_strategy(models, total_time_limit)
             elif step == "golden_features":
                 return self.get_golden_features_params(
                     models, results_path, total_time_limit
@@ -223,15 +251,14 @@
                         "final_loss": None,
                         "train_time": None,
                     }
                 ]
             elif step == "stack":
                 return self.get_params_stack_models(stacked_models)
             elif step == "ensemble_stacked":
-
                 # do we have stacked models?
                 any_stacked = False
                 for m in models:
                     if m._is_stacked:
                         any_stacked = True
                 if not any_stacked:
                     return []
@@ -246,51 +273,382 @@
                         "train_time": None,
                     }
                 ]
 
             # didnt find anything matching the step, return empty array
             return []
         except Exception as e:
+            import traceback
+
+            print(str(e), traceback.format_exc())
             return []
 
+    def fairness_optimization_binary_classification(self, current_models, results_path):
+        df_models, algorithms = self.df_models_algorithms(current_models)
+
+        generated_params = []
+        counts = {model_type: 0 for model_type in algorithms}
+
+        # get sensitive features for all samples
+        sensitive_features_path = os.path.join(results_path, "sensitive_features.data")
+        sensitive_features = load_data(sensitive_features_path)
+
+        # get target
+        y_path = os.path.join(results_path, "y.data")
+        target = np.array(load_data(y_path)["target"])
+
+        sensitive_columns = list(sensitive_features.columns)
+
+        for i in range(df_models.shape[0]):
+            model_type = df_models["model_type"].iloc[i]
+
+            if df_models["model_type"].iloc[i] in ["Baseline"]:
+                # we dont optimize Baseline
+                continue
+
+            counts[model_type] += 1
+            if counts[model_type] > 1:
+                continue
+
+            m = df_models["model"].iloc[i]
+
+            if "ratio" in self._fairness_metric.lower():
+                if m.get_worst_fairness() > self._fairness_threshold:
+                    continue
+            else:
+                if m.get_worst_fairness() < self._fairness_threshold:
+                    continue
+
+            fo = m.get_fairness_optimization()
+            fo_step = fo.get("step", 0)
+
+            samples_weight = np.ones(sensitive_features.shape[0])
+
+            fo = m.get_fairness_optimization()
+            weights = fo.get("weights")
+            for k, ws in weights.items():
+                sensitive_values = k.split("@")
+                ii = None
+                for i, sv in enumerate(sensitive_values):
+                    if ii is None:
+                        ii = sensitive_features[sensitive_columns[i]] == sv
+                    else:
+                        ii &= sensitive_features[sensitive_columns[i]] == sv
+
+                samples_weight[ii & (target == 0)] = max(ws[0], 0.01)
+                samples_weight[ii & (target == 1)] = max(
+                    ws[1], 0.01
+                )  # weight cant be negative
+
+            samples_weight = samples_weight * target.shape[0] / np.sum(samples_weight)
+
+            sample_weight_path = os.path.join(
+                results_path, m.get_type() + f"_fairness_sample_weight_{fo_step}.data"
+            )
+            dump_data(
+                sample_weight_path, pd.DataFrame({"sample_weight": samples_weight})
+            )
+
+            fo = m.get_fairness_optimization()
+            fo["step"] = fo_step
+
+            params = copy.deepcopy(m.params)
+            params["fairness_optimization"] = fo
+
+            params["validation_strategy"]["sample_weight_path"] = sample_weight_path
+            params["injected_sample_weight"] = True
+            if "SampleWeigthing" not in params["name"]:
+                params["name"] += "_SampleWeigthing"
+            if fo_step > 0:
+                if "Update" in params["name"]:
+                    n = params["name"].split("_")
+                    params["name"] = "_".join(n[:-2])
+                params["name"] += f"_Update_{fo_step}"
+
+            params["status"] = "initialized"
+            params["final_loss"] = None
+            params["train_time"] = None
+            params["data_type"] = "fairness"
+            if "model_architecture_json" in params["learner"]:
+                del params["learner"]["model_architecture_json"]
+            if self._optuna_time_budget is not None:
+                params["optuna_time_budget"] = self._optuna_time_budget
+                params["optuna_init_params"] = self._optuna_init_params
+                params["optuna_verbose"] = self._optuna_verbose
+
+            unique_params_key = MljarTuner.get_params_key(params)
+
+            if unique_params_key not in self._unique_params_keys:
+                generated_params += [params]
+
+        return generated_params
+
+    def fairness_optimization_regression(self, current_models, results_path):
+        df_models, algorithms = self.df_models_algorithms(current_models)
+
+        generated_params = []
+        counts = {model_type: 0 for model_type in algorithms}
+
+        # get sensitive features for all samples
+        sensitive_features_path = os.path.join(results_path, "sensitive_features.data")
+        sensitive_features = load_data(sensitive_features_path)
+
+        # get target
+        y_path = os.path.join(results_path, "y.data")
+        target = np.array(load_data(y_path)["target"])
+
+        sensitive_columns = list(sensitive_features.columns)
+
+        for i in range(df_models.shape[0]):
+            model_type = df_models["model_type"].iloc[i]
+
+            if df_models["model_type"].iloc[i] in ["Baseline"]:
+                # we dont optimize Baseline
+                continue
+
+            counts[model_type] += 1
+
+            m = df_models["model"].iloc[i]
+
+            if "ratio" in self._fairness_metric.lower():
+                if m.get_worst_fairness() > self._fairness_threshold:
+                    continue
+            else:
+                if m.get_worst_fairness() < self._fairness_threshold:
+                    continue
+
+            fo = m.get_fairness_optimization()
+            fo_step = fo.get("step", 0)
+
+            samples_weight = np.ones(sensitive_features.shape[0])
+
+            fo = m.get_fairness_optimization()
+            weights = fo.get("weights")
+
+            for k, ws in weights.items():
+                sensitive_values = k.split("@")
+                ii = None
+                for i, sv in enumerate(sensitive_values):
+                    if ii is None:
+                        ii = sensitive_features[sensitive_columns[i]] == sv
+                    else:
+                        ii &= sensitive_features[sensitive_columns[i]] == sv
+
+                samples_weight[ii] = max(ws, 0.01)
+
+            samples_weight = samples_weight * target.shape[0] / np.sum(samples_weight)
+
+            sample_weight_path = os.path.join(
+                results_path, m.get_type() + f"_fairness_sample_weight_{fo_step}.data"
+            )
+            dump_data(
+                sample_weight_path, pd.DataFrame({"sample_weight": samples_weight})
+            )
+
+            fo = m.get_fairness_optimization()
+            fo["step"] = fo_step
+
+            params = copy.deepcopy(m.params)
+            params["fairness_optimization"] = fo
+
+            params["validation_strategy"]["sample_weight_path"] = sample_weight_path
+            params["injected_sample_weight"] = True
+            if "SampleWeigthing" not in params["name"]:
+                params["name"] += "_SampleWeigthing"
+
+            if fo_step > 0:
+                if "Update" in params["name"]:
+                    n = params["name"].split("_")
+                    params["name"] = "_".join(n[:-2])
+                params["name"] += f"_Update_{fo_step}"
+
+            params["status"] = "initialized"
+            params["final_loss"] = None
+            params["train_time"] = None
+            params["data_type"] = "fairness"
+            if "model_architecture_json" in params["learner"]:
+                del params["learner"]["model_architecture_json"]
+            if self._optuna_time_budget is not None:
+                params["optuna_time_budget"] = self._optuna_time_budget
+                params["optuna_init_params"] = self._optuna_init_params
+                params["optuna_verbose"] = self._optuna_verbose
+
+            unique_params_key = MljarTuner.get_params_key(params)
+
+            if unique_params_key not in self._unique_params_keys:
+                generated_params += [params]
+
+        return generated_params
+
+    def fairness_optimization_multiclass_classification(
+        self, current_models, results_path
+    ):
+        df_models, algorithms = self.df_models_algorithms(
+            current_models
+        )  # , sort_by_worst_fairness=True)
+
+        generated_params = []
+        counts = {model_type: 0 for model_type in algorithms}
+
+        # get sensitive features for all samples
+        sensitive_features_path = os.path.join(results_path, "sensitive_features.data")
+        sensitive_features = load_data(sensitive_features_path)
+
+        # get target
+        y_path = os.path.join(results_path, "y.data")
+        target = np.array(load_data(y_path)["target"])
+
+        sensitive_columns = list(sensitive_features.columns)
+
+        for i in range(df_models.shape[0]):
+            model_type = df_models["model_type"].iloc[i]
+
+            if df_models["model_type"].iloc[i] in ["Baseline"]:
+                # we dont optimize Baseline
+                continue
+
+            counts[model_type] += 1
+
+            m = df_models["model"].iloc[i]
+
+            if "ratio" in self._fairness_metric.lower():
+                if m.get_worst_fairness() > self._fairness_threshold:
+                    continue
+            else:
+                if m.get_worst_fairness() < self._fairness_threshold:
+                    continue
+
+            fo = m.get_fairness_optimization()
+            fo_step = fo.get("step", 0)
+
+            samples_weight = np.ones(sensitive_features.shape[0])
+
+            fo = m.get_fairness_optimization()
+            weights = fo.get("weights")
+            target_values = fo.get("target_values")
+
+            for k, ws in weights.items():
+                sensitive_values = k.split("@")
+                ii = None
+                for i, sv in enumerate(sensitive_values):
+                    if ii is None:
+                        ii = sensitive_features[sensitive_columns[i]] == sv
+                    else:
+                        ii &= sensitive_features[sensitive_columns[i]] == sv
+
+                for j, t in enumerate(target_values):
+                    samples_weight[ii & (target == t)] = max(ws[j], 0.01)
+
+            samples_weight = samples_weight * target.shape[0] / np.sum(samples_weight)
+
+            sample_weight_path = os.path.join(
+                results_path, m.get_type() + f"_fairness_sample_weight_{fo_step}.data"
+            )
+            dump_data(
+                sample_weight_path, pd.DataFrame({"sample_weight": samples_weight})
+            )
+
+            fo = m.get_fairness_optimization()
+            fo["step"] = fo_step
+
+            params = copy.deepcopy(m.params)
+            params["fairness_optimization"] = fo
+
+            params["validation_strategy"]["sample_weight_path"] = sample_weight_path
+            params["injected_sample_weight"] = True
+            if "SampleWeigthing" not in params["name"]:
+                params["name"] += "_SampleWeigthing"
+            if fo_step > 0:
+                if "Update" in params["name"]:
+                    n = params["name"].split("_")
+                    params["name"] = "_".join(n[:-2])
+                params["name"] += f"_Update_{fo_step}"
+
+            params["status"] = "initialized"
+            params["final_loss"] = None
+            params["train_time"] = None
+            params["data_type"] = "fairness"
+            if "model_architecture_json" in params["learner"]:
+                del params["learner"]["model_architecture_json"]
+            if self._optuna_time_budget is not None:
+                params["optuna_time_budget"] = self._optuna_time_budget
+                params["optuna_init_params"] = self._optuna_init_params
+                params["optuna_verbose"] = self._optuna_verbose
+
+            unique_params_key = MljarTuner.get_params_key(params)
+
+            if unique_params_key not in self._unique_params_keys:
+                generated_params += [params]
+
+        return generated_params
+
+    def fairness_optimization(self, current_models, results_path):
+        if self._ml_task == BINARY_CLASSIFICATION:
+            return self.fairness_optimization_binary_classification(
+                current_models, results_path
+            )
+        if self._ml_task == REGRESSION:
+            return self.fairness_optimization_regression(current_models, results_path)
+        if self._ml_task == MULTICLASS_CLASSIFICATION:
+            return self.fairness_optimization_multiclass_classification(
+                current_models, results_path
+            )
+        return []
+
     def get_params_stack_models(self, stacked_models):
         if stacked_models is None or len(stacked_models) == 0:
             return []
 
         X_train_stacked_path = ""
         added_columns = []
 
-        model_types = ["Xgboost", "LightGBM", "CatBoost"]
+        # model_types = ["Xgboost", "LightGBM", "CatBoost"]
+        model_types = [
+            "Xgboost",
+            "LightGBM",
+            "CatBoost",
+            "Random Forest",
+            "Extra Trees",
+            "Neural Network",
+        ]
         generated_params = {m: [] for m in model_types}
         types_score_order = []
         # resue old params
         for m in stacked_models:
             # use only Xgboost, LightGBM and CatBoost as stacked models
             if m.get_type() not in model_types:
                 continue
 
             if m.get_type() not in types_score_order:
                 types_score_order += [m.get_type()]
 
-            if m.params.get("injected_sample_weight", False):
+            # the below condition is only true for fair models
+            if self._fairness_metric is None and m.params.get(
+                "injected_sample_weight", False
+            ):
                 # dont use boost_on_errors model for stacking
                 # there will be additional boost_on_errors step
                 continue
 
             params = copy.deepcopy(m.params)
 
             params["validation_strategy"]["X_path"] = params["validation_strategy"][
                 "X_path"
-            ].replace("X.parquet", "X_stacked.parquet")
+            ].replace("X.data", "X_stacked.data")
 
             params["name"] = params["name"] + "_Stacked"
             params["is_stacked"] = True
             params["status"] = "initialized"
             params["final_loss"] = None
             params["train_time"] = None
+            params["data_type"] += "_stacked"
+            if self._optuna_time_budget is not None:
+                params["optuna_time_budget"] = self._optuna_time_budget
+                params["optuna_init_params"] = self._optuna_init_params
+                params["optuna_verbose"] = self._optuna_verbose
 
             if "model_architecture_json" in params["learner"]:
                 # the new model will be created with wider input size
                 del params["learner"]["model_architecture_json"]
 
             if self._ml_task == REGRESSION:
                 # scale added predictions in regression if the target was scaled (in the case of NN)
@@ -329,14 +687,15 @@
             if params is None:
                 continue
 
             params["name"] = self.get_model_name(model_type, models_cnt + 1)
             params["status"] = "initialized"
             params["final_loss"] = None
             params["train_time"] = None
+            params["data_type"] = "original"
 
             unique_params_key = MljarTuner.get_params_key(params)
             if unique_params_key not in self._unique_params_keys:
                 generated_params += [params]
                 models_cnt += 1
         return generated_params
 
@@ -354,23 +713,23 @@
                 if params is None:
                     continue
 
                 params["name"] = self.get_model_name(model_type, models_cnt + 1)
                 params["status"] = "initialized"
                 params["final_loss"] = None
                 params["train_time"] = None
+                params["data_type"] = "original"
 
                 unique_params_key = MljarTuner.get_params_key(params)
                 if unique_params_key not in self._unique_params_keys:
                     generated_params += [params]
                     models_cnt += 1
         return generated_params
 
     def skip_if_rows_cols_limit(self, model_type):
-
         max_rows_limit = AlgorithmsRegistry.get_max_rows_limit(
             self._ml_task, model_type
         )
         max_cols_limit = AlgorithmsRegistry.get_max_cols_limit(
             self._ml_task, model_type
         )
 
@@ -380,15 +739,14 @@
         if max_cols_limit is not None:
             if self._data_info["cols"] > max_cols_limit:
                 return True
 
         return False
 
     def default_params(self, models_cnt):
-
         generated_params = []
         for model_type in [
             "LightGBM",
             "Xgboost",
             "CatBoost",
             "Neural Network",
             "Random Forest",
@@ -403,29 +761,57 @@
 
             logger.info(f"Get default parameters for {model_type} (#{models_cnt + 1})")
             params = self._get_model_params(
                 model_type, seed=models_cnt + 1, params_type="default"
             )
             if params is None:
                 continue
+            special = "Default_" if self._optuna_time_budget is None else "Optuna_"
             params["name"] = self.get_model_name(
-                model_type, models_cnt + 1, special="Default_"
+                model_type, models_cnt + 1, special=special
             )
             params["status"] = "initialized"
             params["final_loss"] = None
             params["train_time"] = None
+            params["data_type"] = "original"
+            if self._optuna_time_budget is not None:
+                params["optuna_time_budget"] = self._optuna_time_budget
+                params["optuna_init_params"] = self._optuna_init_params
+                params["optuna_verbose"] = self._optuna_verbose
 
             unique_params_key = MljarTuner.get_params_key(params)
             if unique_params_key not in self._unique_params_keys:
                 generated_params += [params]
                 models_cnt += 1
+
         return generated_params
 
-    def get_not_so_random_params(self, models_cnt):
+    def get_fairness_sample_weight(self, current_models, model_type):
+        try:
+            df_models, algorithms = self.df_models_algorithms(current_models)
+            # df_models are sorted based on fairness metric
+            df_models = df_models[df_models.model_type == model_type]
+
+            if df_models.shape[0]:
+                m = df_models["model"].iloc[0]
+                swp = m.params["validation_strategy"]["sample_weight_path"]
+
+                name_suffix = "_SampleWeigthing"
+                name = m.params["name"]
+                if "Update" in name:
+                    words = name.split("_")
+                    i = words.index("Update")
+                    name_suffix += f"_Update_{words[i+1]}"
+
+                return swp, name_suffix
+        except Exception:
+            pass
+        return None, None
 
+    def get_not_so_random_params(self, models_cnt, current_models):
         model_types = [
             "Xgboost",
             "LightGBM",
             "CatBoost",
             "Random Forest",
             "Extra Trees",
             "Neural Network",
@@ -438,26 +824,40 @@
             if model_type not in self._algorithms:
                 continue
 
             if self.skip_if_rows_cols_limit(model_type):
                 continue
             # minus 1 because already have 1 default
             for i in range(self._start_random_models - 1):
-
                 logger.info(
                     f"Generate not-so-random parameters for {model_type} (#{models_cnt+1})"
                 )
                 params = self._get_model_params(model_type, seed=i + 1)
                 if params is None:
                     continue
 
                 params["name"] = self.get_model_name(model_type, models_cnt + 1)
                 params["status"] = "initialized"
                 params["final_loss"] = None
                 params["train_time"] = None
+                params["data_type"] = "original"
+                if self._optuna_time_budget is not None:
+                    params["optuna_time_budget"] = self._optuna_time_budget
+                    params["optuna_init_params"] = self._optuna_init_params
+                    params["optuna_verbose"] = self._optuna_verbose
+
+                if self._fairness_metric is not None:
+                    swp, name_suffix = self.get_fairness_sample_weight(
+                        current_models, model_type
+                    )
+                    if swp is not None:
+                        params["validation_strategy"]["sample_weight_path"] = swp
+                        params["injected_sample_weight"] = True
+                    if name_suffix is not None:
+                        params["name"] += name_suffix
 
                 unique_params_key = MljarTuner.get_params_key(params)
                 if unique_params_key not in self._unique_params_keys:
                     generated_params[model_type] += [params]
                     models_cnt += 1
 
         """
@@ -505,26 +905,24 @@
 
     def get_hill_climbing_params(self, current_models):
         df_models, algorithms = self.df_models_algorithms(current_models)
         generated_params = []
         counts = {model_type: 0 for model_type in algorithms}
 
         for i in range(df_models.shape[0]):
-
             model_type = df_models["model_type"].iloc[i]
             counts[model_type] += 1
             if counts[model_type] > self._top_models_to_improve:
                 continue
 
             m = df_models["model"].iloc[i]
 
             for p in HillClimbing.get(
                 m.params.get("learner"), self._ml_task, len(current_models) + self._seed
             ):
-
                 model_indices = [
                     int(m.get_name().split("_")[0]) for m in current_models
                 ]
                 model_max_index = np.max(model_indices)
 
                 logger.info(
                     "Hill climbing step, for model #{0}".format(model_max_index + 1)
@@ -533,14 +931,20 @@
                     all_params = copy.deepcopy(m.params)
                     all_params["learner"] = p
 
                     all_params["name"] = self.get_model_name(
                         all_params["learner"]["model_type"],
                         model_max_index + 1 + len(generated_params),
                     )
+                    if "SampleWeigthing" in m.get_name():
+                        all_params["name"] += "_SampleWeigthing"
+                        n = m.get_name().split("_")
+                        if "Update" in n:
+                            i = n.index("Update")
+                            all_params["name"] += f"_Update_{n[i+1]}"
 
                     if "golden_features" in all_params["preprocessing"]:
                         all_params["name"] += "_GoldenFeatures"
                     if "drop_features" in all_params["preprocessing"] and len(
                         all_params["preprocessing"]["drop_features"]
                     ):
                         all_params["name"] += "_SelectedFeatures"
@@ -566,24 +970,26 @@
 
     def get_loo_categorical_strategy(self, current_models, total_time_limit):
         return self.get_categorical_strategy(
             current_models, PreprocessingTuner.CATEGORICALS_LOO, total_time_limit
         )
 
     def get_categorical_strategy(self, current_models, strategy, total_time_limit):
-
+        model_selection_time_limit = (
+            None if total_time_limit is None else 0.1 * total_time_limit
+        )
         df_models, algorithms = self.df_models_algorithms(
-            current_models, time_limit=0.1 * total_time_limit
+            current_models, time_limit=model_selection_time_limit
         )
         generated_params = []
         for m_type in algorithms:
             # try to add categorical strategy only for below algorithms
             if m_type not in [
                 "Xgboost",
-                "LightGBM",
+                # "LightGBM", # use built-in categoricals (but need to int encode)
                 # "Neural Network",
                 # "Random Forest",
                 # "Extra Trees",
             ]:
                 continue
             models = df_models[df_models.model_type == m_type]["model"]
 
@@ -636,23 +1042,33 @@
                     PreprocessingTuner.CATEGORICALS_MIX,
                 ]:
                     params["name"] = params["name"].replace("_" + st, "")
                 params["name"] += f"_{strategy}"
                 params["status"] = "initialized"
                 params["final_loss"] = None
                 params["train_time"] = None
+                params["data_type"] = params.get("data_type", "") + "_" + strategy
+                if self._optuna_time_budget is not None:
+                    params["optuna_time_budget"] = self._optuna_time_budget
+                    params["optuna_init_params"] = self._optuna_init_params
+                    params["optuna_verbose"] = self._optuna_verbose
+
                 if "model_architecture_json" in params["learner"]:
                     del params["learner"]["model_architecture_json"]
                 unique_params_key = MljarTuner.get_params_key(params)
                 if unique_params_key not in self._unique_params_keys:
                     generated_params += [params]
         return generated_params
 
     def df_models_algorithms(
-        self, current_models, time_limit=None, exclude_golden=False
+        self,
+        current_models,
+        time_limit=None,
+        exclude_golden=False,
+        sort_by_worst_fairness=False,
     ):
         scores = [m.get_final_loss() for m in current_models]
         model_types = [m.get_type() for m in current_models]
         names = [m.get_name() for m in current_models]
         train_times = [m.get_train_time() for m in current_models]
 
         df_models = pd.DataFrame(
@@ -660,94 +1076,141 @@
                 "model": current_models,
                 "score": scores,
                 "model_type": model_types,
                 "name": names,
                 "train_time": train_times,
             }
         )
+        if self._fairness_metric is not None:
+            worst_fairness = [m.get_worst_fairness() for m in current_models]
+            df_models["worst_fairness"] = worst_fairness
+            best_fairness = [m.get_best_fairness() for m in current_models]
+            df_models["best_fairness"] = best_fairness
+
         if time_limit is not None:
             df_models = df_models[df_models.train_time < time_limit]
             df_models.reset_index(drop=True, inplace=True)
 
         if exclude_golden:
             ii = df_models["name"].apply(lambda x: "GoldenFeatures" in x)
             df_models = df_models[~ii]
             df_models.reset_index(drop=True, inplace=True)
 
         df_models.sort_values(by="score", ascending=True, inplace=True)
+
+        if self._fairness_metric is not None:
+            sort_by_worst_fairness = True
+
+            ascending = True
+            if "ratio" in self._fairness_metric.lower():
+                ascending = False
+            if sort_by_worst_fairness:
+                df_models.sort_values(
+                    by="worst_fairness", ascending=ascending, inplace=True
+                )
+            else:
+                df_models.sort_values(
+                    by="best_fairness", ascending=ascending, inplace=True
+                )
+
         model_types = list(df_models.model_type)
         u, idx = np.unique(model_types, return_index=True)
         algorithms = u[np.argsort(idx)]
 
         return df_models, algorithms
 
     def get_golden_features_params(
         self, current_models, results_path, total_time_limit
     ):
-
+        model_selection_time_limit = (
+            None if total_time_limit is None else 0.1 * total_time_limit
+        )
         df_models, algorithms = self.df_models_algorithms(
-            current_models, time_limit=0.1 * total_time_limit
+            current_models, time_limit=model_selection_time_limit
         )
 
         generated_params = []
         for i in range(min(3, df_models.shape[0])):
             m = df_models["model"].iloc[i]
 
             params = copy.deepcopy(m.params)
             params["preprocessing"]["golden_features"] = {
                 "results_path": results_path,
                 "ml_task": self._ml_task,
+                "n_jobs": self._n_jobs,
             }
+            if (
+                self._golden_features is not None
+                and not isinstance(self._golden_features, bool)
+                and isinstance(self._golden_features, int)
+            ):
+                params["preprocessing"]["golden_features"][
+                    "features_count"
+                ] = self._golden_features
+
             params["name"] += "_GoldenFeatures"
             params["status"] = "initialized"
             params["final_loss"] = None
             params["train_time"] = None
+            params["data_type"] = params.get("data_type", "") + "_golden_features"
+            if self._optuna_time_budget is not None:
+                params["optuna_time_budget"] = self._optuna_time_budget
+                params["optuna_init_params"] = self._optuna_init_params
+                params["optuna_verbose"] = self._optuna_verbose
 
             if "model_architecture_json" in params["learner"]:
                 del params["learner"]["model_architecture_json"]
             unique_params_key = MljarTuner.get_params_key(params)
             if unique_params_key not in self._unique_params_keys:
                 generated_params += [params]
         return generated_params
 
     def get_kmeans_features_params(
         self, current_models, results_path, total_time_limit
     ):
-
+        model_selection_time_limit = (
+            None if total_time_limit is None else 0.1 * total_time_limit
+        )
         df_models, algorithms = self.df_models_algorithms(
-            current_models, time_limit=0.1 * total_time_limit, exclude_golden=True
+            current_models, time_limit=model_selection_time_limit, exclude_golden=True
         )
 
         generated_params = []
         for i in range(min(3, df_models.shape[0])):
             m = df_models["model"].iloc[i]
 
             params = copy.deepcopy(m.params)
             params["preprocessing"]["kmeans_features"] = {"results_path": results_path}
             params["name"] += "_KMeansFeatures"
             params["status"] = "initialized"
             params["final_loss"] = None
             params["train_time"] = None
+            params["data_type"] = params.get("data_type", "") + "_kmeans_features"
+            if self._optuna_time_budget is not None:
+                params["optuna_time_budget"] = self._optuna_time_budget
+                params["optuna_init_params"] = self._optuna_init_params
+                params["optuna_verbose"] = self._optuna_verbose
 
             if "model_architecture_json" in params["learner"]:
                 del params["learner"]["model_architecture_json"]
             unique_params_key = MljarTuner.get_params_key(params)
             if unique_params_key not in self._unique_params_keys:
                 generated_params += [params]
         return generated_params
 
     def time_features_selection(self, current_models, total_time_limit):
-
+        model_selection_time_limit = (
+            None if total_time_limit is None else 0.1 * total_time_limit
+        )
         df_models, algorithms = self.df_models_algorithms(
-            current_models, time_limit=0.1 * total_time_limit
+            current_models, time_limit=model_selection_time_limit
         )
 
         time_needed = 0
         for m_type in algorithms:
-
             if m_type not in [
                 "Xgboost",
                 "LightGBM",
                 "CatBoost",
                 "Neural Network",
                 "Random Forest",
                 "Extra Trees",
@@ -764,29 +1227,31 @@
                     time_needed += 2.0 * m.get_train_time()
                 else:
                     time_needed += m.get_train_time()
 
         return time_needed
 
     def get_params_to_insert_random_feature(self, current_models, total_time_limit):
-
         time_needed = self.time_features_selection(current_models, total_time_limit)
 
-        if time_needed > 0.1 * total_time_limit:
+        if total_time_limit is not None and time_needed > 0.1 * total_time_limit:
             print("Not enough time to perform features selection. Skip")
             print(
                 "Time needed for features selection ~", np.round(time_needed), "seconds"
             )
             print(
                 f"Please increase total_time_limit to at least ({int(np.round(10.0*time_needed))+60} seconds) to have features selection"
             )
             return None
 
+        model_selection_time_limit = (
+            None if total_time_limit is None else 0.1 * total_time_limit
+        )
         df_models, algorithms = self.df_models_algorithms(
-            current_models, time_limit=0.1 * total_time_limit
+            current_models, time_limit=model_selection_time_limit
         )
         if df_models.shape[0] == 0:
             return None
 
         m = df_models.iloc[0]["model"]
 
         params = copy.deepcopy(m.params)
@@ -794,38 +1259,45 @@
         params["name"] += "_RandomFeature"
         params["status"] = "initialized"
         params["final_loss"] = None
         params["train_time"] = None
         params["explain_level"] = 1
         if "model_architecture_json" in params["learner"]:
             del params["learner"]["model_architecture_json"]
+        if self._optuna_time_budget is not None:
+            # dont tune algorithm with random feature inserted
+            # algorithm will be tuned after feature selection
+            params["optuna_time_budget"] = None
+            params["optuna_init_params"] = {}
 
         unique_params_key = MljarTuner.get_params_key(params)
         if unique_params_key not in self._unique_params_keys:
             return [params]
         return None
 
     def get_features_selection_params(
         self, current_models, results_path, total_time_limit
     ):
-
         fname = os.path.join(results_path, "drop_features.json")
         if not os.path.exists(fname):
             return None
 
         drop_features = json.load(open(fname, "r"))
         print("Drop features", drop_features)
 
         # in case of droping only one feature (random_feature)
         # skip this step
         if len(drop_features) <= 1:
             return None
 
+        model_selection_time_limit = (
+            None if total_time_limit is None else 0.1 * total_time_limit
+        )
         df_models, algorithms = self.df_models_algorithms(
-            current_models, time_limit=0.1 * total_time_limit
+            current_models, time_limit=model_selection_time_limit
         )
 
         generated_params = []
         for m_type in algorithms:
             # try to do features selection only for below algorithms
             if m_type not in [
                 "Xgboost",
@@ -843,35 +1315,64 @@
 
                 params = copy.deepcopy(m.params)
                 params["preprocessing"]["drop_features"] = drop_features
                 params["name"] += "_SelectedFeatures"
                 params["status"] = "initialized"
                 params["final_loss"] = None
                 params["train_time"] = None
+                params["data_type"] = (
+                    params.get("data_type", "") + "_features_selection"
+                )
+                if self._optuna_time_budget is not None:
+                    params["optuna_time_budget"] = self._optuna_time_budget
+                    params["optuna_init_params"] = self._optuna_init_params
+                    params["optuna_verbose"] = self._optuna_verbose
+
                 if "model_architecture_json" in params["learner"]:
                     del params["learner"]["model_architecture_json"]
                 unique_params_key = MljarTuner.get_params_key(params)
                 if unique_params_key not in self._unique_params_keys:
                     generated_params += [params]
         return generated_params
 
     def _get_model_params(self, model_type, seed, params_type="random"):
         model_info = AlgorithmsRegistry.registry[self._ml_task][model_type]
 
         model_params = None
         if params_type == "default":
-
             model_params = model_info["default_params"]
             model_params["seed"] = seed
 
         else:
             model_params = RandomParameters.get(model_info["params"], seed + self._seed)
         if model_params is None:
             return None
 
+        # set eval metric
+        if model_info["class"].algorithm_short_name == "Xgboost":
+            model_params["eval_metric"] = xgboost_eval_metric(
+                self._ml_task, self._eval_metric
+            )
+        if model_info["class"].algorithm_short_name == "LightGBM":
+            metric, custom_metric = lightgbm_eval_metric(
+                self._ml_task, self._eval_metric
+            )
+            model_params["metric"] = metric
+            model_params["custom_eval_metric_name"] = custom_metric
+        if model_info["class"].algorithm_short_name == "CatBoost":
+            model_params["eval_metric"] = catboost_eval_metric(
+                self._ml_task, self._eval_metric
+            )
+        elif model_info["class"].algorithm_short_name in [
+            "Random Forest",
+            "Extra Trees",
+        ]:
+            model_params["eval_metric_name"] = self._eval_metric
+            model_params["ml_task"] = self._ml_task
+
         required_preprocessing = model_info["required_preprocessing"]
         model_additional = model_info["additional"]
         preprocessing_params = PreprocessingTuner.get(
             required_preprocessing, self._data_info, self._ml_task
         )
 
         model_params = {
@@ -880,22 +1381,29 @@
             "validation_strategy": self._validation_strategy,
             "learner": {
                 "model_type": model_info["class"].algorithm_short_name,
                 "ml_task": self._ml_task,
                 "n_jobs": self._n_jobs,
                 **model_params,
             },
+            "automl_random_state": self._seed,
         }
 
         if self._data_info.get("num_class") is not None:
             model_params["learner"]["num_class"] = self._data_info.get("num_class")
 
         model_params["ml_task"] = self._ml_task
         model_params["explain_level"] = self._explain_level
 
+        if self._fairness_metric is not None:
+            model_params["fairness_metric"] = self._fairness_metric
+            model_params["fairness_threshold"] = self._fairness_threshold
+            model_params["privileged_groups"] = self._privileged_groups
+            model_params["underprivileged_groups"] = self._underprivileged_groups
+
         return model_params
 
     @staticmethod
     def get_params_key(params):
         key = "key_"
         for main_key in ["preprocessing", "learner", "validation_strategy"]:
             key += "_" + main_key
@@ -907,17 +1415,19 @@
 
     def add_key(self, model):
         if model.get_type() != "Ensemble":
             key = MljarTuner.get_params_key(model.params)
             self._unique_params_keys += [key]
 
     def boost_params(self, current_models, results_path, total_time_limit):
-
+        model_selection_time_limit = (
+            None if total_time_limit is None else 0.1 * total_time_limit
+        )
         df_models, algorithms = self.df_models_algorithms(
-            current_models, time_limit=0.1 * total_time_limit
+            current_models, time_limit=model_selection_time_limit
         )
         best_model = None
         for i in range(df_models.shape[0]):
             if df_models["model_type"].iloc[i] in [
                 "Ensemble",
                 "Neural Network",
                 "Nearest Neighbors",
@@ -951,31 +1461,37 @@
 
         df_preds = df_preds.sort_values(by="res", ascending=True)
         df_preds["order"] = range(residua.shape[0])
         df_preds["order"] = (df_preds["order"]) / residua.shape[0] / 5.0 + 0.9
         df_preds = df_preds.sort_values(by="lp", ascending=True)
 
         sample_weight_path = os.path.join(
-            results_path, best_model.get_name() + "_sample_weight.parquet"
+            results_path, best_model.get_name() + "_sample_weight.data"
         )
-        pd.DataFrame({"sample_weight": df_preds["order"]}).to_parquet(
-            sample_weight_path, index=False
+        dump_data(
+            sample_weight_path, pd.DataFrame({"sample_weight": df_preds["order"]})
         )
 
         generated_params = []
 
         params = copy.deepcopy(best_model.params)
 
         params["validation_strategy"]["sample_weight_path"] = sample_weight_path
         params["injected_sample_weight"] = True
         params["name"] += "_BoostOnErrors"
         params["status"] = "initialized"
         params["final_loss"] = None
         params["train_time"] = None
+        params["data_type"] = "boost_on_error"
         if "model_architecture_json" in params["learner"]:
             del params["learner"]["model_architecture_json"]
+        if self._optuna_time_budget is not None:
+            params["optuna_time_budget"] = self._optuna_time_budget
+            params["optuna_init_params"] = self._optuna_init_params
+            params["optuna_verbose"] = self._optuna_verbose
+
         unique_params_key = MljarTuner.get_params_key(params)
 
         if unique_params_key not in self._unique_params_keys:
             generated_params += [params]
 
         return generated_params
```

### Comparing `mljar-supervised-0.9.1/supervised/tuner/preprocessing_tuner.py` & `mljar-supervised-1.0.0/supervised/tuner/preprocessing_tuner.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     @staticmethod
     def get(
         required_preprocessing,
         data_info,
         machinelearning_task,
         categorical_strategy=CATEGORICALS_ALL_INT,
     ):
-
         columns_preprocessing = {}
         columns_info = data_info["columns_info"]
 
         for col, preprocessing_needed in columns_info.items():
             preprocessing_to_apply = []
 
             # remove empty columns and columns with only one variable
@@ -54,15 +53,14 @@
             # convert to categorical only for categorical types
             convert_to_integer_will_be_applied = False
             if (
                 "convert_categorical"
                 in required_preprocessing  # the algorithm needs converted categoricals
                 and "categorical" in preprocessing_needed  # the feature is categorical
             ):
-
                 if categorical_strategy == PreprocessingTuner.CATEGORICALS_MIX:
                     if PreprocessingCategorical.MANY_CATEGORIES in preprocessing_needed:
                         preprocessing_to_apply += [
                             PreprocessingCategorical.CONVERT_INTEGER
                         ]
                         convert_to_integer_will_be_applied = True  # maybe scale needed
                     else:
```

### Comparing `mljar-supervised-0.9.1/supervised/tuner/random_parameters.py` & `mljar-supervised-1.0.0/supervised/tuner/random_parameters.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-0.9.1/supervised/tuner/hill_climbing.py` & `mljar-supervised-1.0.0/supervised/tuner/hill_climbing.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,28 +24,35 @@
             "num_class",
             "model_type",
             "seed",
             "ml_task",
             "explain_level",
             "model_architecture_json",
             "n_jobs",
+            "metric",
+            "eval_metric",
+            "custom_eval_metric_name",
+            "eval_metric_name",
         ]:
             if k in keys:
                 keys.remove(k)
 
         model_type = params["model_type"]
         if model_type == "Baseline":
             return [None, None]
         model_info = AlgorithmsRegistry.registry[ml_task][model_type]
         model_params = model_info["params"]
 
         permuted_keys = np.random.permutation(keys)
         key_to_update = None
         values = None
+
         for key_to_update in permuted_keys:
+            if key_to_update not in model_params:
+                continue
             values = model_params[key_to_update]
             if len(values) > 1:
                 break
         if values is None:
             return [None, None]
 
         left, right = None, None
```

### Comparing `mljar-supervised-0.9.1/supervised/base_automl.py` & `mljar-supervised-1.0.0/supervised/base_automl.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import os
+import gc
 import sys
 import json
 import copy
 import time
+import types
 import numpy as np
 import pandas as pd
 import logging
-import traceback
 import shutil
+import joblib
 from tabulate import tabulate
 from abc import ABC
 from copy import deepcopy
 
 from sklearn.base import BaseEstimator
 from sklearn.utils.validation import check_array
 from sklearn.metrics import r2_score, accuracy_score
@@ -31,24 +33,37 @@
 from supervised.preprocessing.exclude_missing_target import ExcludeRowsMissingTarget
 from supervised.tuner.data_info import DataInfo
 from supervised.tuner.mljar_tuner import MljarTuner
 from supervised.utils.config import mem
 from supervised.utils.config import LOG_LEVEL
 from supervised.utils.leaderboard_plots import LeaderboardPlots
 from supervised.utils.metric import Metric
-from supervised.preprocessing.eda import EDA
+from supervised.utils.metric import UserDefinedEvalMetric
+from supervised.utils.automl_plots import AutoMLPlots
+
+# disable EDA
+# from supervised.preprocessing.eda import EDA
 from supervised.preprocessing.preprocessing_utils import PreprocessingUtils
 from supervised.tuner.time_controller import TimeController
 from supervised.utils.data_validation import (
     check_positive_integer,
     check_greater_than_zero_integer,
     check_bool,
     check_greater_than_zero_integer_or_float,
     check_integer,
 )
+from supervised.utils.utils import dump_data, load_data
+import matplotlib.font_manager as font_manager
+
+# Get a list of all font families available on the system
+font_families = font_manager.findSystemFonts()
+
+# Load the font file for the first font family in the list and get the name of the first font family
+REPORT_FONT = font_manager.FontProperties(fname=font_families[0]).get_name()
+
 
 logger = logging.getLogger(__name__)
 logger.setLevel(LOG_LEVEL)
 
 
 class BaseAutoML(BaseEstimator, ABC):
     """
@@ -94,27 +109,34 @@
         # https://scikit-learn.org/stable/developers/develop.html#universal-attributes
         self.n_features_in_ = None  # for scikit-learn api
         self.tuner = None
         self._boost_on_errors = None
         self._kmeans_features = None
         self._mix_encoding = None
         self._max_single_prediction_time = None
+        self._optuna_time_budget = None
+        self._optuna_init_params = {}
+        self._fairness_metric = None
+        self._fairness_threshold = None
+        self._privileged_groups = []
+        self._underprivileged_groups = []
+        self._optuna_verbose = True
         self._n_jobs = -1
 
     def _get_tuner_params(
         self, start_random_models, hill_climbing_steps, top_models_to_improve
     ):
         return {
             "start_random_models": start_random_models,
             "hill_climbing_steps": hill_climbing_steps,
             "top_models_to_improve": top_models_to_improve,
         }
 
     def _check_can_load(self):
-        """ Checks if AutoML can be loaded from a folder"""
+        """Checks if AutoML can be loaded from a folder"""
         if self.results_path is not None:
             # Dir exists and can be loaded
             if os.path.exists(self.results_path) and os.path.exists(
                 os.path.join(self.results_path, "params.json")
             ):
                 self.load(self.results_path)
                 self._results_path = self.results_path
@@ -141,15 +163,15 @@
             self._validation_strategy = params.get(
                 "validation_strategy", self._validation_strategy
             )
             self._verbose = params.get("verbose", self._verbose)
             self._explain_level = params.get("explain_level", self._explain_level)
             self._golden_features = params.get("golden_features", self._golden_features)
             self._features_selection = params.get(
-                "features_selectiom", self._features_selection
+                "features_selection", self._features_selection
             )
             self._start_random_models = params.get(
                 "start_random_models", self._start_random_models
             )
             self._hill_climbing_steps = params.get(
                 "hill_climbing_steps", self._hill_climbing_steps
             )
@@ -162,37 +184,43 @@
             self._max_single_prediction_time = params.get(
                 "max_single_prediction_time", self._max_single_prediction_time
             )
             self._n_jobs = params.get("n_jobs", self._n_jobs)
             self._random_state = params.get("random_state", self._random_state)
             stacked_models = params.get("stacked")
 
+            best_model_name = params.get("best_model")
             load_on_predict = params.get("load_on_predict")
             self._fit_level = params.get("fit_level")
             lazy_load = not (
                 self._fit_level is not None and self._fit_level == "finished"
             )
             load_models = self._model_subpaths
             if load_on_predict is not None and self._fit_level == "finished":
                 load_models = load_on_predict
+                # just in case there is check for which models should be loaded
+                # fix https://github.com/mljar/mljar-supervised/issues/395
+                models_needed = self.models_needed_on_predict(best_model_name)
+                # join them and return unique list
+                load_models = list(np.unique(load_models + models_needed))
+
             models_map = {}
 
             for model_subpath in load_models:
                 if model_subpath.endswith("Ensemble") or model_subpath.endswith(
                     "Ensemble_Stacked"
                 ):
                     ens = Ensemble.load(path, model_subpath, models_map)
                     self._models += [ens]
                     models_map[ens.get_name()] = ens
                 else:
                     m = ModelFramework.load(path, model_subpath, lazy_load)
                     self._models += [m]
                     models_map[m.get_name()] = m
 
-            best_model_name = params.get("best_model")
             self._best_model = None
             if best_model_name is not None:
                 self._best_model = models_map.get(best_model_name)
 
             if stacked_models is not None and (
                 self._best_model._is_stacked or self._fit_level != "finished"
             ):
@@ -218,27 +246,44 @@
             "model_type": [],
             "metric_type": [],
             "metric_value": [],
             "train_time": [],
         }
         if self._max_single_prediction_time is not None:
             ldb["single_prediction_time"] = []
+
+        sensitive_features_names = []
+        if self._fairness_metric is not None and len(self._models):
+            sensitive_features_names = self._models[0].get_sensitive_features_names()
+            ldb["fairness_metric"] = []
+            for sf in sensitive_features_names:
+                ldb[f"fairness_{sf}"] = []
+            ldb["is_fair"] = []
+
         for m in self._models:
             # filter model with random feature
             if filter_random_feature and "RandomFeature" in m.get_name():
                 continue
             ldb["name"] += [m.get_name()]
             ldb["model_type"] += [m.get_type()]
             ldb["metric_type"] += [self._eval_metric]
             ldb["metric_value"] += [m.get_final_loss()]
             ldb["train_time"] += [np.round(m.get_train_time(), 2)]
             if self._max_single_prediction_time is not None:
-                ldb["single_prediction_time"] += [
-                    np.round(m._single_prediction_time, 4)
-                ]
+                if m._single_prediction_time is not None:
+                    ldb["single_prediction_time"] += [
+                        np.round(m._single_prediction_time, 4)
+                    ]
+                else:
+                    ldb["single_prediction_time"] += [None]
+            if self._fairness_metric is not None:
+                ldb["fairness_metric"] += [self._fairness_metric]
+                for sf in sensitive_features_names:
+                    ldb[f"fairness_{sf}"] += [m.get_fairness_metric(sf)]
+                ldb["is_fair"] += [m.is_fair()]
 
         ldb = pd.DataFrame(ldb)
         # need to add argument for sorting
         # minimize_direction = m.get_metric().get_minimize_direction()
         # ldb = ldb.sort_values("metric_value", ascending=minimize_direction)
 
         if original_metric_values:
@@ -297,15 +342,14 @@
             folds = self._validation_strategy.get("k_folds", 1)
             return repeats * folds
         except Exception as e:
             pass
         return 1
 
     def train_model(self, params):
-
         # do we have enough time to train?
         # if not, skip
         if not self._time_ctrl.enough_time(
             params["learner"]["model_type"], self._fit_level
         ):
             logger.info(f"Cannot train {params['name']} because of the time constraint")
             return False
@@ -349,43 +393,52 @@
 
         # start training
         logger.info(
             f"Train model #{len(self._models)+1} / Model name: {params['name']}"
         )
         mf.train(results_path, model_subpath)
 
+        # keep info about the model
+        self.keep_model(mf, model_subpath)
+
         # save the model
         mf.save(results_path, model_subpath)
 
-        # and keep info about the model
-        self.keep_model(mf, model_subpath)
         return True
 
     def verbose_print(self, msg):
         if self._verbose > 0:
             # self._progress_bar.write(msg)
             print(msg)
 
     def ensemble_step(self, is_stacked=False):
         if self._train_ensemble and len(self._models) > 1:
-
             ensemble_subpath = "Ensemble_Stacked" if is_stacked else "Ensemble"
             ensemble_path = os.path.join(self._results_path, ensemble_subpath)
             self.create_dir(ensemble_path)
 
             self.ensemble = Ensemble(
                 self._eval_metric,
                 self._ml_task,
                 is_stacked=is_stacked,
                 max_single_prediction_time=self._max_single_prediction_time,
-            )
-            oofs, target, sample_weight = self.ensemble.get_oof_matrix(self._models)
-            self.ensemble.fit(oofs, target, sample_weight)
-            self.ensemble.save(self._results_path, ensemble_subpath)
+                fairness_metric=self._fairness_metric,
+                fairness_threshold=self._fairness_threshold,
+                privileged_groups=self._privileged_groups,
+                underprivileged_groups=self._underprivileged_groups,
+            )
+            (
+                oofs,
+                target,
+                sample_weight,
+                sensitive_features,
+            ) = self.ensemble.get_oof_matrix(self._models)
+            self.ensemble.fit(oofs, target, sample_weight, sensitive_features)
             self.keep_model(self.ensemble, ensemble_subpath)
+            self.ensemble.save(self._results_path, ensemble_subpath)
             return True
         return False
 
     def can_we_stack_them(self, y):
         # if multiclass and too many classes then No
         return True
 
@@ -408,28 +461,29 @@
             cols = [f for f in oof.columns if "prediction" in f]
             oof = oof[cols]
             oof.columns = [f"{m.get_name()}_{c}" for c in cols]
             all_oofs += [oof]
 
         org_index = X.index.copy()
         X.reset_index(drop=True, inplace=True)
-        X_stacked = pd.concat(all_oofs + [X], axis=1)
+        X_stacked = pd.concat([X] + all_oofs, axis=1)
 
         X_stacked.index = org_index.copy()
         X.index = org_index.copy()
         return X_stacked
 
     def _perform_model_stacking(self):
-
         if self._stacked_models is not None:
             return
 
         ldb = self.get_leaderboard(filter_random_feature=True)
+        if self._fairness_metric is not None:
+            # get only fair models if we train with sensitive features
+            ldb = ldb[ldb["is_fair"]]
         ldb = ldb.sort_values(by="metric_value", ascending=True)
-
         models_map = {m.get_name(): m for m in self._models if not m._is_stacked}
         self._stacked_models = []
         models_limit = 10
 
         for model_type in np.unique(ldb.model_type):
             if model_type in ["Baseline"]:
                 continue
@@ -465,29 +519,36 @@
             # but for small data it can be less
             if time_left < self.get_stacking_minimum_time_needed():
                 return
         # too many classes and models
         if self._ml_task == MULTICLASS_CLASSIFICATION:
             if self.n_classes * len(self._models) > 1000:
                 return
+        # if we are training with sensitive features
+        # then we will stack only fair models
+        # if there are no fair models then we skip this step
+        if self._fairness_metric is not None:
+            if not [m for m in self._models if m.is_fair()]:
+                self.verbose_print("Skip stacking. We can stack only fair models.")
+                return
 
         self._perform_model_stacking()
 
-        X_stacked_path = os.path.join(self._results_path, "X_stacked.parquet")
+        X_stacked_path = os.path.join(self._results_path, "X_stacked.data")
         if os.path.exists(X_stacked_path):
             return
 
-        X = pd.read_parquet(self._X_path)
+        X = load_data(self._X_path)
         org_columns = X.columns.tolist()
         X_stacked = self.get_stacked_data(X)
         new_columns = X_stacked.columns.tolist()
         added_columns = [c for c in new_columns if c not in org_columns]
 
         # save stacked train data
-        X_stacked.to_parquet(X_stacked_path, index=False)
+        dump_data(X_stacked_path, X_stacked)
 
         """
         # resue old params
         for m in self._stacked_models:
             # print(m.get_type())
             # use only Xgboost, LightGBM and CatBoost as stacked models
             if m.get_type() not in ["Xgboost", "LightGBM", "CatBoost"]:
@@ -511,55 +572,71 @@
                 if scale is not None:
                     for col in added_columns:
                         params["preprocessing"]["columns_preprocessing"][col] = [
                             scale]
             self.train_model(params)
         """
 
-    def _save_data(self, X, y, sample_weight=None):
+    def _save_data(self, X, y, sample_weight=None, cv=None, sensitive_features=None):
         # save information about original data
-        self._save_data_info(X, y, sample_weight)
+        self._save_data_info(X, y, sample_weight, sensitive_features)
 
         # handle drastic imbalance
         # assure at least 20 samples of each class
         # for binary and multiclass classification
-        self._handle_drastic_imbalance(X, y, sample_weight)
+        self._handle_drastic_imbalance(X, y, sample_weight, sensitive_features)
 
         # prepare path for saving files
-        self._X_path = os.path.join(self._results_path, "X.parquet")
-        self._y_path = os.path.join(self._results_path, "y.parquet")
+        self._X_path = os.path.join(self._results_path, "X.data")
+        self._y_path = os.path.join(self._results_path, "y.data")
         self._sample_weight_path = None
         if sample_weight is not None:
             self._sample_weight_path = os.path.join(
-                self._results_path, "sample_weight.parquet"
+                self._results_path, "sample_weight.data"
+            )
+            dump_data(
+                self._sample_weight_path, pd.DataFrame({"sample_weight": sample_weight})
             )
-            pd.DataFrame({"sample_weight": sample_weight}).to_parquet(
-                self._sample_weight_path, index=False
+        self._sensitive_features_path = None
+        if sensitive_features is not None:
+            self._sensitive_features_path = os.path.join(
+                self._results_path, "sensitive_features.data"
             )
+            dump_data(self._sensitive_features_path, sensitive_features)
 
-        X.to_parquet(self._X_path, index=False)
+        dump_data(self._X_path, X)
 
         if self._ml_task == MULTICLASS_CLASSIFICATION:
             y = y.astype(str)
 
-        pd.DataFrame({"target": y}).to_parquet(self._y_path, index=False)
+        dump_data(self._y_path, pd.DataFrame({"target": y}))
 
         # set paths in validation parameters
         self._validation_strategy["X_path"] = self._X_path
         self._validation_strategy["y_path"] = self._y_path
         self._validation_strategy["results_path"] = self._results_path
         if sample_weight is not None:
             self._validation_strategy["sample_weight_path"] = self._sample_weight_path
+        if sensitive_features is not None:
+            self._validation_strategy[
+                "sensitive_features_path"
+            ] = self._sensitive_features_path
+
+        if cv is not None:
+            self._validation_strategy["cv_path"] = os.path.join(
+                self._results_path, "cv.data"
+            )
+            joblib.dump(cv, self._validation_strategy["cv_path"])
 
         if self._max_single_prediction_time is not None:
             self._one_sample = X.iloc[:1].copy(deep=True)
 
-        self._drop_data_variables(X)
-
-    def _handle_drastic_imbalance(self, X, y, sample_weight=None):
+    def _handle_drastic_imbalance(
+        self, X, y, sample_weight=None, sensitive_features=None
+    ):
         if self._ml_task == REGRESSION:
             return
         classes, cnts = np.unique(y, return_counts=True)
         min_samples_per_class = 20
         if self._validation_strategy is not None:
             min_samples_per_class = max(
                 min_samples_per_class, self._validation_strategy.get("k_folds", 0)
@@ -574,24 +651,33 @@
                 )
                 if sample_weight is not None:
                     new_sample_weight = (
                         sample_weight[y == classes[i]]
                         .sample(n=append_samples, replace=True, random_state=1)
                         .reset_index(drop=True)
                     )
+                if sensitive_features is not None:
+                    new_sensitive_features = (
+                        sensitive_features[y == classes[i]]
+                        .sample(n=append_samples, replace=True, random_state=1)
+                        .reset_index(drop=True)
+                    )
                 for j in range(new_X.shape[0]):
                     X.loc[X.shape[0]] = new_X.loc[j]
                     y.loc[y.shape[0]] = classes[i]
                     if sample_weight is not None:
                         sample_weight.loc[
                             sample_weight.shape[0]
                         ] = new_sample_weight.loc[j]
+                    if sensitive_features is not None:
+                        sensitive_features.loc[
+                            sensitive_features.shape[0]
+                        ] = new_sensitive_features.loc[j]
 
-    def _save_data_info(self, X, y, sample_weight=None):
-
+    def _save_data_info(self, X, y, sample_weight=None, sensitive_features=None):
         target_is_numeric = pd.api.types.is_numeric_dtype(y)
         if self._ml_task == MULTICLASS_CLASSIFICATION:
             y = y.astype(str)
 
         columns_and_target_info = DataInfo.compute(X, y, self._ml_task)
 
         self.n_features_in_ = X.shape[1]
@@ -602,38 +688,26 @@
             "rows": y.shape[0],
             "cols": X.shape[1],
             "target_is_numeric": target_is_numeric,
             "columns_info": columns_and_target_info["columns_info"],
             "target_info": columns_and_target_info["target_info"],
             "n_features": self.n_features_in_,
             "is_sample_weighted": sample_weight is not None,
+            "is_fairness_applied": sensitive_features is not None,
         }
         # Add n_classes if not regression
         if self._ml_task != REGRESSION:
             self._data_info["n_classes"] = self.n_classes
 
         if columns_and_target_info.get("num_class") is not None:
             self._data_info["num_class"] = columns_and_target_info["num_class"]
         data_info_path = os.path.join(self._results_path, "data_info.json")
         with open(data_info_path, "w") as fout:
             fout.write(json.dumps(self._data_info, indent=4))
 
-    def _drop_data_variables(self, X):
-
-        X.drop(X.columns, axis=1, inplace=True)
-
-    def _load_data_variables(self, X_train):
-        if X_train.shape[1] == 0:
-            X = pd.read_parquet(self._X_path)
-            for c in X.columns:
-                X_train.insert(loc=X_train.shape[1], column=c, value=X[c])
-
-        os.remove(self._X_path)
-        os.remove(self._y_path)
-
     def save_progress(self, step=None, generated_params=None):
         if step is not None and generated_params is not None:
             self._all_params[step] = generated_params
 
         state = {}
 
         state["fit_level"] = self._fit_level
@@ -664,15 +738,15 @@
         if self.n_features_in_ != n_features:
             raise ValueError(
                 f"Number of features of the model must match the input. Model n_features_in_ is {self.n_features_in_} and input n_features is {n_features}. Reshape your data."
             )
 
     # This method builds pandas.Dataframe from input. The input can be numpy.ndarray, matrix, or pandas.Dataframe
     # This method is used to build dataframes in `fit()` and in `predict`. That's the reason y can be None (`predict()` method)
-    def _build_dataframe(self, X, y=None, sample_weight=None):
+    def _build_dataframe(self, X, y=None, sample_weight=None, sensitive_features=None):
         if X is None or X.shape[0] == 0:
             raise AutoMLException("Empty input dataset")
         # If Inputs are not pandas dataframes use scikit-learn validation for X array
         if not isinstance(X, pd.DataFrame):
             # Validate X as array
             X = check_array(X, ensure_2d=False, force_all_finite=False)
             # Force X to be 2D
@@ -709,51 +783,77 @@
                 sample_weight = check_array(sample_weight, ensure_2d=False)
                 sample_weight = pd.Series(np.array(sample_weight), name="sample_weight")
             elif isinstance(sample_weight, pd.DataFrame):
                 sample_weight = np.array(sample_weight.iloc[:, 0])
                 sample_weight = check_array(sample_weight, ensure_2d=False)
                 sample_weight = pd.Series(np.array(sample_weight), name="sample_weight")
 
-        X, y, sample_weight = ExcludeRowsMissingTarget.transform(
-            X, y, sample_weight, warn=True
+        if sensitive_features is not None:
+            if isinstance(sensitive_features, np.ndarray):
+                sensitive_features = check_array(sensitive_features, ensure_2d=False)
+                sensitive_features = pd.DataFrame(
+                    sensitive_features,
+                    columns=[
+                        "sensitive_" + str(i)
+                        for i in range(1, len(sensitive_features[0]) + 1)
+                    ],
+                )
+            elif isinstance(sensitive_features, pd.Series):
+                sensitive_features = pd.DataFrame(sensitive_features)
+
+        X, y, sample_weight, sensitive_features = ExcludeRowsMissingTarget.transform(
+            X, y, sample_weight, sensitive_features, warn=True
         )
 
         X.reset_index(drop=True, inplace=True)
         y.reset_index(drop=True, inplace=True)
 
         if sample_weight is not None:
             sample_weight.reset_index(drop=True, inplace=True)
 
-        return X, y, sample_weight
+        if sensitive_features is not None:
+            sensitive_features.reset_index(drop=True, inplace=True)
 
-    def _apply_constraints(self):
+            for col in sensitive_features.columns:
+                if not sensitive_features[col].dtype.name in ["category", "object"]:
+                    self.verbose_print("Sensitive features should be categorical")
+                    self.verbose_print(
+                        f"Apply automatic binarization for feature {col}"
+                    )
+                    sensitive_features[col] = pd.DataFrame(
+                        pd.qcut(sensitive_features[col], q=2).astype(str)
+                    )
+                    self.verbose_print(
+                        f"New values {list(sensitive_features[col].unique())} for feature {col} are applied"
+                    )
+
+        return X, y, sample_weight, sensitive_features
 
+    def _apply_constraints(self):
         if "Neural Network" in self._algorithms and self._n_jobs != -1:
             self._algorithms.remove("Neural Network")
             self.verbose_print(
                 "Neural Network algorithm was disabled because it doesn't support n_jobs parameter."
             )
-        if "Linear" in self._algorithms and not (self.n_rows_in_ < 10000 and self.n_features_in_ < 1000):
+        if "Linear" in self._algorithms and not (
+            self.n_rows_in_ < 10000 and self.n_features_in_ < 1000
+        ):
             self._algorithms.remove("Linear")
-            self.verbose_print(
-                "Linear algorithm was disabled."
-            )
+            self.verbose_print("Linear algorithm was disabled.")
 
         # remove algorithms in the case of multiclass
         # and too many classes and columns
         if self._ml_task == MULTICLASS_CLASSIFICATION:
-
             if self.n_classes >= 10 and self.n_features_in_ * self.n_classes > 500:
                 if self.algorithms == "auto":
                     for a in ["CatBoost"]:
                         if a in self._algorithms:
                             self._algorithms.remove(a)
 
             if self.n_features_in_ * self.n_classes > 1000:
-
                 if self.algorithms == "auto":
                     for a in ["Xgboost", "CatBoost"]:
                         if a in self._algorithms:
                             self._algorithms.remove(a)
                 if self.validation_strategy == "auto":
                     self._validation_strategy = {
                         "validation_type": "split",
@@ -806,21 +906,26 @@
             self.verbose_print(f"Adjust validation. Remove: {self._model_subpaths[0]}")
             k_folds = 5
             if folds_cnt >= 15:
                 k_folds = 10
             # too small dataset for stacking
             if self.n_rows_in_ < 500:
                 self._stack_models = False
-                self.verbose_print("*** Disable stacking for small dataset (nrows < 500)")
+                self.verbose_print(
+                    "*** Disable stacking for small dataset (nrows < 500)"
+                )
 
             self._validation_strategy["validation_type"] = "kfold"
             del self._validation_strategy["train_ratio"]
             self._validation_strategy["k_folds"] = k_folds
             self.tuner._validation_strategy = self._validation_strategy
-            shutil.rmtree(self._model_subpaths[0], ignore_errors=True)
+            shutil.rmtree(
+                os.path.join(self._results_path, self._model_subpaths[0]),
+                ignore_errors=True,
+            )
             del self._models[0]
             del self._model_subpaths[0]
             del self.tuner._unique_params_keys[0]
             self._adjust_validation = False
             cv = []
             if self._validation_strategy.get("shuffle", False):
                 cv += ["Shuffle"]
@@ -833,15 +938,14 @@
             # cant stack models for train/test split
             self._stack_models = False
             self.verbose_print("Disable stacking for split validation")
 
         self._apply_constraints_stack_models()
 
     def _apply_constraints_stack_models(self):
-
         if self._validation_strategy["validation_type"] == "split":
             if self._stack_models:
                 self.verbose_print("Disable stacking for split validation")
             self._stack_models = False
             self._boost_on_errors = False
         if "repeats" in self._validation_strategy:
             if self._stack_models:
@@ -862,23 +966,25 @@
                 self._time_ctrl._steps.remove("stack")
             if (
                 "boost_on_errors" in self._time_ctrl._steps
                 and not self._boost_on_errors
             ):
                 self._time_ctrl._steps.remove("boost_on_errors")
 
-    def _fit(self, X, y, sample_weight=None):
+    def _fit(self, X, y, sample_weight=None, cv=None, sensitive_features=None):
         """Fits the AutoML model with data"""
         if self._fit_level == "finished":
             print(
                 "This model has already been fitted. You can use predict methods or select a new 'results_path' for a new a 'fit()'."
             )
             return
         # Validate input and build dataframes
-        X, y, sample_weight = self._build_dataframe(X, y, sample_weight)
+        X, y, sample_weight, sensitive_features = self._build_dataframe(
+            X, y, sample_weight, sensitive_features
+        )
 
         self.n_rows_in_ = X.shape[0]
         self.n_features_in_ = X.shape[1]
         self.n_classes = len(np.unique(y[~pd.isnull(y)]))
 
         # Get attributes (__init__ params)
         self._mode = self._get_mode()
@@ -898,83 +1004,122 @@
         self._start_random_models = self._get_start_random_models()
         self._hill_climbing_steps = self._get_hill_climbing_steps()
         self._top_models_to_improve = self._get_top_models_to_improve()
         self._boost_on_errors = self._get_boost_on_errors()
         self._kmeans_features = self._get_kmeans_features()
         self._mix_encoding = self._get_mix_encoding()
         self._max_single_prediction_time = self._get_max_single_prediction_time()
+        self._optuna_time_budget = self._get_optuna_time_budget()
+        self._optuna_init_params = self._get_optuna_init_params()
+        self._optuna_verbose = self._get_optuna_verbose()
         self._n_jobs = self._get_n_jobs()
         self._random_state = self._get_random_state()
 
+        if sensitive_features is not None:
+            self._fairness_metric = self._get_fairness_metric()
+            self._fairness_threshold = self._get_fairness_threshold()
+            self._privileged_groups = self._get_privileged_groups()
+            self._underprivileged_groups = self._get_underprivileged_groups()
+
         self._adjust_validation = False
         self._apply_constraints()
         if not self._adjust_validation:
             # if there is no validation adjustement
             # then we can apply stack_models constraints immediately
             # if there is validation adjustement
             # then we will apply contraints after the adjustement
             self._apply_constraints_stack_models()
 
         try:
-
             self.load_progress()
             if self._fit_level == "finished":
                 print(
                     "This model has already been fitted. You can use predict methods or select a new 'results_path' for a new 'fit()'."
                 )
                 return
             self._check_can_load()
 
             self.verbose_print(f"AutoML directory: {self._results_path}")
+            if self._mode == "Optuna":
+                ttl = int(len(self._algorithms) * self._optuna_time_budget)
+                self.verbose_print("Expected computing time:")
+                self.verbose_print(
+                    f"Time for tuning with Optuna: len(algorithms) * optuna_time_budget = {int(len(self._algorithms) * self._optuna_time_budget)} seconds"
+                )
+                self.verbose_print(
+                    f"There is no time limit for ML model training after Optuna tuning (total_time_limit parameter is ignored)."
+                )
+
             self.verbose_print(
                 f"The task is {self._ml_task} with evaluation metric {self._eval_metric}"
             )
             self.verbose_print(f"AutoML will use algorithms: {self._algorithms}")
             if self._stack_models:
                 self.verbose_print("AutoML will stack models")
             if self._train_ensemble:
-                self.verbose_print("AutoML will ensemble availabe models")
+                self.verbose_print("AutoML will ensemble available models")
 
             self._start_time = time.time()
             if self._time_ctrl is not None:
                 self._start_time -= self._time_ctrl.already_spend()
 
             # Automatic Exloratory Data Analysis
-            if self._explain_level == 2:
-                EDA.compute(X, y, os.path.join(self._results_path, "EDA"))
+            # I disabled EDA, because it won't be supported
+            # I recomend use pandas_profiling or Sweetviz
+            # if self._explain_level == 2:
+            #     EDA.compute(X, y, os.path.join(self._results_path, "EDA"))
 
             # Save data
-            self._save_data(X.copy(deep=False), y, sample_weight)
+
+            self._save_data(
+                X.copy(deep=False),
+                y.copy(deep=False),
+                None if sample_weight is None else sample_weight.copy(deep=False),
+                cv,
+                None
+                if sensitive_features is None
+                else sensitive_features.copy(deep=False),
+            )
 
             tuner = MljarTuner(
                 self._get_tuner_params(
                     self._start_random_models,
                     self._hill_climbing_steps,
                     self._top_models_to_improve,
                 ),
                 self._algorithms,
                 self._ml_task,
+                self._eval_metric,
                 self._validation_strategy,
                 self._explain_level,
                 self._data_info,
                 self._golden_features,
                 self._features_selection,
                 self._train_ensemble,
                 self._stack_models,
                 self._adjust_validation,
                 self._boost_on_errors,
                 self._kmeans_features,
                 self._mix_encoding,
+                self._optuna_time_budget,
+                self._optuna_init_params,
+                self._optuna_verbose,
                 self._n_jobs,
                 self._random_state,
+                self._fairness_metric,
+                self._fairness_threshold,
+                self._privileged_groups,
+                self._underprivileged_groups,
             )
             self.tuner = tuner
 
             steps = tuner.steps()
-            self.verbose_print(f"AutoML steps: {steps}")
+            self.verbose_print(
+                f'AutoML steps: {[s for s in steps if "update_" not in s]}'
+            )
             if self._time_ctrl is None:
                 self._time_ctrl = TimeController(
                     self._start_time,
                     self._total_time_limit,
                     self._model_time_limit,
                     steps,
                     self._algorithms,
@@ -1013,17 +1158,18 @@
                         self._models,
                         self._results_path,
                         self._stacked_models,
                         self._total_time_limit,
                     )
 
                 if generated_params is None or not generated_params:
-                    self.verbose_print(
-                        f"Skip {step} because no parameters were generated."
-                    )
+                    if "_update_" not in step:
+                        self.verbose_print(
+                            f"Skip {step} because no parameters were generated."
+                        )
                     continue
                 if generated_params:
                     if not self._time_ctrl.enough_time_for_step(self._fit_level):
                         self.verbose_print(f"Skip {step} because of the time limit.")
                         continue
                     else:
                         model_str = "models" if len(generated_params) > 1 else "model"
@@ -1057,14 +1203,16 @@
 
                     except NotTrainedException as e:
                         params["status"] = "error"
                         self.verbose_print(
                             params.get("name") + " not trained. " + str(e)
                         )
                     except Exception as e:
+                        import traceback
+
                         self._update_errors_report(
                             params.get("name"), str(e) + "\n" + traceback.format_exc()
                         )
                         params["status"] = "error"
 
                     self.save_progress(step, generated_params)
 
@@ -1075,24 +1223,41 @@
             self.select_and_save_best(show_warnings=True)
 
             self.verbose_print(
                 f"AutoML fit time: {np.round(time.time() - self._start_time,2)} seconds"
             )
             self.verbose_print(f"AutoML best model: {self._best_model.get_name()}")
 
+            if self._fairness_metric is not None:
+                # check if we have fair model
+                has_fair_model = False
+                for m in self._models:
+                    if m.is_fair():
+                        has_fair_model = True
+                        break
+                if not has_fair_model:
+                    self.verbose_print(
+                        "AutoML can't construct model that meets your fairness criteria."
+                    )
+                    self.verbose_print("What you can do?")
+                    self.verbose_print(
+                        "1. Please include more samples that are not biased."
+                    )
+                    self.verbose_print(
+                        "2. Please examine the most unfairly treated samples."
+                    )
+                    self.verbose_print("3. Please change fairness threshold.")
+
         except Exception as e:
             raise e
-        finally:
-            if self._X_path is not None:
-                self._load_data_variables(X)
 
         return self
 
     def _update_errors_report(self, model_name, error_msg):
-        """Append error message to errors.md file. """
+        """Append error message to errors.md file."""
         errors_filename = os.path.join(self._get_results_path(), "errors.md")
         with open(errors_filename, "a") as fout:
             self.verbose_print(f"There was an error during {model_name} training.")
             self.verbose_print(f"Please check {errors_filename} for details.")
             fout.write(f"## Error for {model_name}\n\n")
             fout.write(error_msg)
             link = "https://github.com/mljar/mljar-supervised/issues/new"
@@ -1100,25 +1265,56 @@
                 f"\n\nPlease set a GitHub issue with above error message at: {link}"
             )
             fout.write("\n\n")
 
     def select_and_save_best(self, show_warnings=False):
         # Select best model based on the lowest loss
         self._best_model = None
+
         if self._models:
-            model_list = [
-                m
-                for m in self._models
-                if m.is_valid() and m.is_fast_enough(self._max_single_prediction_time)
-            ]
-            if model_list:
-                self._best_model = min(
-                    model_list,
-                    key=lambda x: x.get_final_loss(),
-                )
+            if self._fairness_metric is not None:
+                models = [
+                    m
+                    for m in self._models
+                    if m.is_valid()
+                    # and m.is_fast_enough(self._max_single_prediction_time)
+                    and m.is_fair()
+                ]
+
+                if models:
+                    # if there are fair models, we select the one with best performance
+                    self._best_model = min(
+                        models,
+                        key=lambda x: x.get_final_loss(),
+                    )
+                else:
+                    # if no models are fair, we select the most fair model
+                    if "ratio" in self._fairness_metric.lower():
+                        self._best_model = max(
+                            [m for m in self._models if m.is_valid()],
+                            key=lambda x: x.get_best_fairness(),
+                        )
+                    else:
+                        self._best_model = min(
+                            [m for m in self._models if m.is_valid()],
+                            key=lambda x: x.get_best_fairness(),
+                        )
+
+            else:
+                model_list = [
+                    m
+                    for m in self._models
+                    if m.is_valid()
+                    and m.is_fast_enough(self._max_single_prediction_time)
+                ]
+                if model_list:
+                    self._best_model = min(
+                        model_list,
+                        key=lambda x: x.get_final_loss(),
+                    )
         # if none selected please select again and warn the user
         if (
             len(self._models)
             and self._best_model is None
             and self._max_single_prediction_time is not None
         ):
             if show_warnings:
@@ -1163,22 +1359,18 @@
                 "random_state": self._random_state,
                 "saved": self._model_subpaths,
                 "fit_level": self._fit_level,
             }
             if self._best_model is not None:
                 params["best_model"] = self._best_model.get_name()
                 load_on_predict = []
+                load_on_predict += self._best_model.involved_model_names()
                 if self._best_model._is_stacked and self._stacked_models is not None:
-                    load_on_predict += [m.get_name() for m in self._stacked_models]
-                if "Ensemble" in self._best_model.get_type():
-                    load_on_predict += [
-                        ens["model"].get_name()
-                        for ens in self._best_model.selected_models
-                    ]
-                load_on_predict += [self._best_model.get_name()]
+                    for m in self._stacked_models:
+                        load_on_predict += m.involved_model_names()
                 params["load_on_predict"] = list(np.unique(load_on_predict))
 
             if self._stacked_models is not None:
                 params["stacked"] = [m.get_name() for m in self._stacked_models]
             fout.write(json.dumps(params, indent=4))
 
         if self._models:
@@ -1191,18 +1383,72 @@
                 ldb.name == self._best_model.get_name(), "Best model"
             ] = "**the best**"
             ldb["name"] = [f"[{m}]({m}/README.md)" for m in ldb["name"].values]
 
             with open(os.path.join(self._results_path, "README.md"), "w") as fout:
                 fout.write(f"# AutoML Leaderboard\n\n")
                 fout.write(tabulate(ldb.values, ldb.columns, tablefmt="pipe"))
-                LeaderboardPlots.compute(ldb, self._results_path, fout)
+                LeaderboardPlots.compute(
+                    ldb, self._results_path, fout, self._fairness_threshold
+                )
 
-    def _base_predict(self, X, model=None):
+                if self._fit_level == "finished":
+                    AutoMLPlots.add(self._results_path, self._models, fout)
 
+    def get_ensemble_models(self, ensemble_name="Ensemble"):
+        try:
+            params = json.load(
+                open(os.path.join(self.results_path, ensemble_name, "ensemble.json"))
+            )
+            return [m["model"] for m in params["selected_models"]]
+        except Exception as e:
+            return []
+
+    def models_needed_on_predict(self, required_model_name):
+        params = json.load(open(os.path.join(self.results_path, "params.json")))
+        saved_models = params.get("saved", [])
+        stacked_models = params.get("stacked", [])
+
+        if required_model_name not in saved_models:
+            raise AutoMLException(
+                f"Can't load model {required_model_name}. Please check if the model's name is correct."
+            )
+        # single model needed
+        if (
+            "Stacked" not in required_model_name
+            and "Ensemble" not in required_model_name
+        ):
+            return [required_model_name]
+        ensemble_models = self.get_ensemble_models("Ensemble")
+        # ensemble of single models
+        if required_model_name == "Ensemble":
+            return ensemble_models + [required_model_name]
+        # single model on stacked data
+        if required_model_name != "Stacked_Ensemble":
+            return list(
+                np.unique(
+                    ensemble_models
+                    + ["Ensemble"]
+                    + stacked_models
+                    + [required_model_name]
+                )
+            )
+        # must be stacked ensemble
+        stacked_ensemble_models = self.get_ensemble_models("Stacked_Ensemble")
+        return list(
+            np.unique(
+                ensemble_models
+                + ["Ensemble"]
+                + stacked_models
+                + stacked_ensemble_models
+                + [required_model_name]
+            )
+        )
+
+    def _base_predict(self, X, model=None):
         if model is None:
             if self._best_model is None:
                 self.load(self.results_path)
             model = self._best_model
 
         if model is None:
             raise AutoMLException(
@@ -1255,24 +1501,23 @@
                 {True: pos_label, False: neg_label}
             )
             return predictions
         elif self._ml_task == MULTICLASS_CLASSIFICATION:
             target_is_numeric = self._data_info.get("target_is_numeric", False)
             if target_is_numeric:
                 try:
-                    predictions["label"] = predictions["label"].astype(np.int32)
+                    predictions["label"] = predictions["label"].astype(int)
                 except Exception as e:
-                    predictions["label"] = predictions["label"].astype(np.float)
+                    predictions["label"] = predictions["label"].astype(float)
             return predictions
         # Regression
         else:
             return predictions
 
     def _predict(self, X):
-
         predictions = self._base_predict(X)
         # Return predictions
         # If classification task the result is in column 'label'
         # If regression task the result is in column 'prediction'
         return (
             predictions["label"].to_numpy()
             if self._ml_task != REGRESSION
@@ -1306,20 +1551,20 @@
         return (
             r2_score(y, predictions, sample_weight=sample_weight)
             if self._ml_task == REGRESSION
             else accuracy_score(y, predictions, sample_weight=sample_weight)
         )
 
     def _get_mode(self):
-        """ Gets the current mode"""
+        """Gets the current mode"""
         self._validate_mode()
         return deepcopy(self.mode)
 
     def _get_ml_task(self):
-        """ Gets the current ml_task. If "auto" it is determined"""
+        """Gets the current ml_task. If "auto" it is determined"""
         self._validate_ml_task()
         if self.ml_task == "auto":
             classes_number = self.n_classes
             if classes_number == 2:
                 self._estimator_type = "classifier"  # for sk-learn api
                 return BINARY_CLASSIFICATION
             elif classes_number <= 20:
@@ -1328,15 +1573,15 @@
             else:
                 self._estimator_type = "regressor"  # for sk-learn api
                 return REGRESSION
         else:
             return deepcopy(self.ml_task)
 
     def _get_results_path(self):
-        """ Gets the current results_path"""
+        """Gets the current results_path"""
         # if we already have the results path set, please return it
         if self._results_path is not None:
             return self._results_path
 
         self._validate_results_path()
 
         path = self.results_path
@@ -1368,25 +1613,28 @@
             raise AutoMLException(
                 f"Cannot set directory for AutoML. Directory '{path}' is not empty."
             )
 
         raise AutoMLException("Cannot set directory for AutoML results")
 
     def _get_total_time_limit(self):
-        """ Gets the current total_time_limit"""
+        """Gets the current total_time_limit"""
         self._validate_total_time_limit()
+        if self._get_mode() == "Optuna":
+            return None  # there no training limit for model in the Optuna mode
+            # just train and be happy with super models :)
         return deepcopy(self.total_time_limit)
 
     def _get_model_time_limit(self):
-        """ Gets the current model_time_limit"""
+        """Gets the current model_time_limit"""
         self._validate_model_time_limit()
         return deepcopy(self.model_time_limit)
 
     def _get_algorithms(self):
-        """ Gets the current algorithms. If "auto" it is determined"""
+        """Gets the current algorithms. If "auto" it is determined"""
         self._validate_algorithms()
         if self.algorithms == "auto":
             if self._get_mode() == "Explain":
                 return [
                     "Baseline",
                     "Linear",
                     "Decision Tree",
@@ -1411,45 +1659,61 @@
                     "Extra Trees",
                     "LightGBM",
                     "Xgboost",
                     "CatBoost",
                     "Neural Network",
                     "Nearest Neighbors",
                 ]
+            if self._get_mode() == "Optuna":
+                return [
+                    "Random Forest",
+                    "Extra Trees",
+                    "LightGBM",
+                    "Xgboost",
+                    "CatBoost",
+                    "Neural Network",
+                ]
         else:
             return deepcopy(self.algorithms)
 
     def _get_train_ensemble(self):
-        """ Gets the current train_ensemble"""
+        """Gets the current train_ensemble"""
         self._validate_train_ensemble()
         return deepcopy(self.train_ensemble)
 
     def _get_stack_models(self):
-        """ Gets the current stack_models"""
+        """Gets the current stack_models"""
         self._validate_stack_models()
         if self.stack_models == "auto":
-            return True if self.mode == "Compete" else False
+            val = self._get_validation_strategy()
+            if val.get("validation_type", "") == "custom":
+                return False
+            return True if self.mode in ["Compete", "Optuna"] else False
         else:
             return deepcopy(self.stack_models)
 
     def _get_eval_metric(self):
-        """ Gets the current eval_metric"""
+        """Gets the current eval_metric"""
         self._validate_eval_metric()
+        if isinstance(self.eval_metric, types.FunctionType):
+            UserDefinedEvalMetric().set_metric(self.eval_metric)
+            return "user_defined_metric"
+
         if self.eval_metric == "auto":
             if self._get_ml_task() == BINARY_CLASSIFICATION:
                 return "logloss"
             elif self._get_ml_task() == MULTICLASS_CLASSIFICATION:
                 return "logloss"
             elif self._get_ml_task() == REGRESSION:
                 return "rmse"
         else:
             return deepcopy(self.eval_metric)
 
     def _get_validation_strategy(self):
-        """ Gets the current validation_strategy"""
+        """Gets the current validation_strategy"""
         strat = {}
         self._validate_validation_strategy()
         if self.validation_strategy == "auto":
             if self._get_mode() == "Explain":
                 strat = {
                     "validation_type": "split",
                     "train_ratio": 0.75,
@@ -1459,15 +1723,15 @@
             elif self._get_mode() == "Perform":
                 strat = {
                     "validation_type": "kfold",
                     "k_folds": 5,
                     "shuffle": True,
                     "stratify": True,
                 }
-            elif self._get_mode() == "Compete":
+            elif self._get_mode() in ["Compete", "Optuna"]:
                 strat = {
                     "validation_type": "kfold",
                     "k_folds": 10,
                     "shuffle": True,
                     "stratify": True,
                 }
             if self._get_ml_task() == REGRESSION:
@@ -1485,246 +1749,307 @@
 
     def _get_verbose(self):
         """Gets the current verbose"""
         self._validate_verbose()
         return deepcopy(self.verbose)
 
     def _get_explain_level(self):
-        """ Gets the current explain_level"""
+        """Gets the current explain_level"""
         self._validate_explain_level()
         if self.explain_level == "auto":
             if self._get_mode() == "Explain":
                 return 2
             if self._get_mode() == "Perform":
                 return 1
             if self._get_mode() == "Compete":
                 return 0
+            if self._get_mode() == "Optuna":
+                return 0
         else:
             return deepcopy(self.explain_level)
 
     def _get_golden_features(self):
         self._validate_golden_features()
         if self.golden_features == "auto":
             if self._get_mode() == "Explain":
                 return False
             if self._get_mode() == "Perform":
                 return True
             if self._get_mode() == "Compete":
                 return True
+            if self._get_mode() == "Optuna":
+                return False
         else:
             return deepcopy(self.golden_features)
 
     def _get_features_selection(self):
-        """ Gets the current features_selection"""
+        """Gets the current features_selection"""
         self._validate_features_selection()
         if self.features_selection == "auto":
             if self._get_mode() == "Explain":
                 return False
             if self._get_mode() == "Perform":
                 return True
             if self._get_mode() == "Compete":
                 return True
+            if self._get_mode() == "Optuna":
+                return False
         else:
             return deepcopy(self.features_selection)
 
     def _get_start_random_models(self):
-        """ Gets the current start_random_models"""
+        """Gets the current start_random_models"""
         self._validate_start_random_models()
         if self.start_random_models == "auto":
             if self._get_mode() == "Explain":
                 return 1
             if self._get_mode() == "Perform":
                 return 5
             if self._get_mode() == "Compete":
                 return 10
+            if self._get_mode() == "Optuna":
+                return 1  # just 1, because it will be tuned by Optuna
         else:
             return deepcopy(self.start_random_models)
 
     def _get_hill_climbing_steps(self):
-        """ Gets the current hill_climbing_steps"""
+        """Gets the current hill_climbing_steps"""
         self._validate_hill_climbing_steps()
         if self.hill_climbing_steps == "auto":
             if self._get_mode() == "Explain":
                 return 0
             if self._get_mode() == "Perform":
                 return 2
             if self._get_mode() == "Compete":
                 return 2
+            if self._get_mode() == "Optuna":
+                return 0  # all tuning is done in Optuna
         else:
             return deepcopy(self.hill_climbing_steps)
 
     def _get_top_models_to_improve(self):
-        """ Gets the current top_models_to_improve"""
+        """Gets the current top_models_to_improve"""
         self._validate_top_models_to_improve()
         if self.top_models_to_improve == "auto":
             if self._get_mode() == "Explain":
                 return 0
             if self._get_mode() == "Perform":
                 return 2
             if self._get_mode() == "Compete":
                 return 3
+            if self._get_mode() == "Optuna":
+                return 0
         else:
             return deepcopy(self.top_models_to_improve)
 
     def _get_boost_on_errors(self):
-        """ Gets the current boost_on_errors"""
+        """Gets the current boost_on_errors"""
         self._validate_boost_on_errors()
         if self.boost_on_errors == "auto":
+            val = self._get_validation_strategy()
+            if val.get("validation_type", "") == "custom":
+                return False
             if self._get_mode() == "Explain":
                 return False
             if self._get_mode() == "Perform":
                 return False
             if self._get_mode() == "Compete":
                 return True
+            if self._get_mode() == "Optuna":
+                return False
         else:
             return deepcopy(self.boost_on_errors)
 
     def _get_kmeans_features(self):
-        """ Gets the current kmeans_features"""
+        """Gets the current kmeans_features"""
         self._validate_kmeans_features()
         if self.kmeans_features == "auto":
             if self._get_mode() == "Explain":
                 return False
             if self._get_mode() == "Perform":
                 return False
             if self._get_mode() == "Compete":
                 return True
+            if self._get_mode() == "Optuna":
+                return False
         else:
             return deepcopy(self.kmeans_features)
 
     def _get_mix_encoding(self):
-        """ Gets the current mix_encoding"""
+        """Gets the current mix_encoding"""
         self._validate_mix_encoding()
         if self.mix_encoding == "auto":
             if self._get_mode() == "Explain":
                 return False
             if self._get_mode() == "Perform":
                 return False
             if self._get_mode() == "Compete":
                 return True
+            if self._get_mode() == "Optuna":
+                return False
         else:
             return deepcopy(self.mix_encoding)
 
     def _get_max_single_prediction_time(self):
-        """ Gets the current max_single_prediction_time"""
+        """Gets the current max_single_prediction_time"""
         self._validate_max_single_prediction_time()
         if self.max_single_prediction_time is None:
             if self._get_mode() == "Perform":
                 return 0.5  # prediction time should be under 0.5 second
             return None
         else:
             return deepcopy(self.max_single_prediction_time)
 
+    def _get_optuna_time_budget(self):
+        """Gets the current optuna_time_budget"""
+        self._validate_optuna_time_budget()
+
+        if self.optuna_time_budget is None:
+            if self._get_mode() == "Optuna":
+                return 3600
+            return None
+        else:
+            if self._get_mode() != "Optuna":
+                # use only for mode Optuna
+                return None
+            return deepcopy(self.optuna_time_budget)
+
+    def _get_optuna_init_params(self):
+        """Gets the current optuna_init_params"""
+        self._validate_optuna_init_params()
+        if self._get_mode() != "Optuna":
+            # use only for mode Optuna
+            return {}
+        return deepcopy(self.optuna_init_params)
+
+    def _get_optuna_verbose(self):
+        """Gets the current optuna_verbose"""
+        self._validate_optuna_verbose()
+        # use only for mode Optuna
+        if self._get_mode() != "Optuna":
+            return True
+        return deepcopy(self.optuna_verbose)
+
     def _get_n_jobs(self):
-        """ Gets the current n_jobs"""
+        """Gets the current n_jobs"""
         self._validate_n_jobs()
         return deepcopy(self.n_jobs)
 
     def _get_random_state(self):
-        """ Gets the current random_state"""
+        """Gets the current random_state"""
         self._validate_random_state()
         return deepcopy(self.random_state)
 
     def _validate_mode(self):
-        """ Validates mode parameter"""
-        valid_modes = ["Explain", "Perform", "Compete"]
+        """Validates mode parameter"""
+        valid_modes = ["Explain", "Perform", "Compete", "Optuna"]
         if self.mode not in valid_modes:
             raise ValueError(
                 f"Expected 'mode' to be {' or '.join(valid_modes)}, got '{self.mode}'"
             )
 
     def _validate_ml_task(self):
-        """ Validates ml_task parameter"""
+        """Validates ml_task parameter"""
         if isinstance(self.ml_task, str) and self.ml_task == "auto":
             return
 
         if self.ml_task not in AlgorithmsRegistry.get_supported_ml_tasks():
             raise ValueError(
                 f"Expected 'ml_task' to be {' or '.join(AlgorithmsRegistry.get_supported_ml_tasks())}, got '{self.ml_task}''"
             )
 
     def _validate_results_path(self):
-        """ Validates path parameter"""
+        """Validates path parameter"""
         if self.results_path is None or isinstance(self.results_path, str):
             return
 
         raise ValueError(
             f"Expected 'results_path' to be of type string, got '{type(self.results_path)}''"
         )
 
     def _validate_total_time_limit(self):
-        """ Validates total_time_limit parameter"""
-        check_greater_than_zero_integer(self.total_time_limit, "total_time_limit")
+        """Validates total_time_limit parameter"""
+        if self.total_time_limit is None:
+            return
+        if self.total_time_limit is not None:
+            check_greater_than_zero_integer(self.total_time_limit, "total_time_limit")
 
     def _validate_model_time_limit(self):
-        """ Validates model_time_limit parameter"""
+        """Validates model_time_limit parameter"""
         if self.model_time_limit is not None:
             check_greater_than_zero_integer(self.model_time_limit, "model_time_limit")
 
     def _validate_algorithms(self):
-        """ Validates algorithms parameter"""
+        """Validates algorithms parameter"""
         if isinstance(self.algorithms, str) and self.algorithms == "auto":
             return
 
         for algo in self.algorithms:
             if algo not in list(AlgorithmsRegistry.registry[self._ml_task].keys()):
                 raise ValueError(
                     f"The algorithm {algo} is not allowed to use for ML task: {self._ml_task}. Allowed algorithms: {list(AlgorithmsRegistry.registry[self._ml_task].keys())}"
                 )
 
     def _validate_train_ensemble(self):
-        """ Validates train_ensemble parameter"""
+        """Validates train_ensemble parameter"""
         # `train_ensemble` defaults to True, no further checking required
         check_bool(self.train_ensemble, "train_ensemble")
 
     def _validate_stack_models(self):
-        """ Validates stack_models parameter"""
+        """Validates stack_models parameter"""
         # `stack_models` defaults to "auto". If "auto" return, else check if is valid bool
         if isinstance(self.stack_models, str) and self.stack_models == "auto":
             return
 
         check_bool(self.stack_models, "stack_models")
 
     def _validate_eval_metric(self):
-        """ Validates eval_metric parameter"""
-        # `stack_models` defaults to "auto". If not "auto", check if is valid bool
+        """Validates eval_metric parameter"""
+        if isinstance(self.eval_metric, types.FunctionType):
+            return
+
         if isinstance(self.eval_metric, str) and self.eval_metric == "auto":
             return
 
         if (self._get_ml_task() == BINARY_CLASSIFICATION) and self.eval_metric not in [
             "logloss",
             "auc",
+            "f1",
+            "average_precision",
+            "accuracy",
         ]:
             raise ValueError(
                 f"Metric {self.eval_metric} is not allowed in ML task: {self._get_ml_task()}. \
-                    Use 'logloss'"
+                    Use 'logloss', 'auc', 'f1', 'average_precision', or 'accuracy'"
             )
 
         elif (
             self._get_ml_task() == MULTICLASS_CLASSIFICATION
-        ) and self.eval_metric != "logloss":
+        ) and self.eval_metric not in ["logloss", "f1", "accuracy"]:
             raise ValueError(
                 f"Metric {self.eval_metric} is not allowed in ML task: {self._get_ml_task()}. \
-                    Use 'logloss'"
+                    Use 'logloss', 'f1', or 'accuracy'"
             )
 
         elif self._get_ml_task() == REGRESSION and self.eval_metric not in [
             "rmse",
             "mse",
             "mae",
             "r2",
             "mape",
+            "spearman",
+            "pearson",
         ]:
             raise ValueError(
                 f"Metric {self.eval_metric} is not allowed in ML task: {self._get_ml_task()}. \
-                Use 'rmse'"
+                Use 'rmse', 'mse', 'mae', 'r2', 'mape', 'spearman', or 'pearson'"
             )
 
     def _validate_validation_strategy(self):
-        """ Validates validation parameter"""
+        """Validates validation parameter"""
         if (
             isinstance(self.validation_strategy, str)
             and self.validation_strategy == "auto"
         ):
             return
 
         # only validation_type is mandatory
@@ -1735,263 +2060,460 @@
             raise ValueError(
                 f"Expected 'validation_strategy' to be a dict, got '{type(self.validation_strategy)}'"
             )
         if not all(key in self.validation_strategy for key in required_keys):
             raise ValueError(f"Expected dict with keys: {' , '.join(required_keys)}")
 
     def _validate_verbose(self):
-        """ Validates verbose parameter"""
+        """Validates verbose parameter"""
         check_positive_integer(self.verbose, "verbose")
 
     def _validate_explain_level(self):
-        """ Validates explain_level parameter"""
+        """Validates explain_level parameter"""
         if isinstance(self.explain_level, str) and self.explain_level == "auto":
             return
         valid_explain_levels = [0, 1, 2]
         # Check if explain level is 0 or greater integer
         if not (
             isinstance(self.explain_level, int)
             and self.explain_level in valid_explain_levels
         ):
             raise ValueError(
                 f"Expected 'explain_level' to be {' or '.join([str(x) for x in valid_explain_levels])}, got '{self.explain_level}'"
             )
 
     def _validate_golden_features(self):
-        """ Validates golden_features parameter"""
+        """Validates golden_features parameter"""
         if isinstance(self.golden_features, str) and self.golden_features == "auto":
             return
+        if isinstance(self.golden_features, int):
+            return
         check_bool(self.golden_features, "golden_features")
 
     def _validate_features_selection(self):
-        """ Validates features_selection parameter"""
+        """Validates features_selection parameter"""
         if (
             isinstance(self.features_selection, str)
             and self.features_selection == "auto"
         ):
             return
         check_bool(self.features_selection, "features_selection")
 
     def _validate_start_random_models(self):
-        """ Validates start_random_models parameter"""
+        """Validates start_random_models parameter"""
         if (
             isinstance(self.start_random_models, str)
             and self.start_random_models == "auto"
         ):
             return
         check_greater_than_zero_integer(self.start_random_models, "start_random_models")
 
     def _validate_hill_climbing_steps(self):
-        """ Validates hill_climbing_steps parameter"""
+        """Validates hill_climbing_steps parameter"""
         if (
             isinstance(self.hill_climbing_steps, str)
             and self.hill_climbing_steps == "auto"
         ):
             return
         check_positive_integer(self.hill_climbing_steps, "hill_climbing_steps")
 
     def _validate_top_models_to_improve(self):
-        """ Validates top_models_to_improve parameter"""
+        """Validates top_models_to_improve parameter"""
         if (
             isinstance(self.top_models_to_improve, str)
             and self.top_models_to_improve == "auto"
         ):
             return
         check_positive_integer(self.top_models_to_improve, "top_models_to_improve")
 
     def _validate_boost_on_errors(self):
-        """ Validates boost_on_errors parameter"""
+        """Validates boost_on_errors parameter"""
         if isinstance(self.boost_on_errors, str) and self.boost_on_errors == "auto":
             return
         check_bool(self.boost_on_errors, "boost_on_errors")
 
     def _validate_kmeans_features(self):
-        """ Validates kmeans_features parameter"""
+        """Validates kmeans_features parameter"""
         if isinstance(self.kmeans_features, str) and self.kmeans_features == "auto":
             return
         check_bool(self.kmeans_features, "kmeans_features")
 
     def _validate_mix_encoding(self):
-        """ Validates mix_encoding parameter"""
+        """Validates mix_encoding parameter"""
         if isinstance(self.mix_encoding, str) and self.mix_encoding == "auto":
             return
         check_bool(self.mix_encoding, "mix_encoding")
 
     def _validate_max_single_prediction_time(self):
-        """ Validates max_single_prediction_time parameter"""
+        """Validates max_single_prediction_time parameter"""
         if self.max_single_prediction_time is None:
             return
         check_greater_than_zero_integer_or_float(
             self.max_single_prediction_time, "max_single_prediction_time"
         )
 
+    def _validate_optuna_time_budget(self):
+        """Validates optuna_time_budget parameter"""
+        if self.optuna_time_budget is None:
+            return
+        check_greater_than_zero_integer(self.optuna_time_budget, "optuna_time_budget")
+
+    def _validate_optuna_init_params(self):
+        """Validates optuna_init_params parameter"""
+        if self.optuna_init_params is None:
+            return
+        if type(self.optuna_init_params) is not dict:
+            raise ValueError(
+                f"Expected 'optuna_init_params' to be a dict, got '{type(self.optuna_init_params)}'"
+            )
+
+    def _validate_optuna_verbose(self):
+        """Validates optuna_verbose parameter"""
+        if self.optuna_verbose is None:
+            return
+        check_bool(self.optuna_verbose, "optuna_verbose")
+
     def _validate_n_jobs(self):
-        """ Validates mix_encoding parameter"""
+        """Validates mix_encoding parameter"""
         check_integer(self.n_jobs, "n_jobs")
 
     def _validate_random_state(self):
-        """ Validates random_state parameter"""
+        """Validates random_state parameter"""
         check_positive_integer(self.random_state, "random_state")
 
+    def _validate_fairness_metric(self):
+        """Validates fariness_metric parameter"""
+        if isinstance(self.fairness_metric, str) and self.fairness_metric == "auto":
+            return
+
+        if (
+            self._get_ml_task() in [BINARY_CLASSIFICATION, MULTICLASS_CLASSIFICATION]
+        ) and self.fairness_metric not in [
+            "demographic_parity_difference",
+            "demographic_parity_ratio",
+            "equalized_odds_difference",
+            "equalized_odds_ratio",
+        ]:
+            raise ValueError(
+                f"Metric {self.fairness_metric} is not allowed in ML task: {self._get_ml_task()}. \
+                    Use `demographic_parity_difference`, `demographic_parity_ratio`, `equalized_odds_difference` or `equalized_odds_ratio`"
+            )
+        if (self._get_ml_task() == REGRESSION) and self.fairness_metric not in [
+            "group_loss_difference",
+            "group_loss_ratio",
+        ]:
+            raise ValueError(
+                f"Metric {self.fairness_metric} is not allowed in ML task: {self._get_ml_task()}. \
+                    Use `group_loss`"
+            )
+
+    def _get_fairness_metric(self):
+        """Gets the fairness metric"""
+        self._validate_fairness_metric()
+        if self.fairness_metric == "auto":
+            if self._get_ml_task() == BINARY_CLASSIFICATION:
+                return "demographic_parity_ratio"
+            if self._get_ml_task() == REGRESSION:
+                return "group_loss_ratio"
+            if self._get_ml_task() == MULTICLASS_CLASSIFICATION:
+                return "demographic_parity_ratio"
+        else:
+            return deepcopy(self.fairness_metric)
+
+    def _get_fairness_threshold(self):
+        """Gets the fairness threshold"""
+        if self.fairness_threshold == "auto":
+            if self._get_ml_task() in [
+                BINARY_CLASSIFICATION,
+                MULTICLASS_CLASSIFICATION,
+            ]:
+                thresholds = {
+                    "demographic_parity_difference": 0.1,
+                    "demographic_parity_ratio": 0.8,
+                    "equalized_odds_difference": 0.1,
+                    "equalized_odds_ratio": 0.8,
+                }
+                return thresholds.get(self._fairness_metric, 0.8)
+            elif self._get_ml_task() == REGRESSION:
+                thresholds = {
+                    "group_loss_ratio": 0.8,
+                }
+                if self._fairness_metric == "group_loss_difference":
+                    raise AutoMLException(
+                        "We can't set default fairness threshold value. Please set `fairness_threshold` value in AutoML constructor."
+                    )
+                return thresholds.get(self._fairness_metric, 0.8)
+        else:
+            return deepcopy(self.fairness_threshold)
+
+    def _get_privileged_groups(self):
+        """Gets privileged groups for fair training"""
+        if self.privileged_groups == "auto":
+            return []
+        else:
+            return deepcopy(self.privileged_groups)
+
+    def _get_underprivileged_groups(self):
+        """Gets underprivileged groups for fair training"""
+        if self.underprivileged_groups == "auto":
+            return []
+        else:
+            return deepcopy(self.underprivileged_groups)
+
     def to_json(self):
         if self._best_model is None:
             return None
 
         return {
             "best_model": self._best_model.to_json(),
             "threshold": self._threshold,
             "ml_task": self._ml_task,
         }
 
     def from_json(self, json_data):
-
         if json_data["best_model"]["algorithm_short_name"] == "Ensemble":
             self._best_model = Ensemble()
             self._best_model.from_json(json_data["best_model"])
         else:
             self._best_model = ModelFramework(json_data["best_model"].get("params"))
             self._best_model.from_json(json_data["best_model"])
         self._threshold = json_data.get("threshold")
 
         self._ml_task = json_data.get("ml_task")
 
-    def _md_to_html(self, md_fname, page_type):
-        import markdown
-
-        if not os.path.exists(md_fname):
-            return None
-        content = ""
-        with open(md_fname) as fin:
-            content = fin.read()
-
-        content = content.replace("README.md", "README.html")
-        content_html = markdown.markdown(
-            content, extensions=["markdown.extensions.tables"]
-        )
-        content_html = content_html.replace("<img ", '<img style="width:80%" ')
-        content_html = content_html.replace("<table>", '<table class="styled-table">')
-        content_html = content_html.replace("<tr>", '<tr style="text-align: right;">')
-
-        styles = '<link rel="stylesheet" href="style.css">\n\n'
-        if page_type == "sub":
-            styles = '<link rel="stylesheet" href="../style.css">\n\n'
-        beginning = styles
-
-        if page_type == "main":
-            beginning += """<img src="https://raw.githubusercontent.com/mljar/visual-identity/main/media/mljar_AutomatedML.png" style="height:128px; margin-left: auto;
-margin-right: auto;display: block;"/>\n\n"""
-            if os.path.exists(os.path.join(self._results_path, "EDA")):
-                beginning += '<a href="EDA/README.html">Automatic Exploratory Data Analysis Report</a>'
-
-        content_html = beginning + content_html
-
-        html_fname = md_fname.replace("README.md", "README.html")
-        with open(html_fname, "w") as fout:
-            fout.write(content_html)
-
-        return html_fname
-
-    def _report(self, width=900, height=1200):
-
-        from IPython.display import IFrame
-
-        main_readme_html = os.path.join(self._results_path, "README.html")
-        if not os.path.exists(main_readme_html) or 1:
-            fname = os.path.join(self._results_path, "README.md")
-            main_readme_html = self._md_to_html(fname, "main")
-            for f in os.listdir(self._results_path):
-                fname = os.path.join(self._results_path, f, "README.md")
-                if os.path.exists(fname):
-                    self._md_to_html(fname, "sub")
-            with open(os.path.join(self._results_path, "style.css"), "w") as fout:
-                fout.write(
-                    """
-.styled-table {
+    report_style = f"""
+.styled-table {{
     border-collapse: collapse;
     font-size: 0.9em;
     font-family:Courier New;
-}
+}}
 
-.styled-table td, .styled-table th {
+.styled-table td, .styled-table th {{
     border: 1px solid #ddd;
     padding: 8px;
-}
+{{
 
-.styled-table tr:nth-child(even){background-color: #f2f2f2;}
+.styled-table tr:nth-child(even){{background-color: #f2f2f2;}}
 
-.styled-table tr:hover {background-color: #e0ecf5;}
+.styled-table tr:hover {{background-color: #e0ecf5;}}
 
-.styled-table th {
+.styled-table thead {{
     padding-top: 6px;
     padding-bottom: 6px;
     text-align: left;
     background-color: #0099cc;
     color: white;
-}
+}}
 
-body {
-    font-family: Arial;
+body {{
+    font-family: {REPORT_FONT};
+    font-size: 1.0em;
     background-color: rgba(236, 243, 249, 0.15);
-}
+}}
 
-h1 {
+h1 {{
     color: #004666;
     border-bottom: 1px solid rgba(0,70,102,0.3)
-}
-h2 {
+}}
+h2 {{
     color: #004666;
     padding-bottom: 5px;
     margin-bottom: 0px;
-}
+}}
 
-ul {
+ul {{
     margin-top: 0px;
-}
+}}
 
-p {
+p {{
     margin-top: 5px;
-}
+}}
 
-h3 {
+h3 {{
     color: #004666;
     padding-bottom: 5px;
     margin-bottom: 0px;
-}
+}}
+a {{
+    font-weight: bold;
+    color: #004666;
+}}
+
+a:hover {{
+    cursor: pointer;
+    color: #0099CC;
+}}
+
 
 """
+
+    def _md_to_html(self, md_fname, page_type, dir_path, me=None):
+        import markdown
+        import base64
+
+        if not os.path.exists(md_fname):
+            return None
+        content = ""
+        with open(md_fname) as fin:
+            content = fin.read()
+
+        content = content.replace("README.md", "README.html")
+        content_html = markdown.markdown(
+            content, extensions=["markdown.extensions.tables"]
+        )
+        content_html = content_html.replace("<img ", '<img style="width:750px" ')
+        content_html = content_html.replace("<table>", '<table class="styled-table">')
+        content_html = content_html.replace("<tr>", '<tr style="text-align: right;">')
+
+        # replace png figures to base64
+        for f in os.listdir(dir_path):
+            if ".png" in f:
+                encoded_string = ""
+                with open(os.path.join(dir_path, f), "rb") as image_file:
+                    encoded_string = base64.b64encode(image_file.read())
+                    encoded_string = encoded_string.decode("utf-8")
+                encoded_figure = f"data:image/png;base64, {encoded_string}"
+                content_html = content_html.replace(f, encoded_figure)
+
+        # insert svg figures
+        for f in os.listdir(dir_path):
+            if ".svg" in f:
+                with open(os.path.join(dir_path, f), "rb") as image_file:
+                    svg_plot = image_file.read()
+                    svg_plot = svg_plot.decode("utf-8")
+
+                arr = content_html.split("\n")
+                new_content = []
+                for i in arr:
+                    if f in i:
+                        new_content += [f"<p>{svg_plot}</p>"]
+                    else:
+                        new_content += [i]
+                content_html = "\n".join(new_content)
+
+        # change links
+        if page_type == "main":
+            for f in os.listdir(dir_path):
+                if os.path.exists(os.path.join(dir_path, f, "README.md")):
+                    old = f'href="{f}/README.html"'
+                    new = f"onclick=\"toggleShow('{f}');toggleShow('main')\" "
+                    content_html = content_html.replace(old, new)
+
+        # other links
+        if me is not None:
+            old = 'href="../README.html"'
+            new = f"onclick=\"toggleShow('{me}');toggleShow('main')\" "
+            content_html = content_html.replace(old, new)
+
+        beginning = ""
+
+        if page_type == "main":
+            beginning += """<img src="https://raw.githubusercontent.com/mljar/visual-identity/main/media/mljar_AutomatedML.png" style="height:128px; margin-left: auto;
+margin-right: auto;display: block;"/>\n\n"""
+            # disable EDA
+            # if os.path.exists(os.path.join(self._results_path, "EDA")):
+            #     beginning += "<a onclick=\"toggleShow('EDA');toggleShow('main')\" >Automatic Exploratory Data Analysis Report</a>"
+            if os.path.exists(os.path.join(self._results_path, "optuna/README.md")):
+                beginning += "<h2><a onclick=\"toggleShow('optuna');toggleShow('main')\" >&#187; Optuna Params Tuning Report</a></h2>"
+
+        content_html = beginning + content_html
+
+        return content_html
+
+    def _show_report(self, main_readme_html, width=900, height=1200):
+        from IPython.display import HTML, IFrame
+
+        if os.environ.get("KAGGLE_KERNEL_RUN_TYPE") is None:
+            with open(main_readme_html) as fin:
+                return HTML(fin.read())
+        else:
+            return IFrame(main_readme_html, width=width, height=height)
+
+    def _report(self, width=900, height=1200):
+        self._results_path = self._get_results_path()
+        main_readme_html = os.path.join(self._results_path, "README.html")
+
+        if os.path.exists(main_readme_html):
+            return self._show_report(main_readme_html, width, height)
+
+        body = ""
+        fname = os.path.join(self._results_path, "README.md")
+        body += (
+            '<div id="main">\n'
+            + self._md_to_html(fname, "main", self._results_path)
+            + "\n\n</div>\n\n"
+        )
+
+        for f in os.listdir(self._results_path):
+            fname = os.path.join(self._results_path, f, "README.md")
+            if os.path.exists(fname):
+                body += (
+                    f'<div id="{f}" style="display: none">\n'
+                    + self._md_to_html(
+                        fname, "sub", os.path.join(self._results_path, f), f
+                    )
+                    + "\n\n</div>\n\n"
                 )
 
-        if main_readme_html is not None:
-            return IFrame(main_readme_html, width, height)
+        body += """
+    <script>
+        function toggleShow(elementId) {
+            var x = document.getElementById(elementId);
+            if (x.style.display === "none") {
+                x.style.display = "block";
+            } else {
+                x.style.display = "none";
+            }
+        }
+    </script>
+        """
 
+        report_content = f"""
+<!DOCTYPE html>
+<html>
+<head>
+    <style>
+    {self.report_style}
+    </style>
+</head>
+<body>
+    {body}
+</body>
+</html>
+"""
+        with open(main_readme_html, "w") as fout:
+            fout.write(report_content)
+
+        return self._show_report(main_readme_html, width, height)
 
     def _need_retrain(self, X, y, sample_weight, decrease):
-        
         metric = self._best_model.get_metric()
 
-        X, y, sample_weight = ExcludeRowsMissingTarget.transform(
+        X, y, sample_weight, _ = ExcludeRowsMissingTarget.transform(
             X, y, sample_weight, warn=True
         )
 
         if self._ml_task == BINARY_CLASSIFICATION:
-            prediction = self._predict_proba(X)[:,1]
+            prediction = self._predict_proba(X)[:, 1]
         if self._ml_task == MULTICLASS_CLASSIFICATION:
             prediction = self._predict_proba(X)
         else:
             prediction = self._predict(X)
 
         sign = -1.0 if Metric.optimize_negative(metric.name) else 1.0
 
-        
         new_score = metric(y, prediction, sample_weight)
         old_score = self._best_model.get_final_loss()
 
         change = np.abs((old_score - new_score) / old_score)
 
-        # always minimize the score 
+        # always minimize the score
         if new_score > old_score:
-            self.verbose_print(f"Model performance decreased by {np.round(change*100.0,2)}%")
+            self.verbose_print(
+                f"Model performance decreased by {np.round(change*100.0,2)}%"
+            )
             return change > decrease
         else:
-            self.verbose_print(f"Model performance increased by {np.round(change*100.0,2)}%")
-            return False    
-        
+            self.verbose_print(
+                f"Model performance increased by {np.round(change*100.0,2)}%"
+            )
+            return False
```

### Comparing `mljar-supervised-0.9.1/supervised/callbacks/max_iters_constraint.py` & `mljar-supervised-1.0.0/supervised/callbacks/max_iters_constraint.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-0.9.1/supervised/callbacks/callback_list.py` & `mljar-supervised-1.0.0/supervised/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-0.9.1/supervised/callbacks/terminate_on_nan.py` & `mljar-supervised-1.0.0/supervised/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-0.9.1/supervised/callbacks/learner_time_constraint.py` & `mljar-supervised-1.0.0/supervised/callbacks/learner_time_constraint.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-0.9.1/supervised/callbacks/early_stopping.py` & `mljar-supervised-1.0.0/supervised/callbacks/early_stopping.py`

 * *Files 9% similar despite different names*

```diff
@@ -108,15 +108,14 @@
         self.loss_values[self.learner.uid]["train"] += [train_loss]
         self.loss_values[self.learner.uid]["validation"] += [validation_loss]
         self.loss_values[self.learner.uid]["iters"] += [logs.get("iter_cnt")]
 
         if self.metric.improvement(
             previous=self.best_loss[self.learner.uid], current=validation_loss
         ):
-
             y_validation_true = predictions.get("y_validation_true")
             self.no_improvement_cnt = 0
             self.best_iter[self.learner.uid] = logs.get("iter_cnt")
             self.best_loss[self.learner.uid] = validation_loss
 
             if len(y_validation_true.shape) == 1 or y_validation_true.shape[1] == 1:
                 self.best_y_predicted[self.learner.uid] = pd.DataFrame(
@@ -138,15 +137,16 @@
                 self.multiple_target = True
                 self.target_columns = y_validation_true.columns
 
             y_validation_predicted = predictions.get("y_validation_predicted")
 
             if len(y_validation_predicted.shape) == 1:
                 # only one prediction column (binary classification or regression)
-                self.best_y_predicted[self.learner.uid]["prediction"] = np.array(
+                col = predictions.get("validation_columns", "prediction")
+                self.best_y_predicted[self.learner.uid][col] = np.array(
                     y_validation_predicted
                 )
             else:
                 # several columns in multiclass classification
                 cols = predictions.get("validation_columns")
                 for i_col in range(y_validation_predicted.shape[1]):
                     self.best_y_predicted[self.learner.uid][
@@ -156,14 +156,24 @@
 
             # store sample_weight
             sample_weight_validation = predictions.get("sample_weight_validation")
             if sample_weight_validation is not None:
                 self.best_y_predicted[self.learner.uid]["sample_weight"] = np.array(
                     sample_weight_validation
                 )
+            # store sensitive features
+            sensitive_features_validation = predictions.get(
+                "sensitive_features_validation"
+            )
+
+            if sensitive_features_validation is not None:
+                for col in list(sensitive_features_validation.columns):
+                    self.best_y_predicted[self.learner.uid][
+                        f"sensitive_{col}"
+                    ] = np.array(sensitive_features_validation[col])
 
             self.best_models[self.learner.uid] = self.learner.copy()
             # if local copy is not available, save model and keep path
             if self.best_models[self.learner.uid] is None:
                 self.best_model_paths[self.learner.uid] = self.learner.save()
         else:
             self.no_improvement_cnt += 1
```

### Comparing `mljar-supervised-0.9.1/supervised/callbacks/total_time_constraint.py` & `mljar-supervised-1.0.0/supervised/callbacks/total_time_constraint.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
                 # then the training will be stopped after first fold (above condition)
                 raise NotTrainedException(
                     "Force to stop the training. "
                     "Total time for AutoML training already exceeded."
                 )
 
     def on_iteration_end(self, logs, predictions):
-
         total_elapsed_time = np.round(time.time() - self.total_time_start, 2)
 
         if self.total_time_limit is not None:
             log.debug(
                 f"Total elapsed time {total_elapsed_time} seconds. "
                 + f"Time left {np.round(self.total_time_limit - total_elapsed_time, 2)} seconds."
             )
```

### Comparing `mljar-supervised-0.9.1/supervised/callbacks/callback.py` & `mljar-supervised-1.0.0/supervised/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `mljar-supervised-0.9.1/supervised/callbacks/metric_logger.py` & `mljar-supervised-1.0.0/supervised/callbacks/metric_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         for metric in self.metrics:
             self.loss_values[learner.uid]["train"][metric.name] = []
             self.loss_values[learner.uid]["validation"][metric.name] = []
 
         self.current_learner_uid = learner.uid
 
     def on_iteration_end(self, logs, predictions):
-
         for metric in self.metrics:
             train_loss = 0
             if predictions.get("y_train_predicted") is not None:
                 train_loss = metric(
                     predictions.get("y_train_true"),
                     predictions.get("y_train_predicted"),
                 )
```

### Comparing `mljar-supervised-0.9.1/supervised/validation/validation_step.py` & `mljar-supervised-1.0.0/supervised/validation/validation_step.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 import logging
 
 log = logging.getLogger(__name__)
 
 from supervised.validation.validator_kfold import KFoldValidator
 from supervised.validation.validator_split import SplitValidator
-from supervised.validation.validator_with_dataset import WithDatasetValidator
+from supervised.validation.validator_custom import CustomValidator
 
 from supervised.exceptions import AutoMLException
 
 
 class ValidationStep:
     def __init__(self, params):
-
         # kfold is default validation technique
         self.validation_type = params.get("validation_type", "kfold")
 
         if self.validation_type == "kfold":
             self.validator = KFoldValidator(params)
         elif self.validation_type == "split":
             self.validator = SplitValidator(params)
+        elif self.validation_type == "custom":
+            self.validator = CustomValidator(params)
         else:
             raise AutoMLException(
                 f"The validation type ({self.validation_type}) is not implemented."
             )
-        """
-        
-        elif self.validation_type == "with_dataset":
-            self.validator = WithDatasetValidator(params, data)
-        else:
-            msg = "Unknown validation type: {0}".format(self.validation_type)
-            raise ValidationStepException(msg)
-        """
 
     def get_split(self, k, repeat=0):
         return self.validator.get_split(k, repeat)
 
     def split(self):
         return self.validator.split()
```

### Comparing `mljar-supervised-0.9.1/supervised/validation/validator_kfold.py` & `mljar-supervised-1.0.0/supervised/validation/validator_kfold.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 log = logging.getLogger(__name__)
 
 from sklearn.model_selection import StratifiedKFold
 from sklearn.model_selection import KFold
 
 from supervised.validation.validator_base import BaseValidator
 from supervised.exceptions import AutoMLException
-
+from supervised.utils.utils import load_data
 from supervised.utils.config import mem
 import time
 
 
 class KFoldValidator(BaseValidator):
     def __init__(self, params):
         BaseValidator.__init__(self, params)
@@ -61,26 +61,25 @@
                     )
                 ]
 
         self._results_path = self.params.get("results_path")
         self._X_path = self.params.get("X_path")
         self._y_path = self.params.get("y_path")
         self._sample_weight_path = self.params.get("sample_weight_path")
+        self._sensitive_features_path = self.params.get("sensitive_features_path")
 
         if self._X_path is None or self._y_path is None:
             raise AutoMLException("No data path set in KFoldValidator params")
 
         folds_path = os.path.join(self._results_path, "folds")
 
         if not os.path.exists(folds_path):
-
             os.mkdir(folds_path)
-
-            X = pd.read_parquet(self._X_path)
-            y = pd.read_parquet(self._y_path)
+            X = load_data(self._X_path)
+            y = load_data(self._y_path)
             y = y["target"]
 
             if isinstance(y[0], bytes):
                 # see https://github.com/scikit-learn/scikit-learn/issues/16980
                 y = y.astype(str)
 
             for repeat_cnt, skf in enumerate(self.skf):
@@ -97,51 +96,59 @@
                         self._results_path,
                         "folds",
                         f"fold_{fold_cnt}{repeat_str}_validation_indices.npy",
                     )
 
                     np.save(train_index_file, train_index)
                     np.save(validation_index_file, validation_index)
-
             del X
             del y
             gc.collect()
 
         else:
             log.debug("Folds split already done, reuse it")
 
     def get_split(self, k, repeat=0):
-
         repeat_str = f"_repeat_{repeat}" if self.repeats > 1 else ""
 
         train_index_file = os.path.join(
             self._results_path, "folds", f"fold_{k}{repeat_str}_train_indices.npy"
         )
         validation_index_file = os.path.join(
             self._results_path, "folds", f"fold_{k}{repeat_str}_validation_indices.npy"
         )
 
         train_index = np.load(train_index_file)
         validation_index = np.load(validation_index_file)
 
-        X = pd.read_parquet(self._X_path)
-        y = pd.read_parquet(self._y_path)
+        X = load_data(self._X_path)
+        y = load_data(self._y_path)
         y = y["target"]
 
         sample_weight = None
         if self._sample_weight_path is not None:
-            sample_weight = pd.read_parquet(self._sample_weight_path)
+            sample_weight = load_data(self._sample_weight_path)
             sample_weight = sample_weight["sample_weight"]
 
+        sensitive_features = None
+        if self._sensitive_features_path is not None:
+            sensitive_features = load_data(self._sensitive_features_path)
+
         train_data = {"X": X.loc[train_index], "y": y.loc[train_index]}
         validation_data = {"X": X.loc[validation_index], "y": y.loc[validation_index]}
         if sample_weight is not None:
             train_data["sample_weight"] = sample_weight.loc[train_index]
             validation_data["sample_weight"] = sample_weight.loc[validation_index]
 
+        if sensitive_features is not None:
+            train_data["sensitive_features"] = sensitive_features.loc[train_index]
+            validation_data["sensitive_features"] = sensitive_features.loc[
+                validation_index
+            ]
+
         return (train_data, validation_data)
 
     def get_n_splits(self):
         return self.k_folds
 
     def get_repeats(self):
         return self.repeats
```

### Comparing `mljar-supervised-0.9.1/supervised/model_framework.py` & `mljar-supervised-1.0.0/supervised/model_framework.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import pandas as pd
 import time
 import zipfile
 import os
 import copy
 import logging
 import json
+import gc
+import sys
 
 from supervised.callbacks.callback_list import CallbackList
 from supervised.validation.validation_step import ValidationStep
 from supervised.algorithms.factory import AlgorithmFactory
 from supervised.preprocessing.preprocessing import Preprocessing
 from supervised.preprocessing.exclude_missing_target import ExcludeRowsMissingTarget
 from supervised.algorithms.registry import AlgorithmsRegistry
@@ -27,14 +29,19 @@
 
 logger = logging.getLogger(__name__)
 logger.setLevel(LOG_LEVEL)
 
 from supervised.utils.config import mem
 from supervised.utils.learning_curves import LearningCurves
 
+import optuna
+import joblib
+
+from supervised.tuner.optuna.tuner import OptunaTuner
+
 
 class ModelFramework:
     def __init__(self, params, callbacks=[]):
         logger.debug("ModelFramework.__init__")
         self.uid = str(uuid.uuid4())
 
         for i in ["learner", "validation_strategy"]:  # mandatory parameters
@@ -65,28 +72,43 @@
         self.metric_name = None
         self.oof_predictions = None
         self._additional_metrics = None
         self._threshold = None  # used only for binary classifiers
         self._max_time_for_learner = params.get("max_time_for_learner", 3600)
         self._oof_predictions_fname = None
         self._single_prediction_time = None  # prediction time on single sample
+        self._optuna_time_budget = params.get("optuna_time_budget")
+        self._optuna_init_params = params.get("optuna_init_params", {})
+        self._optuna_verbose = params.get("optuna_verbose", True)
+
+        self._fairness_metric = params.get("fairness_metric")
+        self._fairness_threshold = params.get("fairness_threshold")
+        self._privileged_groups = params.get("privileged_groups", [])
+        self._underprivileged_groups = params.get("underprivileged_groups", [])
+        self._fairness_optimization = params.get("fairness_optimization")
+        self._is_fair = None
+
+        # the automl random state from AutoML constructor, used in Optuna optimizer
+        self._automl_random_state = params.get("automl_random_state", 42)
 
     def get_train_time(self):
         return self.train_time
 
     def predictions(
         self,
         learner,
         preproces,
         X_train,
         y_train,
         sample_weight,
+        sensitive_features,
         X_validation,
         y_validation,
         sample_weight_validation,
+        sensitive_features_validation,
     ):
         y_train_true = y_train
         y_train_predicted = learner.predict(X_train)
         y_validation_true = y_validation
         y_validation_predicted = learner.predict(X_validation)
 
         y_train_true = preproces.inverse_scale_target(y_train_true)
@@ -98,32 +120,58 @@
         if self._ml_task == MULTICLASS_CLASSIFICATION:
             # y_train_true = preproces.inverse_categorical_target(y_train_true)
             # y_validation_true = preproces.inverse_categorical_target(y_validation_true)
             # get columns, omit the last one (it is label)
             y_validation_columns = preproces.prepare_target_labels(
                 y_validation_predicted
             ).columns.tolist()[:-1]
+        elif self._ml_task == BINARY_CLASSIFICATION:
+            class_names = self.preprocessings[-1].get_target_class_names()
+            y_validation_columns = "prediction"
+            if not ("0" in class_names and "1" in class_names):
+                y_validation_columns = (
+                    f"prediction_0_for_{class_names[0]}_1_for_{class_names[1]}"
+                )
+        else:
+            y_validation_columns = "prediction"
 
         return {
             "y_train_true": y_train_true,
             "y_train_predicted": y_train_predicted,
             "sample_weight": sample_weight,
+            "sensitive_features": sensitive_features,
             "y_validation_true": y_validation_true,
             "y_validation_predicted": y_validation_predicted,
             "sample_weight_validation": sample_weight_validation,
+            "sensitive_features_validation": sensitive_features_validation,
             "validation_index": X_validation.index,
             "validation_columns": y_validation_columns,
         }
 
     def train(self, results_path, model_subpath):
         logger.debug(f"ModelFramework.train {self.learner_params.get('model_type')}")
 
         start_time = time.time()
         np.random.seed(self.learner_params["seed"])
 
+        optuna_tuner = None
+        if self._optuna_time_budget is not None and OptunaTuner.is_optimizable(
+            self.learner_params.get("model_type", "")
+        ):
+            optuna_tuner = OptunaTuner(
+                results_path,
+                ml_task=self._ml_task,
+                eval_metric=self.get_metric(),
+                time_budget=self._optuna_time_budget,
+                init_params=self._optuna_init_params,
+                verbose=self._optuna_verbose,
+                n_jobs=self.learner_params.get("n_jobs", -1),
+                random_state=self._automl_random_state,
+            )
+
         self.validation = ValidationStep(self.validation_params)
 
         repeats = self.validation.get_repeats()
         for repeat in range(repeats):
             for k_fold in range(self.validation.get_n_splits()):
                 train_data, validation_data = self.validation.get_split(k_fold, repeat)
                 logger.debug(
@@ -155,14 +203,41 @@
                     sample_weight_validation,
                 ) = self.preprocessings[-1].transform(
                     validation_data["X"],
                     validation_data["y"],
                     validation_data.get("sample_weight"),
                 )
 
+                # skip preprocessing for sensitive features
+                # TODO: need to add sensitive features in preprocessing because some rows might be skipped (missing target)
+                # then we need to skip some rows in sensitive features as well
+                # TODO: drop rows if there is missing data in sensitive feature?
+
+                # get sensitive features from data split
+                sensitive_features = train_data.get("sensitive_features")
+                sensitive_features_validation = validation_data.get(
+                    "sensitive_features"
+                )
+
+                if optuna_tuner is not None:
+                    optuna_start_time = time.time()
+                    self.learner_params = optuna_tuner.optimize(
+                        self.learner_params.get("model_type", ""),
+                        self.params.get("data_type", ""),
+                        X_train,
+                        y_train,
+                        sample_weight,
+                        X_validation,
+                        y_validation,
+                        sample_weight_validation,
+                        self.learner_params,
+                    )
+                    # exclude optuna optimize time from model training
+                    start_time += time.time() - optuna_start_time
+
                 self.learner_params["explain_level"] = self._explain_level
                 self.learners += [
                     AlgorithmFactory.get_algorithm(copy.deepcopy(self.learner_params))
                 ]
                 learner = self.learners[-1]
                 learner.set_learner_name(k_fold, repeat, repeats)
 
@@ -170,15 +245,14 @@
                 self.callbacks.on_learner_train_start()
 
                 log_to_file = os.path.join(
                     results_path, model_subpath, f"{learner.name}_training.log"
                 )
 
                 for i in range(learner.max_iters):
-
                     self.callbacks.on_iteration_start()
 
                     learner.fit(
                         X_train,
                         y_train,
                         sample_weight,
                         X_validation,
@@ -197,17 +271,19 @@
                         {"iter_cnt": i},
                         self.predictions(
                             learner,
                             self.preprocessings[-1],
                             X_train,
                             y_train,
                             sample_weight,
+                            sensitive_features,
                             X_validation,
                             y_validation,
                             sample_weight_validation,
+                            sensitive_features_validation,
                         ),
                     )
 
                     if learner.stop_training:
                         break
                     learner.update({"step": i})
 
@@ -231,14 +307,36 @@
                 # save learner and free the memory
                 p = os.path.join(model_path, learner.get_fname())
                 learner.save(p)
                 del learner.model
                 learner.model = None
                 # end of learner training
 
+                # clear data
+                del X_train
+                del y_train
+                del X_validation
+                del y_validation
+
+                if sample_weight is not None:
+                    del sample_weight
+                    del train_data["sample_weight"]
+                if sample_weight_validation is not None:
+                    del sample_weight_validation
+                    del validation_data["sample_weight"]
+
+                del train_data["X"]
+                del train_data["y"]
+                del validation_data["X"]
+                del validation_data["y"]
+                del train_data
+                del validation_data
+
+                gc.collect()
+
         # end of validation loop
         self.callbacks.on_framework_train_end()
         # self.get_additional_metrics()
         self._additional_metrics = self.get_additional_metrics()
 
         self.train_time = time.time() - start_time
         logger.debug("ModelFramework end of training")
@@ -274,15 +372,15 @@
 
         early_stopping = self.callbacks.get("early_stopping")
         if early_stopping is None:
             return None
         self.oof_predictions = early_stopping.best_y_oof
 
         ###############################################################
-        # in case of Neural Network and one-hot coded multiclass target
+        # in case of one-hot coded multiclass target
         target_cols = [
             c for c in self.oof_predictions.columns.tolist() if "target" in c
         ]
         if len(target_cols) > 1:
             target = self.oof_predictions[target_cols[0]].copy()
             target.name = "target"
             for i, t in enumerate(target_cols):
@@ -312,17 +410,27 @@
 
     def get_type(self):
         return self.learner_params.get("model_type")
 
     def get_name(self):
         return self._name
 
+    def involved_model_names(self):
+        """Returns the list of all models involved in the current model.
+        For single model, it returns the list with the name of the model.
+        For ensemble model, it returns the list with the name of the ensemble and all internal models
+        (used to build ensemble).
+        For single model but trained on stacked data, it returns the list with the name of the model
+        (names of models used in stacking are not included)."""
+        return [self._name]
+
     def is_valid(self):
         """is_valid is used in Ensemble to check if it has more than 1 model in it.
-        If Ensemble has only 1 model in it, then Ensemble shouldn't be used as best model"""
+        If Ensemble has only 1 model in it, then Ensemble shouldn't be used as best model
+        """
         return True
 
     def is_fast_enough(self, max_single_prediction_time):
         # dont need to check
         if max_single_prediction_time is None:
             return True
 
@@ -352,44 +460,144 @@
         y_predicted_final = self.preprocessings[0].prepare_target_labels(
             y_predicted_average
         )
 
         return y_predicted_final
 
     def get_additional_metrics(self):
-
         if self._additional_metrics is None:
             # 'target' - the target after processing used for model training
             # 'prediction' - out of folds predictions of the model
             oof_predictions = self.get_out_of_folds()
             prediction_cols = [c for c in oof_predictions.columns if "prediction" in c]
             target_cols = [c for c in oof_predictions.columns if "target" in c]
 
             target = oof_predictions[target_cols]
 
             oof_preds = None
             if self._ml_task == MULTICLASS_CLASSIFICATION:
                 oof_preds = self.preprocessings[0].prepare_target_labels(
                     oof_predictions[prediction_cols].values
                 )
-
             else:
                 oof_preds = oof_predictions[prediction_cols]
 
             sample_weight = None
             if "sample_weight" in oof_predictions.columns:
                 sample_weight = oof_predictions["sample_weight"]
 
+            sensitive_features = None
+            sensitive_cols = [c for c in oof_predictions.columns if "sensitive" in c]
+            if sensitive_cols:
+                sensitive_features = oof_predictions[sensitive_cols]
+
             self._additional_metrics = AdditionalMetrics.compute(
-                target, oof_preds, sample_weight, self._ml_task
+                target,
+                oof_preds,
+                sample_weight,
+                self._ml_task,
+                sensitive_features,
+                self._fairness_metric
+                if self._ml_task != REGRESSION
+                else f"{self._fairness_metric}@{self.get_metric_name()}",
+                self._fairness_threshold,
+                self._privileged_groups,
+                self._underprivileged_groups,
+                self._fairness_optimization,
             )
             if self._ml_task == BINARY_CLASSIFICATION:
                 self._threshold = float(self._additional_metrics["threshold"])
         return self._additional_metrics
 
+    def get_sensitive_features_names(self):
+        metrics = self.get_additional_metrics()
+        fm = metrics.get("fairness_metrics", {})
+        return [i for i in list(fm.keys()) if i != "fairness_optimization"]
+
+    def get_fairness_metric(self, col_name):
+        metrics = self.get_additional_metrics()
+        fm = metrics.get("fairness_metrics", {})
+        return fm.get(col_name, {}).get("fairness_metric_value")
+
+    def get_fairness_optimization(self):
+        metrics = self.get_additional_metrics()
+        fm = metrics.get("fairness_metrics", {})
+        return fm.get("fairness_optimization", {})
+
+    def get_worst_fairness(self):
+        # We have fairness metrics per sensitive feature.
+        # The worst fairness metric is:
+        # - for ratio metrics, the lowest fairness value from all sensitive features
+        # - for difference metrics, the highest fairness value from all sensitive features
+        # It is needed as bias mitigation stop criteria.
+
+        metrics = self.get_additional_metrics()
+
+        fm = metrics.get("fairness_metrics", {})
+        worst_value = None
+        for col_name, values in fm.items():
+            if col_name == "fairness_optimization":
+                continue
+            if "ratio" in self._fairness_metric.lower():
+                if worst_value is None:
+                    worst_value = values.get("fairness_metric_value", 0)
+                else:
+                    worst_value = min(
+                        worst_value, values.get("fairness_metric_value", 0)
+                    )
+            else:
+                if worst_value is None:
+                    worst_value = values.get("fairness_metric_value", 1)
+                else:
+                    worst_value = max(
+                        worst_value, values.get("fairness_metric_value", 1)
+                    )
+
+        return worst_value
+
+    def get_best_fairness(self):
+        # We have fairness metrics per sensitive feature.
+        # The best fairness metric is:
+        # - for ratio metrics, the highest fairness value from all sensitive features
+        # - for difference metrics, the lowest fairness value from all sensitive features
+        # It is needed as bias mitigation stop criteria.
+
+        metrics = self.get_additional_metrics()
+        fm = metrics.get("fairness_metrics", {})
+        best_value = None
+        for col_name, values in fm.items():
+            if col_name == "fairness_optimization":
+                continue
+            if "ratio" in self._fairness_metric.lower():
+                if best_value is None:
+                    best_value = values.get("fairness_metric_value", 0)
+                else:
+                    best_value = max(best_value, values.get("fairness_metric_value", 0))
+            else:
+                if best_value is None:
+                    best_value = values.get("fairness_metric_value", 1)
+                else:
+                    best_value = min(best_value, values.get("fairness_metric_value", 1))
+
+        return best_value
+
+    def is_fair(self):
+        if self._is_fair is not None:
+            return self._is_fair
+        metrics = self.get_additional_metrics()
+        fm = metrics.get("fairness_metrics", {})
+        for col, m in fm.items():
+            if col == "fairness_optimization":
+                continue
+            if not m.get("is_fair", True):
+                self._is_fair = False
+                return False
+        self._is_fair = True
+        return False
+
     def save(self, results_path, model_subpath):
         start_time = time.time()
         model_path = os.path.join(results_path, model_subpath)
         logger.info(f"Save the model {model_path}")
 
         type_of_predictions = (
             "validation" if "k_folds" not in self.validation_params else "out_of_folds"
@@ -402,29 +610,34 @@
         predictions.to_csv(self._oof_predictions_fname, index=False)
 
         saved = [os.path.join(model_subpath, l.get_fname()) for l in self.learners]
 
         with open(os.path.join(model_path, "framework.json"), "w") as fout:
             preprocessing = [p.to_json() for p in self.preprocessings]
             learners_params = [learner.get_params() for learner in self.learners]
+
             desc = {
                 "uid": self.uid,
                 "name": self._name,
                 "preprocessing": preprocessing,
                 "learners": learners_params,
                 "params": self.params,
                 "saved": saved,
                 "predictions_fname": predictions_fname,
                 "metric_name": self.get_metric_name(),
                 "final_loss": self.get_final_loss(),
                 "train_time": self.get_train_time(),
                 "is_stacked": self._is_stacked,
+                "joblib_version": joblib.__version__,
             }
+            desc["final_loss"] = str(desc["final_loss"])
             if self._threshold is not None:
                 desc["threshold"] = self._threshold
+            if self._single_prediction_time is not None:
+                desc["single_prediction_time"] = self._single_prediction_time
             fout.write(json.dumps(desc, indent=4))
 
         learning_curve_metric = self.learners[0].get_metric_name()
         if learning_curve_metric is None:
             learning_curve_metric = self.get_metric_name()
 
         LearningCurves.plot(
@@ -476,22 +689,37 @@
 
     @staticmethod
     def load(results_path, model_subpath, lazy_load=True):
         model_path = os.path.join(results_path, model_subpath)
         logger.info(f"Loading model framework from {model_path}")
 
         json_desc = json.load(open(os.path.join(model_path, "framework.json")))
+
+        joblib_version_computer = joblib.__version__
+        joblib_version_framework = json_desc.get("joblib_version")
+
+        if (
+            joblib_version_framework is not None
+            and joblib_version_computer != joblib_version_framework
+        ):
+            raise AutoMLException(
+                f"Joblib version mismatch. Computer: {joblib_version_computer}, Framework: {joblib_version_framework}. Change to Framework version!"
+            )
+
         mf = ModelFramework(json_desc["params"])
         mf.uid = json_desc.get("uid", mf.uid)
         mf._name = json_desc.get("name", mf._name)
         mf._threshold = json_desc.get("threshold")
         mf.train_time = json_desc.get("train_time", mf.train_time)
         mf.final_loss = json_desc.get("final_loss", mf.final_loss)
         mf.metric_name = json_desc.get("metric_name", mf.metric_name)
         mf._is_stacked = json_desc.get("is_stacked", mf._is_stacked)
+        mf._single_prediction_time = json_desc.get(
+            "single_prediction_time", mf._single_prediction_time
+        )
         predictions_fname = json_desc.get("predictions_fname")
         if predictions_fname is not None:
             mf._oof_predictions_fname = os.path.join(results_path, predictions_fname)
 
         mf.learners = []
         for learner_desc, learner_subpath in zip(
             json_desc.get("learners"), json_desc.get("saved")
```

### Comparing `mljar-supervised-0.9.1/supervised/ensemble.py` & `mljar-supervised-1.0.0/supervised/ensemble.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import time
 import uuid
 import json
 import operator
 
 from supervised.algorithms.algorithm import BaseAlgorithm
 from supervised.algorithms.registry import BINARY_CLASSIFICATION
+from supervised.algorithms.registry import REGRESSION
 from supervised.algorithms.registry import MULTICLASS_CLASSIFICATION
 from supervised.model_framework import ModelFramework
 from supervised.utils.metric import Metric
 from supervised.utils.config import LOG_LEVEL
 from supervised.utils.additional_metrics import AdditionalMetrics
 from supervised.exceptions import NotTrainedException
 
@@ -23,24 +24,27 @@
 import matplotlib.pyplot as plt
 from tabulate import tabulate
 
 from supervised.utils.learning_curves import LearningCurves
 
 
 class Ensemble:
-
     algorithm_name = "Greedy Ensemble"
     algorithm_short_name = "Ensemble"
 
     def __init__(
         self,
         optimize_metric="logloss",
         ml_task=BINARY_CLASSIFICATION,
         is_stacked=False,
         max_single_prediction_time=None,
+        fairness_metric=None,
+        fairness_threshold=None,
+        privileged_groups=None,
+        underprivileged_groups=None,
     ):
         self.library_version = "0.1"
         self.uid = str(uuid.uuid4())
 
         self.metric = Metric({"name": optimize_metric})
         self.best_loss = self.metric.get_maximum()  # the best loss obtained by ensemble
         self.models_map = None
@@ -60,14 +64,21 @@
         self._scores = []
         self.oof_predictions = None
         self._oof_predictions_fname = None
         self._single_prediction_time = None  # prediction time on single sample
         self._max_single_prediction_time = max_single_prediction_time
         self.model_prediction_time = {}
 
+        self._fairness_metric = fairness_metric
+        self._fairness_threshold = fairness_threshold
+        self._privileged_groups = privileged_groups
+        self._underprivileged_groups = underprivileged_groups
+        self._is_fair = None
+        self.sensitive_features = None
+
     def get_train_time(self):
         return self.train_time
 
     def get_final_loss(self):
         return self.best_loss
 
     def is_valid(self):
@@ -87,46 +98,55 @@
     def get_type(self):
         prefix = ""  # "Stacked" if self._is_stacked else ""
         return prefix + self.algorithm_short_name
 
     def get_name(self):
         return self._name
 
+    def involved_model_names(self):
+        """Returns the list of all models involved in the current model.
+        For single model, it returns the list with the name of the model.
+        For ensemble model, it returns the list with the name of the ensemble and all internal models
+        (used to build ensemble).
+        For single model but trained on stacked data, it returns the list with the name of the model
+        (names of models used in stacking are not included)."""
+        if self.selected_models is None or not self.selected_models:
+            return [self._name]
+        l = []
+        for m in self.selected_models:
+            l += m["model"].involved_model_names()
+        return [self._name] + l
+
     def get_metric_name(self):
         return self.metric.name
 
     def get_metric(self):
         return self.metric
 
     def get_out_of_folds(self):
-        """ Needed when ensemble is treated as model and we want to compute additional metrics for it """
+        """Needed when ensemble is treated as model and we want to compute additional metrics for it"""
         # single prediction (in case of binary classification and regression)
         if self.oof_predictions is not None:
             return self.oof_predictions.copy(deep=True)
 
         if self._oof_predictions_fname is not None:
             self.oof_predictions = pd.read_csv(self._oof_predictions_fname)
             return self.oof_predictions.copy(deep=True)
 
-        if self.total_best_sum.shape[1] == 1:
-            tmp_df = pd.DataFrame({"prediction": self.total_best_sum["prediction"]})
-            tmp_df["target"] = self.target[self.target_columns]
-            return tmp_df
-
         ensemble_oof = pd.DataFrame(
-            data=self.total_best_sum,
-            columns=self.total_best_sum.columns
-            # [
-            # "prediction_{}".format(i) for i in range(self.total_best_sum.shape[1])
-            # ]
+            data=self.total_best_sum, columns=self.total_best_sum.columns
         )
         ensemble_oof["target"] = self.target
         if self.sample_weight is not None:
             ensemble_oof["sample_weight"] = self.sample_weight
 
+        # if self.sensitive_features is not None:
+        #    for col in self.sensitive_features.columns:
+        #        ensemble_oof[col] = self.sensitive_features[col]
+
         self.oof_predictions = ensemble_oof
         return ensemble_oof
 
     def _get_mean(self, oof_selected, best_sum, best_count):
         resp = copy.deepcopy(oof_selected)
         if best_count > 1:
             resp += best_sum
@@ -145,37 +165,46 @@
             if not [
                 m for m in models if m.is_fast_enough(self._max_single_prediction_time)
             ]:
                 raise NotTrainedException(
                     "Can't contruct ensemble with prediction time smaller than limit."
                 )
 
+        # check if we can construct fair ensemble
+        if self._fairness_metric is not None:
+            if not [m for m in models if m.is_fair()]:
+                raise NotTrainedException("Can't contruct fair ensemble.")
+
         oofs = {}
+        sensitive_features = None
         for m in models:
             # do not use model with RandomFeature
             if "RandomFeature" in m.get_name():
                 continue
 
             # ensemble only the same level of stack
             # if m._is_stacked != self._is_stacked:
             #    continue
             oof = m.get_out_of_folds()
             prediction_cols = [c for c in oof.columns if "prediction" in c]
             oofs[m.get_name()] = oof[prediction_cols]  # oof["prediction"]
             if self.target is None:
-
                 self.target_columns = [c for c in oof.columns if "target" in c]
                 self.target = oof[
                     self.target_columns
                 ]  # it will be needed for computing advance model statistics
 
             if self.sample_weight is None and "sample_weight" in oof.columns:
                 self.sample_weight = oof["sample_weight"]
 
-        return oofs, self.target, self.sample_weight
+            sensitive_cols = [c for c in oof.columns if "sensitive" in c]
+            if sensitive_cols and sensitive_features is None:
+                sensitive_features = oof[sensitive_cols]
+
+        return oofs, self.target, self.sample_weight, sensitive_features
 
     def get_additional_metrics(self):
         if self._additional_metrics is None:
             logger.debug("Get additional metrics for Ensemble")
             # 'target' - the target after processing used for model training
             # 'prediction' - out of folds predictions of the model
             oof_predictions = self.get_out_of_folds()
@@ -194,23 +223,120 @@
                 oof_preds["label"] = oof_preds["label"].map(labels)
 
             sample_weight = None
             if "sample_weight" in oof_predictions.columns:
                 sample_weight = oof_predictions["sample_weight"]
 
             self._additional_metrics = AdditionalMetrics.compute(
-                oof_predictions[target_cols], oof_preds, sample_weight, self._ml_task
+                oof_predictions[target_cols],
+                oof_preds,
+                sample_weight,
+                self._ml_task,
+                self.sensitive_features,
+                self._fairness_metric
+                if self._ml_task != REGRESSION
+                else f"{self._fairness_metric}@{self.get_metric_name()}",
+                self._fairness_threshold,
+                self._privileged_groups,
+                self._underprivileged_groups,
             )
             if self._ml_task == BINARY_CLASSIFICATION:
                 self._threshold = float(self._additional_metrics["threshold"])
 
         return self._additional_metrics
 
-    def fit(self, oofs, y, sample_weight=None):
+    def get_sensitive_features_names(self):
+        metrics = self.get_additional_metrics()
+        fm = metrics.get("fairness_metrics", {})
+        return [i for i in list(fm.keys()) if i != "fairness_optimization"]
+
+    def get_fairness_metric(self, col_name):
+        metrics = self.get_additional_metrics()
+        fm = metrics.get("fairness_metrics", {})
+        return fm.get(col_name, {}).get("fairness_metric_value")
+
+    def get_fairness_optimization(self):
+        metrics = self.get_additional_metrics()
+        fm = metrics.get("fairness_metrics", {})
+        return fm.get("fairness_optimization", {})
+
+    def get_worst_fairness(self):
+        # We have fairness metrics per sensitive feature.
+        # The worst fairness metric is:
+        # - for ratio metrics, the lowest fairness value from all sensitive features
+        # - for difference metrics, the highest fairness value from all sensitive features
+        # It is needed as bias mitigation stop criteria.
+
+        metrics = self.get_additional_metrics()
+
+        fm = metrics.get("fairness_metrics", {})
+        worst_value = None
+        for col_name, values in fm.items():
+            if col_name == "fairness_optimization":
+                continue
+            if "ratio" in self._fairness_metric.lower():
+                if worst_value is None:
+                    worst_value = values.get("fairness_metric_value", 0)
+                else:
+                    worst_value = min(
+                        worst_value, values.get("fairness_metric_value", 0)
+                    )
+            else:
+                if worst_value is None:
+                    worst_value = values.get("fairness_metric_value", 1)
+                else:
+                    worst_value = max(
+                        worst_value, values.get("fairness_metric_value", 1)
+                    )
+
+        return worst_value
+
+    def get_best_fairness(self):
+        # We have fairness metrics per sensitive feature.
+        # The best fairness metric is:
+        # - for ratio metrics, the highest fairness value from all sensitive features
+        # - for difference metrics, the lowest fairness value from all sensitive features
+        # It is needed as bias mitigation stop criteria.
+
+        metrics = self.get_additional_metrics()
+        fm = metrics.get("fairness_metrics", {})
+        best_value = None
+        for col_name, values in fm.items():
+            if col_name == "fairness_optimization":
+                continue
+            if "ratio" in self._fairness_metric.lower():
+                if best_value is None:
+                    best_value = values.get("fairness_metric_value", 0)
+                else:
+                    best_value = max(best_value, values.get("fairness_metric_value", 0))
+            else:
+                if best_value is None:
+                    best_value = values.get("fairness_metric_value", 1)
+                else:
+                    best_value = min(best_value, values.get("fairness_metric_value", 1))
+
+        return best_value
+
+    def is_fair(self):
+        if self._is_fair is not None:
+            return self._is_fair
+        metrics = self.get_additional_metrics()
+        fm = metrics.get("fairness_metrics", {})
+        for col, m in fm.items():
+            if col == "fairness_optimization":
+                continue
+            if not m.get("is_fair", True):
+                self._is_fair = False
+                return False
+        self._is_fair = True
+        return False
+
+    def fit(self, oofs, y, sample_weight=None, sensitive_features=None):
         logger.debug("Ensemble.fit")
+        self.sensitive_features = sensitive_features
         start_time = time.time()
         selected_algs_cnt = 0  # number of selected algorithms
         self.best_algs = []  # selected algoritms indices from each loop
 
         total_prediction_time = 0
         best_sum = None  # sum of best algorihtms
         for j in range(len(oofs)):  # iterate over all solutions
@@ -223,17 +349,22 @@
                     and model_name in self.model_prediction_time
                 ):
                     if (
                         total_prediction_time + self.model_prediction_time[model_name]
                         > self._max_single_prediction_time
                     ):
                         continue
+                # skip unfair models
+                if (
+                    self._fairness_metric is not None
+                    and not self.models_map[model_name].is_fair()
+                ):
+                    continue
                 y_ens = self._get_mean(oofs[model_name], best_sum, j + 1)
                 score = self.metric(y, y_ens, sample_weight)
-
                 if self.metric.improvement(previous=min_score, current=score):
                     min_score = score
                     best_model = model_name
 
             if best_model is None:
                 continue
             # there is improvement, save it
```

### Comparing `mljar-supervised-0.9.1/README.md` & `mljar-supervised-1.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,91 @@
 # MLJAR Automated Machine Learning for Humans
 
-[![Build Status](https://travis-ci.org/mljar/mljar-supervised.svg?branch=master)](https://travis-ci.org/mljar/mljar-supervised)
-[![Coverage Status](https://coveralls.io/repos/github/mljar/mljar-supervised/badge.svg?branch=master)](https://coveralls.io/github/mljar/mljar-supervised?branch=master)
+[![Tests status](https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml/badge.svg)](https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml)
 [![PyPI version](https://badge.fury.io/py/mljar-supervised.svg)](https://badge.fury.io/py/mljar-supervised)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/version.svg)](https://anaconda.org/conda-forge/mljar-supervised)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/mljar-supervised.svg)](https://pypi.python.org/pypi/mljar-supervised/)
-
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/platforms.svg)](https://anaconda.org/conda-forge/mljar-supervised)
+[![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/license.svg)](https://anaconda.org/conda-forge/mljar-supervised)
+[![Downloads](https://pepy.tech/badge/mljar-supervised)](https://pepy.tech/project/mljar-supervised)
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/mljar/mljar-examples/master/media/AutoML_overview_mljar_v3.svg" width="100%" />
 </p>
 
 ---
 
 **Documentation**: <a href="https://supervised.mljar.com/" target="_blank">https://supervised.mljar.com/</a>
 
 **Source Code**: <a href="https://github.com/mljar/mljar-supervised" target="_blank">https://github.com/mljar/mljar-supervised</a>
 
+**Looking for commercial support**: Please contact us by [email](https://mljar.com/contact/) for details
+
+
+<p align="center">
+  <img src="https://github.com/mljar/visual-identity/raw/main/robots/robot_docs.png" width="40%" />
+</p>
+
+
+
 ---
 
 ## Table of Contents
 
- - [Automated Machine Learning](https://github.com/mljar/mljar-supervised#automated-machine-learning-rocket)
- - [What's good in it?](https://github.com/mljar/mljar-supervised#whats-good-in-it-boom)
- - [Atomatic Documentation](https://github.com/mljar/mljar-supervised#automatic-documentation)
- - [Available Modes](https://github.com/mljar/mljar-supervised#available-modes-books)
+ - [Automated Machine Learning](https://github.com/mljar/mljar-supervised#automated-machine-learning)
+ - [What's good in it?](https://github.com/mljar/mljar-supervised#whats-good-in-it)
+ - [Automatic Documentation](https://github.com/mljar/mljar-supervised#automatic-documentation)
+ - [Available Modes](https://github.com/mljar/mljar-supervised#available-modes)
  - [Examples](https://github.com/mljar/mljar-supervised#examples)
+ - [FAQ](https://github.com/mljar/mljar-supervised#faq)
  - [Documentation](https://github.com/mljar/mljar-supervised#documentation)
- - [Installation](https://github.com/mljar/mljar-supervised#installation-package)
+ - [Installation](https://github.com/mljar/mljar-supervised#installation)
+ - [Demo](https://github.com/mljar/mljar-supervised#demo)
  - [Contributing](https://github.com/mljar/mljar-supervised#contributing)
- - [License](https://github.com/mljar/mljar-supervised#license-necktie)
- - [MLJAR](https://github.com/mljar/mljar-supervised#mljar-heart)
+ - [Cite](https://github.com/mljar/mljar-supervised#cite)
+ - [License](https://github.com/mljar/mljar-supervised#license)
+ - [Commercial support](https://github.com/mljar/mljar-supervised#commercial-support)
+ - [MLJAR](https://github.com/mljar/mljar-supervised#mljar)
+ 
 
-## Automated Machine Learning :rocket: 
+# Automated Machine Learning 
 
 The `mljar-supervised` is an Automated Machine Learning Python package that works with tabular data. It is designed to save time for a data scientist. It abstracts the common way to preprocess the data, construct the machine learning models, and perform hyper-parameters tuning to find the best model :trophy:. It is no black-box as you can see exactly how the ML pipeline is constructed (with a detailed Markdown report for each ML model). 
 
 The `mljar-supervised` will help you with:
  - explaining and understanding your data (Automatic Exploratory Data Analysis),
  - trying many different machine learning models (Algorithm Selection and Hyper-Parameters tuning),
- - creating Markdown reports from analysis with details about all models (Atomatic-Documentation),
+ - creating Markdown reports from analysis with details about all models (Automatic-Documentation),
  - saving, re-running and loading the analysis and ML models.
 
-It has three built-in modes of work:
+It has four built-in modes of work:
  - `Explain` mode, which is ideal for explaining and understanding the data, with many data explanations, like decision trees visualization, linear models coefficients display, permutation importances and SHAP explanations of data,
  - `Perform` for building ML pipelines to use in production,
  - `Compete` mode that trains highly-tuned ML models with ensembling and stacking, with a purpose to use in ML competitions.
+ - `Optuna` mode that can be used to search for highly-tuned ML models, should be used when the performance is the most important, and computation time is not limited (it is available from version `0.10.0`)
 
 Of course, you can further customize the details of each `mode` to meet the requirements.
 
-## What's good in it? :boom:
+## What's good in it? 
 
 - It is using many algorithms: `Baseline`, `Linear`, `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, `CatBoost`, `Neural Networks`, and `Nearest Neighbors`.
 - It can compute Ensemble based on greedy algorithm from [Caruana paper](http://www.cs.cornell.edu/~alexn/papers/shotgun.icml04.revised.rev2.pdf).
 - It can stack models to build level 2 ensemble (available in `Compete` mode or after setting `stack_models` parameter).
 - It can do features preprocessing, like: missing values imputation and converting categoricals. What is more, it can also handle target values preprocessing.
 - It can do advanced features engineering, like: [Golden Features](https://supervised.mljar.com/features/golden_features/), [Features Selection](https://supervised.mljar.com/features/features_selection/), Text and Time Transformations.
 - It can tune hyper-parameters with `not-so-random-search` algorithm (random-search over defined set of values) and hill climbing to fine-tune final models.
 - It can compute the `Baseline` for your data. That you will know if you need Machine Learning or not!
 - It has extensive explanations. This package is training simple `Decision Trees` with `max_depth <= 5`, so you can easily visualize them with amazing [dtreeviz](https://github.com/parrt/dtreeviz) to better understand your data.
 - The `mljar-supervised` is using simple linear regression and include its coefficients in the summary report, so you can check which features are used the most in the linear model.
 - It cares about explainability of models: for every algorithm, the feature importance is computed based on permutation. Additionally, for every algorithm the SHAP explanations are computed: feature importance, dependence plots, and decision plots (explanations can be switched off with `explain_level` parameter).
-- There is automatic documnetation for every ML experiment run with AutoML. The `mljar-supervised` creates markdown reports from AutoML training full of ML details, metrics and charts. 
+- There is automatic documentation for every ML experiment run with AutoML. The `mljar-supervised` creates markdown reports from AutoML training full of ML details, metrics and charts. 
+
+<p align="center">
+  <img src="https://raw.githubusercontent.com/mljar/visual-identity/main/media/infograph.png" width="100%" />
+</p>
 
 # Automatic Documentation
 
 ## The AutoML Report
 
 The report from running AutoML will contain the table with infomation about each model score and time needed to train the model. For each model there is a link, which you can click to see model's details. The performance of all ML models is presented as scatter and box plots so you can visually inspect which algorithms perform the best :trophy:.
 
@@ -84,18 +105,22 @@
 ## The `LightGBM` Report
 
 The example for `LightGBM` summary:
 
 ![Decision Tree summary](https://github.com/mljar/mljar-examples/blob/master/media/lightgbm_summary.gif)
 
 
-## Available Modes :books:
+## Available Modes
 
 In the [docs](https://supervised.mljar.com/features/modes/) you can find details about AutoML modes are presented in the table .
 
+<p align="center">
+  <img src="https://raw.githubusercontent.com/mljar/visual-identity/main/media/mljar_modes.png" width="100%" />
+</p>
+
 ### Explain 
 
 ```py
 automl = AutoML(mode="Explain")
 ```
 
 It is aimed to be used when the user wants to explain and understand the data.
@@ -121,14 +146,62 @@
 ```
 
 It should be used for machine learning competitions.
  - It adapts the validation strategy depending on dataset size and `total_time_limit`. It can be: train/test split (80/20), 5-fold CV or 10-fold CV. 
  - It is using: `Linear`, `Decision Tree`, `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, `CatBoost`, `Neural Network` and `Nearest Neighbors`. It uses ensemble and **stacking**. 
  - It has only learning curves in the reports.
 
+### Optuna
+
+```py
+automl = AutoML(mode="Optuna", optuna_time_budget=3600)
+```
+
+It should be used when the performance is the most important and time is not limited.
+- It is using 10-fold CV
+- It is using: `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, and `CatBoost`. Those algorithms are tuned by `Optuna` framework for `optuna_time_budget` seconds, each. Algorithms are tuned with original data, without advanced feature engineering.
+- It is using advanced feature engineering, stacking and ensembling. The hyperparameters found for original data are reused with those steps.
+- It produces learning curves in the reports.
+
+## How to save and load AutoML?
+
+All models in the AutoML are saved and loaded automatically. No need to call `save()` or `load()`.
+
+### Example:
+
+#### Train AutoML
+
+```python
+automl = AutoML(results_path="AutoML_classifier")
+automl.fit(X, y)
+```
+
+You will have all models saved in the `AutoML_classifier` directory. Each model will have a separate directory with the `README.md` file with all details from the training.
+
+#### Compute predictions
+```python
+automl = AutoML(results_path="AutoML_classifier")
+automl.predict(X)
+```
+
+The  AutoML automatically loads models from the `results_path` directory. If you will call `fit()` on already trained AutoML then you will get a warning message that AutoML is already fitted.
+
+
+### Why do you automatically save all models?
+
+All models are automatically saved to be able to restore the training after interruption. For example, you are training AutoML for 48 hours, and after 47 hours there is some unexpected interruption. In MLJAR AutoML you just call the same training code after the interruption and AutoML reloads already trained models and finish the training.
+
+## Supported evaluation metrics (`eval_metric` argument in `AutoML()`)
+
+- for binary classification: `logloss`, `auc`, `f1`, `average_precision`, `accuracy`- default is `logloss`
+- for mutliclass classification: `logloss`, `f1`, `accuracy` - default is `logloss`
+- for regression: `rmse`, `mse`, `mae`, `r2`, `mape`, `spearman`, `pearson` - default is `rmse`
+
+If you don't find `eval_metric` that you need, please add a new issue. We will add it.
+
 # Examples
 
 ## :point_right: Binary Classification Example
 
 There is a simple interface available with `fit` and `predict` methods.
 
 ```python
@@ -199,26 +272,26 @@
 predictions = automl.predict_all(X_test)
 print(predictions.head())
 print("Test accuracy:", accuracy_score(y_test, predictions["label"].astype(int)))
 ```
 
 ## :point_right: Regression Example
 
-Regression example on Boston house prices data. On test data it scores ~ 10.85 mean squared error (MSE).
+Regression example on `California Housing` house prices data.
 
 ```python
 import numpy as np
 import pandas as pd
-from sklearn.datasets import load_boston
+from sklearn.datasets import fetch_california_housing
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import mean_squared_error
 from supervised.automl import AutoML # mljar-supervised
 
 # Load the data
-housing = load_boston()
+housing = fetch_california_housing()
 X_train, X_test, y_train, y_test = train_test_split(
     pd.DataFrame(housing.data, columns=housing.feature_names),
     housing.target,
     test_size=0.25,
     random_state=123,
 )
 
@@ -233,26 +306,106 @@
 
 ## :point_right: More Examples
 
 - [**Income classification**](https://github.com/mljar/mljar-examples/tree/master/Income_classification) - it is a binary classification task on census data
 - [**Iris classification**](https://github.com/mljar/mljar-examples/tree/master/Iris_classification) - it is a multiclass classification on Iris flowers data
 - [**House price regression**](https://github.com/mljar/mljar-examples/tree/master/House_price_regression) - it is a regression task on Boston houses data
 
-# Documentation :books:
+# FAQ
+
+<details><summary>What method is used for hyperparameters optimization?</summary>
+  - For modes: `Explain`, `Perform` and `Compete` there is used a random search method combined with hill climbing. In this approach all checked models are saved and used for building Ensemble.
+  - For mode: `Optuna` the Optuna framework is used. It is using TPE sampler for tuning. Models checked during Optuna hyperparameters search are not saved, only the best model is saved (final model from tuning). You can check the details about checked hyperparameters from optuna by checking study files in `optuna` directory in your AutoML `results_path`.
+</details>
+
+<details><summary>How to save and load AutoML?</summary>
+
+The save and load of AutoML models is automatic. All models created during AutoML training are saved in the directory set in `results_path` (argument of `AutoML()` constructor). If there is no `results_path` set, then the directory is created based on following name convention: `AutoML_{number}` the `number` will be number from 1 to 1000 (depends which directory name will be free).
+
+Example save and load:
+
+```python
+automl = AutoML(results_path='AutoML_1')
+automl.fit(X, y)
+```
+
+The all models from AutoML are saved in `AutoML_1` directory.
+
+To load models:
+
+```python
+automl = AutoML(results_path='AutoML_1')
+automl.predict(X)
+```
+
+</details>
+
+<details><summary>How to set ML task (select between classification or regression)?</summary>
+
+The MLJAR AutoML can work with:
+- binary classification
+- multi-class classification
+- regression
+
+The ML task detection is automatic based on target values. There can be situation if you want to manually force AutoML to select the ML task, then you need to set `ml_task` parameter. It can be set to `'binary_classification'`, `'multiclass_classification'`, `'regression'`.
+
+Example:
+```python
+automl = AutoML(ml_task='regression')
+automl.fit(X, y)
+```
+In the above example the regression model will be fitted.
+
+</details>
+
+<details><summary>How to reuse Optuna hyperparameters?</summary>
+  
+  You can reuse Optuna hyperparameters that were found in other AutoML training. You need to pass them in `optuna_init_params` argument. All hyperparameters found during Optuna tuning are saved in the `optuna/optuna.json` file (inside `results_path` directory).
+  
+ Example:
+ 
+ ```python
+ optuna_init = json.loads(open('previous_AutoML_training/optuna/optuna.json').read())
+ 
+ automl = AutoML(
+     mode='Optuna',
+     optuna_init_params=optuna_init
+ )
+ automl.fit(X, y)
+ ```
+  
+ When reusing Optuna hyperparameters the Optuna tuning is simply skipped. The model will be trained with hyperparameters set in `optuna_init_params`. Right now there is no option to continue Optuna tuning with seed parameters.
+  
+  
+</details>
+
+
+<details><summary>How to know the order of classes for binary or multiclass problem when using predict_proba?</summary>
+
+To get predicted probabilites with information about class label please use the `predict_all()` method. It returns the pandas DataFrame with class names in the columns. The order of predicted columns is the same in the `predict_proba()` and `predict_all()` methods. The `predict_all()` method will additionaly have the column with the predicted class label.
+
+</details>
+
+# Documentation  
 
 For details please check [mljar-supervised docs](https://supervised.mljar.com).
 
-# Installation :package: 
+# Installation  
 
 From PyPi repository:
 
 ```
 pip install mljar-supervised
 ```
 
+To install this package with conda run:
+```
+conda install -c conda-forge mljar-supervised
+```
+
 From source code:
 
 ```
 git clone https://github.com/mljar/mljar-supervised.git
 cd mljar-supervised
 python setup.py install
 ```
@@ -272,28 +425,68 @@
 RUN apt-get update && apt-get -y update
 RUN apt-get install -y build-essential python3-pip python3-dev
 RUN pip3 -q install pip --upgrade
 RUN pip3 install mljar-supervised jupyter
 CMD ["jupyter", "notebook", "--port=8888", "--no-browser", "--ip=0.0.0.0", "--allow-root"]
 ```
 
+Install from GitHub with pip:
+```
+pip install -q -U git+https://github.com/mljar/mljar-supervised.git@master
+```
+# Demo
+
+In the below demo GIF you will see:
+- MLJAR AutoML trained in Jupyter Notebook on titanic dataset
+- overview of created files
+- showcase of selected plots created during AutoML training
+- algorithm comparison report along with their plots
+- example of README file and csv file with results
+
+![](https://github.com/mljar/mljar-examples/raw/master/media/mljar_files.gif)
+
 # Contributing
 
 To get started take a look at our [Contribution Guide](https://supervised.mljar.com/contributing/) for information about our process and where you can fit in!
 
 ### Contributors
 <a href="https://github.com/mljar/mljar-supervised/graphs/contributors">
   <img src="https://contributors-img.web.app/image?repo=mljar/mljar-supervised" />
 </a>
 
+# Cite
+
+Would you like to cite MLJAR? Great! :)
+
+You can cite MLJAR as following:
+
+```
+@misc{mljar,
+  author    = {Aleksandra P\l{}o\'{n}ska and Piotr P\l{}o\'{n}ski},
+  year      = {2021},
+  publisher = {MLJAR},
+  address   = {\L{}apy, Poland},
+  title     = {MLJAR: State-of-the-art Automated Machine Learning Framework for Tabular Data.  Version 0.10.3},
+  url       = {https://github.com/mljar/mljar-supervised}
+}
+```
+
+Would love to hear from you how have you used MLJAR AutoML in your project. 
+Please feel free to let us know at 
+![image](https://user-images.githubusercontent.com/6959032/118103228-f5ea9a00-b3d9-11eb-87ed-8cfb1f873f91.png)
+
 
-# License :necktie:
+# License  
 
 The `mljar-supervised` is provided with [MIT license](https://github.com/mljar/mljar-supervised/blob/master/LICENSE).
 
-# MLJAR :heart:
+# Commercial support
+
+Looking for commercial support? Do you need new feature implementation? Please contact us by [email](https://mljar.com/contact/) for details.
+
+# MLJAR 
 <p align="center">
   <img src="https://github.com/mljar/mljar-examples/blob/master/media/large_logo.png" width="314" />
 </p>
 
 The `mljar-supervised` is an open-source project created by [MLJAR](https://mljar.com). We care about ease of use in the Machine Learning. 
 The [mljar.com](https://mljar.com) provides a beautiful and simple user interface for building machine learning models.
```

#### html2text {}

```diff
@@ -1,119 +1,167 @@
-# MLJAR Automated Machine Learning for Humans [![Build Status](https://travis-
-ci.org/mljar/mljar-supervised.svg?branch=master)](https://travis-ci.org/mljar/
-mljar-supervised) [![Coverage Status](https://coveralls.io/repos/github/mljar/
-mljar-supervised/badge.svg?branch=master)](https://coveralls.io/github/mljar/
-mljar-supervised?branch=master) [![PyPI version](https://badge.fury.io/py/
-mljar-supervised.svg)](https://badge.fury.io/py/mljar-supervised) [![PyPI
-pyversions](https://img.shields.io/pypi/pyversions/mljar-supervised.svg)]
-(https://pypi.python.org/pypi/mljar-supervised/)
+# MLJAR Automated Machine Learning for Humans [![Tests status](https://
+github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml/badge.svg)]
+(https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml) [!
+[PyPI version](https://badge.fury.io/py/mljar-supervised.svg)](https://
+badge.fury.io/py/mljar-supervised) [![Anaconda-Server Badge](https://
+anaconda.org/conda-forge/mljar-supervised/badges/version.svg)](https://
+anaconda.org/conda-forge/mljar-supervised) [![PyPI pyversions](https://
+img.shields.io/pypi/pyversions/mljar-supervised.svg)](https://pypi.python.org/
+pypi/mljar-supervised/) [![Anaconda-Server Badge](https://anaconda.org/conda-
+forge/mljar-supervised/badges/platforms.svg)](https://anaconda.org/conda-forge/
+mljar-supervised) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/
+mljar-supervised/badges/license.svg)](https://anaconda.org/conda-forge/mljar-
+supervised) [![Downloads](https://pepy.tech/badge/mljar-supervised)](https://
+pepy.tech/project/mljar-supervised)
      [https://raw.githubusercontent.com/mljar/mljar-examples/master/media/
                          AutoML_overview_mljar_v3.svg]
 --- **Documentation**: https://supervised.mljar.com/ **Source Code**: https://
-github.com/mljar/mljar-supervised --- ## Table of Contents - [Automated Machine
-Learning](https://github.com/mljar/mljar-supervised#automated-machine-learning-
-rocket) - [What's good in it?](https://github.com/mljar/mljar-supervised#whats-
-good-in-it-boom) - [Atomatic Documentation](https://github.com/mljar/mljar-
-supervised#automatic-documentation) - [Available Modes](https://github.com/
-mljar/mljar-supervised#available-modes-books) - [Examples](https://github.com/
-mljar/mljar-supervised#examples) - [Documentation](https://github.com/mljar/
-mljar-supervised#documentation) - [Installation](https://github.com/mljar/
-mljar-supervised#installation-package) - [Contributing](https://github.com/
-mljar/mljar-supervised#contributing) - [License](https://github.com/mljar/
-mljar-supervised#license-necktie) - [MLJAR](https://github.com/mljar/mljar-
-supervised#mljar-heart) ## Automated Machine Learning :rocket: The `mljar-
-supervised` is an Automated Machine Learning Python package that works with
-tabular data. It is designed to save time for a data scientist. It abstracts
-the common way to preprocess the data, construct the machine learning models,
-and perform hyper-parameters tuning to find the best model :trophy:. It is no
-black-box as you can see exactly how the ML pipeline is constructed (with a
-detailed Markdown report for each ML model). The `mljar-supervised` will help
-you with: - explaining and understanding your data (Automatic Exploratory Data
-Analysis), - trying many different machine learning models (Algorithm Selection
-and Hyper-Parameters tuning), - creating Markdown reports from analysis with
-details about all models (Atomatic-Documentation), - saving, re-running and
-loading the analysis and ML models. It has three built-in modes of work: -
-`Explain` mode, which is ideal for explaining and understanding the data, with
-many data explanations, like decision trees visualization, linear models
-coefficients display, permutation importances and SHAP explanations of data, -
-`Perform` for building ML pipelines to use in production, - `Compete` mode that
-trains highly-tuned ML models with ensembling and stacking, with a purpose to
-use in ML competitions. Of course, you can further customize the details of
-each `mode` to meet the requirements. ## What's good in it? :boom: - It is
-using many algorithms: `Baseline`, `Linear`, `Random Forest`, `Extra Trees`,
-`LightGBM`, `Xgboost`, `CatBoost`, `Neural Networks`, and `Nearest Neighbors`.
-- It can compute Ensemble based on greedy algorithm from [Caruana paper](http:/
-/www.cs.cornell.edu/~alexn/papers/shotgun.icml04.revised.rev2.pdf). - It can
-stack models to build level 2 ensemble (available in `Compete` mode or after
-setting `stack_models` parameter). - It can do features preprocessing, like:
-missing values imputation and converting categoricals. What is more, it can
-also handle target values preprocessing. - It can do advanced features
-engineering, like: [Golden Features](https://supervised.mljar.com/features/
-golden_features/), [Features Selection](https://supervised.mljar.com/features/
-features_selection/), Text and Time Transformations. - It can tune hyper-
-parameters with `not-so-random-search` algorithm (random-search over defined
-set of values) and hill climbing to fine-tune final models. - It can compute
-the `Baseline` for your data. That you will know if you need Machine Learning
-or not! - It has extensive explanations. This package is training simple
-`Decision Trees` with `max_depth <= 5`, so you can easily visualize them with
-amazing [dtreeviz](https://github.com/parrt/dtreeviz) to better understand your
-data. - The `mljar-supervised` is using simple linear regression and include
-its coefficients in the summary report, so you can check which features are
-used the most in the linear model. - It cares about explainability of models:
-for every algorithm, the feature importance is computed based on permutation.
-Additionally, for every algorithm the SHAP explanations are computed: feature
-importance, dependence plots, and decision plots (explanations can be switched
-off with `explain_level` parameter). - There is automatic documnetation for
-every ML experiment run with AutoML. The `mljar-supervised` creates markdown
-reports from AutoML training full of ML details, metrics and charts. #
-Automatic Documentation ## The AutoML Report The report from running AutoML
+github.com/mljar/mljar-supervised **Looking for commercial support**: Please
+contact us by [email](https://mljar.com/contact/) for details
+   [https://github.com/mljar/visual-identity/raw/main/robots/robot_docs.png]
+--- ## Table of Contents - [Automated Machine Learning](https://github.com/
+mljar/mljar-supervised#automated-machine-learning) - [What's good in it?]
+(https://github.com/mljar/mljar-supervised#whats-good-in-it) - [Automatic
+Documentation](https://github.com/mljar/mljar-supervised#automatic-
+documentation) - [Available Modes](https://github.com/mljar/mljar-
+supervised#available-modes) - [Examples](https://github.com/mljar/mljar-
+supervised#examples) - [FAQ](https://github.com/mljar/mljar-supervised#faq) -
+[Documentation](https://github.com/mljar/mljar-supervised#documentation) -
+[Installation](https://github.com/mljar/mljar-supervised#installation) - [Demo]
+(https://github.com/mljar/mljar-supervised#demo) - [Contributing](https://
+github.com/mljar/mljar-supervised#contributing) - [Cite](https://github.com/
+mljar/mljar-supervised#cite) - [License](https://github.com/mljar/mljar-
+supervised#license) - [Commercial support](https://github.com/mljar/mljar-
+supervised#commercial-support) - [MLJAR](https://github.com/mljar/mljar-
+supervised#mljar) # Automated Machine Learning The `mljar-supervised` is an
+Automated Machine Learning Python package that works with tabular data. It is
+designed to save time for a data scientist. It abstracts the common way to
+preprocess the data, construct the machine learning models, and perform hyper-
+parameters tuning to find the best model :trophy:. It is no black-box as you
+can see exactly how the ML pipeline is constructed (with a detailed Markdown
+report for each ML model). The `mljar-supervised` will help you with: -
+explaining and understanding your data (Automatic Exploratory Data Analysis), -
+trying many different machine learning models (Algorithm Selection and Hyper-
+Parameters tuning), - creating Markdown reports from analysis with details
+about all models (Automatic-Documentation), - saving, re-running and loading
+the analysis and ML models. It has four built-in modes of work: - `Explain`
+mode, which is ideal for explaining and understanding the data, with many data
+explanations, like decision trees visualization, linear models coefficients
+display, permutation importances and SHAP explanations of data, - `Perform` for
+building ML pipelines to use in production, - `Compete` mode that trains
+highly-tuned ML models with ensembling and stacking, with a purpose to use in
+ML competitions. - `Optuna` mode that can be used to search for highly-tuned ML
+models, should be used when the performance is the most important, and
+computation time is not limited (it is available from version `0.10.0`) Of
+course, you can further customize the details of each `mode` to meet the
+requirements. ## What's good in it? - It is using many algorithms: `Baseline`,
+`Linear`, `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, `CatBoost`,
+`Neural Networks`, and `Nearest Neighbors`. - It can compute Ensemble based on
+greedy algorithm from [Caruana paper](http://www.cs.cornell.edu/~alexn/papers/
+shotgun.icml04.revised.rev2.pdf). - It can stack models to build level 2
+ensemble (available in `Compete` mode or after setting `stack_models`
+parameter). - It can do features preprocessing, like: missing values imputation
+and converting categoricals. What is more, it can also handle target values
+preprocessing. - It can do advanced features engineering, like: [Golden
+Features](https://supervised.mljar.com/features/golden_features/), [Features
+Selection](https://supervised.mljar.com/features/features_selection/), Text and
+Time Transformations. - It can tune hyper-parameters with `not-so-random-
+search` algorithm (random-search over defined set of values) and hill climbing
+to fine-tune final models. - It can compute the `Baseline` for your data. That
+you will know if you need Machine Learning or not! - It has extensive
+explanations. This package is training simple `Decision Trees` with `max_depth
+<= 5`, so you can easily visualize them with amazing [dtreeviz](https://
+github.com/parrt/dtreeviz) to better understand your data. - The `mljar-
+supervised` is using simple linear regression and include its coefficients in
+the summary report, so you can check which features are used the most in the
+linear model. - It cares about explainability of models: for every algorithm,
+the feature importance is computed based on permutation. Additionally, for
+every algorithm the SHAP explanations are computed: feature importance,
+dependence plots, and decision plots (explanations can be switched off with
+`explain_level` parameter). - There is automatic documentation for every ML
+experiment run with AutoML. The `mljar-supervised` creates markdown reports
+from AutoML training full of ML details, metrics and charts.
+     [https://raw.githubusercontent.com/mljar/visual-identity/main/media/
+                                infograph.png]
+# Automatic Documentation ## The AutoML Report The report from running AutoML
 will contain the table with infomation about each model score and time needed
 to train the model. For each model there is a link, which you can click to see
 model's details. The performance of all ML models is presented as scatter and
 box plots so you can visually inspect which algorithms perform the best :
 trophy:. ![AutoML leaderboard](https://github.com/mljar/mljar-examples/blob/
 master/media/automl_summary.gif) ## The `Decision Tree` Report The example for
 `Decision Tree` summary with trees visualization. For classification tasks
 additional metrics are provided: - confusion matrix - threshold (optimized in
 the case of binary classification task) - F1 score - Accuracy - Precision,
 Recall, MCC ![Decision Tree summary](https://github.com/mljar/mljar-examples/
 blob/master/media/decision_tree_summary.gif) ## The `LightGBM` Report The
 example for `LightGBM` summary: ![Decision Tree summary](https://github.com/
 mljar/mljar-examples/blob/master/media/lightgbm_summary.gif) ## Available Modes
-:books: In the [docs](https://supervised.mljar.com/features/modes/) you can
-find details about AutoML modes are presented in the table . ### Explain ```py
-automl = AutoML(mode="Explain") ``` It is aimed to be used when the user wants
-to explain and understand the data. - It is using 75%/25% train/test split. -
-It is using: `Baseline`, `Linear`, `Decision Tree`, `Random Forest`, `Xgboost`,
-`Neural Network` algorithms and ensemble. - It has full explanations: learning
-curves, importance plots, and SHAP plots. ### Perform ```py automl = AutoML
-(mode="Perform") ``` It should be used when the user wants to train a model
-that will be used in real-life use cases. - It is using 5-fold CV. - It is
-using: `Linear`, `Random Forest`, `LightGBM`, `Xgboost`, `CatBoost` and `Neural
-Network`. It uses ensembling. - It has learning curves and importance plots in
-reports. ### Compete ```py automl = AutoML(mode="Compete") ``` It should be
-used for machine learning competitions. - It adapts the validation strategy
-depending on dataset size and `total_time_limit`. It can be: train/test split
-(80/20), 5-fold CV or 10-fold CV. - It is using: `Linear`, `Decision Tree`,
-`Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, `CatBoost`, `Neural
-Network` and `Nearest Neighbors`. It uses ensemble and **stacking**. - It has
-only learning curves in the reports. # Examples ## :point_right: Binary
-Classification Example There is a simple interface available with `fit` and
-`predict` methods. ```python import pandas as pd from sklearn.model_selection
-import train_test_split from supervised.automl import AutoML df = pd.read_csv
-( "https://raw.githubusercontent.com/pplonski/datasets-for-start/master/adult/
-data.csv", skipinitialspace=True, ) X_train, X_test, y_train, y_test =
-train_test_split( df[df.columns[:-1]], df["income"], test_size=0.25 ) automl =
-AutoML() automl.fit(X_train, y_train) predictions = automl.predict(X_test) ```
-AutoML `fit` will print: ```py Create directory AutoML_1 AutoML task to be
-solved: binary_classification AutoML will use algorithms: ['Baseline',
-'Linear', 'Decision Tree', 'Random Forest', 'Xgboost', 'Neural Network'] AutoML
-will optimize for metric: logloss 1_Baseline final logloss 0.5519845471086654
-time 0.08 seconds 2_DecisionTree final logloss 0.3655910192804364 time 10.28
-seconds 3_Linear final logloss 0.38139916864708445 time 3.19 seconds
+In the [docs](https://supervised.mljar.com/features/modes/) you can find
+details about AutoML modes are presented in the table .
+     [https://raw.githubusercontent.com/mljar/visual-identity/main/media/
+                               mljar_modes.png]
+### Explain ```py automl = AutoML(mode="Explain") ``` It is aimed to be used
+when the user wants to explain and understand the data. - It is using 75%/25%
+train/test split. - It is using: `Baseline`, `Linear`, `Decision Tree`, `Random
+Forest`, `Xgboost`, `Neural Network` algorithms and ensemble. - It has full
+explanations: learning curves, importance plots, and SHAP plots. ### Perform
+```py automl = AutoML(mode="Perform") ``` It should be used when the user wants
+to train a model that will be used in real-life use cases. - It is using 5-fold
+CV. - It is using: `Linear`, `Random Forest`, `LightGBM`, `Xgboost`, `CatBoost`
+and `Neural Network`. It uses ensembling. - It has learning curves and
+importance plots in reports. ### Compete ```py automl = AutoML(mode="Compete")
+``` It should be used for machine learning competitions. - It adapts the
+validation strategy depending on dataset size and `total_time_limit`. It can
+be: train/test split (80/20), 5-fold CV or 10-fold CV. - It is using: `Linear`,
+`Decision Tree`, `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`,
+`CatBoost`, `Neural Network` and `Nearest Neighbors`. It uses ensemble and
+**stacking**. - It has only learning curves in the reports. ### Optuna ```py
+automl = AutoML(mode="Optuna", optuna_time_budget=3600) ``` It should be used
+when the performance is the most important and time is not limited. - It is
+using 10-fold CV - It is using: `Random Forest`, `Extra Trees`, `LightGBM`,
+`Xgboost`, and `CatBoost`. Those algorithms are tuned by `Optuna` framework for
+`optuna_time_budget` seconds, each. Algorithms are tuned with original data,
+without advanced feature engineering. - It is using advanced feature
+engineering, stacking and ensembling. The hyperparameters found for original
+data are reused with those steps. - It produces learning curves in the reports.
+## How to save and load AutoML? All models in the AutoML are saved and loaded
+automatically. No need to call `save()` or `load()`. ### Example: #### Train
+AutoML ```python automl = AutoML(results_path="AutoML_classifier") automl.fit
+(X, y) ``` You will have all models saved in the `AutoML_classifier` directory.
+Each model will have a separate directory with the `README.md` file with all
+details from the training. #### Compute predictions ```python automl = AutoML
+(results_path="AutoML_classifier") automl.predict(X) ``` The AutoML
+automatically loads models from the `results_path` directory. If you will call
+`fit()` on already trained AutoML then you will get a warning message that
+AutoML is already fitted. ### Why do you automatically save all models? All
+models are automatically saved to be able to restore the training after
+interruption. For example, you are training AutoML for 48 hours, and after 47
+hours there is some unexpected interruption. In MLJAR AutoML you just call the
+same training code after the interruption and AutoML reloads already trained
+models and finish the training. ## Supported evaluation metrics (`eval_metric`
+argument in `AutoML()`) - for binary classification: `logloss`, `auc`, `f1`,
+`average_precision`, `accuracy`- default is `logloss` - for mutliclass
+classification: `logloss`, `f1`, `accuracy` - default is `logloss` - for
+regression: `rmse`, `mse`, `mae`, `r2`, `mape`, `spearman`, `pearson` - default
+is `rmse` If you don't find `eval_metric` that you need, please add a new
+issue. We will add it. # Examples ## :point_right: Binary Classification
+Example There is a simple interface available with `fit` and `predict` methods.
+```python import pandas as pd from sklearn.model_selection import
+train_test_split from supervised.automl import AutoML df = pd.read_csv( "https:
+//raw.githubusercontent.com/pplonski/datasets-for-start/master/adult/data.csv",
+skipinitialspace=True, ) X_train, X_test, y_train, y_test = train_test_split
+( df[df.columns[:-1]], df["income"], test_size=0.25 ) automl = AutoML()
+automl.fit(X_train, y_train) predictions = automl.predict(X_test) ``` AutoML
+`fit` will print: ```py Create directory AutoML_1 AutoML task to be solved:
+binary_classification AutoML will use algorithms: ['Baseline', 'Linear',
+'Decision Tree', 'Random Forest', 'Xgboost', 'Neural Network'] AutoML will
+optimize for metric: logloss 1_Baseline final logloss 0.5519845471086654 time
+0.08 seconds 2_DecisionTree final logloss 0.3655910192804364 time 10.28 seconds
+3_Linear final logloss 0.38139916864708445 time 3.19 seconds
 4_Default_RandomForest final logloss 0.2975204390214936 time 79.19 seconds
 5_Default_Xgboost final logloss 0.2731086827200411 time 5.17 seconds
 6_Default_NeuralNetwork final logloss 0.319812276905242 time 21.19 seconds
 Ensemble final logloss 0.2731086821194617 time 1.43 seconds ``` - the AutoML
 results in [Markdown report](https://github.com/mljar/mljar-examples/tree/
 master/Income_classification/AutoML_1#automl-leaderboard) - the Xgboost
 [Markdown report](https://github.com/mljar/mljar-examples/blob/master/
@@ -135,46 +183,103 @@
 AutoML # load the data digits = load_digits() X_train, X_test, y_train, y_test
 = train_test_split( pd.DataFrame(digits.data), digits.target,
 stratify=digits.target, test_size=0.25, random_state=123 ) # train models with
 AutoML automl = AutoML(mode="Perform") automl.fit(X_train, y_train) # compute
 the accuracy on test data predictions = automl.predict_all(X_test) print
 (predictions.head()) print("Test accuracy:", accuracy_score(y_test, predictions
 ["label"].astype(int))) ``` ## :point_right: Regression Example Regression
-example on Boston house prices data. On test data it scores ~ 10.85 mean
-squared error (MSE). ```python import numpy as np import pandas as pd from
-sklearn.datasets import load_boston from sklearn.model_selection import
-train_test_split from sklearn.metrics import mean_squared_error from
-supervised.automl import AutoML # mljar-supervised # Load the data housing =
-load_boston() X_train, X_test, y_train, y_test = train_test_split( pd.DataFrame
-(housing.data, columns=housing.feature_names), housing.target, test_size=0.25,
+example on `California Housing` house prices data. ```python import numpy as np
+import pandas as pd from sklearn.datasets import fetch_california_housing from
+sklearn.model_selection import train_test_split from sklearn.metrics import
+mean_squared_error from supervised.automl import AutoML # mljar-supervised #
+Load the data housing = fetch_california_housing() X_train, X_test, y_train,
+y_test = train_test_split( pd.DataFrame(housing.data,
+columns=housing.feature_names), housing.target, test_size=0.25,
 random_state=123, ) # train models with AutoML automl = AutoML(mode="Explain")
 automl.fit(X_train, y_train) # compute the MSE on test data predictions =
 automl.predict(X_test) print("Test MSE:", mean_squared_error(y_test,
 predictions)) ``` ## :point_right: More Examples - [**Income classification**]
 (https://github.com/mljar/mljar-examples/tree/master/Income_classification) -
 it is a binary classification task on census data - [**Iris classification**]
 (https://github.com/mljar/mljar-examples/tree/master/Iris_classification) - it
 is a multiclass classification on Iris flowers data - [**House price
 regression**](https://github.com/mljar/mljar-examples/tree/master/
-House_price_regression) - it is a regression task on Boston houses data #
-Documentation :books: For details please check [mljar-supervised docs](https://
-supervised.mljar.com). # Installation :package: From PyPi repository: ``` pip
-install mljar-supervised ``` From source code: ``` git clone https://
-github.com/mljar/mljar-supervised.git cd mljar-supervised python setup.py
-install ``` Installation for development ``` git clone https://github.com/
-mljar/mljar-supervised.git virtualenv venv --python=python3.6 source venv/bin/
-activate pip install -r requirements.txt pip install -r requirements_dev.txt
-``` Running in the docker: ``` FROM python:3.7-slim-buster RUN apt-get update
-&& apt-get -y update RUN apt-get install -y build-essential python3-pip
-python3-dev RUN pip3 -q install pip --upgrade RUN pip3 install mljar-supervised
-jupyter CMD ["jupyter", "notebook", "--port=8888", "--no-browser", "--
-ip=0.0.0.0", "--allow-root"] ``` # Contributing To get started take a look at
-our [Contribution Guide](https://supervised.mljar.com/contributing/) for
-information about our process and where you can fit in! ### Contributors
-[https://contributors-img.web.app/image?repo=mljar/mljar-supervised] # License
-:necktie: The `mljar-supervised` is provided with [MIT license](https://
-github.com/mljar/mljar-supervised/blob/master/LICENSE). # MLJAR :heart:
+House_price_regression) - it is a regression task on Boston houses data # FAQ
+What method is used for hyperparameters optimization? - For modes: `Explain`,
+`Perform` and `Compete` there is used a random search method combined with hill
+climbing. In this approach all checked models are saved and used for building
+Ensemble. - For mode: `Optuna` the Optuna framework is used. It is using TPE
+sampler for tuning. Models checked during Optuna hyperparameters search are not
+saved, only the best model is saved (final model from tuning). You can check
+the details about checked hyperparameters from optuna by checking study files
+in `optuna` directory in your AutoML `results_path`.  How to save and load
+AutoML? The save and load of AutoML models is automatic. All models created
+during AutoML training are saved in the directory set in `results_path`
+(argument of `AutoML()` constructor). If there is no `results_path` set, then
+the directory is created based on following name convention: `AutoML_{number}`
+the `number` will be number from 1 to 1000 (depends which directory name will
+be free). Example save and load: ```python automl = AutoML
+(results_path='AutoML_1') automl.fit(X, y) ``` The all models from AutoML are
+saved in `AutoML_1` directory. To load models: ```python automl = AutoML
+(results_path='AutoML_1') automl.predict(X) ```  How to set ML task (select
+between classification or regression)? The MLJAR AutoML can work with: - binary
+classification - multi-class classification - regression The ML task detection
+is automatic based on target values. There can be situation if you want to
+manually force AutoML to select the ML task, then you need to set `ml_task`
+parameter. It can be set to `'binary_classification'`,
+`'multiclass_classification'`, `'regression'`. Example: ```python automl =
+AutoML(ml_task='regression') automl.fit(X, y) ``` In the above example the
+regression model will be fitted.  How to reuse Optuna hyperparameters? You can
+reuse Optuna hyperparameters that were found in other AutoML training. You need
+to pass them in `optuna_init_params` argument. All hyperparameters found during
+Optuna tuning are saved in the `optuna/optuna.json` file (inside `results_path`
+directory). Example: ```python optuna_init = json.loads(open
+('previous_AutoML_training/optuna/optuna.json').read()) automl = AutoML
+( mode='Optuna', optuna_init_params=optuna_init ) automl.fit(X, y) ``` When
+reusing Optuna hyperparameters the Optuna tuning is simply skipped. The model
+will be trained with hyperparameters set in `optuna_init_params`. Right now
+there is no option to continue Optuna tuning with seed parameters.  How to know
+the order of classes for binary or multiclass problem when using predict_proba?
+To get predicted probabilites with information about class label please use the
+`predict_all()` method. It returns the pandas DataFrame with class names in the
+columns. The order of predicted columns is the same in the `predict_proba()`
+and `predict_all()` methods. The `predict_all()` method will additionaly have
+the column with the predicted class label.  # Documentation For details please
+check [mljar-supervised docs](https://supervised.mljar.com). # Installation
+From PyPi repository: ``` pip install mljar-supervised ``` To install this
+package with conda run: ``` conda install -c conda-forge mljar-supervised ```
+From source code: ``` git clone https://github.com/mljar/mljar-supervised.git
+cd mljar-supervised python setup.py install ``` Installation for development
+``` git clone https://github.com/mljar/mljar-supervised.git virtualenv venv --
+python=python3.6 source venv/bin/activate pip install -r requirements.txt pip
+install -r requirements_dev.txt ``` Running in the docker: ``` FROM python:3.7-
+slim-buster RUN apt-get update && apt-get -y update RUN apt-get install -
+y build-essential python3-pip python3-dev RUN pip3 -q install pip --upgrade RUN
+pip3 install mljar-supervised jupyter CMD ["jupyter", "notebook", "--
+port=8888", "--no-browser", "--ip=0.0.0.0", "--allow-root"] ``` Install from
+GitHub with pip: ``` pip install -q -U git+https://github.com/mljar/mljar-
+supervised.git@master ``` # Demo In the below demo GIF you will see: - MLJAR
+AutoML trained in Jupyter Notebook on titanic dataset - overview of created
+files - showcase of selected plots created during AutoML training - algorithm
+comparison report along with their plots - example of README file and csv file
+with results ![](https://github.com/mljar/mljar-examples/raw/master/media/
+mljar_files.gif) # Contributing To get started take a look at our [Contribution
+Guide](https://supervised.mljar.com/contributing/) for information about our
+process and where you can fit in! ### Contributors [https://contributors-
+img.web.app/image?repo=mljar/mljar-supervised] # Cite Would you like to cite
+MLJAR? Great! :) You can cite MLJAR as following: ``` @misc{mljar, author =
+{Aleksandra P\l{}o\'{n}ska and Piotr P\l{}o\'{n}ski}, year = {2021}, publisher
+= {MLJAR}, address = {\L{}apy, Poland}, title = {MLJAR: State-of-the-art
+Automated Machine Learning Framework for Tabular Data. Version 0.10.3}, url =
+{https://github.com/mljar/mljar-supervised} } ``` Would love to hear from you
+how have you used MLJAR AutoML in your project. Please feel free to let us know
+at ![image](https://user-images.githubusercontent.com/6959032/118103228-
+f5ea9a00-b3d9-11eb-87ed-8cfb1f873f91.png) # License The `mljar-supervised` is
+provided with [MIT license](https://github.com/mljar/mljar-supervised/blob/
+master/LICENSE). # Commercial support Looking for commercial support? Do you
+need new feature implementation? Please contact us by [email](https://
+mljar.com/contact/) for details. # MLJAR
   [https://github.com/mljar/mljar-examples/blob/master/media/large_logo.png]
 The `mljar-supervised` is an open-source project created by [MLJAR](https://
 mljar.com). We care about ease of use in the Machine Learning. The [mljar.com]
 (https://mljar.com) provides a beautiful and simple user interface for building
 machine learning models.
```

### Comparing `mljar-supervised-0.9.1/PKG-INFO` & `mljar-supervised-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,99 @@
 Metadata-Version: 2.1
 Name: mljar-supervised
-Version: 0.9.1
+Version: 1.0.0
 Summary: Automated Machine Learning for Humans
 Home-page: https://github.com/mljar/mljar-supervised
-Author: MLJAR, Inc.
+Author: MLJAR, Sp. z o.o.
 Author-email: contact@mljar.com
 License: MIT
 Description: # MLJAR Automated Machine Learning for Humans
         
-        [![Build Status](https://travis-ci.org/mljar/mljar-supervised.svg?branch=master)](https://travis-ci.org/mljar/mljar-supervised)
-        [![Coverage Status](https://coveralls.io/repos/github/mljar/mljar-supervised/badge.svg?branch=master)](https://coveralls.io/github/mljar/mljar-supervised?branch=master)
+        [![Tests status](https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml/badge.svg)](https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml)
         [![PyPI version](https://badge.fury.io/py/mljar-supervised.svg)](https://badge.fury.io/py/mljar-supervised)
+        [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/version.svg)](https://anaconda.org/conda-forge/mljar-supervised)
         [![PyPI pyversions](https://img.shields.io/pypi/pyversions/mljar-supervised.svg)](https://pypi.python.org/pypi/mljar-supervised/)
-        
+        [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/platforms.svg)](https://anaconda.org/conda-forge/mljar-supervised)
+        [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/license.svg)](https://anaconda.org/conda-forge/mljar-supervised)
+        [![Downloads](https://pepy.tech/badge/mljar-supervised)](https://pepy.tech/project/mljar-supervised)
         
         <p align="center">
           <img src="https://raw.githubusercontent.com/mljar/mljar-examples/master/media/AutoML_overview_mljar_v3.svg" width="100%" />
         </p>
         
         ---
         
         **Documentation**: <a href="https://supervised.mljar.com/" target="_blank">https://supervised.mljar.com/</a>
         
         **Source Code**: <a href="https://github.com/mljar/mljar-supervised" target="_blank">https://github.com/mljar/mljar-supervised</a>
         
+        **Looking for commercial support**: Please contact us by [email](https://mljar.com/contact/) for details
+        
+        
+        <p align="center">
+          <img src="https://github.com/mljar/visual-identity/raw/main/robots/robot_docs.png" width="40%" />
+        </p>
+        
+        
+        
         ---
         
         ## Table of Contents
         
-         - [Automated Machine Learning](https://github.com/mljar/mljar-supervised#automated-machine-learning-rocket)
-         - [What's good in it?](https://github.com/mljar/mljar-supervised#whats-good-in-it-boom)
-         - [Atomatic Documentation](https://github.com/mljar/mljar-supervised#automatic-documentation)
-         - [Available Modes](https://github.com/mljar/mljar-supervised#available-modes-books)
+         - [Automated Machine Learning](https://github.com/mljar/mljar-supervised#automated-machine-learning)
+         - [What's good in it?](https://github.com/mljar/mljar-supervised#whats-good-in-it)
+         - [Automatic Documentation](https://github.com/mljar/mljar-supervised#automatic-documentation)
+         - [Available Modes](https://github.com/mljar/mljar-supervised#available-modes)
          - [Examples](https://github.com/mljar/mljar-supervised#examples)
+         - [FAQ](https://github.com/mljar/mljar-supervised#faq)
          - [Documentation](https://github.com/mljar/mljar-supervised#documentation)
-         - [Installation](https://github.com/mljar/mljar-supervised#installation-package)
+         - [Installation](https://github.com/mljar/mljar-supervised#installation)
+         - [Demo](https://github.com/mljar/mljar-supervised#demo)
          - [Contributing](https://github.com/mljar/mljar-supervised#contributing)
-         - [License](https://github.com/mljar/mljar-supervised#license-necktie)
-         - [MLJAR](https://github.com/mljar/mljar-supervised#mljar-heart)
+         - [Cite](https://github.com/mljar/mljar-supervised#cite)
+         - [License](https://github.com/mljar/mljar-supervised#license)
+         - [Commercial support](https://github.com/mljar/mljar-supervised#commercial-support)
+         - [MLJAR](https://github.com/mljar/mljar-supervised#mljar)
+         
         
-        ## Automated Machine Learning :rocket: 
+        # Automated Machine Learning 
         
         The `mljar-supervised` is an Automated Machine Learning Python package that works with tabular data. It is designed to save time for a data scientist. It abstracts the common way to preprocess the data, construct the machine learning models, and perform hyper-parameters tuning to find the best model :trophy:. It is no black-box as you can see exactly how the ML pipeline is constructed (with a detailed Markdown report for each ML model). 
         
         The `mljar-supervised` will help you with:
          - explaining and understanding your data (Automatic Exploratory Data Analysis),
          - trying many different machine learning models (Algorithm Selection and Hyper-Parameters tuning),
-         - creating Markdown reports from analysis with details about all models (Atomatic-Documentation),
+         - creating Markdown reports from analysis with details about all models (Automatic-Documentation),
          - saving, re-running and loading the analysis and ML models.
         
-        It has three built-in modes of work:
+        It has four built-in modes of work:
          - `Explain` mode, which is ideal for explaining and understanding the data, with many data explanations, like decision trees visualization, linear models coefficients display, permutation importances and SHAP explanations of data,
          - `Perform` for building ML pipelines to use in production,
          - `Compete` mode that trains highly-tuned ML models with ensembling and stacking, with a purpose to use in ML competitions.
+         - `Optuna` mode that can be used to search for highly-tuned ML models, should be used when the performance is the most important, and computation time is not limited (it is available from version `0.10.0`)
         
         Of course, you can further customize the details of each `mode` to meet the requirements.
         
-        ## What's good in it? :boom:
+        ## What's good in it? 
         
         - It is using many algorithms: `Baseline`, `Linear`, `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, `CatBoost`, `Neural Networks`, and `Nearest Neighbors`.
         - It can compute Ensemble based on greedy algorithm from [Caruana paper](http://www.cs.cornell.edu/~alexn/papers/shotgun.icml04.revised.rev2.pdf).
         - It can stack models to build level 2 ensemble (available in `Compete` mode or after setting `stack_models` parameter).
         - It can do features preprocessing, like: missing values imputation and converting categoricals. What is more, it can also handle target values preprocessing.
         - It can do advanced features engineering, like: [Golden Features](https://supervised.mljar.com/features/golden_features/), [Features Selection](https://supervised.mljar.com/features/features_selection/), Text and Time Transformations.
         - It can tune hyper-parameters with `not-so-random-search` algorithm (random-search over defined set of values) and hill climbing to fine-tune final models.
         - It can compute the `Baseline` for your data. That you will know if you need Machine Learning or not!
         - It has extensive explanations. This package is training simple `Decision Trees` with `max_depth <= 5`, so you can easily visualize them with amazing [dtreeviz](https://github.com/parrt/dtreeviz) to better understand your data.
         - The `mljar-supervised` is using simple linear regression and include its coefficients in the summary report, so you can check which features are used the most in the linear model.
         - It cares about explainability of models: for every algorithm, the feature importance is computed based on permutation. Additionally, for every algorithm the SHAP explanations are computed: feature importance, dependence plots, and decision plots (explanations can be switched off with `explain_level` parameter).
-        - There is automatic documnetation for every ML experiment run with AutoML. The `mljar-supervised` creates markdown reports from AutoML training full of ML details, metrics and charts. 
+        - There is automatic documentation for every ML experiment run with AutoML. The `mljar-supervised` creates markdown reports from AutoML training full of ML details, metrics and charts. 
+        
+        <p align="center">
+          <img src="https://raw.githubusercontent.com/mljar/visual-identity/main/media/infograph.png" width="100%" />
+        </p>
         
         # Automatic Documentation
         
         ## The AutoML Report
         
         The report from running AutoML will contain the table with infomation about each model score and time needed to train the model. For each model there is a link, which you can click to see model's details. The performance of all ML models is presented as scatter and box plots so you can visually inspect which algorithms perform the best :trophy:.
         
@@ -92,18 +113,22 @@
         ## The `LightGBM` Report
         
         The example for `LightGBM` summary:
         
         ![Decision Tree summary](https://github.com/mljar/mljar-examples/blob/master/media/lightgbm_summary.gif)
         
         
-        ## Available Modes :books:
+        ## Available Modes
         
         In the [docs](https://supervised.mljar.com/features/modes/) you can find details about AutoML modes are presented in the table .
         
+        <p align="center">
+          <img src="https://raw.githubusercontent.com/mljar/visual-identity/main/media/mljar_modes.png" width="100%" />
+        </p>
+        
         ### Explain 
         
         ```py
         automl = AutoML(mode="Explain")
         ```
         
         It is aimed to be used when the user wants to explain and understand the data.
@@ -129,14 +154,62 @@
         ```
         
         It should be used for machine learning competitions.
          - It adapts the validation strategy depending on dataset size and `total_time_limit`. It can be: train/test split (80/20), 5-fold CV or 10-fold CV. 
          - It is using: `Linear`, `Decision Tree`, `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, `CatBoost`, `Neural Network` and `Nearest Neighbors`. It uses ensemble and **stacking**. 
          - It has only learning curves in the reports.
         
+        ### Optuna
+        
+        ```py
+        automl = AutoML(mode="Optuna", optuna_time_budget=3600)
+        ```
+        
+        It should be used when the performance is the most important and time is not limited.
+        - It is using 10-fold CV
+        - It is using: `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, and `CatBoost`. Those algorithms are tuned by `Optuna` framework for `optuna_time_budget` seconds, each. Algorithms are tuned with original data, without advanced feature engineering.
+        - It is using advanced feature engineering, stacking and ensembling. The hyperparameters found for original data are reused with those steps.
+        - It produces learning curves in the reports.
+        
+        ## How to save and load AutoML?
+        
+        All models in the AutoML are saved and loaded automatically. No need to call `save()` or `load()`.
+        
+        ### Example:
+        
+        #### Train AutoML
+        
+        ```python
+        automl = AutoML(results_path="AutoML_classifier")
+        automl.fit(X, y)
+        ```
+        
+        You will have all models saved in the `AutoML_classifier` directory. Each model will have a separate directory with the `README.md` file with all details from the training.
+        
+        #### Compute predictions
+        ```python
+        automl = AutoML(results_path="AutoML_classifier")
+        automl.predict(X)
+        ```
+        
+        The  AutoML automatically loads models from the `results_path` directory. If you will call `fit()` on already trained AutoML then you will get a warning message that AutoML is already fitted.
+        
+        
+        ### Why do you automatically save all models?
+        
+        All models are automatically saved to be able to restore the training after interruption. For example, you are training AutoML for 48 hours, and after 47 hours there is some unexpected interruption. In MLJAR AutoML you just call the same training code after the interruption and AutoML reloads already trained models and finish the training.
+        
+        ## Supported evaluation metrics (`eval_metric` argument in `AutoML()`)
+        
+        - for binary classification: `logloss`, `auc`, `f1`, `average_precision`, `accuracy`- default is `logloss`
+        - for mutliclass classification: `logloss`, `f1`, `accuracy` - default is `logloss`
+        - for regression: `rmse`, `mse`, `mae`, `r2`, `mape`, `spearman`, `pearson` - default is `rmse`
+        
+        If you don't find `eval_metric` that you need, please add a new issue. We will add it.
+        
         # Examples
         
         ## :point_right: Binary Classification Example
         
         There is a simple interface available with `fit` and `predict` methods.
         
         ```python
@@ -207,26 +280,26 @@
         predictions = automl.predict_all(X_test)
         print(predictions.head())
         print("Test accuracy:", accuracy_score(y_test, predictions["label"].astype(int)))
         ```
         
         ## :point_right: Regression Example
         
-        Regression example on Boston house prices data. On test data it scores ~ 10.85 mean squared error (MSE).
+        Regression example on `California Housing` house prices data.
         
         ```python
         import numpy as np
         import pandas as pd
-        from sklearn.datasets import load_boston
+        from sklearn.datasets import fetch_california_housing
         from sklearn.model_selection import train_test_split
         from sklearn.metrics import mean_squared_error
         from supervised.automl import AutoML # mljar-supervised
         
         # Load the data
-        housing = load_boston()
+        housing = fetch_california_housing()
         X_train, X_test, y_train, y_test = train_test_split(
             pd.DataFrame(housing.data, columns=housing.feature_names),
             housing.target,
             test_size=0.25,
             random_state=123,
         )
         
@@ -241,26 +314,106 @@
         
         ## :point_right: More Examples
         
         - [**Income classification**](https://github.com/mljar/mljar-examples/tree/master/Income_classification) - it is a binary classification task on census data
         - [**Iris classification**](https://github.com/mljar/mljar-examples/tree/master/Iris_classification) - it is a multiclass classification on Iris flowers data
         - [**House price regression**](https://github.com/mljar/mljar-examples/tree/master/House_price_regression) - it is a regression task on Boston houses data
         
-        # Documentation :books:
+        # FAQ
+        
+        <details><summary>What method is used for hyperparameters optimization?</summary>
+          - For modes: `Explain`, `Perform` and `Compete` there is used a random search method combined with hill climbing. In this approach all checked models are saved and used for building Ensemble.
+          - For mode: `Optuna` the Optuna framework is used. It is using TPE sampler for tuning. Models checked during Optuna hyperparameters search are not saved, only the best model is saved (final model from tuning). You can check the details about checked hyperparameters from optuna by checking study files in `optuna` directory in your AutoML `results_path`.
+        </details>
+        
+        <details><summary>How to save and load AutoML?</summary>
+        
+        The save and load of AutoML models is automatic. All models created during AutoML training are saved in the directory set in `results_path` (argument of `AutoML()` constructor). If there is no `results_path` set, then the directory is created based on following name convention: `AutoML_{number}` the `number` will be number from 1 to 1000 (depends which directory name will be free).
+        
+        Example save and load:
+        
+        ```python
+        automl = AutoML(results_path='AutoML_1')
+        automl.fit(X, y)
+        ```
+        
+        The all models from AutoML are saved in `AutoML_1` directory.
+        
+        To load models:
+        
+        ```python
+        automl = AutoML(results_path='AutoML_1')
+        automl.predict(X)
+        ```
+        
+        </details>
+        
+        <details><summary>How to set ML task (select between classification or regression)?</summary>
+        
+        The MLJAR AutoML can work with:
+        - binary classification
+        - multi-class classification
+        - regression
+        
+        The ML task detection is automatic based on target values. There can be situation if you want to manually force AutoML to select the ML task, then you need to set `ml_task` parameter. It can be set to `'binary_classification'`, `'multiclass_classification'`, `'regression'`.
+        
+        Example:
+        ```python
+        automl = AutoML(ml_task='regression')
+        automl.fit(X, y)
+        ```
+        In the above example the regression model will be fitted.
+        
+        </details>
+        
+        <details><summary>How to reuse Optuna hyperparameters?</summary>
+          
+          You can reuse Optuna hyperparameters that were found in other AutoML training. You need to pass them in `optuna_init_params` argument. All hyperparameters found during Optuna tuning are saved in the `optuna/optuna.json` file (inside `results_path` directory).
+          
+         Example:
+         
+         ```python
+         optuna_init = json.loads(open('previous_AutoML_training/optuna/optuna.json').read())
+         
+         automl = AutoML(
+             mode='Optuna',
+             optuna_init_params=optuna_init
+         )
+         automl.fit(X, y)
+         ```
+          
+         When reusing Optuna hyperparameters the Optuna tuning is simply skipped. The model will be trained with hyperparameters set in `optuna_init_params`. Right now there is no option to continue Optuna tuning with seed parameters.
+          
+          
+        </details>
+        
+        
+        <details><summary>How to know the order of classes for binary or multiclass problem when using predict_proba?</summary>
+        
+        To get predicted probabilites with information about class label please use the `predict_all()` method. It returns the pandas DataFrame with class names in the columns. The order of predicted columns is the same in the `predict_proba()` and `predict_all()` methods. The `predict_all()` method will additionaly have the column with the predicted class label.
+        
+        </details>
+        
+        # Documentation  
         
         For details please check [mljar-supervised docs](https://supervised.mljar.com).
         
-        # Installation :package: 
+        # Installation  
         
         From PyPi repository:
         
         ```
         pip install mljar-supervised
         ```
         
+        To install this package with conda run:
+        ```
+        conda install -c conda-forge mljar-supervised
+        ```
+        
         From source code:
         
         ```
         git clone https://github.com/mljar/mljar-supervised.git
         cd mljar-supervised
         python setup.py install
         ```
@@ -280,35 +433,77 @@
         RUN apt-get update && apt-get -y update
         RUN apt-get install -y build-essential python3-pip python3-dev
         RUN pip3 -q install pip --upgrade
         RUN pip3 install mljar-supervised jupyter
         CMD ["jupyter", "notebook", "--port=8888", "--no-browser", "--ip=0.0.0.0", "--allow-root"]
         ```
         
+        Install from GitHub with pip:
+        ```
+        pip install -q -U git+https://github.com/mljar/mljar-supervised.git@master
+        ```
+        # Demo
+        
+        In the below demo GIF you will see:
+        - MLJAR AutoML trained in Jupyter Notebook on titanic dataset
+        - overview of created files
+        - showcase of selected plots created during AutoML training
+        - algorithm comparison report along with their plots
+        - example of README file and csv file with results
+        
+        ![](https://github.com/mljar/mljar-examples/raw/master/media/mljar_files.gif)
+        
         # Contributing
         
         To get started take a look at our [Contribution Guide](https://supervised.mljar.com/contributing/) for information about our process and where you can fit in!
         
         ### Contributors
         <a href="https://github.com/mljar/mljar-supervised/graphs/contributors">
           <img src="https://contributors-img.web.app/image?repo=mljar/mljar-supervised" />
         </a>
         
+        # Cite
+        
+        Would you like to cite MLJAR? Great! :)
+        
+        You can cite MLJAR as following:
+        
+        ```
+        @misc{mljar,
+          author    = {Aleksandra P\l{}o\'{n}ska and Piotr P\l{}o\'{n}ski},
+          year      = {2021},
+          publisher = {MLJAR},
+          address   = {\L{}apy, Poland},
+          title     = {MLJAR: State-of-the-art Automated Machine Learning Framework for Tabular Data.  Version 0.10.3},
+          url       = {https://github.com/mljar/mljar-supervised}
+        }
+        ```
+        
+        Would love to hear from you how have you used MLJAR AutoML in your project. 
+        Please feel free to let us know at 
+        ![image](https://user-images.githubusercontent.com/6959032/118103228-f5ea9a00-b3d9-11eb-87ed-8cfb1f873f91.png)
+        
         
-        # License :necktie:
+        # License  
         
         The `mljar-supervised` is provided with [MIT license](https://github.com/mljar/mljar-supervised/blob/master/LICENSE).
         
-        # MLJAR :heart:
+        # Commercial support
+        
+        Looking for commercial support? Do you need new feature implementation? Please contact us by [email](https://mljar.com/contact/) for details.
+        
+        # MLJAR 
         <p align="center">
           <img src="https://github.com/mljar/mljar-examples/blob/master/media/large_logo.png" width="314" />
         </p>
         
         The `mljar-supervised` is an open-source project created by [MLJAR](https://mljar.com). We care about ease of use in the Machine Learning. 
         The [mljar.com](https://mljar.com) provides a beautiful and simple user interface for building machine learning models.
         
 Keywords: automated machine learning,automl,machine learning,data science,data mining,mljar
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,122 +1,170 @@
-Metadata-Version: 2.1 Name: mljar-supervised Version: 0.9.1 Summary: Automated
+Metadata-Version: 2.1 Name: mljar-supervised Version: 1.0.0 Summary: Automated
 Machine Learning for Humans Home-page: https://github.com/mljar/mljar-
-supervised Author: MLJAR, Inc. Author-email: contact@mljar.com License: MIT
-Description: # MLJAR Automated Machine Learning for Humans [![Build Status]
-(https://travis-ci.org/mljar/mljar-supervised.svg?branch=master)](https://
-travis-ci.org/mljar/mljar-supervised) [![Coverage Status](https://coveralls.io/
-repos/github/mljar/mljar-supervised/badge.svg?branch=master)](https://
-coveralls.io/github/mljar/mljar-supervised?branch=master) [![PyPI version]
-(https://badge.fury.io/py/mljar-supervised.svg)](https://badge.fury.io/py/
-mljar-supervised) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/
-mljar-supervised.svg)](https://pypi.python.org/pypi/mljar-supervised/)
+supervised Author: MLJAR, Sp. z o.o. Author-email: contact@mljar.com License:
+MIT Description: # MLJAR Automated Machine Learning for Humans [![Tests status]
+(https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml/
+badge.svg)](https://github.com/mljar/mljar-supervised/actions/workflows/run-
+tests.yml) [![PyPI version](https://badge.fury.io/py/mljar-supervised.svg)]
+(https://badge.fury.io/py/mljar-supervised) [![Anaconda-Server Badge](https://
+anaconda.org/conda-forge/mljar-supervised/badges/version.svg)](https://
+anaconda.org/conda-forge/mljar-supervised) [![PyPI pyversions](https://
+img.shields.io/pypi/pyversions/mljar-supervised.svg)](https://pypi.python.org/
+pypi/mljar-supervised/) [![Anaconda-Server Badge](https://anaconda.org/conda-
+forge/mljar-supervised/badges/platforms.svg)](https://anaconda.org/conda-forge/
+mljar-supervised) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/
+mljar-supervised/badges/license.svg)](https://anaconda.org/conda-forge/mljar-
+supervised) [![Downloads](https://pepy.tech/badge/mljar-supervised)](https://
+pepy.tech/project/mljar-supervised)
      [https://raw.githubusercontent.com/mljar/mljar-examples/master/media/
                          AutoML_overview_mljar_v3.svg]
 --- **Documentation**: https://supervised.mljar.com/ **Source Code**: https://
-github.com/mljar/mljar-supervised --- ## Table of Contents - [Automated Machine
-Learning](https://github.com/mljar/mljar-supervised#automated-machine-learning-
-rocket) - [What's good in it?](https://github.com/mljar/mljar-supervised#whats-
-good-in-it-boom) - [Atomatic Documentation](https://github.com/mljar/mljar-
-supervised#automatic-documentation) - [Available Modes](https://github.com/
-mljar/mljar-supervised#available-modes-books) - [Examples](https://github.com/
-mljar/mljar-supervised#examples) - [Documentation](https://github.com/mljar/
-mljar-supervised#documentation) - [Installation](https://github.com/mljar/
-mljar-supervised#installation-package) - [Contributing](https://github.com/
-mljar/mljar-supervised#contributing) - [License](https://github.com/mljar/
-mljar-supervised#license-necktie) - [MLJAR](https://github.com/mljar/mljar-
-supervised#mljar-heart) ## Automated Machine Learning :rocket: The `mljar-
-supervised` is an Automated Machine Learning Python package that works with
-tabular data. It is designed to save time for a data scientist. It abstracts
-the common way to preprocess the data, construct the machine learning models,
-and perform hyper-parameters tuning to find the best model :trophy:. It is no
-black-box as you can see exactly how the ML pipeline is constructed (with a
-detailed Markdown report for each ML model). The `mljar-supervised` will help
-you with: - explaining and understanding your data (Automatic Exploratory Data
-Analysis), - trying many different machine learning models (Algorithm Selection
-and Hyper-Parameters tuning), - creating Markdown reports from analysis with
-details about all models (Atomatic-Documentation), - saving, re-running and
-loading the analysis and ML models. It has three built-in modes of work: -
-`Explain` mode, which is ideal for explaining and understanding the data, with
-many data explanations, like decision trees visualization, linear models
-coefficients display, permutation importances and SHAP explanations of data, -
-`Perform` for building ML pipelines to use in production, - `Compete` mode that
-trains highly-tuned ML models with ensembling and stacking, with a purpose to
-use in ML competitions. Of course, you can further customize the details of
-each `mode` to meet the requirements. ## What's good in it? :boom: - It is
-using many algorithms: `Baseline`, `Linear`, `Random Forest`, `Extra Trees`,
-`LightGBM`, `Xgboost`, `CatBoost`, `Neural Networks`, and `Nearest Neighbors`.
-- It can compute Ensemble based on greedy algorithm from [Caruana paper](http:/
-/www.cs.cornell.edu/~alexn/papers/shotgun.icml04.revised.rev2.pdf). - It can
-stack models to build level 2 ensemble (available in `Compete` mode or after
-setting `stack_models` parameter). - It can do features preprocessing, like:
-missing values imputation and converting categoricals. What is more, it can
-also handle target values preprocessing. - It can do advanced features
-engineering, like: [Golden Features](https://supervised.mljar.com/features/
-golden_features/), [Features Selection](https://supervised.mljar.com/features/
-features_selection/), Text and Time Transformations. - It can tune hyper-
-parameters with `not-so-random-search` algorithm (random-search over defined
-set of values) and hill climbing to fine-tune final models. - It can compute
-the `Baseline` for your data. That you will know if you need Machine Learning
-or not! - It has extensive explanations. This package is training simple
-`Decision Trees` with `max_depth <= 5`, so you can easily visualize them with
-amazing [dtreeviz](https://github.com/parrt/dtreeviz) to better understand your
-data. - The `mljar-supervised` is using simple linear regression and include
-its coefficients in the summary report, so you can check which features are
-used the most in the linear model. - It cares about explainability of models:
-for every algorithm, the feature importance is computed based on permutation.
-Additionally, for every algorithm the SHAP explanations are computed: feature
-importance, dependence plots, and decision plots (explanations can be switched
-off with `explain_level` parameter). - There is automatic documnetation for
-every ML experiment run with AutoML. The `mljar-supervised` creates markdown
-reports from AutoML training full of ML details, metrics and charts. #
-Automatic Documentation ## The AutoML Report The report from running AutoML
+github.com/mljar/mljar-supervised **Looking for commercial support**: Please
+contact us by [email](https://mljar.com/contact/) for details
+   [https://github.com/mljar/visual-identity/raw/main/robots/robot_docs.png]
+--- ## Table of Contents - [Automated Machine Learning](https://github.com/
+mljar/mljar-supervised#automated-machine-learning) - [What's good in it?]
+(https://github.com/mljar/mljar-supervised#whats-good-in-it) - [Automatic
+Documentation](https://github.com/mljar/mljar-supervised#automatic-
+documentation) - [Available Modes](https://github.com/mljar/mljar-
+supervised#available-modes) - [Examples](https://github.com/mljar/mljar-
+supervised#examples) - [FAQ](https://github.com/mljar/mljar-supervised#faq) -
+[Documentation](https://github.com/mljar/mljar-supervised#documentation) -
+[Installation](https://github.com/mljar/mljar-supervised#installation) - [Demo]
+(https://github.com/mljar/mljar-supervised#demo) - [Contributing](https://
+github.com/mljar/mljar-supervised#contributing) - [Cite](https://github.com/
+mljar/mljar-supervised#cite) - [License](https://github.com/mljar/mljar-
+supervised#license) - [Commercial support](https://github.com/mljar/mljar-
+supervised#commercial-support) - [MLJAR](https://github.com/mljar/mljar-
+supervised#mljar) # Automated Machine Learning The `mljar-supervised` is an
+Automated Machine Learning Python package that works with tabular data. It is
+designed to save time for a data scientist. It abstracts the common way to
+preprocess the data, construct the machine learning models, and perform hyper-
+parameters tuning to find the best model :trophy:. It is no black-box as you
+can see exactly how the ML pipeline is constructed (with a detailed Markdown
+report for each ML model). The `mljar-supervised` will help you with: -
+explaining and understanding your data (Automatic Exploratory Data Analysis), -
+trying many different machine learning models (Algorithm Selection and Hyper-
+Parameters tuning), - creating Markdown reports from analysis with details
+about all models (Automatic-Documentation), - saving, re-running and loading
+the analysis and ML models. It has four built-in modes of work: - `Explain`
+mode, which is ideal for explaining and understanding the data, with many data
+explanations, like decision trees visualization, linear models coefficients
+display, permutation importances and SHAP explanations of data, - `Perform` for
+building ML pipelines to use in production, - `Compete` mode that trains
+highly-tuned ML models with ensembling and stacking, with a purpose to use in
+ML competitions. - `Optuna` mode that can be used to search for highly-tuned ML
+models, should be used when the performance is the most important, and
+computation time is not limited (it is available from version `0.10.0`) Of
+course, you can further customize the details of each `mode` to meet the
+requirements. ## What's good in it? - It is using many algorithms: `Baseline`,
+`Linear`, `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, `CatBoost`,
+`Neural Networks`, and `Nearest Neighbors`. - It can compute Ensemble based on
+greedy algorithm from [Caruana paper](http://www.cs.cornell.edu/~alexn/papers/
+shotgun.icml04.revised.rev2.pdf). - It can stack models to build level 2
+ensemble (available in `Compete` mode or after setting `stack_models`
+parameter). - It can do features preprocessing, like: missing values imputation
+and converting categoricals. What is more, it can also handle target values
+preprocessing. - It can do advanced features engineering, like: [Golden
+Features](https://supervised.mljar.com/features/golden_features/), [Features
+Selection](https://supervised.mljar.com/features/features_selection/), Text and
+Time Transformations. - It can tune hyper-parameters with `not-so-random-
+search` algorithm (random-search over defined set of values) and hill climbing
+to fine-tune final models. - It can compute the `Baseline` for your data. That
+you will know if you need Machine Learning or not! - It has extensive
+explanations. This package is training simple `Decision Trees` with `max_depth
+<= 5`, so you can easily visualize them with amazing [dtreeviz](https://
+github.com/parrt/dtreeviz) to better understand your data. - The `mljar-
+supervised` is using simple linear regression and include its coefficients in
+the summary report, so you can check which features are used the most in the
+linear model. - It cares about explainability of models: for every algorithm,
+the feature importance is computed based on permutation. Additionally, for
+every algorithm the SHAP explanations are computed: feature importance,
+dependence plots, and decision plots (explanations can be switched off with
+`explain_level` parameter). - There is automatic documentation for every ML
+experiment run with AutoML. The `mljar-supervised` creates markdown reports
+from AutoML training full of ML details, metrics and charts.
+     [https://raw.githubusercontent.com/mljar/visual-identity/main/media/
+                                infograph.png]
+# Automatic Documentation ## The AutoML Report The report from running AutoML
 will contain the table with infomation about each model score and time needed
 to train the model. For each model there is a link, which you can click to see
 model's details. The performance of all ML models is presented as scatter and
 box plots so you can visually inspect which algorithms perform the best :
 trophy:. ![AutoML leaderboard](https://github.com/mljar/mljar-examples/blob/
 master/media/automl_summary.gif) ## The `Decision Tree` Report The example for
 `Decision Tree` summary with trees visualization. For classification tasks
 additional metrics are provided: - confusion matrix - threshold (optimized in
 the case of binary classification task) - F1 score - Accuracy - Precision,
 Recall, MCC ![Decision Tree summary](https://github.com/mljar/mljar-examples/
 blob/master/media/decision_tree_summary.gif) ## The `LightGBM` Report The
 example for `LightGBM` summary: ![Decision Tree summary](https://github.com/
 mljar/mljar-examples/blob/master/media/lightgbm_summary.gif) ## Available Modes
-:books: In the [docs](https://supervised.mljar.com/features/modes/) you can
-find details about AutoML modes are presented in the table . ### Explain ```py
-automl = AutoML(mode="Explain") ``` It is aimed to be used when the user wants
-to explain and understand the data. - It is using 75%/25% train/test split. -
-It is using: `Baseline`, `Linear`, `Decision Tree`, `Random Forest`, `Xgboost`,
-`Neural Network` algorithms and ensemble. - It has full explanations: learning
-curves, importance plots, and SHAP plots. ### Perform ```py automl = AutoML
-(mode="Perform") ``` It should be used when the user wants to train a model
-that will be used in real-life use cases. - It is using 5-fold CV. - It is
-using: `Linear`, `Random Forest`, `LightGBM`, `Xgboost`, `CatBoost` and `Neural
-Network`. It uses ensembling. - It has learning curves and importance plots in
-reports. ### Compete ```py automl = AutoML(mode="Compete") ``` It should be
-used for machine learning competitions. - It adapts the validation strategy
-depending on dataset size and `total_time_limit`. It can be: train/test split
-(80/20), 5-fold CV or 10-fold CV. - It is using: `Linear`, `Decision Tree`,
-`Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, `CatBoost`, `Neural
-Network` and `Nearest Neighbors`. It uses ensemble and **stacking**. - It has
-only learning curves in the reports. # Examples ## :point_right: Binary
-Classification Example There is a simple interface available with `fit` and
-`predict` methods. ```python import pandas as pd from sklearn.model_selection
-import train_test_split from supervised.automl import AutoML df = pd.read_csv
-( "https://raw.githubusercontent.com/pplonski/datasets-for-start/master/adult/
-data.csv", skipinitialspace=True, ) X_train, X_test, y_train, y_test =
-train_test_split( df[df.columns[:-1]], df["income"], test_size=0.25 ) automl =
-AutoML() automl.fit(X_train, y_train) predictions = automl.predict(X_test) ```
-AutoML `fit` will print: ```py Create directory AutoML_1 AutoML task to be
-solved: binary_classification AutoML will use algorithms: ['Baseline',
-'Linear', 'Decision Tree', 'Random Forest', 'Xgboost', 'Neural Network'] AutoML
-will optimize for metric: logloss 1_Baseline final logloss 0.5519845471086654
-time 0.08 seconds 2_DecisionTree final logloss 0.3655910192804364 time 10.28
-seconds 3_Linear final logloss 0.38139916864708445 time 3.19 seconds
+In the [docs](https://supervised.mljar.com/features/modes/) you can find
+details about AutoML modes are presented in the table .
+     [https://raw.githubusercontent.com/mljar/visual-identity/main/media/
+                               mljar_modes.png]
+### Explain ```py automl = AutoML(mode="Explain") ``` It is aimed to be used
+when the user wants to explain and understand the data. - It is using 75%/25%
+train/test split. - It is using: `Baseline`, `Linear`, `Decision Tree`, `Random
+Forest`, `Xgboost`, `Neural Network` algorithms and ensemble. - It has full
+explanations: learning curves, importance plots, and SHAP plots. ### Perform
+```py automl = AutoML(mode="Perform") ``` It should be used when the user wants
+to train a model that will be used in real-life use cases. - It is using 5-fold
+CV. - It is using: `Linear`, `Random Forest`, `LightGBM`, `Xgboost`, `CatBoost`
+and `Neural Network`. It uses ensembling. - It has learning curves and
+importance plots in reports. ### Compete ```py automl = AutoML(mode="Compete")
+``` It should be used for machine learning competitions. - It adapts the
+validation strategy depending on dataset size and `total_time_limit`. It can
+be: train/test split (80/20), 5-fold CV or 10-fold CV. - It is using: `Linear`,
+`Decision Tree`, `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`,
+`CatBoost`, `Neural Network` and `Nearest Neighbors`. It uses ensemble and
+**stacking**. - It has only learning curves in the reports. ### Optuna ```py
+automl = AutoML(mode="Optuna", optuna_time_budget=3600) ``` It should be used
+when the performance is the most important and time is not limited. - It is
+using 10-fold CV - It is using: `Random Forest`, `Extra Trees`, `LightGBM`,
+`Xgboost`, and `CatBoost`. Those algorithms are tuned by `Optuna` framework for
+`optuna_time_budget` seconds, each. Algorithms are tuned with original data,
+without advanced feature engineering. - It is using advanced feature
+engineering, stacking and ensembling. The hyperparameters found for original
+data are reused with those steps. - It produces learning curves in the reports.
+## How to save and load AutoML? All models in the AutoML are saved and loaded
+automatically. No need to call `save()` or `load()`. ### Example: #### Train
+AutoML ```python automl = AutoML(results_path="AutoML_classifier") automl.fit
+(X, y) ``` You will have all models saved in the `AutoML_classifier` directory.
+Each model will have a separate directory with the `README.md` file with all
+details from the training. #### Compute predictions ```python automl = AutoML
+(results_path="AutoML_classifier") automl.predict(X) ``` The AutoML
+automatically loads models from the `results_path` directory. If you will call
+`fit()` on already trained AutoML then you will get a warning message that
+AutoML is already fitted. ### Why do you automatically save all models? All
+models are automatically saved to be able to restore the training after
+interruption. For example, you are training AutoML for 48 hours, and after 47
+hours there is some unexpected interruption. In MLJAR AutoML you just call the
+same training code after the interruption and AutoML reloads already trained
+models and finish the training. ## Supported evaluation metrics (`eval_metric`
+argument in `AutoML()`) - for binary classification: `logloss`, `auc`, `f1`,
+`average_precision`, `accuracy`- default is `logloss` - for mutliclass
+classification: `logloss`, `f1`, `accuracy` - default is `logloss` - for
+regression: `rmse`, `mse`, `mae`, `r2`, `mape`, `spearman`, `pearson` - default
+is `rmse` If you don't find `eval_metric` that you need, please add a new
+issue. We will add it. # Examples ## :point_right: Binary Classification
+Example There is a simple interface available with `fit` and `predict` methods.
+```python import pandas as pd from sklearn.model_selection import
+train_test_split from supervised.automl import AutoML df = pd.read_csv( "https:
+//raw.githubusercontent.com/pplonski/datasets-for-start/master/adult/data.csv",
+skipinitialspace=True, ) X_train, X_test, y_train, y_test = train_test_split
+( df[df.columns[:-1]], df["income"], test_size=0.25 ) automl = AutoML()
+automl.fit(X_train, y_train) predictions = automl.predict(X_test) ``` AutoML
+`fit` will print: ```py Create directory AutoML_1 AutoML task to be solved:
+binary_classification AutoML will use algorithms: ['Baseline', 'Linear',
+'Decision Tree', 'Random Forest', 'Xgboost', 'Neural Network'] AutoML will
+optimize for metric: logloss 1_Baseline final logloss 0.5519845471086654 time
+0.08 seconds 2_DecisionTree final logloss 0.3655910192804364 time 10.28 seconds
+3_Linear final logloss 0.38139916864708445 time 3.19 seconds
 4_Default_RandomForest final logloss 0.2975204390214936 time 79.19 seconds
 5_Default_Xgboost final logloss 0.2731086827200411 time 5.17 seconds
 6_Default_NeuralNetwork final logloss 0.319812276905242 time 21.19 seconds
 Ensemble final logloss 0.2731086821194617 time 1.43 seconds ``` - the AutoML
 results in [Markdown report](https://github.com/mljar/mljar-examples/tree/
 master/Income_classification/AutoML_1#automl-leaderboard) - the Xgboost
 [Markdown report](https://github.com/mljar/mljar-examples/blob/master/
@@ -138,50 +186,108 @@
 AutoML # load the data digits = load_digits() X_train, X_test, y_train, y_test
 = train_test_split( pd.DataFrame(digits.data), digits.target,
 stratify=digits.target, test_size=0.25, random_state=123 ) # train models with
 AutoML automl = AutoML(mode="Perform") automl.fit(X_train, y_train) # compute
 the accuracy on test data predictions = automl.predict_all(X_test) print
 (predictions.head()) print("Test accuracy:", accuracy_score(y_test, predictions
 ["label"].astype(int))) ``` ## :point_right: Regression Example Regression
-example on Boston house prices data. On test data it scores ~ 10.85 mean
-squared error (MSE). ```python import numpy as np import pandas as pd from
-sklearn.datasets import load_boston from sklearn.model_selection import
-train_test_split from sklearn.metrics import mean_squared_error from
-supervised.automl import AutoML # mljar-supervised # Load the data housing =
-load_boston() X_train, X_test, y_train, y_test = train_test_split( pd.DataFrame
-(housing.data, columns=housing.feature_names), housing.target, test_size=0.25,
+example on `California Housing` house prices data. ```python import numpy as np
+import pandas as pd from sklearn.datasets import fetch_california_housing from
+sklearn.model_selection import train_test_split from sklearn.metrics import
+mean_squared_error from supervised.automl import AutoML # mljar-supervised #
+Load the data housing = fetch_california_housing() X_train, X_test, y_train,
+y_test = train_test_split( pd.DataFrame(housing.data,
+columns=housing.feature_names), housing.target, test_size=0.25,
 random_state=123, ) # train models with AutoML automl = AutoML(mode="Explain")
 automl.fit(X_train, y_train) # compute the MSE on test data predictions =
 automl.predict(X_test) print("Test MSE:", mean_squared_error(y_test,
 predictions)) ``` ## :point_right: More Examples - [**Income classification**]
 (https://github.com/mljar/mljar-examples/tree/master/Income_classification) -
 it is a binary classification task on census data - [**Iris classification**]
 (https://github.com/mljar/mljar-examples/tree/master/Iris_classification) - it
 is a multiclass classification on Iris flowers data - [**House price
 regression**](https://github.com/mljar/mljar-examples/tree/master/
-House_price_regression) - it is a regression task on Boston houses data #
-Documentation :books: For details please check [mljar-supervised docs](https://
-supervised.mljar.com). # Installation :package: From PyPi repository: ``` pip
-install mljar-supervised ``` From source code: ``` git clone https://
-github.com/mljar/mljar-supervised.git cd mljar-supervised python setup.py
-install ``` Installation for development ``` git clone https://github.com/
-mljar/mljar-supervised.git virtualenv venv --python=python3.6 source venv/bin/
-activate pip install -r requirements.txt pip install -r requirements_dev.txt
-``` Running in the docker: ``` FROM python:3.7-slim-buster RUN apt-get update
-&& apt-get -y update RUN apt-get install -y build-essential python3-pip
-python3-dev RUN pip3 -q install pip --upgrade RUN pip3 install mljar-supervised
-jupyter CMD ["jupyter", "notebook", "--port=8888", "--no-browser", "--
-ip=0.0.0.0", "--allow-root"] ``` # Contributing To get started take a look at
-our [Contribution Guide](https://supervised.mljar.com/contributing/) for
-information about our process and where you can fit in! ### Contributors
-[https://contributors-img.web.app/image?repo=mljar/mljar-supervised] # License
-:necktie: The `mljar-supervised` is provided with [MIT license](https://
-github.com/mljar/mljar-supervised/blob/master/LICENSE). # MLJAR :heart:
+House_price_regression) - it is a regression task on Boston houses data # FAQ
+What method is used for hyperparameters optimization? - For modes: `Explain`,
+`Perform` and `Compete` there is used a random search method combined with hill
+climbing. In this approach all checked models are saved and used for building
+Ensemble. - For mode: `Optuna` the Optuna framework is used. It is using TPE
+sampler for tuning. Models checked during Optuna hyperparameters search are not
+saved, only the best model is saved (final model from tuning). You can check
+the details about checked hyperparameters from optuna by checking study files
+in `optuna` directory in your AutoML `results_path`.  How to save and load
+AutoML? The save and load of AutoML models is automatic. All models created
+during AutoML training are saved in the directory set in `results_path`
+(argument of `AutoML()` constructor). If there is no `results_path` set, then
+the directory is created based on following name convention: `AutoML_{number}`
+the `number` will be number from 1 to 1000 (depends which directory name will
+be free). Example save and load: ```python automl = AutoML
+(results_path='AutoML_1') automl.fit(X, y) ``` The all models from AutoML are
+saved in `AutoML_1` directory. To load models: ```python automl = AutoML
+(results_path='AutoML_1') automl.predict(X) ```  How to set ML task (select
+between classification or regression)? The MLJAR AutoML can work with: - binary
+classification - multi-class classification - regression The ML task detection
+is automatic based on target values. There can be situation if you want to
+manually force AutoML to select the ML task, then you need to set `ml_task`
+parameter. It can be set to `'binary_classification'`,
+`'multiclass_classification'`, `'regression'`. Example: ```python automl =
+AutoML(ml_task='regression') automl.fit(X, y) ``` In the above example the
+regression model will be fitted.  How to reuse Optuna hyperparameters? You can
+reuse Optuna hyperparameters that were found in other AutoML training. You need
+to pass them in `optuna_init_params` argument. All hyperparameters found during
+Optuna tuning are saved in the `optuna/optuna.json` file (inside `results_path`
+directory). Example: ```python optuna_init = json.loads(open
+('previous_AutoML_training/optuna/optuna.json').read()) automl = AutoML
+( mode='Optuna', optuna_init_params=optuna_init ) automl.fit(X, y) ``` When
+reusing Optuna hyperparameters the Optuna tuning is simply skipped. The model
+will be trained with hyperparameters set in `optuna_init_params`. Right now
+there is no option to continue Optuna tuning with seed parameters.  How to know
+the order of classes for binary or multiclass problem when using predict_proba?
+To get predicted probabilites with information about class label please use the
+`predict_all()` method. It returns the pandas DataFrame with class names in the
+columns. The order of predicted columns is the same in the `predict_proba()`
+and `predict_all()` methods. The `predict_all()` method will additionaly have
+the column with the predicted class label.  # Documentation For details please
+check [mljar-supervised docs](https://supervised.mljar.com). # Installation
+From PyPi repository: ``` pip install mljar-supervised ``` To install this
+package with conda run: ``` conda install -c conda-forge mljar-supervised ```
+From source code: ``` git clone https://github.com/mljar/mljar-supervised.git
+cd mljar-supervised python setup.py install ``` Installation for development
+``` git clone https://github.com/mljar/mljar-supervised.git virtualenv venv --
+python=python3.6 source venv/bin/activate pip install -r requirements.txt pip
+install -r requirements_dev.txt ``` Running in the docker: ``` FROM python:3.7-
+slim-buster RUN apt-get update && apt-get -y update RUN apt-get install -
+y build-essential python3-pip python3-dev RUN pip3 -q install pip --upgrade RUN
+pip3 install mljar-supervised jupyter CMD ["jupyter", "notebook", "--
+port=8888", "--no-browser", "--ip=0.0.0.0", "--allow-root"] ``` Install from
+GitHub with pip: ``` pip install -q -U git+https://github.com/mljar/mljar-
+supervised.git@master ``` # Demo In the below demo GIF you will see: - MLJAR
+AutoML trained in Jupyter Notebook on titanic dataset - overview of created
+files - showcase of selected plots created during AutoML training - algorithm
+comparison report along with their plots - example of README file and csv file
+with results ![](https://github.com/mljar/mljar-examples/raw/master/media/
+mljar_files.gif) # Contributing To get started take a look at our [Contribution
+Guide](https://supervised.mljar.com/contributing/) for information about our
+process and where you can fit in! ### Contributors [https://contributors-
+img.web.app/image?repo=mljar/mljar-supervised] # Cite Would you like to cite
+MLJAR? Great! :) You can cite MLJAR as following: ``` @misc{mljar, author =
+{Aleksandra P\l{}o\'{n}ska and Piotr P\l{}o\'{n}ski}, year = {2021}, publisher
+= {MLJAR}, address = {\L{}apy, Poland}, title = {MLJAR: State-of-the-art
+Automated Machine Learning Framework for Tabular Data. Version 0.10.3}, url =
+{https://github.com/mljar/mljar-supervised} } ``` Would love to hear from you
+how have you used MLJAR AutoML in your project. Please feel free to let us know
+at ![image](https://user-images.githubusercontent.com/6959032/118103228-
+f5ea9a00-b3d9-11eb-87ed-8cfb1f873f91.png) # License The `mljar-supervised` is
+provided with [MIT license](https://github.com/mljar/mljar-supervised/blob/
+master/LICENSE). # Commercial support Looking for commercial support? Do you
+need new feature implementation? Please contact us by [email](https://
+mljar.com/contact/) for details. # MLJAR
   [https://github.com/mljar/mljar-examples/blob/master/media/large_logo.png]
 The `mljar-supervised` is an open-source project created by [MLJAR](https://
 mljar.com). We care about ease of use in the Machine Learning. The [mljar.com]
 (https://mljar.com) provides a beautiful and simple user interface for building
 machine learning models. Keywords: automated machine learning,automl,machine
 learning,data science,data mining,mljar Platform: UNKNOWN Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
-3.7 Classifier: Programming Language :: Python :: 3.8 Description-Content-Type:
+3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Requires-Python: >=3.7.1 Description-Content-Type:
 text/markdown
```

### Comparing `mljar-supervised-0.9.1/LICENSE` & `mljar-supervised-1.0.0/LICENSE`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018 MLJAR
+Copyright (c) 2018 MLJAR Sp. z o.o.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mljar-supervised-0.9.1/setup.py` & `mljar-supervised-1.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,29 +6,31 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="mljar-supervised",
-    version="0.9.1",
+    version="1.0.0",
     description="Automated Machine Learning for Humans",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mljar/mljar-supervised",
-    author="MLJAR, Inc.",
+    author="MLJAR, Sp. z o.o.",
     author_email="contact@mljar.com",
     license="MIT",
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     install_requires=open("requirements.txt").readlines(),
     include_package_data=True,
+    python_requires='>=3.7.1',
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
     ],
     keywords=[
         "automated machine learning",
         "automl",
         "machine learning",
         "data science",
         "data mining",
```

### Comparing `mljar-supervised-0.9.1/mljar_supervised.egg-info/PKG-INFO` & `mljar-supervised-1.0.0/mljar_supervised.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,99 @@
 Metadata-Version: 2.1
 Name: mljar-supervised
-Version: 0.9.1
+Version: 1.0.0
 Summary: Automated Machine Learning for Humans
 Home-page: https://github.com/mljar/mljar-supervised
-Author: MLJAR, Inc.
+Author: MLJAR, Sp. z o.o.
 Author-email: contact@mljar.com
 License: MIT
 Description: # MLJAR Automated Machine Learning for Humans
         
-        [![Build Status](https://travis-ci.org/mljar/mljar-supervised.svg?branch=master)](https://travis-ci.org/mljar/mljar-supervised)
-        [![Coverage Status](https://coveralls.io/repos/github/mljar/mljar-supervised/badge.svg?branch=master)](https://coveralls.io/github/mljar/mljar-supervised?branch=master)
+        [![Tests status](https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml/badge.svg)](https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml)
         [![PyPI version](https://badge.fury.io/py/mljar-supervised.svg)](https://badge.fury.io/py/mljar-supervised)
+        [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/version.svg)](https://anaconda.org/conda-forge/mljar-supervised)
         [![PyPI pyversions](https://img.shields.io/pypi/pyversions/mljar-supervised.svg)](https://pypi.python.org/pypi/mljar-supervised/)
-        
+        [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/platforms.svg)](https://anaconda.org/conda-forge/mljar-supervised)
+        [![Anaconda-Server Badge](https://anaconda.org/conda-forge/mljar-supervised/badges/license.svg)](https://anaconda.org/conda-forge/mljar-supervised)
+        [![Downloads](https://pepy.tech/badge/mljar-supervised)](https://pepy.tech/project/mljar-supervised)
         
         <p align="center">
           <img src="https://raw.githubusercontent.com/mljar/mljar-examples/master/media/AutoML_overview_mljar_v3.svg" width="100%" />
         </p>
         
         ---
         
         **Documentation**: <a href="https://supervised.mljar.com/" target="_blank">https://supervised.mljar.com/</a>
         
         **Source Code**: <a href="https://github.com/mljar/mljar-supervised" target="_blank">https://github.com/mljar/mljar-supervised</a>
         
+        **Looking for commercial support**: Please contact us by [email](https://mljar.com/contact/) for details
+        
+        
+        <p align="center">
+          <img src="https://github.com/mljar/visual-identity/raw/main/robots/robot_docs.png" width="40%" />
+        </p>
+        
+        
+        
         ---
         
         ## Table of Contents
         
-         - [Automated Machine Learning](https://github.com/mljar/mljar-supervised#automated-machine-learning-rocket)
-         - [What's good in it?](https://github.com/mljar/mljar-supervised#whats-good-in-it-boom)
-         - [Atomatic Documentation](https://github.com/mljar/mljar-supervised#automatic-documentation)
-         - [Available Modes](https://github.com/mljar/mljar-supervised#available-modes-books)
+         - [Automated Machine Learning](https://github.com/mljar/mljar-supervised#automated-machine-learning)
+         - [What's good in it?](https://github.com/mljar/mljar-supervised#whats-good-in-it)
+         - [Automatic Documentation](https://github.com/mljar/mljar-supervised#automatic-documentation)
+         - [Available Modes](https://github.com/mljar/mljar-supervised#available-modes)
          - [Examples](https://github.com/mljar/mljar-supervised#examples)
+         - [FAQ](https://github.com/mljar/mljar-supervised#faq)
          - [Documentation](https://github.com/mljar/mljar-supervised#documentation)
-         - [Installation](https://github.com/mljar/mljar-supervised#installation-package)
+         - [Installation](https://github.com/mljar/mljar-supervised#installation)
+         - [Demo](https://github.com/mljar/mljar-supervised#demo)
          - [Contributing](https://github.com/mljar/mljar-supervised#contributing)
-         - [License](https://github.com/mljar/mljar-supervised#license-necktie)
-         - [MLJAR](https://github.com/mljar/mljar-supervised#mljar-heart)
+         - [Cite](https://github.com/mljar/mljar-supervised#cite)
+         - [License](https://github.com/mljar/mljar-supervised#license)
+         - [Commercial support](https://github.com/mljar/mljar-supervised#commercial-support)
+         - [MLJAR](https://github.com/mljar/mljar-supervised#mljar)
+         
         
-        ## Automated Machine Learning :rocket: 
+        # Automated Machine Learning 
         
         The `mljar-supervised` is an Automated Machine Learning Python package that works with tabular data. It is designed to save time for a data scientist. It abstracts the common way to preprocess the data, construct the machine learning models, and perform hyper-parameters tuning to find the best model :trophy:. It is no black-box as you can see exactly how the ML pipeline is constructed (with a detailed Markdown report for each ML model). 
         
         The `mljar-supervised` will help you with:
          - explaining and understanding your data (Automatic Exploratory Data Analysis),
          - trying many different machine learning models (Algorithm Selection and Hyper-Parameters tuning),
-         - creating Markdown reports from analysis with details about all models (Atomatic-Documentation),
+         - creating Markdown reports from analysis with details about all models (Automatic-Documentation),
          - saving, re-running and loading the analysis and ML models.
         
-        It has three built-in modes of work:
+        It has four built-in modes of work:
          - `Explain` mode, which is ideal for explaining and understanding the data, with many data explanations, like decision trees visualization, linear models coefficients display, permutation importances and SHAP explanations of data,
          - `Perform` for building ML pipelines to use in production,
          - `Compete` mode that trains highly-tuned ML models with ensembling and stacking, with a purpose to use in ML competitions.
+         - `Optuna` mode that can be used to search for highly-tuned ML models, should be used when the performance is the most important, and computation time is not limited (it is available from version `0.10.0`)
         
         Of course, you can further customize the details of each `mode` to meet the requirements.
         
-        ## What's good in it? :boom:
+        ## What's good in it? 
         
         - It is using many algorithms: `Baseline`, `Linear`, `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, `CatBoost`, `Neural Networks`, and `Nearest Neighbors`.
         - It can compute Ensemble based on greedy algorithm from [Caruana paper](http://www.cs.cornell.edu/~alexn/papers/shotgun.icml04.revised.rev2.pdf).
         - It can stack models to build level 2 ensemble (available in `Compete` mode or after setting `stack_models` parameter).
         - It can do features preprocessing, like: missing values imputation and converting categoricals. What is more, it can also handle target values preprocessing.
         - It can do advanced features engineering, like: [Golden Features](https://supervised.mljar.com/features/golden_features/), [Features Selection](https://supervised.mljar.com/features/features_selection/), Text and Time Transformations.
         - It can tune hyper-parameters with `not-so-random-search` algorithm (random-search over defined set of values) and hill climbing to fine-tune final models.
         - It can compute the `Baseline` for your data. That you will know if you need Machine Learning or not!
         - It has extensive explanations. This package is training simple `Decision Trees` with `max_depth <= 5`, so you can easily visualize them with amazing [dtreeviz](https://github.com/parrt/dtreeviz) to better understand your data.
         - The `mljar-supervised` is using simple linear regression and include its coefficients in the summary report, so you can check which features are used the most in the linear model.
         - It cares about explainability of models: for every algorithm, the feature importance is computed based on permutation. Additionally, for every algorithm the SHAP explanations are computed: feature importance, dependence plots, and decision plots (explanations can be switched off with `explain_level` parameter).
-        - There is automatic documnetation for every ML experiment run with AutoML. The `mljar-supervised` creates markdown reports from AutoML training full of ML details, metrics and charts. 
+        - There is automatic documentation for every ML experiment run with AutoML. The `mljar-supervised` creates markdown reports from AutoML training full of ML details, metrics and charts. 
+        
+        <p align="center">
+          <img src="https://raw.githubusercontent.com/mljar/visual-identity/main/media/infograph.png" width="100%" />
+        </p>
         
         # Automatic Documentation
         
         ## The AutoML Report
         
         The report from running AutoML will contain the table with infomation about each model score and time needed to train the model. For each model there is a link, which you can click to see model's details. The performance of all ML models is presented as scatter and box plots so you can visually inspect which algorithms perform the best :trophy:.
         
@@ -92,18 +113,22 @@
         ## The `LightGBM` Report
         
         The example for `LightGBM` summary:
         
         ![Decision Tree summary](https://github.com/mljar/mljar-examples/blob/master/media/lightgbm_summary.gif)
         
         
-        ## Available Modes :books:
+        ## Available Modes
         
         In the [docs](https://supervised.mljar.com/features/modes/) you can find details about AutoML modes are presented in the table .
         
+        <p align="center">
+          <img src="https://raw.githubusercontent.com/mljar/visual-identity/main/media/mljar_modes.png" width="100%" />
+        </p>
+        
         ### Explain 
         
         ```py
         automl = AutoML(mode="Explain")
         ```
         
         It is aimed to be used when the user wants to explain and understand the data.
@@ -129,14 +154,62 @@
         ```
         
         It should be used for machine learning competitions.
          - It adapts the validation strategy depending on dataset size and `total_time_limit`. It can be: train/test split (80/20), 5-fold CV or 10-fold CV. 
          - It is using: `Linear`, `Decision Tree`, `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, `CatBoost`, `Neural Network` and `Nearest Neighbors`. It uses ensemble and **stacking**. 
          - It has only learning curves in the reports.
         
+        ### Optuna
+        
+        ```py
+        automl = AutoML(mode="Optuna", optuna_time_budget=3600)
+        ```
+        
+        It should be used when the performance is the most important and time is not limited.
+        - It is using 10-fold CV
+        - It is using: `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, and `CatBoost`. Those algorithms are tuned by `Optuna` framework for `optuna_time_budget` seconds, each. Algorithms are tuned with original data, without advanced feature engineering.
+        - It is using advanced feature engineering, stacking and ensembling. The hyperparameters found for original data are reused with those steps.
+        - It produces learning curves in the reports.
+        
+        ## How to save and load AutoML?
+        
+        All models in the AutoML are saved and loaded automatically. No need to call `save()` or `load()`.
+        
+        ### Example:
+        
+        #### Train AutoML
+        
+        ```python
+        automl = AutoML(results_path="AutoML_classifier")
+        automl.fit(X, y)
+        ```
+        
+        You will have all models saved in the `AutoML_classifier` directory. Each model will have a separate directory with the `README.md` file with all details from the training.
+        
+        #### Compute predictions
+        ```python
+        automl = AutoML(results_path="AutoML_classifier")
+        automl.predict(X)
+        ```
+        
+        The  AutoML automatically loads models from the `results_path` directory. If you will call `fit()` on already trained AutoML then you will get a warning message that AutoML is already fitted.
+        
+        
+        ### Why do you automatically save all models?
+        
+        All models are automatically saved to be able to restore the training after interruption. For example, you are training AutoML for 48 hours, and after 47 hours there is some unexpected interruption. In MLJAR AutoML you just call the same training code after the interruption and AutoML reloads already trained models and finish the training.
+        
+        ## Supported evaluation metrics (`eval_metric` argument in `AutoML()`)
+        
+        - for binary classification: `logloss`, `auc`, `f1`, `average_precision`, `accuracy`- default is `logloss`
+        - for mutliclass classification: `logloss`, `f1`, `accuracy` - default is `logloss`
+        - for regression: `rmse`, `mse`, `mae`, `r2`, `mape`, `spearman`, `pearson` - default is `rmse`
+        
+        If you don't find `eval_metric` that you need, please add a new issue. We will add it.
+        
         # Examples
         
         ## :point_right: Binary Classification Example
         
         There is a simple interface available with `fit` and `predict` methods.
         
         ```python
@@ -207,26 +280,26 @@
         predictions = automl.predict_all(X_test)
         print(predictions.head())
         print("Test accuracy:", accuracy_score(y_test, predictions["label"].astype(int)))
         ```
         
         ## :point_right: Regression Example
         
-        Regression example on Boston house prices data. On test data it scores ~ 10.85 mean squared error (MSE).
+        Regression example on `California Housing` house prices data.
         
         ```python
         import numpy as np
         import pandas as pd
-        from sklearn.datasets import load_boston
+        from sklearn.datasets import fetch_california_housing
         from sklearn.model_selection import train_test_split
         from sklearn.metrics import mean_squared_error
         from supervised.automl import AutoML # mljar-supervised
         
         # Load the data
-        housing = load_boston()
+        housing = fetch_california_housing()
         X_train, X_test, y_train, y_test = train_test_split(
             pd.DataFrame(housing.data, columns=housing.feature_names),
             housing.target,
             test_size=0.25,
             random_state=123,
         )
         
@@ -241,26 +314,106 @@
         
         ## :point_right: More Examples
         
         - [**Income classification**](https://github.com/mljar/mljar-examples/tree/master/Income_classification) - it is a binary classification task on census data
         - [**Iris classification**](https://github.com/mljar/mljar-examples/tree/master/Iris_classification) - it is a multiclass classification on Iris flowers data
         - [**House price regression**](https://github.com/mljar/mljar-examples/tree/master/House_price_regression) - it is a regression task on Boston houses data
         
-        # Documentation :books:
+        # FAQ
+        
+        <details><summary>What method is used for hyperparameters optimization?</summary>
+          - For modes: `Explain`, `Perform` and `Compete` there is used a random search method combined with hill climbing. In this approach all checked models are saved and used for building Ensemble.
+          - For mode: `Optuna` the Optuna framework is used. It is using TPE sampler for tuning. Models checked during Optuna hyperparameters search are not saved, only the best model is saved (final model from tuning). You can check the details about checked hyperparameters from optuna by checking study files in `optuna` directory in your AutoML `results_path`.
+        </details>
+        
+        <details><summary>How to save and load AutoML?</summary>
+        
+        The save and load of AutoML models is automatic. All models created during AutoML training are saved in the directory set in `results_path` (argument of `AutoML()` constructor). If there is no `results_path` set, then the directory is created based on following name convention: `AutoML_{number}` the `number` will be number from 1 to 1000 (depends which directory name will be free).
+        
+        Example save and load:
+        
+        ```python
+        automl = AutoML(results_path='AutoML_1')
+        automl.fit(X, y)
+        ```
+        
+        The all models from AutoML are saved in `AutoML_1` directory.
+        
+        To load models:
+        
+        ```python
+        automl = AutoML(results_path='AutoML_1')
+        automl.predict(X)
+        ```
+        
+        </details>
+        
+        <details><summary>How to set ML task (select between classification or regression)?</summary>
+        
+        The MLJAR AutoML can work with:
+        - binary classification
+        - multi-class classification
+        - regression
+        
+        The ML task detection is automatic based on target values. There can be situation if you want to manually force AutoML to select the ML task, then you need to set `ml_task` parameter. It can be set to `'binary_classification'`, `'multiclass_classification'`, `'regression'`.
+        
+        Example:
+        ```python
+        automl = AutoML(ml_task='regression')
+        automl.fit(X, y)
+        ```
+        In the above example the regression model will be fitted.
+        
+        </details>
+        
+        <details><summary>How to reuse Optuna hyperparameters?</summary>
+          
+          You can reuse Optuna hyperparameters that were found in other AutoML training. You need to pass them in `optuna_init_params` argument. All hyperparameters found during Optuna tuning are saved in the `optuna/optuna.json` file (inside `results_path` directory).
+          
+         Example:
+         
+         ```python
+         optuna_init = json.loads(open('previous_AutoML_training/optuna/optuna.json').read())
+         
+         automl = AutoML(
+             mode='Optuna',
+             optuna_init_params=optuna_init
+         )
+         automl.fit(X, y)
+         ```
+          
+         When reusing Optuna hyperparameters the Optuna tuning is simply skipped. The model will be trained with hyperparameters set in `optuna_init_params`. Right now there is no option to continue Optuna tuning with seed parameters.
+          
+          
+        </details>
+        
+        
+        <details><summary>How to know the order of classes for binary or multiclass problem when using predict_proba?</summary>
+        
+        To get predicted probabilites with information about class label please use the `predict_all()` method. It returns the pandas DataFrame with class names in the columns. The order of predicted columns is the same in the `predict_proba()` and `predict_all()` methods. The `predict_all()` method will additionaly have the column with the predicted class label.
+        
+        </details>
+        
+        # Documentation  
         
         For details please check [mljar-supervised docs](https://supervised.mljar.com).
         
-        # Installation :package: 
+        # Installation  
         
         From PyPi repository:
         
         ```
         pip install mljar-supervised
         ```
         
+        To install this package with conda run:
+        ```
+        conda install -c conda-forge mljar-supervised
+        ```
+        
         From source code:
         
         ```
         git clone https://github.com/mljar/mljar-supervised.git
         cd mljar-supervised
         python setup.py install
         ```
@@ -280,35 +433,77 @@
         RUN apt-get update && apt-get -y update
         RUN apt-get install -y build-essential python3-pip python3-dev
         RUN pip3 -q install pip --upgrade
         RUN pip3 install mljar-supervised jupyter
         CMD ["jupyter", "notebook", "--port=8888", "--no-browser", "--ip=0.0.0.0", "--allow-root"]
         ```
         
+        Install from GitHub with pip:
+        ```
+        pip install -q -U git+https://github.com/mljar/mljar-supervised.git@master
+        ```
+        # Demo
+        
+        In the below demo GIF you will see:
+        - MLJAR AutoML trained in Jupyter Notebook on titanic dataset
+        - overview of created files
+        - showcase of selected plots created during AutoML training
+        - algorithm comparison report along with their plots
+        - example of README file and csv file with results
+        
+        ![](https://github.com/mljar/mljar-examples/raw/master/media/mljar_files.gif)
+        
         # Contributing
         
         To get started take a look at our [Contribution Guide](https://supervised.mljar.com/contributing/) for information about our process and where you can fit in!
         
         ### Contributors
         <a href="https://github.com/mljar/mljar-supervised/graphs/contributors">
           <img src="https://contributors-img.web.app/image?repo=mljar/mljar-supervised" />
         </a>
         
+        # Cite
+        
+        Would you like to cite MLJAR? Great! :)
+        
+        You can cite MLJAR as following:
+        
+        ```
+        @misc{mljar,
+          author    = {Aleksandra P\l{}o\'{n}ska and Piotr P\l{}o\'{n}ski},
+          year      = {2021},
+          publisher = {MLJAR},
+          address   = {\L{}apy, Poland},
+          title     = {MLJAR: State-of-the-art Automated Machine Learning Framework for Tabular Data.  Version 0.10.3},
+          url       = {https://github.com/mljar/mljar-supervised}
+        }
+        ```
+        
+        Would love to hear from you how have you used MLJAR AutoML in your project. 
+        Please feel free to let us know at 
+        ![image](https://user-images.githubusercontent.com/6959032/118103228-f5ea9a00-b3d9-11eb-87ed-8cfb1f873f91.png)
+        
         
-        # License :necktie:
+        # License  
         
         The `mljar-supervised` is provided with [MIT license](https://github.com/mljar/mljar-supervised/blob/master/LICENSE).
         
-        # MLJAR :heart:
+        # Commercial support
+        
+        Looking for commercial support? Do you need new feature implementation? Please contact us by [email](https://mljar.com/contact/) for details.
+        
+        # MLJAR 
         <p align="center">
           <img src="https://github.com/mljar/mljar-examples/blob/master/media/large_logo.png" width="314" />
         </p>
         
         The `mljar-supervised` is an open-source project created by [MLJAR](https://mljar.com). We care about ease of use in the Machine Learning. 
         The [mljar.com](https://mljar.com) provides a beautiful and simple user interface for building machine learning models.
         
 Keywords: automated machine learning,automl,machine learning,data science,data mining,mljar
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,122 +1,170 @@
-Metadata-Version: 2.1 Name: mljar-supervised Version: 0.9.1 Summary: Automated
+Metadata-Version: 2.1 Name: mljar-supervised Version: 1.0.0 Summary: Automated
 Machine Learning for Humans Home-page: https://github.com/mljar/mljar-
-supervised Author: MLJAR, Inc. Author-email: contact@mljar.com License: MIT
-Description: # MLJAR Automated Machine Learning for Humans [![Build Status]
-(https://travis-ci.org/mljar/mljar-supervised.svg?branch=master)](https://
-travis-ci.org/mljar/mljar-supervised) [![Coverage Status](https://coveralls.io/
-repos/github/mljar/mljar-supervised/badge.svg?branch=master)](https://
-coveralls.io/github/mljar/mljar-supervised?branch=master) [![PyPI version]
-(https://badge.fury.io/py/mljar-supervised.svg)](https://badge.fury.io/py/
-mljar-supervised) [![PyPI pyversions](https://img.shields.io/pypi/pyversions/
-mljar-supervised.svg)](https://pypi.python.org/pypi/mljar-supervised/)
+supervised Author: MLJAR, Sp. z o.o. Author-email: contact@mljar.com License:
+MIT Description: # MLJAR Automated Machine Learning for Humans [![Tests status]
+(https://github.com/mljar/mljar-supervised/actions/workflows/run-tests.yml/
+badge.svg)](https://github.com/mljar/mljar-supervised/actions/workflows/run-
+tests.yml) [![PyPI version](https://badge.fury.io/py/mljar-supervised.svg)]
+(https://badge.fury.io/py/mljar-supervised) [![Anaconda-Server Badge](https://
+anaconda.org/conda-forge/mljar-supervised/badges/version.svg)](https://
+anaconda.org/conda-forge/mljar-supervised) [![PyPI pyversions](https://
+img.shields.io/pypi/pyversions/mljar-supervised.svg)](https://pypi.python.org/
+pypi/mljar-supervised/) [![Anaconda-Server Badge](https://anaconda.org/conda-
+forge/mljar-supervised/badges/platforms.svg)](https://anaconda.org/conda-forge/
+mljar-supervised) [![Anaconda-Server Badge](https://anaconda.org/conda-forge/
+mljar-supervised/badges/license.svg)](https://anaconda.org/conda-forge/mljar-
+supervised) [![Downloads](https://pepy.tech/badge/mljar-supervised)](https://
+pepy.tech/project/mljar-supervised)
      [https://raw.githubusercontent.com/mljar/mljar-examples/master/media/
                          AutoML_overview_mljar_v3.svg]
 --- **Documentation**: https://supervised.mljar.com/ **Source Code**: https://
-github.com/mljar/mljar-supervised --- ## Table of Contents - [Automated Machine
-Learning](https://github.com/mljar/mljar-supervised#automated-machine-learning-
-rocket) - [What's good in it?](https://github.com/mljar/mljar-supervised#whats-
-good-in-it-boom) - [Atomatic Documentation](https://github.com/mljar/mljar-
-supervised#automatic-documentation) - [Available Modes](https://github.com/
-mljar/mljar-supervised#available-modes-books) - [Examples](https://github.com/
-mljar/mljar-supervised#examples) - [Documentation](https://github.com/mljar/
-mljar-supervised#documentation) - [Installation](https://github.com/mljar/
-mljar-supervised#installation-package) - [Contributing](https://github.com/
-mljar/mljar-supervised#contributing) - [License](https://github.com/mljar/
-mljar-supervised#license-necktie) - [MLJAR](https://github.com/mljar/mljar-
-supervised#mljar-heart) ## Automated Machine Learning :rocket: The `mljar-
-supervised` is an Automated Machine Learning Python package that works with
-tabular data. It is designed to save time for a data scientist. It abstracts
-the common way to preprocess the data, construct the machine learning models,
-and perform hyper-parameters tuning to find the best model :trophy:. It is no
-black-box as you can see exactly how the ML pipeline is constructed (with a
-detailed Markdown report for each ML model). The `mljar-supervised` will help
-you with: - explaining and understanding your data (Automatic Exploratory Data
-Analysis), - trying many different machine learning models (Algorithm Selection
-and Hyper-Parameters tuning), - creating Markdown reports from analysis with
-details about all models (Atomatic-Documentation), - saving, re-running and
-loading the analysis and ML models. It has three built-in modes of work: -
-`Explain` mode, which is ideal for explaining and understanding the data, with
-many data explanations, like decision trees visualization, linear models
-coefficients display, permutation importances and SHAP explanations of data, -
-`Perform` for building ML pipelines to use in production, - `Compete` mode that
-trains highly-tuned ML models with ensembling and stacking, with a purpose to
-use in ML competitions. Of course, you can further customize the details of
-each `mode` to meet the requirements. ## What's good in it? :boom: - It is
-using many algorithms: `Baseline`, `Linear`, `Random Forest`, `Extra Trees`,
-`LightGBM`, `Xgboost`, `CatBoost`, `Neural Networks`, and `Nearest Neighbors`.
-- It can compute Ensemble based on greedy algorithm from [Caruana paper](http:/
-/www.cs.cornell.edu/~alexn/papers/shotgun.icml04.revised.rev2.pdf). - It can
-stack models to build level 2 ensemble (available in `Compete` mode or after
-setting `stack_models` parameter). - It can do features preprocessing, like:
-missing values imputation and converting categoricals. What is more, it can
-also handle target values preprocessing. - It can do advanced features
-engineering, like: [Golden Features](https://supervised.mljar.com/features/
-golden_features/), [Features Selection](https://supervised.mljar.com/features/
-features_selection/), Text and Time Transformations. - It can tune hyper-
-parameters with `not-so-random-search` algorithm (random-search over defined
-set of values) and hill climbing to fine-tune final models. - It can compute
-the `Baseline` for your data. That you will know if you need Machine Learning
-or not! - It has extensive explanations. This package is training simple
-`Decision Trees` with `max_depth <= 5`, so you can easily visualize them with
-amazing [dtreeviz](https://github.com/parrt/dtreeviz) to better understand your
-data. - The `mljar-supervised` is using simple linear regression and include
-its coefficients in the summary report, so you can check which features are
-used the most in the linear model. - It cares about explainability of models:
-for every algorithm, the feature importance is computed based on permutation.
-Additionally, for every algorithm the SHAP explanations are computed: feature
-importance, dependence plots, and decision plots (explanations can be switched
-off with `explain_level` parameter). - There is automatic documnetation for
-every ML experiment run with AutoML. The `mljar-supervised` creates markdown
-reports from AutoML training full of ML details, metrics and charts. #
-Automatic Documentation ## The AutoML Report The report from running AutoML
+github.com/mljar/mljar-supervised **Looking for commercial support**: Please
+contact us by [email](https://mljar.com/contact/) for details
+   [https://github.com/mljar/visual-identity/raw/main/robots/robot_docs.png]
+--- ## Table of Contents - [Automated Machine Learning](https://github.com/
+mljar/mljar-supervised#automated-machine-learning) - [What's good in it?]
+(https://github.com/mljar/mljar-supervised#whats-good-in-it) - [Automatic
+Documentation](https://github.com/mljar/mljar-supervised#automatic-
+documentation) - [Available Modes](https://github.com/mljar/mljar-
+supervised#available-modes) - [Examples](https://github.com/mljar/mljar-
+supervised#examples) - [FAQ](https://github.com/mljar/mljar-supervised#faq) -
+[Documentation](https://github.com/mljar/mljar-supervised#documentation) -
+[Installation](https://github.com/mljar/mljar-supervised#installation) - [Demo]
+(https://github.com/mljar/mljar-supervised#demo) - [Contributing](https://
+github.com/mljar/mljar-supervised#contributing) - [Cite](https://github.com/
+mljar/mljar-supervised#cite) - [License](https://github.com/mljar/mljar-
+supervised#license) - [Commercial support](https://github.com/mljar/mljar-
+supervised#commercial-support) - [MLJAR](https://github.com/mljar/mljar-
+supervised#mljar) # Automated Machine Learning The `mljar-supervised` is an
+Automated Machine Learning Python package that works with tabular data. It is
+designed to save time for a data scientist. It abstracts the common way to
+preprocess the data, construct the machine learning models, and perform hyper-
+parameters tuning to find the best model :trophy:. It is no black-box as you
+can see exactly how the ML pipeline is constructed (with a detailed Markdown
+report for each ML model). The `mljar-supervised` will help you with: -
+explaining and understanding your data (Automatic Exploratory Data Analysis), -
+trying many different machine learning models (Algorithm Selection and Hyper-
+Parameters tuning), - creating Markdown reports from analysis with details
+about all models (Automatic-Documentation), - saving, re-running and loading
+the analysis and ML models. It has four built-in modes of work: - `Explain`
+mode, which is ideal for explaining and understanding the data, with many data
+explanations, like decision trees visualization, linear models coefficients
+display, permutation importances and SHAP explanations of data, - `Perform` for
+building ML pipelines to use in production, - `Compete` mode that trains
+highly-tuned ML models with ensembling and stacking, with a purpose to use in
+ML competitions. - `Optuna` mode that can be used to search for highly-tuned ML
+models, should be used when the performance is the most important, and
+computation time is not limited (it is available from version `0.10.0`) Of
+course, you can further customize the details of each `mode` to meet the
+requirements. ## What's good in it? - It is using many algorithms: `Baseline`,
+`Linear`, `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, `CatBoost`,
+`Neural Networks`, and `Nearest Neighbors`. - It can compute Ensemble based on
+greedy algorithm from [Caruana paper](http://www.cs.cornell.edu/~alexn/papers/
+shotgun.icml04.revised.rev2.pdf). - It can stack models to build level 2
+ensemble (available in `Compete` mode or after setting `stack_models`
+parameter). - It can do features preprocessing, like: missing values imputation
+and converting categoricals. What is more, it can also handle target values
+preprocessing. - It can do advanced features engineering, like: [Golden
+Features](https://supervised.mljar.com/features/golden_features/), [Features
+Selection](https://supervised.mljar.com/features/features_selection/), Text and
+Time Transformations. - It can tune hyper-parameters with `not-so-random-
+search` algorithm (random-search over defined set of values) and hill climbing
+to fine-tune final models. - It can compute the `Baseline` for your data. That
+you will know if you need Machine Learning or not! - It has extensive
+explanations. This package is training simple `Decision Trees` with `max_depth
+<= 5`, so you can easily visualize them with amazing [dtreeviz](https://
+github.com/parrt/dtreeviz) to better understand your data. - The `mljar-
+supervised` is using simple linear regression and include its coefficients in
+the summary report, so you can check which features are used the most in the
+linear model. - It cares about explainability of models: for every algorithm,
+the feature importance is computed based on permutation. Additionally, for
+every algorithm the SHAP explanations are computed: feature importance,
+dependence plots, and decision plots (explanations can be switched off with
+`explain_level` parameter). - There is automatic documentation for every ML
+experiment run with AutoML. The `mljar-supervised` creates markdown reports
+from AutoML training full of ML details, metrics and charts.
+     [https://raw.githubusercontent.com/mljar/visual-identity/main/media/
+                                infograph.png]
+# Automatic Documentation ## The AutoML Report The report from running AutoML
 will contain the table with infomation about each model score and time needed
 to train the model. For each model there is a link, which you can click to see
 model's details. The performance of all ML models is presented as scatter and
 box plots so you can visually inspect which algorithms perform the best :
 trophy:. ![AutoML leaderboard](https://github.com/mljar/mljar-examples/blob/
 master/media/automl_summary.gif) ## The `Decision Tree` Report The example for
 `Decision Tree` summary with trees visualization. For classification tasks
 additional metrics are provided: - confusion matrix - threshold (optimized in
 the case of binary classification task) - F1 score - Accuracy - Precision,
 Recall, MCC ![Decision Tree summary](https://github.com/mljar/mljar-examples/
 blob/master/media/decision_tree_summary.gif) ## The `LightGBM` Report The
 example for `LightGBM` summary: ![Decision Tree summary](https://github.com/
 mljar/mljar-examples/blob/master/media/lightgbm_summary.gif) ## Available Modes
-:books: In the [docs](https://supervised.mljar.com/features/modes/) you can
-find details about AutoML modes are presented in the table . ### Explain ```py
-automl = AutoML(mode="Explain") ``` It is aimed to be used when the user wants
-to explain and understand the data. - It is using 75%/25% train/test split. -
-It is using: `Baseline`, `Linear`, `Decision Tree`, `Random Forest`, `Xgboost`,
-`Neural Network` algorithms and ensemble. - It has full explanations: learning
-curves, importance plots, and SHAP plots. ### Perform ```py automl = AutoML
-(mode="Perform") ``` It should be used when the user wants to train a model
-that will be used in real-life use cases. - It is using 5-fold CV. - It is
-using: `Linear`, `Random Forest`, `LightGBM`, `Xgboost`, `CatBoost` and `Neural
-Network`. It uses ensembling. - It has learning curves and importance plots in
-reports. ### Compete ```py automl = AutoML(mode="Compete") ``` It should be
-used for machine learning competitions. - It adapts the validation strategy
-depending on dataset size and `total_time_limit`. It can be: train/test split
-(80/20), 5-fold CV or 10-fold CV. - It is using: `Linear`, `Decision Tree`,
-`Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`, `CatBoost`, `Neural
-Network` and `Nearest Neighbors`. It uses ensemble and **stacking**. - It has
-only learning curves in the reports. # Examples ## :point_right: Binary
-Classification Example There is a simple interface available with `fit` and
-`predict` methods. ```python import pandas as pd from sklearn.model_selection
-import train_test_split from supervised.automl import AutoML df = pd.read_csv
-( "https://raw.githubusercontent.com/pplonski/datasets-for-start/master/adult/
-data.csv", skipinitialspace=True, ) X_train, X_test, y_train, y_test =
-train_test_split( df[df.columns[:-1]], df["income"], test_size=0.25 ) automl =
-AutoML() automl.fit(X_train, y_train) predictions = automl.predict(X_test) ```
-AutoML `fit` will print: ```py Create directory AutoML_1 AutoML task to be
-solved: binary_classification AutoML will use algorithms: ['Baseline',
-'Linear', 'Decision Tree', 'Random Forest', 'Xgboost', 'Neural Network'] AutoML
-will optimize for metric: logloss 1_Baseline final logloss 0.5519845471086654
-time 0.08 seconds 2_DecisionTree final logloss 0.3655910192804364 time 10.28
-seconds 3_Linear final logloss 0.38139916864708445 time 3.19 seconds
+In the [docs](https://supervised.mljar.com/features/modes/) you can find
+details about AutoML modes are presented in the table .
+     [https://raw.githubusercontent.com/mljar/visual-identity/main/media/
+                               mljar_modes.png]
+### Explain ```py automl = AutoML(mode="Explain") ``` It is aimed to be used
+when the user wants to explain and understand the data. - It is using 75%/25%
+train/test split. - It is using: `Baseline`, `Linear`, `Decision Tree`, `Random
+Forest`, `Xgboost`, `Neural Network` algorithms and ensemble. - It has full
+explanations: learning curves, importance plots, and SHAP plots. ### Perform
+```py automl = AutoML(mode="Perform") ``` It should be used when the user wants
+to train a model that will be used in real-life use cases. - It is using 5-fold
+CV. - It is using: `Linear`, `Random Forest`, `LightGBM`, `Xgboost`, `CatBoost`
+and `Neural Network`. It uses ensembling. - It has learning curves and
+importance plots in reports. ### Compete ```py automl = AutoML(mode="Compete")
+``` It should be used for machine learning competitions. - It adapts the
+validation strategy depending on dataset size and `total_time_limit`. It can
+be: train/test split (80/20), 5-fold CV or 10-fold CV. - It is using: `Linear`,
+`Decision Tree`, `Random Forest`, `Extra Trees`, `LightGBM`, `Xgboost`,
+`CatBoost`, `Neural Network` and `Nearest Neighbors`. It uses ensemble and
+**stacking**. - It has only learning curves in the reports. ### Optuna ```py
+automl = AutoML(mode="Optuna", optuna_time_budget=3600) ``` It should be used
+when the performance is the most important and time is not limited. - It is
+using 10-fold CV - It is using: `Random Forest`, `Extra Trees`, `LightGBM`,
+`Xgboost`, and `CatBoost`. Those algorithms are tuned by `Optuna` framework for
+`optuna_time_budget` seconds, each. Algorithms are tuned with original data,
+without advanced feature engineering. - It is using advanced feature
+engineering, stacking and ensembling. The hyperparameters found for original
+data are reused with those steps. - It produces learning curves in the reports.
+## How to save and load AutoML? All models in the AutoML are saved and loaded
+automatically. No need to call `save()` or `load()`. ### Example: #### Train
+AutoML ```python automl = AutoML(results_path="AutoML_classifier") automl.fit
+(X, y) ``` You will have all models saved in the `AutoML_classifier` directory.
+Each model will have a separate directory with the `README.md` file with all
+details from the training. #### Compute predictions ```python automl = AutoML
+(results_path="AutoML_classifier") automl.predict(X) ``` The AutoML
+automatically loads models from the `results_path` directory. If you will call
+`fit()` on already trained AutoML then you will get a warning message that
+AutoML is already fitted. ### Why do you automatically save all models? All
+models are automatically saved to be able to restore the training after
+interruption. For example, you are training AutoML for 48 hours, and after 47
+hours there is some unexpected interruption. In MLJAR AutoML you just call the
+same training code after the interruption and AutoML reloads already trained
+models and finish the training. ## Supported evaluation metrics (`eval_metric`
+argument in `AutoML()`) - for binary classification: `logloss`, `auc`, `f1`,
+`average_precision`, `accuracy`- default is `logloss` - for mutliclass
+classification: `logloss`, `f1`, `accuracy` - default is `logloss` - for
+regression: `rmse`, `mse`, `mae`, `r2`, `mape`, `spearman`, `pearson` - default
+is `rmse` If you don't find `eval_metric` that you need, please add a new
+issue. We will add it. # Examples ## :point_right: Binary Classification
+Example There is a simple interface available with `fit` and `predict` methods.
+```python import pandas as pd from sklearn.model_selection import
+train_test_split from supervised.automl import AutoML df = pd.read_csv( "https:
+//raw.githubusercontent.com/pplonski/datasets-for-start/master/adult/data.csv",
+skipinitialspace=True, ) X_train, X_test, y_train, y_test = train_test_split
+( df[df.columns[:-1]], df["income"], test_size=0.25 ) automl = AutoML()
+automl.fit(X_train, y_train) predictions = automl.predict(X_test) ``` AutoML
+`fit` will print: ```py Create directory AutoML_1 AutoML task to be solved:
+binary_classification AutoML will use algorithms: ['Baseline', 'Linear',
+'Decision Tree', 'Random Forest', 'Xgboost', 'Neural Network'] AutoML will
+optimize for metric: logloss 1_Baseline final logloss 0.5519845471086654 time
+0.08 seconds 2_DecisionTree final logloss 0.3655910192804364 time 10.28 seconds
+3_Linear final logloss 0.38139916864708445 time 3.19 seconds
 4_Default_RandomForest final logloss 0.2975204390214936 time 79.19 seconds
 5_Default_Xgboost final logloss 0.2731086827200411 time 5.17 seconds
 6_Default_NeuralNetwork final logloss 0.319812276905242 time 21.19 seconds
 Ensemble final logloss 0.2731086821194617 time 1.43 seconds ``` - the AutoML
 results in [Markdown report](https://github.com/mljar/mljar-examples/tree/
 master/Income_classification/AutoML_1#automl-leaderboard) - the Xgboost
 [Markdown report](https://github.com/mljar/mljar-examples/blob/master/
@@ -138,50 +186,108 @@
 AutoML # load the data digits = load_digits() X_train, X_test, y_train, y_test
 = train_test_split( pd.DataFrame(digits.data), digits.target,
 stratify=digits.target, test_size=0.25, random_state=123 ) # train models with
 AutoML automl = AutoML(mode="Perform") automl.fit(X_train, y_train) # compute
 the accuracy on test data predictions = automl.predict_all(X_test) print
 (predictions.head()) print("Test accuracy:", accuracy_score(y_test, predictions
 ["label"].astype(int))) ``` ## :point_right: Regression Example Regression
-example on Boston house prices data. On test data it scores ~ 10.85 mean
-squared error (MSE). ```python import numpy as np import pandas as pd from
-sklearn.datasets import load_boston from sklearn.model_selection import
-train_test_split from sklearn.metrics import mean_squared_error from
-supervised.automl import AutoML # mljar-supervised # Load the data housing =
-load_boston() X_train, X_test, y_train, y_test = train_test_split( pd.DataFrame
-(housing.data, columns=housing.feature_names), housing.target, test_size=0.25,
+example on `California Housing` house prices data. ```python import numpy as np
+import pandas as pd from sklearn.datasets import fetch_california_housing from
+sklearn.model_selection import train_test_split from sklearn.metrics import
+mean_squared_error from supervised.automl import AutoML # mljar-supervised #
+Load the data housing = fetch_california_housing() X_train, X_test, y_train,
+y_test = train_test_split( pd.DataFrame(housing.data,
+columns=housing.feature_names), housing.target, test_size=0.25,
 random_state=123, ) # train models with AutoML automl = AutoML(mode="Explain")
 automl.fit(X_train, y_train) # compute the MSE on test data predictions =
 automl.predict(X_test) print("Test MSE:", mean_squared_error(y_test,
 predictions)) ``` ## :point_right: More Examples - [**Income classification**]
 (https://github.com/mljar/mljar-examples/tree/master/Income_classification) -
 it is a binary classification task on census data - [**Iris classification**]
 (https://github.com/mljar/mljar-examples/tree/master/Iris_classification) - it
 is a multiclass classification on Iris flowers data - [**House price
 regression**](https://github.com/mljar/mljar-examples/tree/master/
-House_price_regression) - it is a regression task on Boston houses data #
-Documentation :books: For details please check [mljar-supervised docs](https://
-supervised.mljar.com). # Installation :package: From PyPi repository: ``` pip
-install mljar-supervised ``` From source code: ``` git clone https://
-github.com/mljar/mljar-supervised.git cd mljar-supervised python setup.py
-install ``` Installation for development ``` git clone https://github.com/
-mljar/mljar-supervised.git virtualenv venv --python=python3.6 source venv/bin/
-activate pip install -r requirements.txt pip install -r requirements_dev.txt
-``` Running in the docker: ``` FROM python:3.7-slim-buster RUN apt-get update
-&& apt-get -y update RUN apt-get install -y build-essential python3-pip
-python3-dev RUN pip3 -q install pip --upgrade RUN pip3 install mljar-supervised
-jupyter CMD ["jupyter", "notebook", "--port=8888", "--no-browser", "--
-ip=0.0.0.0", "--allow-root"] ``` # Contributing To get started take a look at
-our [Contribution Guide](https://supervised.mljar.com/contributing/) for
-information about our process and where you can fit in! ### Contributors
-[https://contributors-img.web.app/image?repo=mljar/mljar-supervised] # License
-:necktie: The `mljar-supervised` is provided with [MIT license](https://
-github.com/mljar/mljar-supervised/blob/master/LICENSE). # MLJAR :heart:
+House_price_regression) - it is a regression task on Boston houses data # FAQ
+What method is used for hyperparameters optimization? - For modes: `Explain`,
+`Perform` and `Compete` there is used a random search method combined with hill
+climbing. In this approach all checked models are saved and used for building
+Ensemble. - For mode: `Optuna` the Optuna framework is used. It is using TPE
+sampler for tuning. Models checked during Optuna hyperparameters search are not
+saved, only the best model is saved (final model from tuning). You can check
+the details about checked hyperparameters from optuna by checking study files
+in `optuna` directory in your AutoML `results_path`.  How to save and load
+AutoML? The save and load of AutoML models is automatic. All models created
+during AutoML training are saved in the directory set in `results_path`
+(argument of `AutoML()` constructor). If there is no `results_path` set, then
+the directory is created based on following name convention: `AutoML_{number}`
+the `number` will be number from 1 to 1000 (depends which directory name will
+be free). Example save and load: ```python automl = AutoML
+(results_path='AutoML_1') automl.fit(X, y) ``` The all models from AutoML are
+saved in `AutoML_1` directory. To load models: ```python automl = AutoML
+(results_path='AutoML_1') automl.predict(X) ```  How to set ML task (select
+between classification or regression)? The MLJAR AutoML can work with: - binary
+classification - multi-class classification - regression The ML task detection
+is automatic based on target values. There can be situation if you want to
+manually force AutoML to select the ML task, then you need to set `ml_task`
+parameter. It can be set to `'binary_classification'`,
+`'multiclass_classification'`, `'regression'`. Example: ```python automl =
+AutoML(ml_task='regression') automl.fit(X, y) ``` In the above example the
+regression model will be fitted.  How to reuse Optuna hyperparameters? You can
+reuse Optuna hyperparameters that were found in other AutoML training. You need
+to pass them in `optuna_init_params` argument. All hyperparameters found during
+Optuna tuning are saved in the `optuna/optuna.json` file (inside `results_path`
+directory). Example: ```python optuna_init = json.loads(open
+('previous_AutoML_training/optuna/optuna.json').read()) automl = AutoML
+( mode='Optuna', optuna_init_params=optuna_init ) automl.fit(X, y) ``` When
+reusing Optuna hyperparameters the Optuna tuning is simply skipped. The model
+will be trained with hyperparameters set in `optuna_init_params`. Right now
+there is no option to continue Optuna tuning with seed parameters.  How to know
+the order of classes for binary or multiclass problem when using predict_proba?
+To get predicted probabilites with information about class label please use the
+`predict_all()` method. It returns the pandas DataFrame with class names in the
+columns. The order of predicted columns is the same in the `predict_proba()`
+and `predict_all()` methods. The `predict_all()` method will additionaly have
+the column with the predicted class label.  # Documentation For details please
+check [mljar-supervised docs](https://supervised.mljar.com). # Installation
+From PyPi repository: ``` pip install mljar-supervised ``` To install this
+package with conda run: ``` conda install -c conda-forge mljar-supervised ```
+From source code: ``` git clone https://github.com/mljar/mljar-supervised.git
+cd mljar-supervised python setup.py install ``` Installation for development
+``` git clone https://github.com/mljar/mljar-supervised.git virtualenv venv --
+python=python3.6 source venv/bin/activate pip install -r requirements.txt pip
+install -r requirements_dev.txt ``` Running in the docker: ``` FROM python:3.7-
+slim-buster RUN apt-get update && apt-get -y update RUN apt-get install -
+y build-essential python3-pip python3-dev RUN pip3 -q install pip --upgrade RUN
+pip3 install mljar-supervised jupyter CMD ["jupyter", "notebook", "--
+port=8888", "--no-browser", "--ip=0.0.0.0", "--allow-root"] ``` Install from
+GitHub with pip: ``` pip install -q -U git+https://github.com/mljar/mljar-
+supervised.git@master ``` # Demo In the below demo GIF you will see: - MLJAR
+AutoML trained in Jupyter Notebook on titanic dataset - overview of created
+files - showcase of selected plots created during AutoML training - algorithm
+comparison report along with their plots - example of README file and csv file
+with results ![](https://github.com/mljar/mljar-examples/raw/master/media/
+mljar_files.gif) # Contributing To get started take a look at our [Contribution
+Guide](https://supervised.mljar.com/contributing/) for information about our
+process and where you can fit in! ### Contributors [https://contributors-
+img.web.app/image?repo=mljar/mljar-supervised] # Cite Would you like to cite
+MLJAR? Great! :) You can cite MLJAR as following: ``` @misc{mljar, author =
+{Aleksandra P\l{}o\'{n}ska and Piotr P\l{}o\'{n}ski}, year = {2021}, publisher
+= {MLJAR}, address = {\L{}apy, Poland}, title = {MLJAR: State-of-the-art
+Automated Machine Learning Framework for Tabular Data. Version 0.10.3}, url =
+{https://github.com/mljar/mljar-supervised} } ``` Would love to hear from you
+how have you used MLJAR AutoML in your project. Please feel free to let us know
+at ![image](https://user-images.githubusercontent.com/6959032/118103228-
+f5ea9a00-b3d9-11eb-87ed-8cfb1f873f91.png) # License The `mljar-supervised` is
+provided with [MIT license](https://github.com/mljar/mljar-supervised/blob/
+master/LICENSE). # Commercial support Looking for commercial support? Do you
+need new feature implementation? Please contact us by [email](https://
+mljar.com/contact/) for details. # MLJAR
   [https://github.com/mljar/mljar-examples/blob/master/media/large_logo.png]
 The `mljar-supervised` is an open-source project created by [MLJAR](https://
 mljar.com). We care about ease of use in the Machine Learning. The [mljar.com]
 (https://mljar.com) provides a beautiful and simple user interface for building
 machine learning models. Keywords: automated machine learning,automl,machine
 learning,data science,data mining,mljar Platform: UNKNOWN Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python ::
-3.7 Classifier: Programming Language :: Python :: 3.8 Description-Content-Type:
+3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Requires-Python: >=3.7.1 Description-Content-Type:
 text/markdown
```

### Comparing `mljar-supervised-0.9.1/mljar_supervised.egg-info/SOURCES.txt` & `mljar-supervised-1.0.0/mljar_supervised.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -35,14 +35,20 @@
 supervised/callbacks/callback_list.py
 supervised/callbacks/early_stopping.py
 supervised/callbacks/learner_time_constraint.py
 supervised/callbacks/max_iters_constraint.py
 supervised/callbacks/metric_logger.py
 supervised/callbacks/terminate_on_nan.py
 supervised/callbacks/total_time_constraint.py
+supervised/fairness/__init__.py
+supervised/fairness/metrics.py
+supervised/fairness/optimization.py
+supervised/fairness/plots.py
+supervised/fairness/report.py
+supervised/fairness/utils.py
 supervised/preprocessing/__init__.py
 supervised/preprocessing/datetime_transformer.py
 supervised/preprocessing/eda.py
 supervised/preprocessing/encoding_selector.py
 supervised/preprocessing/exclude_missing_target.py
 supervised/preprocessing/goldenfeatures_transformer.py
 supervised/preprocessing/kmeans_transformer.py
@@ -58,30 +64,37 @@
 supervised/tuner/__init__.py
 supervised/tuner/data_info.py
 supervised/tuner/hill_climbing.py
 supervised/tuner/mljar_tuner.py
 supervised/tuner/preprocessing_tuner.py
 supervised/tuner/random_parameters.py
 supervised/tuner/time_controller.py
+supervised/tuner/optuna/__init__.py
+supervised/tuner/optuna/catboost.py
+supervised/tuner/optuna/extra_trees.py
+supervised/tuner/optuna/knn.py
+supervised/tuner/optuna/lightgbm.py
+supervised/tuner/optuna/nn.py
+supervised/tuner/optuna/random_forest.py
+supervised/tuner/optuna/tuner.py
+supervised/tuner/optuna/xgboost.py
 supervised/utils/__init__.py
 supervised/utils/additional_metrics.py
+supervised/utils/additional_plots.py
+supervised/utils/automl_plots.py
 supervised/utils/common.py
 supervised/utils/config.py
 supervised/utils/constants.py
 supervised/utils/data_validation.py
 supervised/utils/importance.py
 supervised/utils/leaderboard_plots.py
 supervised/utils/learning_curves.py
 supervised/utils/metric.py
 supervised/utils/shap.py
 supervised/utils/subsample.py
+supervised/utils/utils.py
 supervised/validation/__init__.py
 supervised/validation/validation_step.py
 supervised/validation/validator_base.py
+supervised/validation/validator_custom.py
 supervised/validation/validator_kfold.py
-supervised/validation/validator_split.py
-supervised/validation/validator_with_dataset.py
-supervised/validation/disabled_t_ests/__init__.py
-supervised/validation/disabled_t_ests/run.py
-supervised/validation/disabled_t_ests/test_validation_step.py
-supervised/validation/disabled_t_ests/test_validator_split.py
-supervised/validation/disabled_t_ests/test_validator_with_dataset.py
+supervised/validation/validator_split.py
```

