# Comparing `tmp/lightwood-23.6.2.0.tar.gz` & `tmp/lightwood-23.6.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightwood-23.6.2.0.tar", last modified: Tue Jun 13 03:08:25 2023, max compression
+gzip compressed data, was "lightwood-23.6.4.0.tar", last modified: Mon Jun 26 14:15:23 2023, max compression
```

## Comparing `lightwood-23.6.2.0.tar` & `lightwood-23.6.4.0.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.239579 lightwood-23.6.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-06-13 03:08:25.239579 lightwood-23.6.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.227579 lightwood-23.6.2.0/lightwood/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/explain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/analysis/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/helpers/acc_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/helpers/conf_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/helpers/feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/helpers/pyod.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/helpers/shap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/analysis/nc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29232 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nc/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nc/icp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nc/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    22328 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nc/nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nc/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/analysis/nn_conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nn_conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nn_conf/temp_scale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/api/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/api/high_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    50810 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/api/json_ai.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/api/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    24999 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/api/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/data/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/data/encoded_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/data/timeseries_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16355 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/data/timeseries_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/encoder/array/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/array/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/array/ts_cat_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/array/ts_num_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/encoder/audio/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/audio/mfcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/encoder/categorical/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/categorical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/categorical/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/categorical/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/categorical/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/categorical/multihot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/categorical/onehot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/encoder/datetime/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/datetime/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/datetime/datetime_sin_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/encoder/identity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/identity/identity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/encoder/image/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/encoder/image/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/image/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/image/helpers/img_to_vec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/image/img_2_vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/encoder/numeric/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/numeric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/numeric/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/numeric/ts_numeric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/encoder/text/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/encoder/text/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/text/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/text/helpers/pretrained_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    29481 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/text/helpers/rnn_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/text/pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/text/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/text/short.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/text/tfidf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/text/vocab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/encoder/time_series/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/time_series/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/encoder/time_series/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/time_series/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/time_series/helpers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/time_series/helpers/rnn_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/time_series/helpers/transformer_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23498 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/time_series/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/time_series/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/ensemble/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/ensemble/best_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/ensemble/mean_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/ensemble/mode_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/ensemble/stacked_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/ensemble/ts_stacked_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/ensemble/weighted_mean_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.239579 lightwood-23.6.2.0/lightwood/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/parallelism.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.239579 lightwood-23.6.2.0/lightwood/mixer/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/arima.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/ets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.239579 lightwood-23.6.2.0/lightwood/mixer/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/helpers/ar_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/helpers/default_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/helpers/qclassic_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/helpers/ranger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/helpers/residual_net.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/helpers/ts.py
--rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/lightgbm_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/neural.py
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/neural_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/nhits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/prophet.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/qclassic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/sktime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/tabtransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/xgboost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-06-13 03:08:25.000000 lightwood-23.6.2.0/lightwood.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-06-13 03:08:25.000000 lightwood-23.6.2.0/lightwood.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:08:25.000000 lightwood-23.6.2.0/lightwood.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-13 03:08:25.000000 lightwood-23.6.2.0/lightwood.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 03:08:25.000000 lightwood-23.6.2.0/lightwood.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 03:08:25.239579 lightwood-23.6.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.782922 lightwood-23.6.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-06-26 14:15:23.782922 lightwood-23.6.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.766922 lightwood-23.6.4.0/lightwood/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.766922 lightwood-23.6.4.0/lightwood/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/explain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.766922 lightwood-23.6.4.0/lightwood/analysis/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/helpers/acc_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/helpers/conf_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/helpers/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/helpers/pyod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/helpers/shap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/analysis/nc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29232 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nc/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nc/icp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nc/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22328 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nc/nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nc/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/analysis/nn_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nn_conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/analysis/nn_conf/temp_scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/api/high_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51184 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/api/json_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/api/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24999 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/api/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/data/encoded_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/data/timeseries_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/data/timeseries_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/encoder/array/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/array/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/array/ts_cat_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/array/ts_num_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/encoder/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/audio/mfcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/encoder/categorical/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/categorical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/categorical/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/categorical/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/categorical/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/categorical/multihot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/categorical/onehot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/encoder/datetime/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/datetime/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/datetime/datetime_sin_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/encoder/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/identity/identity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.770922 lightwood-23.6.4.0/lightwood/encoder/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.774922 lightwood-23.6.4.0/lightwood/encoder/image/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/image/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/image/helpers/img_to_vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/image/img_2_vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.774922 lightwood-23.6.4.0/lightwood/encoder/numeric/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/numeric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/numeric/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/numeric/ts_numeric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.774922 lightwood-23.6.4.0/lightwood/encoder/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.774922 lightwood-23.6.4.0/lightwood/encoder/text/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/text/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/text/helpers/pretrained_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29481 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/text/helpers/rnn_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/text/pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/text/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/text/short.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/text/tfidf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/text/vocab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.774922 lightwood-23.6.4.0/lightwood/encoder/time_series/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/time_series/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.774922 lightwood-23.6.4.0/lightwood/encoder/time_series/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/time_series/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/time_series/helpers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/time_series/helpers/rnn_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/time_series/helpers/transformer_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23548 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/time_series/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/encoder/time_series/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.774922 lightwood-23.6.4.0/lightwood/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/ensemble/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/ensemble/best_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/ensemble/mean_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/ensemble/mode_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/ensemble/stacked_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/ensemble/ts_stacked_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/ensemble/weighted_mean_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.778922 lightwood-23.6.4.0/lightwood/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/parallelism.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/helpers/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.778922 lightwood-23.6.4.0/lightwood/mixer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/arima.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/ets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.782922 lightwood-23.6.4.0/lightwood/mixer/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/helpers/ar_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/helpers/default_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/helpers/qclassic_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/helpers/ranger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/helpers/residual_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/helpers/ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/lightgbm_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/neural.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/neural_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/nhits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/prophet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/qclassic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/sktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/tabtransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/lightwood/mixer/xgboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:15:23.766922 lightwood-23.6.4.0/lightwood.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-06-26 14:15:23.000000 lightwood-23.6.4.0/lightwood.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-06-26 14:15:23.000000 lightwood-23.6.4.0/lightwood.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:15:23.000000 lightwood-23.6.4.0/lightwood.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-26 14:15:23.000000 lightwood-23.6.4.0/lightwood.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-26 14:15:23.000000 lightwood-23.6.4.0/lightwood.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:15:23.782922 lightwood-23.6.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-26 14:15:10.000000 lightwood-23.6.4.0/setup.py
```

### Comparing `lightwood-23.6.2.0/LICENSE` & `lightwood-23.6.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/PKG-INFO` & `lightwood-23.6.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightwood
-Version: 23.6.2.0
+Version: 23.6.4.0
 Summary: Lightwood is a toolkit for automatic machine learning model building
 Home-page: https://github.com/mindsdb/lightwood
 Author: MindsDB Inc
 Author-email: community@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/lightwood
 Description: # Lightwood
@@ -216,15 +216,15 @@
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: extra
 Provides-Extra: extra_ts
-Provides-Extra: xai
+Provides-Extra: dev
 Provides-Extra: quantum
+Provides-Extra: xai
 Provides-Extra: image
 Provides-Extra: audio
-Provides-Extra: dev
-Provides-Extra: extra
 Provides-Extra: all_extras
