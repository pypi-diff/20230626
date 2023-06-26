# Comparing `tmp/normflows-1.7.0.tar.gz` & `tmp/normflows-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/normflows-1.7.0.tar", last modified: Mon Jun 12 11:55:44 2023, max compression
+gzip compressed data, was "dist/normflows-1.7.1.tar", last modified: Mon Jun 26 13:01:32 2023, max compression
```

## Comparing `normflows-1.7.0.tar` & `normflows-1.7.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1072 2021-11-22 13:57:32.000000 normflows-1.7.0/LICENSE
--rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)       42 2021-11-22 13:57:32.000000 normflows-1.7.0/MANIFEST.in
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    15779 2023-06-12 11:55:44.000000 normflows-1.7.0/PKG-INFO
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    15190 2023-06-12 11:53:08.000000 normflows-1.7.0/README.md
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      253 2023-06-12 11:52:41.000000 normflows-1.7.0/normflows/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    16860 2023-06-06 13:57:44.000000 normflows-1.7.0/normflows/core.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     7805 2023-06-06 13:57:44.000000 normflows-1.7.0/normflows/core_test.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows/distributions/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      699 2023-05-31 15:25:11.000000 normflows-1.7.0/normflows/distributions/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    22844 2023-05-30 15:55:17.000000 normflows-1.7.0/normflows/distributions/base.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4884 2023-05-30 15:55:17.000000 normflows-1.7.0/normflows/distributions/base_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2699 2023-01-20 17:41:25.000000 normflows-1.7.0/normflows/distributions/decoder.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1589 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/distributions/decoder_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1756 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/distributions/distribution_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     5745 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/distributions/encoder.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     3493 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/distributions/encoder_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      663 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/distributions/linear_interpolation.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2176 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/distributions/mh_proposal.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     9434 2023-01-23 18:21:11.000000 normflows-1.7.0/normflows/distributions/prior.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1651 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/distributions/prior_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     5694 2023-05-31 15:25:11.000000 normflows-1.7.0/normflows/distributions/target.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1334 2023-05-31 15:25:11.000000 normflows-1.7.0/normflows/distributions/target_test.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows/flows/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      913 2022-07-26 14:04:52.000000 normflows-1.7.0/normflows/flows/__init__.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows/flows/affine/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      218 2022-07-26 14:04:52.000000 normflows-1.7.0/normflows/flows/affine/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4158 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/flows/affine/autoregressive.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      974 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/affine/autoregressive_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     9923 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/flows/affine/coupling.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1662 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/flows/affine/coupling_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     3330 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/affine/glow.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1264 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/affine/glow_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1924 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/base.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1267 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/flows/base_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1325 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/flow_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    18397 2023-01-20 17:41:25.000000 normflows-1.7.0/normflows/flows/mixing.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1360 2023-01-20 17:41:25.000000 normflows-1.7.0/normflows/flows/mixing_test.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows/flows/neural_spline/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      252 2022-07-26 14:04:52.000000 normflows-1.7.0/normflows/flows/neural_spline/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4849 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/neural_spline/autoregressive.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      778 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/neural_spline/autoregressive_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    13084 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/neural_spline/coupling.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1961 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/neural_spline/coupling_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    10166 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/neural_spline/wrapper.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1861 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/neural_spline/wrapper_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2303 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/flows/normalization.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2047 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/flows/periodic.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1332 2023-01-20 17:41:25.000000 normflows-1.7.0/normflows/flows/periodic_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2878 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/planar.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      722 2023-01-20 17:41:25.000000 normflows-1.7.0/normflows/flows/planar_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1491 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/flows/radial.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      506 2023-01-20 17:41:25.000000 normflows-1.7.0/normflows/flows/radial_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4047 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/flows/reshape.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    14772 2023-01-20 17:37:19.000000 normflows-1.7.0/normflows/flows/residual.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2739 2023-01-23 14:38:51.000000 normflows-1.7.0/normflows/flows/residual_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4278 2023-01-20 17:41:25.000000 normflows-1.7.0/normflows/flows/stochastic.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1321 2023-01-20 17:41:25.000000 normflows-1.7.0/normflows/flows/stochastic_test.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows/nets/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      212 2022-07-26 14:04:52.000000 normflows-1.7.0/normflows/nets/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2028 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/nets/cnn.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    25793 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/nets/lipschitz.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     9712 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/nets/made.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4741 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/nets/made_test.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2284 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/nets/mlp.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     6999 2022-07-26 14:04:52.000000 normflows-1.7.0/normflows/nets/resnet.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows/sampling/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)       23 2022-07-26 14:04:52.000000 normflows-1.7.0/normflows/sampling/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1999 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/sampling/hais.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1982 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/transforms.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      656 2023-01-22 11:55:37.000000 normflows-1.7.0/normflows/transforms_test.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows/utils/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      262 2022-07-26 14:04:52.000000 normflows-1.7.0/normflows/utils/__init__.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2046 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/utils/eval.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1660 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/utils/masks.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     5660 2022-12-21 10:20:49.000000 normflows-1.7.0/normflows/utils/nn.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      852 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/utils/optim.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1168 2022-11-09 20:18:25.000000 normflows-1.7.0/normflows/utils/preprocessing.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     7744 2022-07-26 14:04:52.000000 normflows-1.7.0/normflows/utils/splines.py
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2318 2023-01-20 17:41:25.000000 normflows-1.7.0/normflows/utils/splines_test.py
-drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows.egg-info/
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    15779 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows.egg-info/PKG-INFO
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2436 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows.egg-info/SOURCES.txt
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)        1 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows.egg-info/dependency_links.txt
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)       63 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows.egg-info/requires.txt
--rw-rw-r--   0 vstimper  (1000) vstimper  (1000)       10 2023-06-12 11:55:44.000000 normflows-1.7.0/normflows.egg-info/top_level.txt
--rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)       11 2022-07-26 12:32:34.000000 normflows-1.7.0/requirements.txt
--rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)      108 2023-06-12 11:55:44.000000 normflows-1.7.0/setup.cfg
--rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)     1368 2023-06-12 11:52:17.000000 normflows-1.7.0/setup.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-26 13:01:32.000000 normflows-1.7.1/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1072 2021-11-22 13:57:32.000000 normflows-1.7.1/LICENSE
+-rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)       42 2021-11-22 13:57:32.000000 normflows-1.7.1/MANIFEST.in
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    15920 2023-06-26 13:01:32.000000 normflows-1.7.1/PKG-INFO
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    15331 2023-06-26 12:57:08.000000 normflows-1.7.1/README.md
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-26 13:01:32.000000 normflows-1.7.1/normflows/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      253 2023-06-26 12:41:09.000000 normflows-1.7.1/normflows/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    16860 2023-06-06 13:57:44.000000 normflows-1.7.1/normflows/core.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     7805 2023-06-06 13:57:44.000000 normflows-1.7.1/normflows/core_test.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-26 13:01:32.000000 normflows-1.7.1/normflows/distributions/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      699 2023-05-31 15:25:11.000000 normflows-1.7.1/normflows/distributions/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    22844 2023-05-30 15:55:17.000000 normflows-1.7.1/normflows/distributions/base.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4884 2023-05-30 15:55:17.000000 normflows-1.7.1/normflows/distributions/base_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2699 2023-01-20 17:41:25.000000 normflows-1.7.1/normflows/distributions/decoder.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1589 2023-01-22 11:55:37.000000 normflows-1.7.1/normflows/distributions/decoder_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1756 2023-01-22 11:55:37.000000 normflows-1.7.1/normflows/distributions/distribution_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     5745 2023-01-22 11:55:37.000000 normflows-1.7.1/normflows/distributions/encoder.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     3493 2023-01-22 11:55:37.000000 normflows-1.7.1/normflows/distributions/encoder_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      663 2022-11-09 20:18:25.000000 normflows-1.7.1/normflows/distributions/linear_interpolation.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2176 2022-11-09 20:18:25.000000 normflows-1.7.1/normflows/distributions/mh_proposal.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     9434 2023-01-23 18:21:11.000000 normflows-1.7.1/normflows/distributions/prior.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1651 2023-01-22 11:55:37.000000 normflows-1.7.1/normflows/distributions/prior_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     5694 2023-05-31 15:25:11.000000 normflows-1.7.1/normflows/distributions/target.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1334 2023-05-31 15:25:11.000000 normflows-1.7.1/normflows/distributions/target_test.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-26 13:01:32.000000 normflows-1.7.1/normflows/flows/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      913 2022-07-26 14:04:52.000000 normflows-1.7.1/normflows/flows/__init__.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-26 13:01:32.000000 normflows-1.7.1/normflows/flows/affine/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      218 2022-07-26 14:04:52.000000 normflows-1.7.1/normflows/flows/affine/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4158 2022-11-09 20:18:25.000000 normflows-1.7.1/normflows/flows/affine/autoregressive.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      974 2022-12-21 10:20:49.000000 normflows-1.7.1/normflows/flows/affine/autoregressive_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     9923 2023-01-22 11:55:37.000000 normflows-1.7.1/normflows/flows/affine/coupling.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1662 2023-01-22 11:55:37.000000 normflows-1.7.1/normflows/flows/affine/coupling_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     3330 2022-12-21 10:20:49.000000 normflows-1.7.1/normflows/flows/affine/glow.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1264 2022-12-21 10:20:49.000000 normflows-1.7.1/normflows/flows/affine/glow_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1924 2022-12-21 10:20:49.000000 normflows-1.7.1/normflows/flows/base.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1267 2023-01-22 11:55:37.000000 normflows-1.7.1/normflows/flows/base_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1325 2022-12-21 10:20:49.000000 normflows-1.7.1/normflows/flows/flow_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    18397 2023-01-20 17:41:25.000000 normflows-1.7.1/normflows/flows/mixing.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1360 2023-01-20 17:41:25.000000 normflows-1.7.1/normflows/flows/mixing_test.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-26 13:01:32.000000 normflows-1.7.1/normflows/flows/neural_spline/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      252 2022-07-26 14:04:52.000000 normflows-1.7.1/normflows/flows/neural_spline/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4849 2022-12-21 10:20:49.000000 normflows-1.7.1/normflows/flows/neural_spline/autoregressive.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      778 2022-12-21 10:20:49.000000 normflows-1.7.1/normflows/flows/neural_spline/autoregressive_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    13084 2022-12-21 10:20:49.000000 normflows-1.7.1/normflows/flows/neural_spline/coupling.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1961 2022-12-21 10:20:49.000000 normflows-1.7.1/normflows/flows/neural_spline/coupling_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    10166 2022-12-21 10:20:49.000000 normflows-1.7.1/normflows/flows/neural_spline/wrapper.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1861 2022-12-21 10:20:49.000000 normflows-1.7.1/normflows/flows/neural_spline/wrapper_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2303 2022-11-09 20:18:25.000000 normflows-1.7.1/normflows/flows/normalization.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2047 2022-11-09 20:18:25.000000 normflows-1.7.1/normflows/flows/periodic.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1332 2023-01-20 17:41:25.000000 normflows-1.7.1/normflows/flows/periodic_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2878 2022-12-21 10:20:49.000000 normflows-1.7.1/normflows/flows/planar.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      722 2023-01-20 17:41:25.000000 normflows-1.7.1/normflows/flows/planar_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1491 2022-12-21 10:20:49.000000 normflows-1.7.1/normflows/flows/radial.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      506 2023-01-20 17:41:25.000000 normflows-1.7.1/normflows/flows/radial_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4047 2022-11-09 20:18:25.000000 normflows-1.7.1/normflows/flows/reshape.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    14772 2023-01-20 17:37:19.000000 normflows-1.7.1/normflows/flows/residual.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2739 2023-01-23 14:38:51.000000 normflows-1.7.1/normflows/flows/residual_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4278 2023-01-20 17:41:25.000000 normflows-1.7.1/normflows/flows/stochastic.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1321 2023-01-20 17:41:25.000000 normflows-1.7.1/normflows/flows/stochastic_test.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-26 13:01:32.000000 normflows-1.7.1/normflows/nets/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      212 2022-07-26 14:04:52.000000 normflows-1.7.1/normflows/nets/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2028 2022-12-21 10:20:49.000000 normflows-1.7.1/normflows/nets/cnn.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    25793 2022-12-21 10:20:49.000000 normflows-1.7.1/normflows/nets/lipschitz.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     9712 2022-11-09 20:18:25.000000 normflows-1.7.1/normflows/nets/made.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     4741 2022-12-21 10:20:49.000000 normflows-1.7.1/normflows/nets/made_test.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2284 2022-12-21 10:20:49.000000 normflows-1.7.1/normflows/nets/mlp.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     6999 2022-07-26 14:04:52.000000 normflows-1.7.1/normflows/nets/resnet.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-26 13:01:32.000000 normflows-1.7.1/normflows/sampling/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)       23 2022-07-26 14:04:52.000000 normflows-1.7.1/normflows/sampling/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1999 2022-11-09 20:18:25.000000 normflows-1.7.1/normflows/sampling/hais.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1982 2023-01-22 11:55:37.000000 normflows-1.7.1/normflows/transforms.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      656 2023-01-22 11:55:37.000000 normflows-1.7.1/normflows/transforms_test.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-26 13:01:32.000000 normflows-1.7.1/normflows/utils/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      262 2022-07-26 14:04:52.000000 normflows-1.7.1/normflows/utils/__init__.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2046 2022-11-09 20:18:25.000000 normflows-1.7.1/normflows/utils/eval.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1660 2022-11-09 20:18:25.000000 normflows-1.7.1/normflows/utils/masks.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     5660 2022-12-21 10:20:49.000000 normflows-1.7.1/normflows/utils/nn.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)      852 2022-11-09 20:18:25.000000 normflows-1.7.1/normflows/utils/optim.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     1168 2022-11-09 20:18:25.000000 normflows-1.7.1/normflows/utils/preprocessing.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     7744 2022-07-26 14:04:52.000000 normflows-1.7.1/normflows/utils/splines.py
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2318 2023-01-20 17:41:25.000000 normflows-1.7.1/normflows/utils/splines_test.py
+drwxrwxr-x   0 vstimper  (1000) vstimper  (1000)        0 2023-06-26 13:01:32.000000 normflows-1.7.1/normflows.egg-info/
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)    15920 2023-06-26 13:01:32.000000 normflows-1.7.1/normflows.egg-info/PKG-INFO
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)     2436 2023-06-26 13:01:32.000000 normflows-1.7.1/normflows.egg-info/SOURCES.txt
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)        1 2023-06-26 13:01:32.000000 normflows-1.7.1/normflows.egg-info/dependency_links.txt
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)       63 2023-06-26 13:01:32.000000 normflows-1.7.1/normflows.egg-info/requires.txt
+-rw-rw-r--   0 vstimper  (1000) vstimper  (1000)       10 2023-06-26 13:01:32.000000 normflows-1.7.1/normflows.egg-info/top_level.txt
+-rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)       11 2022-07-26 12:32:34.000000 normflows-1.7.1/requirements.txt
+-rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)      108 2023-06-26 13:01:32.000000 normflows-1.7.1/setup.cfg
+-rwxrwxr-x   0 vstimper  (1000) vstimper  (1000)     1368 2023-06-26 12:41:09.000000 normflows-1.7.1/setup.py
```

### Comparing `normflows-1.7.0/LICENSE` & `normflows-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/PKG-INFO` & `normflows-1.7.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,23 @@
-Metadata-Version: 2.1
-Name: normflows
-Version: 1.7.0
-Summary: Pytorch implementation of normalizing flows
-Home-page: https://github.com/VincentStimper/normalizing-flows
-Author: Vincent Stimper
-Author-email: vincent.stimper@tuebingen.mpg.de
-License: MIT
-Download-URL: https://github.com/VincentStimper/normalizing-flows/archive/refs/heads/master.zip
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-License-File: LICENSE
-
 # `normflows`: A PyTorch Package for Normalizing Flows
 
 [![documentation](https://github.com/VincentStimper/normalizing-flows/actions/workflows/mkdocs.yaml/badge.svg)](https://vincentstimper.github.io/normalizing-flows/)
 ![unit-tests](https://github.com/VincentStimper/normalizing-flows/actions/workflows/pytest.yaml/badge.svg)
 ![code coverage](https://raw.githubusercontent.com/VincentStimper/normalizing-flows/coverage-badge/coverage.svg?raw=true)
-[![License: MIT](https://img.shields.io/badge/Licence-MIT-lightgrey)](https://opensource.org/licenses/MIT)
-[![arXiv](https://img.shields.io/badge/arXiv-2302.12014-b31b1b.svg)](https://arxiv.org/abs/2302.12014) 
-[![PyPI](https://img.shields.io/badge/PyPI-1.7.0-blue.svg)](https://pypi.org/project/normflows/)
+[![License: MIT](https://img.shields.io/badge/Licence-MIT-b31b1b.svg)](https://opensource.org/licenses/MIT)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05361/status.svg)](https://doi.org/10.21105/joss.05361)
+[![PyPI](https://img.shields.io/badge/PyPI-1.7.1-blue.svg)](https://pypi.org/project/normflows/)
 [![Downloads](https://static.pepy.tech/personalized-badge/normflows?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/normflows)
 
 
 `normflows` is a PyTorch implementation of discrete normalizing flows. Many popular flow architectures are implemented,
 see the [list below](#implemented-flows). The package can be easily [installed via pip](#installation).
 The basic usage is described [here](#usage), and a [full documentation](https://vincentstimper.github.io/normalizing-flows/) 
-is available as well. A more detailed description of this package is given in out accompanying 
-[paper](https://arxiv.org/abs/2302.12014).
+is available as well. A more detailed description of this package is given in our
+[accompanying paper](https://joss.theoj.org/papers/10.21105/joss.05361).
 
 Several sample use cases are provided in the 
 [`examples` folder](https://github.com/VincentStimper/normalizing-flows/blob/master/examples), 
 including [Glow](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/glow.ipynb),
 a [VAE](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/vae.py), and
 a [Residual Flow](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/residual.ipynb).
 Moreover, two simple applications are highlighed in the [examples section](#examples). You can run them 
@@ -188,15 +171,15 @@
 
 In [another example](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/paper_example_nsf_colab.ipynb),
 which is available in [Colab](https://colab.research.google.com/github/VincentStimper/normalizing-flows/blob/master/examples/paper_example_nsf_colab.ipynb)
 as well, we apply a Neural Spline Flow model to a distribution defined on a cylinder. The resulting density is visualized below.
 
 ![Neural Spline Flow applied to target distribution on a cylinder](https://raw.githubusercontent.com/VincentStimper/normalizing-flows/master/figures/nsf_cylinder_3d.png)
 
-This example is considered in the [paper](https://arxiv.org/abs/2302.12014) accompanying this repository.
+This example is considered in the [paper](https://joss.theoj.org/papers/10.21105/joss.05361) accompanying this repository.
 
 ## Support
 
 If you have problems, please read the [package documentation](https://vincentstimper.github.io/normalizing-flows/)
 and check out the [examples section](#examples) above. You are also welcome to 
 [create issues on GitHub](https://github.com/VincentStimper/normalizing-flows/issues) to get help. Note that it is
 worthwhile browsing the existing [open](https://github.com/VincentStimper/normalizing-flows/issues?q=is%3Aopen+is%3Aissue) 
@@ -241,29 +224,34 @@
 > [Code available on GitHub.](https://github.com/lollcat/fab-torch)
 
 Moreover, the [`boltzgen`](https://github.com/VincentStimper/boltzmann-generators) package
 has been build upon `normflows`.
 
 ## Citation
 
-If you use `normflows`, please consider citing the [corresponding paper](https://arxiv.org/abs/2302.12014) as follows.
+If you use `normflows`, please cite the 
+[corresponding paper](https://joss.theoj.org/papers/10.21105/joss.05361) as follows.
 
-> Vincent Stimper, David Liu, Andrew Campbell, Vincent Berenz, Lukas Ryll, Bernhard Schölkopf, José Miguel Hernández-Lobato.
-> normflows: A PyTorch Package for Normalizing Flows, arXiv preprint arXiv:2302.12014, 2023.
+> Stimper et al., (2023). normflows: A PyTorch Package for Normalizing Flows. 
+> Journal of Open Source Software, 8(86), 5361, https://doi.org/10.21105/joss.05361
 
 **Bibtex**
 
 ```
-@article{normflows,
-  author = {Vincent Stimper and David Liu and Andrew Campbell and Vincent Berenz and Lukas Ryll and Bernhard Sch{\"o}lkopf and Jos{\'e} Miguel Hern{\'a}ndez-Lobato},
-  title = {normflows: {A} {P}y{T}orch {P}ackage for {N}ormalizing {F}lows},
-  journal = {arXiv preprint arXiv:2302.12014},
+@article{Stimper2023, 
+  author = {Vincent Stimper and David Liu and Andrew Campbell and Vincent Berenz and Lukas Ryll and Bernhard Schölkopf and José Miguel Hernández-Lobato}, 
+  title = {normflows: A PyTorch Package for Normalizing Flows}, 
+  journal = {Journal of Open Source Software}, 
+  volume = {8},
+  number = {86}, 
+  pages = {5361}, 
+  publisher = {The Open Journal}, 
+  doi = {10.21105/joss.05361}, 
+  url = {https://doi.org/10.21105/joss.05361}, 
   year = {2023}
-}
+} 
 ```
 
 
 
 
 
-
-
```

#### html2text {}

```diff
@@ -1,54 +1,45 @@
-Metadata-Version: 2.1 Name: normflows Version: 1.7.0 Summary: Pytorch
-implementation of normalizing flows Home-page: https://github.com/
-VincentStimper/normalizing-flows Author: Vincent Stimper Author-email:
-vincent.stimper@tuebingen.mpg.de License: MIT Download-URL: https://github.com/
-VincentStimper/normalizing-flows/archive/refs/heads/master.zip Platform:
-UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
-Audience :: Developers Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown Provides-Extra: docs License-File:
-LICENSE # `normflows`: A PyTorch Package for Normalizing Flows [!
-[documentation](https://github.com/VincentStimper/normalizing-flows/actions/
-workflows/mkdocs.yaml/badge.svg)](https://vincentstimper.github.io/normalizing-
-flows/) ![unit-tests](https://github.com/VincentStimper/normalizing-flows/
-actions/workflows/pytest.yaml/badge.svg) ![code coverage](https://
-raw.githubusercontent.com/VincentStimper/normalizing-flows/coverage-badge/
-coverage.svg?raw=true) [![License: MIT](https://img.shields.io/badge/Licence-
-MIT-lightgrey)](https://opensource.org/licenses/MIT) [![arXiv](https://
-img.shields.io/badge/arXiv-2302.12014-b31b1b.svg)](https://arxiv.org/abs/
-2302.12014) [![PyPI](https://img.shields.io/badge/PyPI-1.7.0-blue.svg)](https:/
-/pypi.org/project/normflows/) [![Downloads](https://static.pepy.tech/
-personalized-badge/
+# `normflows`: A PyTorch Package for Normalizing Flows [![documentation](https:
+//github.com/VincentStimper/normalizing-flows/actions/workflows/mkdocs.yaml/
+badge.svg)](https://vincentstimper.github.io/normalizing-flows/) ![unit-tests]
+(https://github.com/VincentStimper/normalizing-flows/actions/workflows/
+pytest.yaml/badge.svg) ![code coverage](https://raw.githubusercontent.com/
+VincentStimper/normalizing-flows/coverage-badge/coverage.svg?raw=true) [!
+[License: MIT](https://img.shields.io/badge/Licence-MIT-b31b1b.svg)](https://
+opensource.org/licenses/MIT) [![DOI](https://joss.theoj.org/papers/10.21105/
+joss.05361/status.svg)](https://doi.org/10.21105/joss.05361) [![PyPI](https://
+img.shields.io/badge/PyPI-1.7.1-blue.svg)](https://pypi.org/project/normflows/
+) [![Downloads](https://static.pepy.tech/personalized-badge/
 normflows?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)]
 (https://pepy.tech/project/normflows) `normflows` is a PyTorch implementation
 of discrete normalizing flows. Many popular flow architectures are implemented,
 see the [list below](#implemented-flows). The package can be easily [installed
 via pip](#installation). The basic usage is described [here](#usage), and a
 [full documentation](https://vincentstimper.github.io/normalizing-flows/) is
-available as well. A more detailed description of this package is given in out
-accompanying [paper](https://arxiv.org/abs/2302.12014). Several sample use
-cases are provided in the [`examples` folder](https://github.com/
-VincentStimper/normalizing-flows/blob/master/examples), including [Glow](https:
-//github.com/VincentStimper/normalizing-flows/blob/master/examples/glow.ipynb),
-a [VAE](https://github.com/VincentStimper/normalizing-flows/blob/master/
-examples/vae.py), and a [Residual Flow](https://github.com/VincentStimper/
-normalizing-flows/blob/master/examples/residual.ipynb). Moreover, two simple
-applications are highlighed in the [examples section](#examples). You can run
-them yourself in Google Colab using the links below to get a feeling for
-`normflows`. | Link | Description | |------------------------------------------
+available as well. A more detailed description of this package is given in our
+[accompanying paper](https://joss.theoj.org/papers/10.21105/joss.05361).
+Several sample use cases are provided in the [`examples` folder](https://
+github.com/VincentStimper/normalizing-flows/blob/master/examples), including
+[Glow](https://github.com/VincentStimper/normalizing-flows/blob/master/
+examples/glow.ipynb), a [VAE](https://github.com/VincentStimper/normalizing-
+flows/blob/master/examples/vae.py), and a [Residual Flow](https://github.com/
+VincentStimper/normalizing-flows/blob/master/examples/residual.ipynb).
+Moreover, two simple applications are highlighed in the [examples section]
+(#examples). You can run them yourself in Google Colab using the links below to
+get a feeling for `normflows`. | Link | Description | |------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
------------------------------------------------|-------------------------------
-------------------------------------------| | [Open_In_Colab] | Real NVP
-applied to a 2D bimodal target distribution | | [Open_In_Colab] | Modeling a
-distribution on a cylinder surface with a neural spline flow | | [Open_In
-Colab] | Modeling and generating CIFAR-10 images with Glow | ## Implemented
-Flows | Architecture | Reference | |--------------|----------------------------
+-----------------------------------------------------------------|-------------
+------------------------------------------------------------| | [Open_In_Colab]
+| Real NVP applied to a 2D bimodal target distribution | | [Open_In_Colab] |
+Modeling a distribution on a cylinder surface with a neural spline flow | |
+[Open_In_Colab] | Modeling and generating CIFAR-10 images with Glow | ##
+Implemented Flows | Architecture | Reference | |--------------|----------------
 -------------------------------------------------------------------------------
-----------------| | Planar Flow | [Rezende & Mohamed, 2015](http://
+----------------------------| | Planar Flow | [Rezende & Mohamed, 2015](http://
 proceedings.mlr.press/v37/rezende15.html) | | Radial Flow | [Rezende & Mohamed,
 2015](http://proceedings.mlr.press/v37/rezende15.html) | | NICE | [Dinh et al.,
 2014](https://arxiv.org/abs/1410.8516) | | Real NVP | [Dinh et al., 2017]
 (https://openreview.net/forum?id=HkpbnH9lx) | | Glow | [Kingma et al., 2018]
 (https://proceedings.neurips.cc/paper/2018/hash/
 d139db6a236200b21cc7f752979132d0-Abstract.html) | | Masked Autoregressive Flow
 | [Papamakarios et al., 2017](https://proceedings.neurips.cc/paper/2017/hash/
@@ -127,54 +118,55 @@
 master/examples/paper_example_nsf_colab.ipynb), which is available in [Colab]
 (https://colab.research.google.com/github/VincentStimper/normalizing-flows/
 blob/master/examples/paper_example_nsf_colab.ipynb) as well, we apply a Neural
 Spline Flow model to a distribution defined on a cylinder. The resulting
 density is visualized below. ![Neural Spline Flow applied to target
 distribution on a cylinder](https://raw.githubusercontent.com/VincentStimper/
 normalizing-flows/master/figures/nsf_cylinder_3d.png) This example is
-considered in the [paper](https://arxiv.org/abs/2302.12014) accompanying this
-repository. ## Support If you have problems, please read the [package
-documentation](https://vincentstimper.github.io/normalizing-flows/) and check
-out the [examples section](#examples) above. You are also welcome to [create
-issues on GitHub](https://github.com/VincentStimper/normalizing-flows/issues)
-to get help. Note that it is worthwhile browsing the existing [open](https://
-github.com/VincentStimper/normalizing-flows/issues?q=is%3Aopen+is%3Aissue) and
-[closed](https://github.com/VincentStimper/normalizing-flows/
-issues?q=is%3Aissue+is%3Aclosed) issues, which might address the problem you
-are facing. ## Contributing If you find a bug or have a feature request, please
-[file an issue on GitHub](https://github.com/VincentStimper/normalizing-flows/
-issues). You are welcome to contribute to the package by fixing the bug or
-adding the feature yourself. If you want to contribute, please add tests for
-the code you added or modified and ensure it passes successfully by running
-`pytest`. This can be done by simply executing ``` pytest ``` within your local
-version of the repository. Make sure you code is well documented, and we also
-encourage contributions to the existing documentation. Once you finished coding
-and testing, please [create a pull request on GitHub](https://docs.github.com/
-en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-
-work-with-pull-requests/creating-a-pull-request). ## Used by The package has
-been used in several research papers, which are listed below. > Andrew
-Campbell, Wenlong Chen, Vincent Stimper, JosÃ© Miguel HernÃ¡ndez-Lobato, and
-Yichuan Zhang. > [A gradient based strategy for Hamiltonian Monte Carlo
-hyperparameter optimization](https://proceedings.mlr.press/v139/
-campbell21a.html). > In Proceedings of the 38th International Conference on
-Machine Learning, pp. 1238â1248. PMLR, 2021. > > [Code available on GitHub.]
-(https://github.com/VincentStimper/hmc-hyperparameter-tuning) > Vincent
-Stimper, Bernhard SchÃ¶lkopf, JosÃ© Miguel HernÃ¡ndez-Lobato. > [Resampling
-Base Distributions of Normalizing Flows](https://proceedings.mlr.press/v151/
-stimper22a). > In Proceedings of The 25th International Conference on
-Artificial Intelligence and Statistics, volume 151, pp. 4915â4936, 2022. > >
-[Code available on GitHub.](https://github.com/VincentStimper/resampled-base-
-flows) > Laurence I. Midgley, Vincent Stimper, Gregor N. C. Simm, Bernhard
-SchÃ¶lkopf, JosÃ© Miguel HernÃ¡ndez-Lobato. > [Flow Annealed Importance
-Sampling Bootstrap](https://arxiv.org/abs/2208.01893). > arXiv preprint arXiv:
-2208.01893, 2022. > > [Code available on GitHub.](https://github.com/lollcat/
-fab-torch) Moreover, the [`boltzgen`](https://github.com/VincentStimper/
-boltzmann-generators) package has been build upon `normflows`. ## Citation If
-you use `normflows`, please consider citing the [corresponding paper](https://
-arxiv.org/abs/2302.12014) as follows. > Vincent Stimper, David Liu, Andrew
-Campbell, Vincent Berenz, Lukas Ryll, Bernhard SchÃ¶lkopf, JosÃ© Miguel
-HernÃ¡ndez-Lobato. > normflows: A PyTorch Package for Normalizing Flows, arXiv
-preprint arXiv:2302.12014, 2023. **Bibtex** ``` @article{normflows, author =
-{Vincent Stimper and David Liu and Andrew Campbell and Vincent Berenz and Lukas
-Ryll and Bernhard Sch{\"o}lkopf and Jos{\'e} Miguel Hern{\'a}ndez-Lobato},
-title = {normflows: {A} {P}y{T}orch {P}ackage for {N}ormalizing {F}lows},
-journal = {arXiv preprint arXiv:2302.12014}, year = {2023} } ```
+considered in the [paper](https://joss.theoj.org/papers/10.21105/joss.05361)
+accompanying this repository. ## Support If you have problems, please read the
+[package documentation](https://vincentstimper.github.io/normalizing-flows/
+) and check out the [examples section](#examples) above. You are also welcome
+to [create issues on GitHub](https://github.com/VincentStimper/normalizing-
+flows/issues) to get help. Note that it is worthwhile browsing the existing
+[open](https://github.com/VincentStimper/normalizing-flows/
+issues?q=is%3Aopen+is%3Aissue) and [closed](https://github.com/VincentStimper/
+normalizing-flows/issues?q=is%3Aissue+is%3Aclosed) issues, which might address
+the problem you are facing. ## Contributing If you find a bug or have a feature
+request, please [file an issue on GitHub](https://github.com/VincentStimper/
+normalizing-flows/issues). You are welcome to contribute to the package by
+fixing the bug or adding the feature yourself. If you want to contribute,
+please add tests for the code you added or modified and ensure it passes
+successfully by running `pytest`. This can be done by simply executing ```
+pytest ``` within your local version of the repository. Make sure you code is
+well documented, and we also encourage contributions to the existing
+documentation. Once you finished coding and testing, please [create a pull
+request on GitHub](https://docs.github.com/en/pull-requests/collaborating-with-
+pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-
+pull-request). ## Used by The package has been used in several research papers,
+which are listed below. > Andrew Campbell, Wenlong Chen, Vincent Stimper, JosÃ©
+Miguel HernÃ¡ndez-Lobato, and Yichuan Zhang. > [A gradient based strategy for
+Hamiltonian Monte Carlo hyperparameter optimization](https://
+proceedings.mlr.press/v139/campbell21a.html). > In Proceedings of the 38th
+International Conference on Machine Learning, pp. 1238â1248. PMLR, 2021. > >
+[Code available on GitHub.](https://github.com/VincentStimper/hmc-
+hyperparameter-tuning) > Vincent Stimper, Bernhard SchÃ¶lkopf, JosÃ© Miguel
+HernÃ¡ndez-Lobato. > [Resampling Base Distributions of Normalizing Flows]
+(https://proceedings.mlr.press/v151/stimper22a). > In Proceedings of The 25th
+International Conference on Artificial Intelligence and Statistics, volume 151,
+pp. 4915â4936, 2022. > > [Code available on GitHub.](https://github.com/
+VincentStimper/resampled-base-flows) > Laurence I. Midgley, Vincent Stimper,
+Gregor N. C. Simm, Bernhard SchÃ¶lkopf, JosÃ© Miguel HernÃ¡ndez-Lobato. > [Flow
+Annealed Importance Sampling Bootstrap](https://arxiv.org/abs/2208.01893). >
+arXiv preprint arXiv:2208.01893, 2022. > > [Code available on GitHub.](https://
+github.com/lollcat/fab-torch) Moreover, the [`boltzgen`](https://github.com/
+VincentStimper/boltzmann-generators) package has been build upon `normflows`.
+## Citation If you use `normflows`, please cite the [corresponding paper]
+(https://joss.theoj.org/papers/10.21105/joss.05361) as follows. > Stimper et
+al., (2023). normflows: A PyTorch Package for Normalizing Flows. > Journal of
+Open Source Software, 8(86), 5361, https://doi.org/10.21105/joss.05361
+**Bibtex** ``` @article{Stimper2023, author = {Vincent Stimper and David Liu
+and Andrew Campbell and Vincent Berenz and Lukas Ryll and Bernhard SchÃ¶lkopf
+and JosÃ© Miguel HernÃ¡ndez-Lobato}, title = {normflows: A PyTorch Package for
+Normalizing Flows}, journal = {Journal of Open Source Software}, volume = {8},
+number = {86}, pages = {5361}, publisher = {The Open Journal}, doi = {10.21105/
+joss.05361}, url = {https://doi.org/10.21105/joss.05361}, year = {2023} } ```
```

### Comparing `normflows-1.7.0/README.md` & `normflows-1.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,40 @@
+Metadata-Version: 2.1
+Name: normflows
+Version: 1.7.1
+Summary: Pytorch implementation of normalizing flows
+Home-page: https://github.com/VincentStimper/normalizing-flows
+Author: Vincent Stimper
+Author-email: vincent.stimper@tuebingen.mpg.de
+License: MIT
+Download-URL: https://github.com/VincentStimper/normalizing-flows/archive/refs/heads/master.zip
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+License-File: LICENSE
+
 # `normflows`: A PyTorch Package for Normalizing Flows
 
 [![documentation](https://github.com/VincentStimper/normalizing-flows/actions/workflows/mkdocs.yaml/badge.svg)](https://vincentstimper.github.io/normalizing-flows/)
 ![unit-tests](https://github.com/VincentStimper/normalizing-flows/actions/workflows/pytest.yaml/badge.svg)
 ![code coverage](https://raw.githubusercontent.com/VincentStimper/normalizing-flows/coverage-badge/coverage.svg?raw=true)
-[![License: MIT](https://img.shields.io/badge/Licence-MIT-lightgrey)](https://opensource.org/licenses/MIT)
-[![arXiv](https://img.shields.io/badge/arXiv-2302.12014-b31b1b.svg)](https://arxiv.org/abs/2302.12014) 
-[![PyPI](https://img.shields.io/badge/PyPI-1.7.0-blue.svg)](https://pypi.org/project/normflows/)
+[![License: MIT](https://img.shields.io/badge/Licence-MIT-b31b1b.svg)](https://opensource.org/licenses/MIT)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05361/status.svg)](https://doi.org/10.21105/joss.05361)
+[![PyPI](https://img.shields.io/badge/PyPI-1.7.1-blue.svg)](https://pypi.org/project/normflows/)
 [![Downloads](https://static.pepy.tech/personalized-badge/normflows?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/normflows)
 
 
 `normflows` is a PyTorch implementation of discrete normalizing flows. Many popular flow architectures are implemented,
 see the [list below](#implemented-flows). The package can be easily [installed via pip](#installation).
 The basic usage is described [here](#usage), and a [full documentation](https://vincentstimper.github.io/normalizing-flows/) 
-is available as well. A more detailed description of this package is given in out accompanying 
-[paper](https://arxiv.org/abs/2302.12014).
+is available as well. A more detailed description of this package is given in our
+[accompanying paper](https://joss.theoj.org/papers/10.21105/joss.05361).
 
 Several sample use cases are provided in the 
 [`examples` folder](https://github.com/VincentStimper/normalizing-flows/blob/master/examples), 
 including [Glow](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/glow.ipynb),
 a [VAE](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/vae.py), and
 a [Residual Flow](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/residual.ipynb).
 Moreover, two simple applications are highlighed in the [examples section](#examples). You can run them 
@@ -171,15 +188,15 @@
 
 In [another example](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/paper_example_nsf_colab.ipynb),
 which is available in [Colab](https://colab.research.google.com/github/VincentStimper/normalizing-flows/blob/master/examples/paper_example_nsf_colab.ipynb)
 as well, we apply a Neural Spline Flow model to a distribution defined on a cylinder. The resulting density is visualized below.
 
 ![Neural Spline Flow applied to target distribution on a cylinder](https://raw.githubusercontent.com/VincentStimper/normalizing-flows/master/figures/nsf_cylinder_3d.png)
 
-This example is considered in the [paper](https://arxiv.org/abs/2302.12014) accompanying this repository.
+This example is considered in the [paper](https://joss.theoj.org/papers/10.21105/joss.05361) accompanying this repository.
 
 ## Support
 
 If you have problems, please read the [package documentation](https://vincentstimper.github.io/normalizing-flows/)
 and check out the [examples section](#examples) above. You are also welcome to 
 [create issues on GitHub](https://github.com/VincentStimper/normalizing-flows/issues) to get help. Note that it is
 worthwhile browsing the existing [open](https://github.com/VincentStimper/normalizing-flows/issues?q=is%3Aopen+is%3Aissue) 
@@ -224,27 +241,36 @@
 > [Code available on GitHub.](https://github.com/lollcat/fab-torch)
 
 Moreover, the [`boltzgen`](https://github.com/VincentStimper/boltzmann-generators) package
 has been build upon `normflows`.
 
 ## Citation
 
-If you use `normflows`, please consider citing the [corresponding paper](https://arxiv.org/abs/2302.12014) as follows.
+If you use `normflows`, please cite the 
+[corresponding paper](https://joss.theoj.org/papers/10.21105/joss.05361) as follows.
 
-> Vincent Stimper, David Liu, Andrew Campbell, Vincent Berenz, Lukas Ryll, Bernhard Schölkopf, José Miguel Hernández-Lobato.
-> normflows: A PyTorch Package for Normalizing Flows, arXiv preprint arXiv:2302.12014, 2023.
+> Stimper et al., (2023). normflows: A PyTorch Package for Normalizing Flows. 
+> Journal of Open Source Software, 8(86), 5361, https://doi.org/10.21105/joss.05361
 
 **Bibtex**
 
 ```
-@article{normflows,
-  author = {Vincent Stimper and David Liu and Andrew Campbell and Vincent Berenz and Lukas Ryll and Bernhard Sch{\"o}lkopf and Jos{\'e} Miguel Hern{\'a}ndez-Lobato},
-  title = {normflows: {A} {P}y{T}orch {P}ackage for {N}ormalizing {F}lows},
-  journal = {arXiv preprint arXiv:2302.12014},
+@article{Stimper2023, 
+  author = {Vincent Stimper and David Liu and Andrew Campbell and Vincent Berenz and Lukas Ryll and Bernhard Schölkopf and José Miguel Hernández-Lobato}, 
+  title = {normflows: A PyTorch Package for Normalizing Flows}, 
+  journal = {Journal of Open Source Software}, 
+  volume = {8},
+  number = {86}, 
+  pages = {5361}, 
+  publisher = {The Open Journal}, 
+  doi = {10.21105/joss.05361}, 
+  url = {https://doi.org/10.21105/joss.05361}, 
   year = {2023}
-}
+} 
 ```
 
 
 
 
 
+
+
```

#### html2text {}

```diff
@@ -1,45 +1,54 @@
-# `normflows`: A PyTorch Package for Normalizing Flows [![documentation](https:
-//github.com/VincentStimper/normalizing-flows/actions/workflows/mkdocs.yaml/
-badge.svg)](https://vincentstimper.github.io/normalizing-flows/) ![unit-tests]
-(https://github.com/VincentStimper/normalizing-flows/actions/workflows/
-pytest.yaml/badge.svg) ![code coverage](https://raw.githubusercontent.com/
-VincentStimper/normalizing-flows/coverage-badge/coverage.svg?raw=true) [!
-[License: MIT](https://img.shields.io/badge/Licence-MIT-lightgrey)](https://
-opensource.org/licenses/MIT) [![arXiv](https://img.shields.io/badge/arXiv-
-2302.12014-b31b1b.svg)](https://arxiv.org/abs/2302.12014) [![PyPI](https://
-img.shields.io/badge/PyPI-1.7.0-blue.svg)](https://pypi.org/project/normflows/
-) [![Downloads](https://static.pepy.tech/personalized-badge/
+Metadata-Version: 2.1 Name: normflows Version: 1.7.1 Summary: Pytorch
+implementation of normalizing flows Home-page: https://github.com/
+VincentStimper/normalizing-flows Author: Vincent Stimper Author-email:
+vincent.stimper@tuebingen.mpg.de License: MIT Download-URL: https://github.com/
+VincentStimper/normalizing-flows/archive/refs/heads/master.zip Platform:
+UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
+Audience :: Developers Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown Provides-Extra: docs License-File:
+LICENSE # `normflows`: A PyTorch Package for Normalizing Flows [!
+[documentation](https://github.com/VincentStimper/normalizing-flows/actions/
+workflows/mkdocs.yaml/badge.svg)](https://vincentstimper.github.io/normalizing-
+flows/) ![unit-tests](https://github.com/VincentStimper/normalizing-flows/
+actions/workflows/pytest.yaml/badge.svg) ![code coverage](https://
+raw.githubusercontent.com/VincentStimper/normalizing-flows/coverage-badge/
+coverage.svg?raw=true) [![License: MIT](https://img.shields.io/badge/Licence-
+MIT-b31b1b.svg)](https://opensource.org/licenses/MIT) [![DOI](https://
+joss.theoj.org/papers/10.21105/joss.05361/status.svg)](https://doi.org/
+10.21105/joss.05361) [![PyPI](https://img.shields.io/badge/PyPI-1.7.1-
+blue.svg)](https://pypi.org/project/normflows/) [![Downloads](https://
+static.pepy.tech/personalized-badge/
 normflows?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)]
 (https://pepy.tech/project/normflows) `normflows` is a PyTorch implementation
 of discrete normalizing flows. Many popular flow architectures are implemented,
 see the [list below](#implemented-flows). The package can be easily [installed
 via pip](#installation). The basic usage is described [here](#usage), and a
 [full documentation](https://vincentstimper.github.io/normalizing-flows/) is
-available as well. A more detailed description of this package is given in out
-accompanying [paper](https://arxiv.org/abs/2302.12014). Several sample use
-cases are provided in the [`examples` folder](https://github.com/
-VincentStimper/normalizing-flows/blob/master/examples), including [Glow](https:
-//github.com/VincentStimper/normalizing-flows/blob/master/examples/glow.ipynb),
-a [VAE](https://github.com/VincentStimper/normalizing-flows/blob/master/
-examples/vae.py), and a [Residual Flow](https://github.com/VincentStimper/
-normalizing-flows/blob/master/examples/residual.ipynb). Moreover, two simple
-applications are highlighed in the [examples section](#examples). You can run
-them yourself in Google Colab using the links below to get a feeling for
-`normflows`. | Link | Description | |------------------------------------------
+available as well. A more detailed description of this package is given in our
+[accompanying paper](https://joss.theoj.org/papers/10.21105/joss.05361).
+Several sample use cases are provided in the [`examples` folder](https://
+github.com/VincentStimper/normalizing-flows/blob/master/examples), including
+[Glow](https://github.com/VincentStimper/normalizing-flows/blob/master/
+examples/glow.ipynb), a [VAE](https://github.com/VincentStimper/normalizing-
+flows/blob/master/examples/vae.py), and a [Residual Flow](https://github.com/
+VincentStimper/normalizing-flows/blob/master/examples/residual.ipynb).
+Moreover, two simple applications are highlighed in the [examples section]
+(#examples). You can run them yourself in Google Colab using the links below to
+get a feeling for `normflows`. | Link | Description | |------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
------------------------------------------------|-------------------------------
-------------------------------------------| | [Open_In_Colab] | Real NVP
-applied to a 2D bimodal target distribution | | [Open_In_Colab] | Modeling a
-distribution on a cylinder surface with a neural spline flow | | [Open_In
-Colab] | Modeling and generating CIFAR-10 images with Glow | ## Implemented
-Flows | Architecture | Reference | |--------------|----------------------------
+-----------------------------------------------------------------|-------------
+------------------------------------------------------------| | [Open_In_Colab]
+| Real NVP applied to a 2D bimodal target distribution | | [Open_In_Colab] |
+Modeling a distribution on a cylinder surface with a neural spline flow | |
+[Open_In_Colab] | Modeling and generating CIFAR-10 images with Glow | ##
+Implemented Flows | Architecture | Reference | |--------------|----------------
 -------------------------------------------------------------------------------
-----------------| | Planar Flow | [Rezende & Mohamed, 2015](http://
+----------------------------| | Planar Flow | [Rezende & Mohamed, 2015](http://
 proceedings.mlr.press/v37/rezende15.html) | | Radial Flow | [Rezende & Mohamed,
 2015](http://proceedings.mlr.press/v37/rezende15.html) | | NICE | [Dinh et al.,
 2014](https://arxiv.org/abs/1410.8516) | | Real NVP | [Dinh et al., 2017]
 (https://openreview.net/forum?id=HkpbnH9lx) | | Glow | [Kingma et al., 2018]
 (https://proceedings.neurips.cc/paper/2018/hash/
 d139db6a236200b21cc7f752979132d0-Abstract.html) | | Masked Autoregressive Flow
 | [Papamakarios et al., 2017](https://proceedings.neurips.cc/paper/2017/hash/
@@ -118,54 +127,55 @@
 master/examples/paper_example_nsf_colab.ipynb), which is available in [Colab]
 (https://colab.research.google.com/github/VincentStimper/normalizing-flows/
 blob/master/examples/paper_example_nsf_colab.ipynb) as well, we apply a Neural
 Spline Flow model to a distribution defined on a cylinder. The resulting
 density is visualized below. ![Neural Spline Flow applied to target
 distribution on a cylinder](https://raw.githubusercontent.com/VincentStimper/
 normalizing-flows/master/figures/nsf_cylinder_3d.png) This example is
-considered in the [paper](https://arxiv.org/abs/2302.12014) accompanying this
-repository. ## Support If you have problems, please read the [package
-documentation](https://vincentstimper.github.io/normalizing-flows/) and check
-out the [examples section](#examples) above. You are also welcome to [create
-issues on GitHub](https://github.com/VincentStimper/normalizing-flows/issues)
-to get help. Note that it is worthwhile browsing the existing [open](https://
-github.com/VincentStimper/normalizing-flows/issues?q=is%3Aopen+is%3Aissue) and
-[closed](https://github.com/VincentStimper/normalizing-flows/
-issues?q=is%3Aissue+is%3Aclosed) issues, which might address the problem you
-are facing. ## Contributing If you find a bug or have a feature request, please
-[file an issue on GitHub](https://github.com/VincentStimper/normalizing-flows/
-issues). You are welcome to contribute to the package by fixing the bug or
-adding the feature yourself. If you want to contribute, please add tests for
-the code you added or modified and ensure it passes successfully by running
-`pytest`. This can be done by simply executing ``` pytest ``` within your local
-version of the repository. Make sure you code is well documented, and we also
-encourage contributions to the existing documentation. Once you finished coding
-and testing, please [create a pull request on GitHub](https://docs.github.com/
-en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-
-work-with-pull-requests/creating-a-pull-request). ## Used by The package has
-been used in several research papers, which are listed below. > Andrew
-Campbell, Wenlong Chen, Vincent Stimper, JosÃ© Miguel HernÃ¡ndez-Lobato, and
-Yichuan Zhang. > [A gradient based strategy for Hamiltonian Monte Carlo
-hyperparameter optimization](https://proceedings.mlr.press/v139/
-campbell21a.html). > In Proceedings of the 38th International Conference on
-Machine Learning, pp. 1238â1248. PMLR, 2021. > > [Code available on GitHub.]
-(https://github.com/VincentStimper/hmc-hyperparameter-tuning) > Vincent
-Stimper, Bernhard SchÃ¶lkopf, JosÃ© Miguel HernÃ¡ndez-Lobato. > [Resampling
-Base Distributions of Normalizing Flows](https://proceedings.mlr.press/v151/
-stimper22a). > In Proceedings of The 25th International Conference on
-Artificial Intelligence and Statistics, volume 151, pp. 4915â4936, 2022. > >
-[Code available on GitHub.](https://github.com/VincentStimper/resampled-base-
-flows) > Laurence I. Midgley, Vincent Stimper, Gregor N. C. Simm, Bernhard
-SchÃ¶lkopf, JosÃ© Miguel HernÃ¡ndez-Lobato. > [Flow Annealed Importance
-Sampling Bootstrap](https://arxiv.org/abs/2208.01893). > arXiv preprint arXiv:
-2208.01893, 2022. > > [Code available on GitHub.](https://github.com/lollcat/
-fab-torch) Moreover, the [`boltzgen`](https://github.com/VincentStimper/
-boltzmann-generators) package has been build upon `normflows`. ## Citation If
-you use `normflows`, please consider citing the [corresponding paper](https://
-arxiv.org/abs/2302.12014) as follows. > Vincent Stimper, David Liu, Andrew
-Campbell, Vincent Berenz, Lukas Ryll, Bernhard SchÃ¶lkopf, JosÃ© Miguel
-HernÃ¡ndez-Lobato. > normflows: A PyTorch Package for Normalizing Flows, arXiv
-preprint arXiv:2302.12014, 2023. **Bibtex** ``` @article{normflows, author =
-{Vincent Stimper and David Liu and Andrew Campbell and Vincent Berenz and Lukas
-Ryll and Bernhard Sch{\"o}lkopf and Jos{\'e} Miguel Hern{\'a}ndez-Lobato},
-title = {normflows: {A} {P}y{T}orch {P}ackage for {N}ormalizing {F}lows},
-journal = {arXiv preprint arXiv:2302.12014}, year = {2023} } ```
+considered in the [paper](https://joss.theoj.org/papers/10.21105/joss.05361)
+accompanying this repository. ## Support If you have problems, please read the
+[package documentation](https://vincentstimper.github.io/normalizing-flows/
+) and check out the [examples section](#examples) above. You are also welcome
+to [create issues on GitHub](https://github.com/VincentStimper/normalizing-
+flows/issues) to get help. Note that it is worthwhile browsing the existing
+[open](https://github.com/VincentStimper/normalizing-flows/
+issues?q=is%3Aopen+is%3Aissue) and [closed](https://github.com/VincentStimper/
+normalizing-flows/issues?q=is%3Aissue+is%3Aclosed) issues, which might address
+the problem you are facing. ## Contributing If you find a bug or have a feature
+request, please [file an issue on GitHub](https://github.com/VincentStimper/
+normalizing-flows/issues). You are welcome to contribute to the package by
+fixing the bug or adding the feature yourself. If you want to contribute,
+please add tests for the code you added or modified and ensure it passes
+successfully by running `pytest`. This can be done by simply executing ```
+pytest ``` within your local version of the repository. Make sure you code is
+well documented, and we also encourage contributions to the existing
+documentation. Once you finished coding and testing, please [create a pull
+request on GitHub](https://docs.github.com/en/pull-requests/collaborating-with-
+pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-
+pull-request). ## Used by The package has been used in several research papers,
+which are listed below. > Andrew Campbell, Wenlong Chen, Vincent Stimper, JosÃ©
+Miguel HernÃ¡ndez-Lobato, and Yichuan Zhang. > [A gradient based strategy for
+Hamiltonian Monte Carlo hyperparameter optimization](https://
+proceedings.mlr.press/v139/campbell21a.html). > In Proceedings of the 38th
+International Conference on Machine Learning, pp. 1238â1248. PMLR, 2021. > >
+[Code available on GitHub.](https://github.com/VincentStimper/hmc-
+hyperparameter-tuning) > Vincent Stimper, Bernhard SchÃ¶lkopf, JosÃ© Miguel
+HernÃ¡ndez-Lobato. > [Resampling Base Distributions of Normalizing Flows]
+(https://proceedings.mlr.press/v151/stimper22a). > In Proceedings of The 25th
+International Conference on Artificial Intelligence and Statistics, volume 151,
+pp. 4915â4936, 2022. > > [Code available on GitHub.](https://github.com/
+VincentStimper/resampled-base-flows) > Laurence I. Midgley, Vincent Stimper,
+Gregor N. C. Simm, Bernhard SchÃ¶lkopf, JosÃ© Miguel HernÃ¡ndez-Lobato. > [Flow
+Annealed Importance Sampling Bootstrap](https://arxiv.org/abs/2208.01893). >
+arXiv preprint arXiv:2208.01893, 2022. > > [Code available on GitHub.](https://
+github.com/lollcat/fab-torch) Moreover, the [`boltzgen`](https://github.com/
+VincentStimper/boltzmann-generators) package has been build upon `normflows`.
+## Citation If you use `normflows`, please cite the [corresponding paper]
+(https://joss.theoj.org/papers/10.21105/joss.05361) as follows. > Stimper et
+al., (2023). normflows: A PyTorch Package for Normalizing Flows. > Journal of
+Open Source Software, 8(86), 5361, https://doi.org/10.21105/joss.05361
+**Bibtex** ``` @article{Stimper2023, author = {Vincent Stimper and David Liu
+and Andrew Campbell and Vincent Berenz and Lukas Ryll and Bernhard SchÃ¶lkopf
+and JosÃ© Miguel HernÃ¡ndez-Lobato}, title = {normflows: A PyTorch Package for
+Normalizing Flows}, journal = {Journal of Open Source Software}, volume = {8},
+number = {86}, pages = {5361}, publisher = {The Open Journal}, doi = {10.21105/
+joss.05361}, url = {https://doi.org/10.21105/joss.05361}, year = {2023} } ```
```

### Comparing `normflows-1.7.0/normflows/core.py` & `normflows-1.7.1/normflows/core.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/core_test.py` & `normflows-1.7.1/normflows/core_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/distributions/__init__.py` & `normflows-1.7.1/normflows/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/distributions/base.py` & `normflows-1.7.1/normflows/distributions/base.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/distributions/base_test.py` & `normflows-1.7.1/normflows/distributions/base_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/distributions/decoder.py` & `normflows-1.7.1/normflows/distributions/decoder.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/distributions/decoder_test.py` & `normflows-1.7.1/normflows/distributions/decoder_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/distributions/distribution_test.py` & `normflows-1.7.1/normflows/distributions/distribution_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/distributions/encoder.py` & `normflows-1.7.1/normflows/distributions/encoder.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/distributions/encoder_test.py` & `normflows-1.7.1/normflows/distributions/encoder_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/distributions/linear_interpolation.py` & `normflows-1.7.1/normflows/distributions/linear_interpolation.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/distributions/mh_proposal.py` & `normflows-1.7.1/normflows/distributions/mh_proposal.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/distributions/prior.py` & `normflows-1.7.1/normflows/distributions/prior.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/distributions/prior_test.py` & `normflows-1.7.1/normflows/distributions/prior_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/distributions/target.py` & `normflows-1.7.1/normflows/distributions/target.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/distributions/target_test.py` & `normflows-1.7.1/normflows/distributions/target_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/__init__.py` & `normflows-1.7.1/normflows/flows/__init__.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/affine/autoregressive.py` & `normflows-1.7.1/normflows/flows/affine/autoregressive.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/affine/autoregressive_test.py` & `normflows-1.7.1/normflows/flows/affine/autoregressive_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/affine/coupling.py` & `normflows-1.7.1/normflows/flows/affine/coupling.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/affine/coupling_test.py` & `normflows-1.7.1/normflows/flows/affine/coupling_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/affine/glow.py` & `normflows-1.7.1/normflows/flows/affine/glow.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/affine/glow_test.py` & `normflows-1.7.1/normflows/flows/affine/glow_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/base.py` & `normflows-1.7.1/normflows/flows/base.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/base_test.py` & `normflows-1.7.1/normflows/flows/base_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/flow_test.py` & `normflows-1.7.1/normflows/flows/flow_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/mixing.py` & `normflows-1.7.1/normflows/flows/mixing.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/mixing_test.py` & `normflows-1.7.1/normflows/flows/mixing_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/neural_spline/autoregressive.py` & `normflows-1.7.1/normflows/flows/neural_spline/autoregressive.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/neural_spline/autoregressive_test.py` & `normflows-1.7.1/normflows/flows/neural_spline/autoregressive_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/neural_spline/coupling.py` & `normflows-1.7.1/normflows/flows/neural_spline/coupling.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/neural_spline/coupling_test.py` & `normflows-1.7.1/normflows/flows/neural_spline/coupling_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/neural_spline/wrapper.py` & `normflows-1.7.1/normflows/flows/neural_spline/wrapper.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/neural_spline/wrapper_test.py` & `normflows-1.7.1/normflows/flows/neural_spline/wrapper_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/normalization.py` & `normflows-1.7.1/normflows/flows/normalization.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/periodic.py` & `normflows-1.7.1/normflows/flows/periodic.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/periodic_test.py` & `normflows-1.7.1/normflows/flows/periodic_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/planar.py` & `normflows-1.7.1/normflows/flows/planar.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/planar_test.py` & `normflows-1.7.1/normflows/flows/planar_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/radial.py` & `normflows-1.7.1/normflows/flows/radial.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/reshape.py` & `normflows-1.7.1/normflows/flows/reshape.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/residual.py` & `normflows-1.7.1/normflows/flows/residual.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/residual_test.py` & `normflows-1.7.1/normflows/flows/residual_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/stochastic.py` & `normflows-1.7.1/normflows/flows/stochastic.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/flows/stochastic_test.py` & `normflows-1.7.1/normflows/flows/stochastic_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/nets/cnn.py` & `normflows-1.7.1/normflows/nets/cnn.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/nets/lipschitz.py` & `normflows-1.7.1/normflows/nets/lipschitz.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/nets/made.py` & `normflows-1.7.1/normflows/nets/made.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/nets/made_test.py` & `normflows-1.7.1/normflows/nets/made_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/nets/mlp.py` & `normflows-1.7.1/normflows/nets/mlp.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/nets/resnet.py` & `normflows-1.7.1/normflows/nets/resnet.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/sampling/hais.py` & `normflows-1.7.1/normflows/sampling/hais.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/transforms.py` & `normflows-1.7.1/normflows/transforms.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/transforms_test.py` & `normflows-1.7.1/normflows/transforms_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/utils/eval.py` & `normflows-1.7.1/normflows/utils/eval.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/utils/masks.py` & `normflows-1.7.1/normflows/utils/masks.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/utils/nn.py` & `normflows-1.7.1/normflows/utils/nn.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/utils/optim.py` & `normflows-1.7.1/normflows/utils/optim.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/utils/preprocessing.py` & `normflows-1.7.1/normflows/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/utils/splines.py` & `normflows-1.7.1/normflows/utils/splines.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows/utils/splines_test.py` & `normflows-1.7.1/normflows/utils/splines_test.py`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/normflows.egg-info/PKG-INFO` & `normflows-1.7.1/normflows.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: normflows
-Version: 1.7.0
+Version: 1.7.1
 Summary: Pytorch implementation of normalizing flows
 Home-page: https://github.com/VincentStimper/normalizing-flows
 Author: Vincent Stimper
 Author-email: vincent.stimper@tuebingen.mpg.de
 License: MIT
 Download-URL: https://github.com/VincentStimper/normalizing-flows/archive/refs/heads/master.zip
 Platform: UNKNOWN
@@ -16,25 +16,25 @@
 License-File: LICENSE
 
 # `normflows`: A PyTorch Package for Normalizing Flows
 
 [![documentation](https://github.com/VincentStimper/normalizing-flows/actions/workflows/mkdocs.yaml/badge.svg)](https://vincentstimper.github.io/normalizing-flows/)
 ![unit-tests](https://github.com/VincentStimper/normalizing-flows/actions/workflows/pytest.yaml/badge.svg)
 ![code coverage](https://raw.githubusercontent.com/VincentStimper/normalizing-flows/coverage-badge/coverage.svg?raw=true)
-[![License: MIT](https://img.shields.io/badge/Licence-MIT-lightgrey)](https://opensource.org/licenses/MIT)
-[![arXiv](https://img.shields.io/badge/arXiv-2302.12014-b31b1b.svg)](https://arxiv.org/abs/2302.12014) 
-[![PyPI](https://img.shields.io/badge/PyPI-1.7.0-blue.svg)](https://pypi.org/project/normflows/)
+[![License: MIT](https://img.shields.io/badge/Licence-MIT-b31b1b.svg)](https://opensource.org/licenses/MIT)
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.05361/status.svg)](https://doi.org/10.21105/joss.05361)
+[![PyPI](https://img.shields.io/badge/PyPI-1.7.1-blue.svg)](https://pypi.org/project/normflows/)
 [![Downloads](https://static.pepy.tech/personalized-badge/normflows?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/normflows)
 
 
 `normflows` is a PyTorch implementation of discrete normalizing flows. Many popular flow architectures are implemented,
 see the [list below](#implemented-flows). The package can be easily [installed via pip](#installation).
 The basic usage is described [here](#usage), and a [full documentation](https://vincentstimper.github.io/normalizing-flows/) 
-is available as well. A more detailed description of this package is given in out accompanying 
-[paper](https://arxiv.org/abs/2302.12014).
+is available as well. A more detailed description of this package is given in our
+[accompanying paper](https://joss.theoj.org/papers/10.21105/joss.05361).
 
 Several sample use cases are provided in the 
 [`examples` folder](https://github.com/VincentStimper/normalizing-flows/blob/master/examples), 
 including [Glow](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/glow.ipynb),
 a [VAE](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/vae.py), and
 a [Residual Flow](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/residual.ipynb).
 Moreover, two simple applications are highlighed in the [examples section](#examples). You can run them 
@@ -188,15 +188,15 @@
 
 In [another example](https://github.com/VincentStimper/normalizing-flows/blob/master/examples/paper_example_nsf_colab.ipynb),
 which is available in [Colab](https://colab.research.google.com/github/VincentStimper/normalizing-flows/blob/master/examples/paper_example_nsf_colab.ipynb)
 as well, we apply a Neural Spline Flow model to a distribution defined on a cylinder. The resulting density is visualized below.
 
 ![Neural Spline Flow applied to target distribution on a cylinder](https://raw.githubusercontent.com/VincentStimper/normalizing-flows/master/figures/nsf_cylinder_3d.png)
 
-This example is considered in the [paper](https://arxiv.org/abs/2302.12014) accompanying this repository.
+This example is considered in the [paper](https://joss.theoj.org/papers/10.21105/joss.05361) accompanying this repository.
 
 ## Support
 
 If you have problems, please read the [package documentation](https://vincentstimper.github.io/normalizing-flows/)
 and check out the [examples section](#examples) above. You are also welcome to 
 [create issues on GitHub](https://github.com/VincentStimper/normalizing-flows/issues) to get help. Note that it is
 worthwhile browsing the existing [open](https://github.com/VincentStimper/normalizing-flows/issues?q=is%3Aopen+is%3Aissue) 
@@ -241,28 +241,35 @@
 > [Code available on GitHub.](https://github.com/lollcat/fab-torch)
 
 Moreover, the [`boltzgen`](https://github.com/VincentStimper/boltzmann-generators) package
 has been build upon `normflows`.
 
 ## Citation
 
-If you use `normflows`, please consider citing the [corresponding paper](https://arxiv.org/abs/2302.12014) as follows.
+If you use `normflows`, please cite the 
+[corresponding paper](https://joss.theoj.org/papers/10.21105/joss.05361) as follows.
 
-> Vincent Stimper, David Liu, Andrew Campbell, Vincent Berenz, Lukas Ryll, Bernhard Schölkopf, José Miguel Hernández-Lobato.
-> normflows: A PyTorch Package for Normalizing Flows, arXiv preprint arXiv:2302.12014, 2023.
+> Stimper et al., (2023). normflows: A PyTorch Package for Normalizing Flows. 
+> Journal of Open Source Software, 8(86), 5361, https://doi.org/10.21105/joss.05361
 
 **Bibtex**
 
 ```
-@article{normflows,
-  author = {Vincent Stimper and David Liu and Andrew Campbell and Vincent Berenz and Lukas Ryll and Bernhard Sch{\"o}lkopf and Jos{\'e} Miguel Hern{\'a}ndez-Lobato},
-  title = {normflows: {A} {P}y{T}orch {P}ackage for {N}ormalizing {F}lows},
-  journal = {arXiv preprint arXiv:2302.12014},
+@article{Stimper2023, 
+  author = {Vincent Stimper and David Liu and Andrew Campbell and Vincent Berenz and Lukas Ryll and Bernhard Schölkopf and José Miguel Hernández-Lobato}, 
+  title = {normflows: A PyTorch Package for Normalizing Flows}, 
+  journal = {Journal of Open Source Software}, 
+  volume = {8},
+  number = {86}, 
+  pages = {5361}, 
+  publisher = {The Open Journal}, 
+  doi = {10.21105/joss.05361}, 
+  url = {https://doi.org/10.21105/joss.05361}, 
   year = {2023}
-}
+} 
 ```
```

#### html2text {}

```diff
@@ -1,54 +1,54 @@
-Metadata-Version: 2.1 Name: normflows Version: 1.7.0 Summary: Pytorch
+Metadata-Version: 2.1 Name: normflows Version: 1.7.1 Summary: Pytorch
 implementation of normalizing flows Home-page: https://github.com/
 VincentStimper/normalizing-flows Author: Vincent Stimper Author-email:
 vincent.stimper@tuebingen.mpg.de License: MIT Download-URL: https://github.com/
 VincentStimper/normalizing-flows/archive/refs/heads/master.zip Platform:
 UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown Provides-Extra: docs License-File:
 LICENSE # `normflows`: A PyTorch Package for Normalizing Flows [!
 [documentation](https://github.com/VincentStimper/normalizing-flows/actions/
 workflows/mkdocs.yaml/badge.svg)](https://vincentstimper.github.io/normalizing-
 flows/) ![unit-tests](https://github.com/VincentStimper/normalizing-flows/
 actions/workflows/pytest.yaml/badge.svg) ![code coverage](https://
 raw.githubusercontent.com/VincentStimper/normalizing-flows/coverage-badge/
 coverage.svg?raw=true) [![License: MIT](https://img.shields.io/badge/Licence-
-MIT-lightgrey)](https://opensource.org/licenses/MIT) [![arXiv](https://
-img.shields.io/badge/arXiv-2302.12014-b31b1b.svg)](https://arxiv.org/abs/
-2302.12014) [![PyPI](https://img.shields.io/badge/PyPI-1.7.0-blue.svg)](https:/
-/pypi.org/project/normflows/) [![Downloads](https://static.pepy.tech/
-personalized-badge/
+MIT-b31b1b.svg)](https://opensource.org/licenses/MIT) [![DOI](https://
+joss.theoj.org/papers/10.21105/joss.05361/status.svg)](https://doi.org/
+10.21105/joss.05361) [![PyPI](https://img.shields.io/badge/PyPI-1.7.1-
+blue.svg)](https://pypi.org/project/normflows/) [![Downloads](https://
+static.pepy.tech/personalized-badge/
 normflows?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)]
 (https://pepy.tech/project/normflows) `normflows` is a PyTorch implementation
 of discrete normalizing flows. Many popular flow architectures are implemented,
 see the [list below](#implemented-flows). The package can be easily [installed
 via pip](#installation). The basic usage is described [here](#usage), and a
 [full documentation](https://vincentstimper.github.io/normalizing-flows/) is
-available as well. A more detailed description of this package is given in out
-accompanying [paper](https://arxiv.org/abs/2302.12014). Several sample use
-cases are provided in the [`examples` folder](https://github.com/
-VincentStimper/normalizing-flows/blob/master/examples), including [Glow](https:
-//github.com/VincentStimper/normalizing-flows/blob/master/examples/glow.ipynb),
-a [VAE](https://github.com/VincentStimper/normalizing-flows/blob/master/
-examples/vae.py), and a [Residual Flow](https://github.com/VincentStimper/
-normalizing-flows/blob/master/examples/residual.ipynb). Moreover, two simple
-applications are highlighed in the [examples section](#examples). You can run
-them yourself in Google Colab using the links below to get a feeling for
-`normflows`. | Link | Description | |------------------------------------------
+available as well. A more detailed description of this package is given in our
+[accompanying paper](https://joss.theoj.org/papers/10.21105/joss.05361).
+Several sample use cases are provided in the [`examples` folder](https://
+github.com/VincentStimper/normalizing-flows/blob/master/examples), including
+[Glow](https://github.com/VincentStimper/normalizing-flows/blob/master/
+examples/glow.ipynb), a [VAE](https://github.com/VincentStimper/normalizing-
+flows/blob/master/examples/vae.py), and a [Residual Flow](https://github.com/
+VincentStimper/normalizing-flows/blob/master/examples/residual.ipynb).
+Moreover, two simple applications are highlighed in the [examples section]
+(#examples). You can run them yourself in Google Colab using the links below to
+get a feeling for `normflows`. | Link | Description | |------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
------------------------------------------------|-------------------------------
-------------------------------------------| | [Open_In_Colab] | Real NVP
-applied to a 2D bimodal target distribution | | [Open_In_Colab] | Modeling a
-distribution on a cylinder surface with a neural spline flow | | [Open_In
-Colab] | Modeling and generating CIFAR-10 images with Glow | ## Implemented
-Flows | Architecture | Reference | |--------------|----------------------------
+-----------------------------------------------------------------|-------------
+------------------------------------------------------------| | [Open_In_Colab]
+| Real NVP applied to a 2D bimodal target distribution | | [Open_In_Colab] |
+Modeling a distribution on a cylinder surface with a neural spline flow | |
+[Open_In_Colab] | Modeling and generating CIFAR-10 images with Glow | ##
+Implemented Flows | Architecture | Reference | |--------------|----------------
 -------------------------------------------------------------------------------
-----------------| | Planar Flow | [Rezende & Mohamed, 2015](http://
+----------------------------| | Planar Flow | [Rezende & Mohamed, 2015](http://
 proceedings.mlr.press/v37/rezende15.html) | | Radial Flow | [Rezende & Mohamed,
 2015](http://proceedings.mlr.press/v37/rezende15.html) | | NICE | [Dinh et al.,
 2014](https://arxiv.org/abs/1410.8516) | | Real NVP | [Dinh et al., 2017]
 (https://openreview.net/forum?id=HkpbnH9lx) | | Glow | [Kingma et al., 2018]
 (https://proceedings.neurips.cc/paper/2018/hash/
 d139db6a236200b21cc7f752979132d0-Abstract.html) | | Masked Autoregressive Flow
 | [Papamakarios et al., 2017](https://proceedings.neurips.cc/paper/2017/hash/
@@ -127,54 +127,55 @@
 master/examples/paper_example_nsf_colab.ipynb), which is available in [Colab]
 (https://colab.research.google.com/github/VincentStimper/normalizing-flows/
 blob/master/examples/paper_example_nsf_colab.ipynb) as well, we apply a Neural
 Spline Flow model to a distribution defined on a cylinder. The resulting
 density is visualized below. ![Neural Spline Flow applied to target
 distribution on a cylinder](https://raw.githubusercontent.com/VincentStimper/
 normalizing-flows/master/figures/nsf_cylinder_3d.png) This example is
-considered in the [paper](https://arxiv.org/abs/2302.12014) accompanying this
-repository. ## Support If you have problems, please read the [package
-documentation](https://vincentstimper.github.io/normalizing-flows/) and check
-out the [examples section](#examples) above. You are also welcome to [create
-issues on GitHub](https://github.com/VincentStimper/normalizing-flows/issues)
-to get help. Note that it is worthwhile browsing the existing [open](https://
-github.com/VincentStimper/normalizing-flows/issues?q=is%3Aopen+is%3Aissue) and
-[closed](https://github.com/VincentStimper/normalizing-flows/
-issues?q=is%3Aissue+is%3Aclosed) issues, which might address the problem you
-are facing. ## Contributing If you find a bug or have a feature request, please
-[file an issue on GitHub](https://github.com/VincentStimper/normalizing-flows/
-issues). You are welcome to contribute to the package by fixing the bug or
-adding the feature yourself. If you want to contribute, please add tests for
-the code you added or modified and ensure it passes successfully by running
-`pytest`. This can be done by simply executing ``` pytest ``` within your local
-version of the repository. Make sure you code is well documented, and we also
-encourage contributions to the existing documentation. Once you finished coding
-and testing, please [create a pull request on GitHub](https://docs.github.com/
-en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-
-work-with-pull-requests/creating-a-pull-request). ## Used by The package has
-been used in several research papers, which are listed below. > Andrew
-Campbell, Wenlong Chen, Vincent Stimper, JosÃ© Miguel HernÃ¡ndez-Lobato, and
-Yichuan Zhang. > [A gradient based strategy for Hamiltonian Monte Carlo
-hyperparameter optimization](https://proceedings.mlr.press/v139/
-campbell21a.html). > In Proceedings of the 38th International Conference on
-Machine Learning, pp. 1238â1248. PMLR, 2021. > > [Code available on GitHub.]
-(https://github.com/VincentStimper/hmc-hyperparameter-tuning) > Vincent
-Stimper, Bernhard SchÃ¶lkopf, JosÃ© Miguel HernÃ¡ndez-Lobato. > [Resampling
-Base Distributions of Normalizing Flows](https://proceedings.mlr.press/v151/
-stimper22a). > In Proceedings of The 25th International Conference on
-Artificial Intelligence and Statistics, volume 151, pp. 4915â4936, 2022. > >
-[Code available on GitHub.](https://github.com/VincentStimper/resampled-base-
-flows) > Laurence I. Midgley, Vincent Stimper, Gregor N. C. Simm, Bernhard
-SchÃ¶lkopf, JosÃ© Miguel HernÃ¡ndez-Lobato. > [Flow Annealed Importance
-Sampling Bootstrap](https://arxiv.org/abs/2208.01893). > arXiv preprint arXiv:
-2208.01893, 2022. > > [Code available on GitHub.](https://github.com/lollcat/
-fab-torch) Moreover, the [`boltzgen`](https://github.com/VincentStimper/
-boltzmann-generators) package has been build upon `normflows`. ## Citation If
-you use `normflows`, please consider citing the [corresponding paper](https://
-arxiv.org/abs/2302.12014) as follows. > Vincent Stimper, David Liu, Andrew
-Campbell, Vincent Berenz, Lukas Ryll, Bernhard SchÃ¶lkopf, JosÃ© Miguel
-HernÃ¡ndez-Lobato. > normflows: A PyTorch Package for Normalizing Flows, arXiv
-preprint arXiv:2302.12014, 2023. **Bibtex** ``` @article{normflows, author =
-{Vincent Stimper and David Liu and Andrew Campbell and Vincent Berenz and Lukas
-Ryll and Bernhard Sch{\"o}lkopf and Jos{\'e} Miguel Hern{\'a}ndez-Lobato},
-title = {normflows: {A} {P}y{T}orch {P}ackage for {N}ormalizing {F}lows},
-journal = {arXiv preprint arXiv:2302.12014}, year = {2023} } ```
+considered in the [paper](https://joss.theoj.org/papers/10.21105/joss.05361)
+accompanying this repository. ## Support If you have problems, please read the
+[package documentation](https://vincentstimper.github.io/normalizing-flows/
+) and check out the [examples section](#examples) above. You are also welcome
+to [create issues on GitHub](https://github.com/VincentStimper/normalizing-
+flows/issues) to get help. Note that it is worthwhile browsing the existing
+[open](https://github.com/VincentStimper/normalizing-flows/
+issues?q=is%3Aopen+is%3Aissue) and [closed](https://github.com/VincentStimper/
+normalizing-flows/issues?q=is%3Aissue+is%3Aclosed) issues, which might address
+the problem you are facing. ## Contributing If you find a bug or have a feature
+request, please [file an issue on GitHub](https://github.com/VincentStimper/
+normalizing-flows/issues). You are welcome to contribute to the package by
+fixing the bug or adding the feature yourself. If you want to contribute,
+please add tests for the code you added or modified and ensure it passes
+successfully by running `pytest`. This can be done by simply executing ```
+pytest ``` within your local version of the repository. Make sure you code is
+well documented, and we also encourage contributions to the existing
+documentation. Once you finished coding and testing, please [create a pull
+request on GitHub](https://docs.github.com/en/pull-requests/collaborating-with-
+pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-
+pull-request). ## Used by The package has been used in several research papers,
+which are listed below. > Andrew Campbell, Wenlong Chen, Vincent Stimper, JosÃ©
+Miguel HernÃ¡ndez-Lobato, and Yichuan Zhang. > [A gradient based strategy for
+Hamiltonian Monte Carlo hyperparameter optimization](https://
+proceedings.mlr.press/v139/campbell21a.html). > In Proceedings of the 38th
+International Conference on Machine Learning, pp. 1238â1248. PMLR, 2021. > >
+[Code available on GitHub.](https://github.com/VincentStimper/hmc-
+hyperparameter-tuning) > Vincent Stimper, Bernhard SchÃ¶lkopf, JosÃ© Miguel
+HernÃ¡ndez-Lobato. > [Resampling Base Distributions of Normalizing Flows]
+(https://proceedings.mlr.press/v151/stimper22a). > In Proceedings of The 25th
+International Conference on Artificial Intelligence and Statistics, volume 151,
+pp. 4915â4936, 2022. > > [Code available on GitHub.](https://github.com/
+VincentStimper/resampled-base-flows) > Laurence I. Midgley, Vincent Stimper,
+Gregor N. C. Simm, Bernhard SchÃ¶lkopf, JosÃ© Miguel HernÃ¡ndez-Lobato. > [Flow
+Annealed Importance Sampling Bootstrap](https://arxiv.org/abs/2208.01893). >
+arXiv preprint arXiv:2208.01893, 2022. > > [Code available on GitHub.](https://
+github.com/lollcat/fab-torch) Moreover, the [`boltzgen`](https://github.com/
+VincentStimper/boltzmann-generators) package has been build upon `normflows`.
+## Citation If you use `normflows`, please cite the [corresponding paper]
+(https://joss.theoj.org/papers/10.21105/joss.05361) as follows. > Stimper et
+al., (2023). normflows: A PyTorch Package for Normalizing Flows. > Journal of
+Open Source Software, 8(86), 5361, https://doi.org/10.21105/joss.05361
+**Bibtex** ``` @article{Stimper2023, author = {Vincent Stimper and David Liu
+and Andrew Campbell and Vincent Berenz and Lukas Ryll and Bernhard SchÃ¶lkopf
+and JosÃ© Miguel HernÃ¡ndez-Lobato}, title = {normflows: A PyTorch Package for
+Normalizing Flows}, journal = {Journal of Open Source Software}, volume = {8},
+number = {86}, pages = {5361}, publisher = {The Open Journal}, doi = {10.21105/
+joss.05361}, url = {https://doi.org/10.21105/joss.05361}, year = {2023} } ```
```

### Comparing `normflows-1.7.0/normflows.egg-info/SOURCES.txt` & `normflows-1.7.1/normflows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `normflows-1.7.0/setup.py` & `normflows-1.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
-__version__ = "1.7.0"
+__version__ = "1.7.1"
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
```