```

### Comparing `lightwood-23.6.2.0/README.md` & `lightwood-23.6.4.0/README.md`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/analysis/__init__.py` & `lightwood-23.6.4.0/lightwood/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/analysis/analyze.py` & `lightwood-23.6.4.0/lightwood/analysis/analyze.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/analysis/base.py` & `lightwood-23.6.4.0/lightwood/analysis/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/analysis/explain.py` & `lightwood-23.6.4.0/lightwood/analysis/explain.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/analysis/helpers/acc_stats.py` & `lightwood-23.6.4.0/lightwood/analysis/helpers/acc_stats.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/analysis/helpers/conf_stats.py` & `lightwood-23.6.4.0/lightwood/analysis/helpers/conf_stats.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/analysis/helpers/feature_importance.py` & `lightwood-23.6.4.0/lightwood/analysis/helpers/feature_importance.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/analysis/helpers/pyod.py` & `lightwood-23.6.4.0/lightwood/analysis/helpers/pyod.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/analysis/helpers/shap.py` & `lightwood-23.6.4.0/lightwood/analysis/helpers/shap.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/analysis/nc/base.py` & `lightwood-23.6.4.0/lightwood/analysis/nc/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/analysis/nc/calibrate.py` & `lightwood-23.6.4.0/lightwood/analysis/nc/calibrate.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/analysis/nc/icp.py` & `lightwood-23.6.4.0/lightwood/analysis/nc/icp.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/analysis/nc/metrics.py` & `lightwood-23.6.4.0/lightwood/analysis/nc/metrics.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/analysis/nc/nc.py` & `lightwood-23.6.4.0/lightwood/analysis/nc/nc.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/analysis/nc/norm.py` & `lightwood-23.6.4.0/lightwood/analysis/nc/norm.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/analysis/nc/util.py` & `lightwood-23.6.4.0/lightwood/analysis/nc/util.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/analysis/nn_conf/temp_scale.py` & `lightwood-23.6.4.0/lightwood/analysis/nn_conf/temp_scale.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/api/__init__.py` & `lightwood-23.6.4.0/lightwood/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/api/high_level.py` & `lightwood-23.6.4.0/lightwood/api/high_level.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/api/json_ai.py` & `lightwood-23.6.4.0/lightwood/api/json_ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -737,15 +737,14 @@
             "module": "transform_timeseries",
             "args": {
                 "timeseries_settings": "$problem_definition.timeseries_settings",
                 "data": "data",
                 "dtype_dict": "$dtype_dict",
                 "target": "$target",
                 "mode": "$mode",
-                "ts_analysis": "$ts_analysis",
                 "pred_args": "$pred_args",
             },
         },
         "timeseries_analyzer": {
             "module": "timeseries_analyzer",
             "args": {
                 "timeseries_settings": "$problem_definition.timeseries_settings",
@@ -1332,16 +1331,26 @@
 
     try:
         import black
     except Exception:
         black = None
 
     if black is not None:
+        try:
+            formatted_predictor_code = black.format_str(predictor_code, mode=black.FileMode())
+
+            if type(predictor_from_code(formatted_predictor_code)).__name__ == 'Predictor':
+                predictor_code = formatted_predictor_code
+            else:
+                log.info('Black formatter output is invalid, predictor code might be a bit ugly')
+
+        except Exception:
+            log.info('Black formatter failed to run, predictor code might be a bit ugly')
+    else:
         log.info('Unable to import black formatter, predictor code might be a bit ugly.')
-        predictor_code = black.format_str(predictor_code, mode=black.FileMode())
 
     return predictor_code
 
 
 def validate_json_ai(json_ai: JsonAI) -> bool:
     """
     Checks the validity of a ``JsonAI`` object
```

### Comparing `lightwood-23.6.2.0/lightwood/api/predictor.py` & `lightwood-23.6.4.0/lightwood/api/predictor.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/api/types.py` & `lightwood-23.6.4.0/lightwood/api/types.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/data/encoded_ds.py` & `lightwood-23.6.4.0/lightwood/data/encoded_ds.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/data/timeseries_transform.py` & `lightwood-23.6.4.0/lightwood/data/timeseries_transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from typing import Dict, Optional
 from functools import partial
 import multiprocessing as mp
 
 import numpy as np
 import pandas as pd
 from lightwood.helpers.parallelism import get_nr_procs
-from lightwood.helpers.ts import get_ts_groups, get_delta, get_group_matches
 
 from type_infer.dtype import dtype
 from lightwood.api.types import TimeseriesSettings, PredictionArguments
 from lightwood.helpers.log import log
 
 
 def transform_timeseries(
-        data: pd.DataFrame, dtype_dict: Dict[str, str], ts_analysis: dict,
+        data: pd.DataFrame, dtype_dict: Dict[str, str],
         timeseries_settings: TimeseriesSettings, target: str, mode: str,
         pred_args: Optional[PredictionArguments] = None
 ) -> pd.DataFrame:
     """
     Block that transforms the dataframe of a time series task to a convenient format for use in posterior phases like model training.
     
     The main transformations performed by this block are:
@@ -25,67 +24,62 @@
       - Windowing functions for historical context based on `TimeseriesSettings.window` parameter.
       - Explicitly add target columns according to the `TimeseriesSettings.horizon` parameter.
       - Flag all rows that are "predictable" based on all `TimeseriesSettings`.
       - Plus, handle all logic for the streaming use case (where forecasts are only emitted for the last observed data point).
     
     :param data: Dataframe with data to transform.
     :param dtype_dict: Dictionary with the types of each column.
-    :param ts_analysis: dictionary with various insights into each series passed as training input.
     :param timeseries_settings: A `TimeseriesSettings` object.
     :param target: The name of the target column to forecast.
     :param mode: Either "train" or "predict", depending on what phase is calling this procedure.
     :param pred_args: Optional prediction arguments to control the transformation process.
     
     :return: A dataframe with all the transformations applied.
     """  # noqa
 
     pred_args = PredictionArguments() if pred_args is None else pred_args
     tss = timeseries_settings
     gb_arr = tss.group_by if tss.group_by is not None else []
     oby = tss.order_by
     window = tss.window
+    oby_col = tss.order_by
 
     if tss.use_previous_target and target not in data.columns:
         raise Exception(f"Cannot transform. Missing historical values for target column {target} (`use_previous_target` is set to True).")  # noqa
 
     for hcol in tss.historical_columns:
         if hcol not in data.columns or data[hcol].isna().any():
             raise Exception(f"Cannot transform. Missing values in historical column {hcol}.")
 
-    # infer frequency with get_delta
-    oby_col = tss.order_by
-    groups = get_ts_groups(data, tss)
-
-    # initial stable sort and per-partition deduplication
+    # initial stable sort and per-partition deduplication TODO: slowish, add a top-level param to disable if needed
     data = data.sort_values(by=oby_col, kind='mergesort')
     data = data.drop_duplicates(subset=[oby_col, *gb_arr], keep='first')
 
-    if not ts_analysis:
-        _, periods, freqs = get_delta(data, dtype_dict, groups, target, tss)
-    else:
-        periods = ts_analysis['periods']
-        freqs = ts_analysis['sample_freqs']
-
     # pass seconds to timestamps according to each group's inferred freq, and force this freq on index
-    subsets = []
-    for group in groups:
-        if (tss.group_by and group != '__default') or not tss.group_by:
-            idxs, subset = get_group_matches(data, group, tss.group_by, copy=True)
-            if subset.shape[0] > 0:
-                if periods.get(group, periods['__default']) == 0 and subset.shape[0] > 1:
-                    raise Exception(
-                        f"Partition is not valid, faulty group {group}. Please make sure you group by a set of columns that ensures unique measurements for each grouping through time.")  # noqa
-
-                index = pd.to_datetime(subset[oby_col], unit='s')
-                subset.index = pd.date_range(start=index.iloc[0],
-                                             freq=freqs.get(group, freqs['__default']),
-                                             periods=len(subset))
-                subset['__mdb_inferred_freq'] = subset.index.freq   # sets constant column because pd.concat forgets freq (see: https://github.com/pandas-dev/pandas/issues/3232)  # noqa
-                subsets.append(subset)
-    original_df = pd.concat(subsets).sort_values(by='__mdb_original_index')
+    grouped = data.groupby(by=tss.group_by) if tss.group_by else data.groupby(lambda x: True)
+    reindexed = []
+    # TODO: introduce MP here
+    for name, group in grouped:
+        name = name if tss.group_by and len(tss.group_by) > 1 else (name, )  # guaranteed tuple type
+        if group.shape[0] > 0:
+            if group[tss.order_by].value_counts().max() > 1 and group.shape[0] > 1:
+                raise Exception(f"Partition is not valid, faulty group {name}. Please make sure you group by a set of columns that ensures unique measurements for each grouping through time.")  # noqa
+
+            index = pd.to_datetime(group[oby_col], unit='s', utc=True)
+            group.index = pd.date_range(start=index.iloc[0], end=index.iloc[-1], periods=len(group))
+            resampled = group
+            group['__mdb_inferred_freq'] = None
+            if len(group) > 2:
+                freq = pd.infer_freq(group.index)
+                if freq is not None:
+                    group['__mdb_inferred_freq'] = freq  # sets constant column because pd.concat forgets freq (see: https://github.com/pandas-dev/pandas/issues/3232)  # noqa
+                    resampled = group.resample(freq).first()
+            reindexed.append(resampled)
+
+    original_df = pd.concat(reindexed).sort_values(by='__mdb_original_index')
 
     if '__mdb_forecast_offset' in original_df.columns:
         """ This special column can be either None or an integer. If this column is passed, then the TS transformation will react to the values within:
 
         * If all rows = `None`, proceed as usual. This ends up generating one HORIZON-length forecast for each row in the DF.
         * If all rows have the same value `N <= 0`, then cutoff the dataframe latest `-N` rows after TS shaping and prime the DF (with `__make_predictions` column) so that a forecast is generated only for the last row (thus more efficient). This enables `WHERE T = LATEST - K` with `0 <= K < WINDOW` syntax upstream in MindsDB.
         * If all rows have the same value `N = 1`, then activate streaming inference mode where a single forecast will be emitted for the timestamp inferred by the `_ts_infer_next_row` method. This enables the (already supported) `WHERE T > LATEST` syntax.
@@ -99,26 +93,20 @@
             offset = 0
         cutoff_mode = offset_available and offset == 1
     else:
         offset_available = False
         offset = 0
         cutoff_mode = False
 
-    original_index_list = []
-    idx = 0
-    for row in original_df.itertuples():
-        if _make_pred(row) or cutoff_mode:
-            original_df.at[row.Index, '__make_predictions'] = True
-            original_index_list.append(idx)
-            idx += 1
-        else:
-            original_df.at[row.Index, '__make_predictions'] = False
-            original_index_list.append(None)
-
-    original_df['original_index'] = original_index_list
+    if '__mdb_forecast_offset' in original_df.columns or cutoff_mode:
+        original_df['__make_predictions'] = True
+        original_df['original_index'] = np.arange(len(original_df))
+    else:
+        original_df['__make_predictions'] = False
+        original_df['original_index'] = None
 
     secondary_type_dict = {}
     if dtype_dict[oby] in (dtype.date, dtype.integer, dtype.float):
         secondary_type_dict[oby] = dtype_dict[oby]
 
     original_df[f'__mdb_original_{oby}'] = original_df[oby]
     group_lengths = []
@@ -187,47 +175,20 @@
 
     if not cutoff_mode and any([i < tss.window for i in group_lengths]):
         if tss.allow_incomplete_history:
             log.warning("Forecasting with incomplete historical context, predictions might be subpar")
         else:
             raise Exception(f'Not enough historical context to make a timeseries prediction (`allow_incomplete_history` is set to False). Please provide a number of rows greater or equal to the window size - currently (number_rows, window_size) = ({min(group_lengths)}, {tss.window}). If you can\'t get enough rows, consider lowering your window size. If you want to force timeseries predictions lacking historical context please set the `allow_incomplete_history` timeseries setting to `True`, but this might lead to subpar predictions depending on the mixer.') # noqa
 
-    df_gb_map = None
     if n_groups > 1:
         df_gb_list = list(combined_df.groupby(tss.group_by))
         df_gb_map = {}
         for gb, df in df_gb_list:
             df_gb_map['_' + '_'.join(str(gb))] = df
 
-    timeseries_row_mapping = {}
-    idx = 0
-
-    if df_gb_map is None:
-        for i in range(len(combined_df)):
-            row = combined_df.iloc[i]
-            if not cutoff_mode:
-                timeseries_row_mapping[idx] = int(
-                    row['original_index']) if row['original_index'] is not None and not np.isnan(
-                    row['original_index']) else None
-            else:
-                timeseries_row_mapping[idx] = idx
-            idx += 1
-    else:
-        for gb in df_gb_map:
-            for i in range(len(df_gb_map[gb])):
-                row = df_gb_map[gb].iloc[i]
-                if not cutoff_mode:
-                    timeseries_row_mapping[idx] = int(
-                        row['original_index']) if row['original_index'] is not None and not np.isnan(
-                        row['original_index']) else None
-                else:
-                    timeseries_row_mapping[idx] = idx
-
-                idx += 1
-
     del combined_df['original_index']
 
     return combined_df
 
 
 def _ts_infer_next_row(df: pd.DataFrame, ob: str) -> pd.DataFrame:
     """
@@ -252,21 +213,14 @@
 
     last_row[ob] += delta
     new_df = df.append(last_row)
     new_df.index = pd.DatetimeIndex(new_index)
     return new_df
 
 
-def _make_pred(row) -> bool:
-    """
-    Indicates whether a prediction should be made for `row` or not.
-    """
-    return not hasattr(row, '__mdb_forecast_offset') or row.make_predictions
-
-
 def _ts_to_obj(df: pd.DataFrame, historical_columns: list) -> pd.DataFrame:
     """
     Casts all historical columns in a dataframe to `object` type.
 
     :param df: Input dataframe
     :param historical_columns: Historical columns to type cast
```

### Comparing `lightwood-23.6.2.0/lightwood/encoder/__init__.py` & `lightwood-23.6.4.0/lightwood/encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/array/array.py` & `lightwood-23.6.4.0/lightwood/encoder/array/array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/array/ts_cat_array.py` & `lightwood-23.6.4.0/lightwood/encoder/array/ts_cat_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/array/ts_num_array.py` & `lightwood-23.6.4.0/lightwood/encoder/array/ts_num_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/audio/mfcc.py` & `lightwood-23.6.4.0/lightwood/encoder/audio/mfcc.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/base.py` & `lightwood-23.6.4.0/lightwood/encoder/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/categorical/autoencoder.py` & `lightwood-23.6.4.0/lightwood/encoder/categorical/autoencoder.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/categorical/binary.py` & `lightwood-23.6.4.0/lightwood/encoder/categorical/binary.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/categorical/gym.py` & `lightwood-23.6.4.0/lightwood/encoder/categorical/gym.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/categorical/multihot.py` & `lightwood-23.6.4.0/lightwood/encoder/categorical/multihot.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/categorical/onehot.py` & `lightwood-23.6.4.0/lightwood/encoder/categorical/onehot.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/datetime/datetime.py` & `lightwood-23.6.4.0/lightwood/encoder/datetime/datetime_sin_normalizer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import datetime
 import calendar
-from typing import Optional
+import numpy as np
+import pandas as pd  # @TODO: remove?
 import torch
 from lightwood.encoder.base import BaseEncoder
+from collections.abc import Iterable
 from lightwood.helpers.general import is_none
 
 
-class DatetimeEncoder(BaseEncoder):
-    """
-    This encoder produces an encoded representation for timestamps.
-
-    The approach consists on decomposing the timestamp objects into its constituent units (e.g. day-of-week, month, year, etc), and describing each of those with a single value that represents the magnitude in a sensible cycle length.
-    """  # noqa
-    def __init__(self, is_target: bool = False):
+class DatetimeNormalizerEncoder(BaseEncoder):
+    def __init__(self, is_target: bool = False, sinusoidal: bool = False):
         super().__init__(is_target)
+        self.sinusoidal = sinusoidal
         self.fields = ['year', 'month', 'day', 'weekday', 'hour', 'minute', 'second']
         self.constants = {'year': 3000.0, 'month': 12.0, 'weekday': 7.0,
                           'hour': 24.0, 'minute': 60.0, 'second': 60.0}
-        self.output_size = 7
+        if self.sinusoidal:
+            self.output_size = 2
+        else:
+            self.output_size = 7
 
     def prepare(self, priming_data):
         if self.is_prepared:
             raise Exception('You can only call "prepare" once for a given encoder.')
 
         self.is_prepared = True
 
@@ -29,34 +30,51 @@
         """
         :param data: # @TODO: receive a consistent data type here; currently either list of lists or pd.Series w/lists
         :return: encoded data
         """
         if not self.is_prepared:
             raise Exception('You need to call "prepare" before calling "encode" or "decode".')
 
-        ret = [self.encode_one(unix_timestamp) for unix_timestamp in data]
+        if isinstance(data, pd.Series):
+            data = data.values
+        if not isinstance(data[0], Iterable):
+            data = [data]
+
+        ret = [self.encode_one(row) for row in data]
 
         return torch.Tensor(ret)
 
-    def encode_one(self, unix_timestamp: Optional[float]):
+    def encode_one(self, data):
         """
         Encodes a list of unix_timestamps, or a list of tensors with unix_timestamps
         :param data: list of unix_timestamps (unix_timestamp resolution is seconds)
         :return: a list of vectors
         """
-        if is_none(unix_timestamp):
-            vector = [0] * len(self.fields)
-        else:
-            c = self.constants
-            date = datetime.datetime.fromtimestamp(unix_timestamp)
-            day_constant = calendar.monthrange(date.year, date.month)[1]
-            vector = [date.year / c['year'], date.month / c['month'], date.day / day_constant,
-                      date.weekday() / c['weekday'], date.hour / c['hour'],
-                      date.minute / c['minute'], date.second / c['second']]
-        return vector
+        ret = []
+        for unix_timestamp in data:
+            if is_none(unix_timestamp):
+                if self.sinusoidal:
+                    vector = [0, 1] * len(self.fields)
+                else:
+                    vector = [0] * len(self.fields)
+            else:
+                c = self.constants
+                if isinstance(unix_timestamp, torch.Tensor):
+                    unix_timestamp = unix_timestamp.item()
+                date = datetime.datetime.fromtimestamp(unix_timestamp)
+                day_constant = calendar.monthrange(date.year, date.month)[1]
+                vector = [date.year / c['year'], date.month / c['month'], date.day / day_constant,
+                          date.weekday() / c['weekday'], date.hour / c['hour'],
+                          date.minute / c['minute'], date.second / c['second']]
+                if self.sinusoidal:
+                    vector = np.array([(np.sin(n), np.cos(n)) for n in vector]).flatten()
+
+            ret.append(vector)
+
+        return ret
 
     def decode(self, encoded_data, return_as_datetime=False):
         ret = []
         if len(encoded_data.shape) > 2 and encoded_data.shape[0] == 1:
             encoded_data = encoded_data.squeeze(0)
 
         for vector in encoded_data.tolist():
@@ -65,14 +83,16 @@
         return ret
 
     def decode_one(self, vector, return_as_datetime=False):
         if sum(vector) == 0:
             decoded = None
 
         else:
+            if self.sinusoidal:
+                vector = list(map(lambda x: np.arcsin(x), vector))[::2]
             c = self.constants
 
             year = max(0, round(vector[0] * c['year']))
             month = max(1, min(12, round(vector[1] * c['month'])))
             day_constant = calendar.monthrange(year, month)[-1]
             day = max(1, min(round(vector[2] * day_constant), day_constant))
             hour = max(0, min(23, round(vector[4] * c['hour'])))
```

### Comparing `lightwood-23.6.2.0/lightwood/encoder/helpers.py` & `lightwood-23.6.4.0/lightwood/encoder/helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/identity/identity.py` & `lightwood-23.6.4.0/lightwood/encoder/identity/identity.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/image/helpers/img_to_vec.py` & `lightwood-23.6.4.0/lightwood/encoder/image/helpers/img_to_vec.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/image/img_2_vec.py` & `lightwood-23.6.4.0/lightwood/encoder/image/img_2_vec.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/numeric/numeric.py` & `lightwood-23.6.4.0/lightwood/encoder/numeric/numeric.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/numeric/ts_numeric.py` & `lightwood-23.6.4.0/lightwood/encoder/numeric/ts_numeric.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/text/helpers/pretrained_helpers.py` & `lightwood-23.6.4.0/lightwood/encoder/text/helpers/pretrained_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/text/helpers/rnn_helpers.py` & `lightwood-23.6.4.0/lightwood/encoder/text/helpers/rnn_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/text/pretrained.py` & `lightwood-23.6.4.0/lightwood/encoder/text/pretrained.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/text/rnn.py` & `lightwood-23.6.4.0/lightwood/encoder/text/rnn.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/text/short.py` & `lightwood-23.6.4.0/lightwood/encoder/text/short.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/text/tfidf.py` & `lightwood-23.6.4.0/lightwood/encoder/text/tfidf.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/text/vocab.py` & `lightwood-23.6.4.0/lightwood/encoder/text/vocab.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/time_series/helpers/common.py` & `lightwood-23.6.4.0/lightwood/encoder/time_series/helpers/common.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 
 import pandas as pd
 
 from lightwood.api.types import TimeseriesSettings
 from type_infer.dtype import dtype
 from lightwood.encoder.helpers import MinMaxNormalizer, CatNormalizer
-from lightwood.helpers.ts import get_group_matches
 
 
 def generate_target_group_normalizers(
         data: pd.DataFrame,
         target: str,
         dtype_dict: dict,
-        groups: list,
         tss: TimeseriesSettings
 ):
     """
     Helper function called from data_source. It generates and fits all needed normalizers for a target variable based on its grouped entities.
     
     :return: modified data with dictionary with normalizers for said target variable based on some grouped-by columns
     """  # noqa
@@ -25,24 +23,23 @@
     # categorical normalizers
     if target_dtype in (dtype.categorical, dtype.binary, dtype.cat_tsarray):
         normalizers['__default'] = CatNormalizer()
         normalizers['__default'].prepare(data)
 
     # numerical normalizers, here we spawn one per each group combination
     else:
-        for combination in groups:
-            if combination not in ('__default', ()):
-                combination = tuple(combination)
-                idxs, subset = get_group_matches(data, combination, tss.group_by)
-                if subset.shape[0] > 0:
-                    target_data = subset[target].values
-                    if target_dtype == dtype.num_tsarray:
-                        target_data = target_data.reshape(-1, 1).astype(float)
-
-                    normalizers[combination] = MinMaxNormalizer(combination=combination)
-                    normalizers[combination].prepare(target_data)
-
-        # ...plus a default one, used at inference time and fitted with all training data
-        normalizers['__default'] = MinMaxNormalizer()
-        normalizers['__default'].prepare(data[target].values)
+        grouped = data.groupby(by=tss.group_by) if tss.group_by else data.groupby(lambda x: '__default')
+        for name, subset in grouped:
+            if subset.shape[0] > 0:
+                target_data = subset[target].values
+                if target_dtype == dtype.num_tsarray:
+                    target_data = target_data.reshape(-1, 1).astype(float)
+
+                normalizers[name] = MinMaxNormalizer(combination=name)
+                normalizers[name].prepare(target_data)
+
+        if not normalizers.get('__default'):
+            # ...plus a default one, used at inference time and fitted with all training data
+            normalizers['__default'] = MinMaxNormalizer()
+            normalizers['__default'].prepare(data[target].values)
 
     return normalizers
```

### Comparing `lightwood-23.6.2.0/lightwood/encoder/time_series/helpers/rnn_helpers.py` & `lightwood-23.6.4.0/lightwood/encoder/time_series/helpers/rnn_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/time_series/helpers/transformer_helpers.py` & `lightwood-23.6.4.0/lightwood/encoder/time_series/helpers/transformer_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/encoder/time_series/rnn.py` & `lightwood-23.6.4.0/lightwood/encoder/time_series/rnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from lightwood.helpers.log import log
 from lightwood.encoder.base import BaseEncoder
 from lightwood.helpers.device import get_device_from_name
 from lightwood.helpers.torch import LightwoodAutocast
 from lightwood.encoder.datetime import DatetimeNormalizerEncoder
 from lightwood.encoder.time_series.helpers.rnn_helpers import EncoderRNNNumerical, DecoderRNNNumerical
 from lightwood.encoder.helpers import MinMaxNormalizer, CatNormalizer
-from lightwood.helpers.ts import get_group_matches
 from lightwood.encoder.time_series.helpers.transformer_helpers import TransformerEncoder, get_chunk, len_to_mask
 
 
 class TimeSeriesEncoder(BaseEncoder):
     """
     Time series encoder. This module can learn features for any `order_by` temporal column, both with and without accompanying target data.
 
@@ -194,20 +193,21 @@
         for dep_name, dep_data in dependency_data.items():
             if dep_name in self.grouped_by:
                 continue
             if dep_data['original_type'] in (dtype.integer, dtype.float):
                 dep_data['group_info'] = {group: dependency_data[group]['data'] for group in self.grouped_by}
                 data = torch.zeros((len(priming_data), lengths_data.max().int().item(), 1))
                 all_idxs = set(range(len(data)))
+                grouped = dep_data['data'].groupby(by=self.grouped_by)
                 for group_name, normalizer in self.dep_norms[dep_name].items():
                     if group_name != '__default':
-                        idxs, subset = get_group_matches(dep_data, normalizer.combination)
+                        subset = grouped.get_group(normalizer.combination)
                         normalized = normalizer.encode(subset).unsqueeze(-1)
-                        data[idxs, :, :] = normalized
-                        all_idxs -= set(idxs)
+                        data[subset.index, :, :] = normalized
+                        all_idxs -= set(subset.index)
                 if len(all_idxs) > 0 and '__default' in self.dep_norms[dep_name].keys():
                     default_norm = self.dep_norms[dep_name]['__default']
                     subset = [dep_data['data'][idx] for idx in list(all_idxs)]
                     data[list(all_idxs), :, :] = torch.Tensor(default_norm.encode(subset)).unsqueeze(-1)
 
             else:
                 # categorical has only one normalizer at all times
@@ -375,22 +375,22 @@
                     dep_info = {
                         'group_info': {group: dependency_data[group] for group in self.grouped_by},
                         'data': dep_data
                     }
                     tensor = torch.zeros((len(dep_data), len(dep_data[0]), 1)).to(self.device)
                     all_idxs = set(range(len(dep_data)))
 
+                    grouped = dep_info['data'].groupby(by=self.grouped_by)
                     for combination in [c for c in self._group_combinations if c != '__default']:
                         normalizer = self.dep_norms[dep].get(tuple(combination), None)
                         if normalizer is None:
                             normalizer = self.dep_norms[dep]['__default']
-                        idxs, subset = get_group_matches(dep_info, normalizer.combination)
-                        if idxs:
-                            tensor[idxs, :, :] = torch.Tensor(normalizer.encode(subset)).unsqueeze(-1).to(self.device)
-                            all_idxs -= set(idxs)
+                        subdf = grouped.get_group(normalizer.combination)
+                        tensor[subdf.index, :, :] = torch.Tensor(normalizer.encode(subdf)).unsqueeze(-1).to(self.device)
+                        all_idxs -= set(subdf.index)
 
                     # encode all remaining rows (not belonging to any grouped combination) with default normalizer
                     if all_idxs:
                         default_norm = self.dep_norms[dep]['__default']
                         subset = [dep_data[idx] for idx in all_idxs]
                         tensor[list(all_idxs), :, :] = torch.Tensor(
                             default_norm.encode(subset)).unsqueeze(-1).to(self.device)
```

### Comparing `lightwood-23.6.2.0/lightwood/encoder/time_series/ts.py` & `lightwood-23.6.4.0/lightwood/encoder/time_series/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/ensemble/__init__.py` & `lightwood-23.6.4.0/lightwood/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/ensemble/base.py` & `lightwood-23.6.4.0/lightwood/ensemble/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/ensemble/best_of.py` & `lightwood-23.6.4.0/lightwood/ensemble/best_of.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/ensemble/mean_ensemble.py` & `lightwood-23.6.4.0/lightwood/ensemble/mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/ensemble/mode_ensemble.py` & `lightwood-23.6.4.0/lightwood/ensemble/mode_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/ensemble/stacked_ensemble.py` & `lightwood-23.6.4.0/lightwood/ensemble/stacked_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/ensemble/ts_stacked_ensemble.py` & `lightwood-23.6.4.0/lightwood/ensemble/ts_stacked_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/ensemble/weighted_mean_ensemble.py` & `lightwood-23.6.4.0/lightwood/ensemble/weighted_mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/helpers/__init__.py` & `lightwood-23.6.4.0/lightwood/helpers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from lightwood.helpers.device import is_cuda_compatible, get_devices
 from lightwood.helpers.general import is_none
-from lightwood.helpers.ts import get_group_matches, get_ts_groups, get_inferred_timestamps, add_tn_num_conf_bounds, \
-    add_tn_cat_conf_bounds
+from lightwood.helpers.ts import get_ts_groups, get_inferred_timestamps, add_tn_num_conf_bounds, add_tn_cat_conf_bounds
 from lightwood.helpers.io import read_from_path_or_url
 from lightwood.helpers.parallelism import get_nr_procs, mut_method_call, run_mut_method
 from lightwood.helpers.numeric import filter_nan_and_none
 from lightwood.helpers.seed import seed
 from lightwood.helpers.torch import average_vectors, concat_vectors_and_pad, LightwoodAutocast
 
 
 __all__ = ['is_cuda_compatible', 'get_devices', 'mut_method_call', 'run_mut_method',
-           'get_group_matches', 'get_ts_groups', 'is_none', 'read_from_path_or_url', 'seed',
+           'get_ts_groups', 'is_none', 'read_from_path_or_url', 'seed',
            'get_inferred_timestamps', 'add_tn_num_conf_bounds', 'add_tn_cat_conf_bounds', 'get_nr_procs',
            'average_vectors', 'concat_vectors_and_pad', 'LightwoodAutocast', 'filter_nan_and_none' ]  # noqa
```

### Comparing `lightwood-23.6.2.0/lightwood/helpers/device.py` & `lightwood-23.6.4.0/lightwood/helpers/device.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/helpers/general.py` & `lightwood-23.6.4.0/lightwood/helpers/general.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,41 @@
+from typing import Iterable
+
+import numpy as np
 from type_infer.helpers import is_nan_numeric
 
 
 def is_none(value):
     """
     Pandas has no way to guarantee "stability" for the type of a column, it choses to arbitrarily change it based on the values.
     Pandas also change the values in the columns based on the types.
     Lightwood relies on having ``None`` values for a cells that represent "missing" or "corrupt".
     
     When we assign ``None`` to a cell in a dataframe this might get turned to `nan` or other values, this function checks if a cell is ``None`` or any other values a pd.DataFrame might convert ``None`` to.
 
     It also checks some extra values (like ``''``) that pandas never converts ``None`` to (hopefully). But lightwood would still consider those values "None values", and this will allow for more generic use later.
     """ # noqa
+    # TODO: consider removing this helper entirely, arguably should move into dataprep_ml
+
+    # start dispatch with types that are expensive to e.g. cast into strings
+    if type(value) in (np.ndarray,) and value.size == 0:
+        return True
+
+    if type(value) != str and isinstance(value, Iterable) and value == []:
+        return True
+    elif type(value) != str and isinstance(value, Iterable):
+        return False
+
     if value is None:
         return True
 
     if is_nan_numeric(value):
         return True
 
     if str(value) == '':
         return True
 
-    if str(value) in ('None', 'nan', 'NaN', 'np.nan'):
+    if str(value) in ('None', 'nan', 'NaN', 'np.nan', 'NAN', 'NONE'):
         return True
 
     return False
```

### Comparing `lightwood-23.6.2.0/lightwood/helpers/io.py` & `lightwood-23.6.4.0/lightwood/helpers/io.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/helpers/log.py` & `lightwood-23.6.4.0/lightwood/helpers/log.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/helpers/parallelism.py` & `lightwood-23.6.4.0/lightwood/helpers/parallelism.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/helpers/templating.py` & `lightwood-23.6.4.0/lightwood/helpers/templating.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/helpers/text.py` & `lightwood-23.6.4.0/lightwood/helpers/text.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/helpers/torch.py` & `lightwood-23.6.4.0/lightwood/helpers/torch.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/helpers/ts.py` & `lightwood-23.6.4.0/lightwood/helpers/ts.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,53 @@
-from typing import List, Tuple, Union, Dict
+from typing import Tuple, Dict
 from datetime import datetime
 
 import numpy as np
 import pandas as pd
-from statsmodels.tsa.stattools import pacf
 
 
 def get_ts_groups(df: pd.DataFrame, tss) -> list:
     group_combinations = ['__default']
     if tss.group_by:
         groups = [tuple([g]) if not isinstance(g, tuple) else g
                   for g in list(df.groupby(by=tss.group_by).groups.keys())]
         group_combinations.extend(groups)
     return group_combinations
 
 
-def get_group_matches(
-        data: Union[pd.Series, pd.DataFrame],
-        combination: tuple,
-        group_columns: List[str],
-        copy: bool = False
-) -> Tuple[list, pd.DataFrame]:
-    """Given a particular group combination, return the data subset that belongs to it."""
-
-    if type(data) == pd.Series:
-        data = pd.DataFrame(data)
-    elif type(data) != pd.DataFrame:
-        raise Exception(f"Wrong data type {type(data)}, must be pandas.DataFrame or pd.Series")
-
-    if combination == '__default':
-        return list(data.index), data
-    else:
-        subset = data
-        for val, col in zip(combination, group_columns):
-            subset = subset[subset[col] == val]
-        if len(subset) > 0:
-            if copy:
-                subset = subset.copy()
-            return list(subset.index), subset
-        else:
-            return [], pd.DataFrame()
-
-
-def get_delta(
-        df: pd.DataFrame,
-        dtype_dict: dict,
-        group_combinations: list,
-        target: str,
-        tss
-) -> Tuple[Dict, Dict, Dict]:
+def get_delta(df: pd.DataFrame, tss) -> Tuple[Dict, Dict, Dict]:
     """
     Infer the sampling interval of each time series, by picking the most popular time interval observed in the training data.
 
     :param df: Dataframe with time series data.
-    :param group_combinations: all tuples with distinct values for `TimeseriesSettings.group_by` columns, defining all available time series.
-    :param target: name of target column
     :param tss: timeseries settings
 
     :return:
     Dictionary with group combination tuples as keys. Values are dictionaries with the inferred delta for each series.
     """  # noqa
-    df = df.copy()
+    df = df.copy()  # TODO: necessary?
     original_col = f'__mdb_original_{tss.order_by}'
     order_col = original_col if original_col in df.columns else tss.order_by
-    deltas = {"__default": df[order_col].astype(float).rolling(window=2).apply(np.diff).value_counts().index[0]}
+    deltas = {"__default": df[order_col].astype(float).diff().value_counts().index[0]}
     freq, period = detect_freq_period(deltas["__default"], tss, len(df))
     periods = {"__default": [period]}
     freqs = {"__default": freq}
 
     if tss.group_by:
-        for group in group_combinations:
-            if group != "__default":
-                _, subset = get_group_matches(df, group, tss.group_by)
-                if subset.shape[0] > 1:
-                    deltas[group] = subset[order_col].rolling(window=2).apply(np.diff).value_counts().index[0]
-                    freq, period = detect_freq_period(deltas[group], tss, len(subset))
-                    freqs[group] = freq
-                    if period:
-                        periods[group] = [period]
-                    else:
-                        periods[group] = [max_pacf(df, group_combinations, target, tss)[group][0]]
-                else:
-                    deltas[group] = 1.0
-                    periods[group] = [1]
-                    freqs[group] = 'S'
+        grouped = df.groupby(by=tss.group_by)
+        for group, subset in grouped:
+            if subset.shape[0] > 1:
+                deltas[group] = subset[order_col].diff().value_counts().index[0]
+                freq, period = detect_freq_period(deltas[group], tss, len(subset))
+                freqs[group] = freq
+                periods[group] = [period] if period is not None else [1]
+            else:
+                deltas[group] = 1.0
+                periods[group] = [1]
+                freqs[group] = 'S'
 
     return deltas, periods, freqs
 
 
 def get_inferred_timestamps(df: pd.DataFrame, col: str, deltas: dict, tss, stat_analysis,
                             time_format='') -> pd.DataFrame:
     horizon = tss.horizon
@@ -245,15 +205,15 @@
     freq, min_diff = sorted(diffs, key=lambda x: x[1])[0]
     multiplier = 1
     if secs_to_interval[freq]:
         multiplier += int(min_diff / secs_to_interval[freq])
     return freq_to_pandas(freq, multiplier=multiplier), freq_to_period.get(freq, 1)
 
 
-def freq_to_pandas(freq, multiplier=1, sample_row=None):
+def freq_to_pandas(freq, multiplier=1):
     mapping = {
         'constant': 'N',
         'nanosecond': 'N',
         'microsecond': 'us',
         'millisecond': 'ms',
         'second': 'S',
         'minute': 'T',
@@ -270,48 +230,25 @@
     #  pandas.pydata.org/docs/user_guide/timeseries.html
     items = [mapping[freq]]
     if multiplier > 1:
         items.insert(0, str(multiplier))
     return ''.join(items)
 
 
-def max_pacf(data: pd.DataFrame, group_combinations, target, tss):
-    def min_k(top_k, data):
-        return min(top_k, len(data))
-
-    top_k = 5
-    k = min_k(top_k, data[target])
-    candidate_sps = {'__default': (1 + np.argpartition(pacf(data[target].values)[1:], -k))[-k:].tolist()[::-1]}
-    if tss.group_by:
-        for group in group_combinations:
-            if group != "__default":
-                _, subset = get_group_matches(data, group, tss.group_by)
-                try:
-                    k = min_k(top_k, subset[target])
-                    candidates = (1 + np.argpartition(pacf(subset[target].values)[1:], -k))[-k:].tolist()[::-1]
-                    candidate_sps[group] = candidates
-                except Exception:
-                    candidate_sps[group] = None
-            if not candidate_sps[group]:
-                candidate_sps[group] = [1]
-
-    return candidate_sps
-
-
 def filter_ts(df: pd.DataFrame, tss, n_rows=1):
     """
     This method triggers only for timeseries datasets.
 
     It returns a dataframe that filters out all but the first ``n_rows`` per group.
     """  # noqa
     if tss.is_timeseries:
         gby = tss.group_by
         if gby is None:
             df = df.iloc[[0]]
         else:
             ndf = pd.DataFrame(columns=df.columns)
-            for group in get_ts_groups(df, tss):
+            grouped = df.groupby(by=tss.group_by)
+            for group, subdf in grouped:
                 if group != '__default':
-                    _, subdf = get_group_matches(df, group, tss.group_by)
                     ndf = pd.concat([ndf, subdf.iloc[:n_rows]])
             df = ndf
     return df
```

### Comparing `lightwood-23.6.2.0/lightwood/mixer/__init__.py` & `lightwood-23.6.4.0/lightwood/mixer/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/mixer/arima.py` & `lightwood-23.6.4.0/lightwood/mixer/arima.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/mixer/base.py` & `lightwood-23.6.4.0/lightwood/mixer/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/mixer/ets.py` & `lightwood-23.6.4.0/lightwood/mixer/ets.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/mixer/gluonts.py` & `lightwood-23.6.4.0/lightwood/mixer/gluonts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import importlib
 from copy import deepcopy
-from typing import Dict, Union, Optional
+from typing import Dict, Union, Optional, List
 
 import numpy as np
 import pandas as pd
 import mxnet as mx
 from sklearn.preprocessing import OrdinalEncoder
 
 from gluonts.dataset.pandas import PandasDataset
 
 from gluonts.mx import DeepAREstimator, Trainer  # @TODO: support for other estimators
 from gluonts.mx.trainer.callback import TrainingHistory
 from gluonts.mx.distribution.student_t import StudentTOutput
 
 from lightwood.helpers.log import log
-from lightwood.helpers.ts import get_group_matches
 from lightwood.mixer.base import BaseMixer
 from lightwood.api.types import PredictionArguments
 from lightwood.data.encoded_ds import EncodedDs, ConcatedEncodedDs
 
 
 class GluonTSMixer(BaseMixer):
     horizon: int
@@ -33,16 +32,16 @@
             window: int,
             dtype_dict: Dict,
             ts_analysis: Dict,
             n_epochs: int = 10,
             early_stop_patience: int = 3,
             distribution_output: str = '',
             seed: int = 0,
-            static_features_cat: Optional[list[str]] = None,
-            static_features_real: Optional[list[str]] = None,
+            static_features_cat: Optional[List[str]] = None,
+            static_features_real: Optional[List[str]] = None,
     ):
         """
         Wrapper around GluonTS probabilistic deep learning models. For now, only DeepAR is supported.
 
         Due to inference speed, predictions are only generated for the last data point (as opposed to other mixers).  
 
         :param stop_after: time budget in seconds.
@@ -165,16 +164,16 @@
         gby = self.ts_analysis["tss"].group_by if self.ts_analysis["tss"].group_by else []
         groups = ds.data_frame[gby[0]].unique().tolist() if gby else None
 
         df = ds.data_frame
         ydf['__original_index'] = df['__mdb_original_index'].values
         input_ds = self._make_initial_ds(df, groups=groups)  # TODO test with novel group
         forecasts = list(self.model.predict(input_ds))
-        for group, group_forecast in zip(groups, forecasts):
-            _, subdf = get_group_matches(df, (group, ), gby)
+        grouped = df.groupby(by=gby) if gby else df.groupby(lambda x: '__default')
+        for (group, subdf), group_forecast in zip(grouped, forecasts):
             idx = ydf[ydf['__original_index'] == max(subdf['__mdb_original_index'])].index.values[0]
             ydf.at[idx, 'prediction'] = [entry for entry in group_forecast.quantile(0.5)]
             ydf.at[idx, 'lower'] = [entry for entry in group_forecast.quantile(1 - conf)]
             ydf.at[idx, 'upper'] = [entry for entry in group_forecast.quantile(conf)]
 
         return ydf
```

### Comparing `lightwood-23.6.2.0/lightwood/mixer/helpers/ar_net.py` & `lightwood-23.6.4.0/lightwood/mixer/helpers/ar_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/mixer/helpers/default_net.py` & `lightwood-23.6.4.0/lightwood/mixer/helpers/default_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/mixer/helpers/qclassic_net.py` & `lightwood-23.6.4.0/lightwood/mixer/helpers/qclassic_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/mixer/helpers/ranger.py` & `lightwood-23.6.4.0/lightwood/mixer/helpers/ranger.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/mixer/helpers/residual_net.py` & `lightwood-23.6.4.0/lightwood/mixer/helpers/residual_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py` & `lightwood-23.6.4.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/mixer/lightgbm.py` & `lightwood-23.6.4.0/lightwood/mixer/lightgbm.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/mixer/lightgbm_array.py` & `lightwood-23.6.4.0/lightwood/mixer/lightgbm_array.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from copy import deepcopy
 from typing import Dict, List, Union, Optional
 
 import numpy as np
 import pandas as pd
 
 from lightwood.helpers.log import log
-from lightwood.mixer.helpers.ts import _apply_stl_on_training, _stl_transform, _stl_inverse_transform
 from lightwood.encoder.base import BaseEncoder
 from lightwood.mixer.base import BaseMixer
 from lightwood.mixer.lightgbm import LightGBM
 from lightwood.api.types import PredictionArguments, TimeseriesSettings
 from lightwood.data.encoded_ds import EncodedDs, ConcatedEncodedDs
 
 
@@ -57,17 +56,14 @@
         self.use_stl = False
         self.stable = True
 
     def _fit(self, train_data: EncodedDs, dev_data: EncodedDs, submodel_method='fit') -> None:
         original_train = deepcopy(train_data.data_frame)
         original_dev = deepcopy(dev_data.data_frame)
 
-        if self.use_stl and self.ts_analysis.get('stl_transforms', False):
-            _apply_stl_on_training(train_data, dev_data, self.target, self.tss, self.ts_analysis)
-
         for timestep in range(self.horizon):
             getattr(self.models[timestep], submodel_method)(train_data, dev_data)
 
         # restore dfs
         train_data.data_frame = original_train
         dev_data.data_frame = original_dev
 
@@ -86,22 +82,16 @@
 
         original_df = deepcopy(ds.data_frame)
         length = sum(ds.encoded_ds_lengths) if isinstance(ds, ConcatedEncodedDs) else len(ds)
         ydf = pd.DataFrame(0,  # zero-filled
                            index=np.arange(length),
                            columns=[f'prediction_{i}' for i in range(self.horizon)])
 
-        if self.use_stl and self.ts_analysis.get('stl_transforms', False):
-            ds.data_frame = _stl_transform(ydf, ds, self.target, self.tss, self.ts_analysis)
-
         for timestep in range(self.horizon):
             ydf[f'prediction_{timestep}'] = self.models[timestep](ds, args)['prediction'].values
 
-        if self.use_stl and self.ts_analysis.get('stl_transforms', False):
-            ydf = _stl_inverse_transform(ydf, ds, self.tss, self.ts_analysis)
-
         if self.models[0].positive_domain:
             ydf = ydf.clip(0)
 
         ydf['prediction'] = ydf.values.tolist()
         ds.data_frame = original_df
         return ydf[['prediction']]
```

### Comparing `lightwood-23.6.2.0/lightwood/mixer/neural.py` & `lightwood-23.6.4.0/lightwood/mixer/neural.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/mixer/neural_ts.py` & `lightwood-23.6.4.0/lightwood/mixer/neural_ts.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from type_infer.dtype import dtype
 from lightwood.api.types import PredictionArguments
 from lightwood.encoder.base import BaseEncoder
 from lightwood.data.encoded_ds import EncodedDs, ConcatedEncodedDs
 from lightwood.mixer.neural import Neural
 from lightwood.mixer.helpers.ar_net import ArNet
 from lightwood.mixer.helpers.default_net import DefaultNet
-from lightwood.mixer.helpers.ts import _apply_stl_on_training, _stl_transform, _stl_inverse_transform
 from lightwood.api.types import TimeseriesSettings
 
 
 class NeuralTs(Neural):
     def __init__(
             self,
             stop_after: float,
@@ -79,18 +78,14 @@
         :param train_data: The network is fit/trained on this
         :param dev_data: Data used for early stopping and hyperparameter determination
         """  # noqa
         self.started = time.time()
         original_train = deepcopy(train_data.data_frame)
         original_dev = deepcopy(dev_data.data_frame)
 
-        # Use STL blocks if available
-        if self.use_stl and self.ts_analysis.get('stl_transforms', False):
-            _apply_stl_on_training(train_data, dev_data, self.target, self.timeseries_settings, self.ts_analysis)
-
         # ConcatedEncodedDs
         self.batch_size = min(200, int(len(train_data) / 10))
         self.batch_size = max(40, self.batch_size)
 
         dev_dl = DataLoader(dev_data, batch_size=self.batch_size, shuffle=False)
         train_dl = DataLoader(train_data, batch_size=self.batch_size, shuffle=False)
 
@@ -137,17 +132,14 @@
         length = sum(ds.encoded_ds_lengths) if isinstance(ds, ConcatedEncodedDs) else len(ds)
         pred_cols = [f'prediction_{i}' for i in range(self.timeseries_settings.horizon)]
         ydf = pd.DataFrame(0,  # zero-filled
                            index=np.arange(length),
                            dtype=object,
                            columns=pred_cols)
 
-        if self.use_stl and self.ts_analysis.get('stl_transforms', False):
-            ds.data_frame = _stl_transform(ydf, ds, self.target, self.timeseries_settings, self.ts_analysis)
-
         with torch.no_grad():
             for idx, (X, Y) in enumerate(ds):
                 X = X.to(self.model.device)
                 Yh = self.model(X)
                 Yh = torch.unsqueeze(Yh, 0) if len(Yh.shape) < 2 else Yh
 
                 kwargs = {}
@@ -163,17 +155,14 @@
                 decoded_predictions.extend(decoded_prediction)
 
         decoded_predictions = np.array(decoded_predictions)
         if len(decoded_predictions.shape) == 1:
             decoded_predictions = np.expand_dims(decoded_predictions, axis=1)
         ydf[pred_cols] = decoded_predictions
 
-        if self.use_stl and self.ts_analysis.get('stl_transforms', False):
-            ydf = _stl_inverse_transform(ydf, ds, self.timeseries_settings, self.ts_analysis)
-
         ydf['prediction'] = ydf.values.tolist()
 
         if self.timeseries_settings.horizon == 1:
             ydf['prediction'] = [p[0] for p in ydf['prediction']]
 
         if args.predict_proba and self.supports_proba:
             raw_predictions = np.array(all_probs).squeeze(axis=1)
```

### Comparing `lightwood-23.6.2.0/lightwood/mixer/nhits.py` & `lightwood-23.6.4.0/lightwood/mixer/nhits.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/mixer/prophet.py` & `lightwood-23.6.4.0/lightwood/mixer/prophet.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/mixer/qclassic.py` & `lightwood-23.6.4.0/lightwood/mixer/qclassic.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/mixer/random_forest.py` & `lightwood-23.6.4.0/lightwood/mixer/random_forest.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/mixer/regression.py` & `lightwood-23.6.4.0/lightwood/mixer/regression.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/mixer/sktime.py` & `lightwood-23.6.4.0/lightwood/mixer/sktime.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import inspect
 import importlib
 from copy import deepcopy
 from datetime import datetime
-from itertools import product
 from typing import Dict, Union, Optional
 
 import optuna
 import numpy as np
 import pandas as pd
 from sktime.forecasting.compose import TransformedTargetForecaster
 from sktime.forecasting.base import ForecastingHorizon, BaseForecaster
 from sktime.performance_metrics.forecasting import MeanAbsolutePercentageError
 from sktime.forecasting.statsforecast import StatsForecastAutoARIMA as AutoARIMA
 
 from lightwood.helpers.log import log
 from lightwood.mixer.base import BaseMixer
 from lightwood.api.types import PredictionArguments
-from lightwood.helpers.ts import get_group_matches
 from lightwood.data.encoded_ds import EncodedDs, ConcatedEncodedDs
 
 
 class SkTime(BaseMixer):
     forecaster: str
     horizon: int
     target: str
@@ -130,14 +128,15 @@
             self._fit(data)
 
     def _fit(self, data):
         """
         Internal method that fits forecasters to a given dataframe.
         """
         df = data.data_frame.sort_values(by=f'__mdb_original_{self.ts_analysis["tss"].order_by}')
+        gby = self.ts_analysis['tss'].group_by
 
         if not self.hyperparam_search and not self.study:
             module_name = self.model_path
         else:
             finished_study = sum([int(trial.state.is_finished()) for trial in self.study.trials]) == self.n_trials
             if finished_study:
                 log.info(f'Selected best model: {self.study.best_params["class"]}')
@@ -147,20 +146,21 @@
 
         sktime_module = importlib.import_module('.'.join(['sktime', 'forecasting', module_name.split(".")[0]]))
         try:
             model_class = getattr(sktime_module, module_name.split(".")[1])
         except AttributeError:
             model_class = AutoARIMA  # use AutoARIMA when the provided class does not exist
 
-        for group in self.ts_analysis['group_combinations']:
+        grouped = df.groupby(by=gby) if gby else df.groupby(lambda x: '__default')
+        for group, series_data in grouped:
             kwargs = {}
-            sp = self.sp if self.sp else self.ts_analysis['periods'].get(group, '__default')[0]
+            sp = self.sp if self.sp else self.ts_analysis['periods'].get(group, [1])[0]
 
             options = self.model_kwargs
-            options['sp'] = sp                   # seasonality period
+            options['sp'] = sp               # seasonality period
             options['suppress_warnings'] = True  # ignore warnings if possible
             options['error_action'] = 'raise'    # avoids fit() failing silently
 
             if self.model_path == 'fbprophet.Prophet':
                 options['freq'] = self.freq
 
             for k, v in options.items():
@@ -177,22 +177,19 @@
 
             model_pipeline.append(("forecaster", model_class(**kwargs)))
 
             self.models[group] = TransformedTargetForecaster(model_pipeline)
 
             oby_col = self.ts_analysis['tss'].order_by
             if self.grouped_by == ['__default']:
-                series_data = df
                 series_oby = df[oby_col]
-                self.cutoffs[group] = series_oby.index[-1]  # defines the 'present' time for each partition
             else:
-                series_idxs, series_data = get_group_matches(df, group, self.grouped_by)
                 series_oby = series_data[oby_col]
-                self.cutoffs[group] = series_idxs[-1]  # defines the 'present' time for each partition
 
+            self.cutoffs[group] = series_oby.index[-1]  # defines the 'present' time for each partition
             series = series_data[self.target]
             if series_data.size > self.ts_analysis['tss'].window:
                 series = series.sort_index(ascending=True)
                 series = series.reset_index(drop=True)
                 series = series.loc[~pd.isnull(series.values)]  # remove NaN  # @TODO: benchmark imputation vs this?
 
                 if self.model_path == 'fbprophet.Prophet':
@@ -203,15 +200,15 @@
                             # out of bounds with true freq in __default group is fine, we skip it
                             continue
 
                 series = series.astype(float)
 
                 # if data is huge, filter out old records for quicker fitting
                 if self.auto_size:
-                    cutoff = min(len(series), max(500, options['sp'] * self.cutoff_factor))
+                    cutoff = min(len(series), max(500, options.get('sp', 1) * self.cutoff_factor))
                     series = series.iloc[-cutoff:]
                 try:
                     self.models[group].fit(series, fh=self.fh)
                 except Exception:
                     self.models[group] = model_class()  # with default options (i.e. no seasonality, among others)
                     self.models[group].fit(series, fh=self.fh)
 
@@ -241,42 +238,33 @@
         """  # noqa
         if args.predict_proba:
             log.warning('This mixer does not output probability estimates')
 
         df = deepcopy(ds.data_frame)
         df = df.rename_axis('__sktime_index').reset_index()
 
-        length = sum(ds.encoded_ds_lengths) if isinstance(ds, ConcatedEncodedDs) else len(ds)
+        gby = self.ts_analysis['tss'].group_by
         ydf = pd.DataFrame(0,  # zero-filled
                            index=df.index,
                            columns=['prediction'],
                            dtype=object)
 
-        group_values = {gcol: df[gcol].tolist() for gcol in self.grouped_by} \
-            if self.ts_analysis['tss'].group_by \
-            else {'': ['__default' for _ in range(length)]}
-
         pending_idxs = set(df.index)
-        all_group_combinations = list(product(*[set(x) for x in group_values.values()]))
-        for group in all_group_combinations:
-            group = tuple(group)
-            group = '__default' if group[0] == '__default' else group
-            series_idxs, series_data = get_group_matches(df, group, self.grouped_by)
-
+        grouped = df.groupby(by=gby) if gby else df.groupby(lambda x: '__default')
+        for group, series_data in grouped:
             if series_data.size > 0:
                 start_ts = series_data['__sktime_index'].iloc[0]
                 series = series_data[self.target]
-                series_idxs = sorted(series_idxs)
+                series_idxs = series.index
                 if self.models.get(group, False) and self.models[group].is_fitted:
                     freq = self.ts_analysis['deltas'][group]
                     delta = (start_ts - self.cutoffs[group]).total_seconds()
                     offset = round(delta / freq)
                     forecaster = self.models[group]
                     ydf = self._call_groupmodel(ydf, forecaster, series, offset=offset)
-                    # log.debug(f'[SkTime] Forecasting for group {group}, start at {start_ts} (offset by {offset} for cutoff at {self.cutoffs[group]} (relative {self.models[group].cutoff}))')  # noqa
                 else:
                     log.warning(f"Applying naive forecaster for novel group {group}. Performance might not be optimal.")
                     ydf = self._call_default(ydf, series.values, series_idxs)
                 pending_idxs -= set(series_idxs)
 
         # apply default model in all remaining novel-group rows
         if len(pending_idxs) > 0:
```

### Comparing `lightwood-23.6.2.0/lightwood/mixer/tabtransformer.py` & `lightwood-23.6.4.0/lightwood/mixer/tabtransformer.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/mixer/unit.py` & `lightwood-23.6.4.0/lightwood/mixer/unit.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood/mixer/xgboost.py` & `lightwood-23.6.4.0/lightwood/mixer/xgboost.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood.egg-info/PKG-INFO` & `lightwood-23.6.4.0/lightwood.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightwood
-Version: 23.6.2.0
+Version: 23.6.4.0
 Summary: Lightwood is a toolkit for automatic machine learning model building
 Home-page: https://github.com/mindsdb/lightwood
 Author: MindsDB Inc
 Author-email: community@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/lightwood
 Description: # Lightwood
@@ -216,15 +216,15 @@
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: extra
 Provides-Extra: extra_ts
-Provides-Extra: xai
+Provides-Extra: dev
 Provides-Extra: quantum
+Provides-Extra: xai
 Provides-Extra: image
 Provides-Extra: audio
-Provides-Extra: dev
-Provides-Extra: extra
 Provides-Extra: all_extras
```

### Comparing `lightwood-23.6.2.0/lightwood.egg-info/SOURCES.txt` & `lightwood-23.6.4.0/lightwood.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightwood-23.6.2.0/lightwood.egg-info/requires.txt` & `lightwood-23.6.4.0/lightwood.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-type_infer>=0.0.10
-dataprep_ml>=0.0.9
+type_infer>=0.0.13
+dataprep_ml>=0.0.13
 mindsdb-evaluator>=0.0.9
 numpy
 nltk<3.6,>=3
 python-dateutil>=2.8.1
 pandas<1.5.0,>=1.1.5
 schema>=0.6.8
 torch<2.1,>=2.0.0
@@ -16,42 +16,42 @@
 wheel>=0.32.2
 scikit-learn<=1.0.2,>=1.0.0
 dataclasses_json>=0.5.4
 dill==0.3.6
 sktime<0.15.0,>=0.14.0
 statsforecast==1.4.0
 torch_optimizer==0.1.0
-black>=21.9b0
+black==23.3.0
 typing_extensions
 colorlog==6.5.0
 statsmodels>=0.12.0
 langid==1.1.6
 pydateinfer==0.3.0
 protobuf<3.21.0
 xgboost<=1.8.0,>=1.6.0
 tab-transformer-pytorch>=0.2.1
 typing-inspect
 six
 regex
 
 [all_extras]
-pyod==1.0.4
-gluonts<0.12.0,>=0.11.0
-autopep8>=1.5.7
-shap>=0.40.0
-neuralforecast==1.5.0
-qiskit==0.31.0
-prophet==1.1
-lightgbm<=3.3.3,>=3.3.0
 torchvision
 suod
-pystan==2.19.1.1
-pillow>8.3.1
+lightgbm<=3.3.3,>=3.3.0
+neuralforecast==1.5.0
+prophet==1.1
+qiskit==0.31.0
 librosa==0.8.1
 mxnet<2.0.0,>=1.6.0
+pystan==2.19.1.1
+autopep8>=1.5.7
+pyod==1.0.4
+shap>=0.40.0
+gluonts<0.12.0,>=0.11.0
+pillow>8.3.1
 
 [audio]
 librosa==0.8.1
 
 [dev]
 autopep8>=1.5.7
```

### Comparing `lightwood-23.6.2.0/requirements.txt` & `lightwood-23.6.4.0/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-type_infer >=0.0.10
-dataprep_ml >=0.0.9
+type_infer >=0.0.13
+dataprep_ml >=0.0.13
 mindsdb-evaluator >=0.0.9
 numpy
 nltk >=3,<3.6
 python-dateutil >=2.8.1
 pandas >=1.1.5, <1.5.0
 schema >=0.6.8
 torch >=2.0.0, <2.1
@@ -16,15 +16,15 @@
 wheel >=0.32.2
 scikit-learn >=1.0.0, <=1.0.2
 dataclasses_json >=0.5.4
 dill ==0.3.6
 sktime >=0.14.0,<0.15.0
 statsforecast ==1.4.0
 torch_optimizer ==0.1.0
-black >=21.9b0
+black ==23.3.0
 typing_extensions
 colorlog ==6.5.0
 statsmodels >=0.12.0
 langid==1.1.6
 pydateinfer==0.3.0
 protobuf<3.21.0
 xgboost>=1.6.0, <=1.8.0
```

### Comparing `lightwood-23.6.2.0/setup.py` & `lightwood-23.6.4.0/setup.py`

 * *Files identical despite different names*

