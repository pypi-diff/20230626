# Comparing `tmp/cca_zoo-2.0.5.tar.gz` & `tmp/cca_zoo-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cca_zoo-2.0.5.tar", last modified: Thu Jun 22 16:16:00 2023, max compression
+gzip compressed data, was "dist/cca_zoo-2.0.6.tar", last modified: Mon Jun 26 11:32:50 2023, max compression
```

## Comparing `cca_zoo-2.0.5.tar` & `cca_zoo-2.0.6.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:16:00.000000 cca_zoo-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-22 16:16:00.000000 cca_zoo-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:16:00.000000 cca_zoo-2.0.5/cca_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:16:00.000000 cca_zoo-2.0.5/cca_zoo/classical/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_gcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_grcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:16:00.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/_altmaxvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/_deflation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/_elasticnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/_ey.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/_gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/_gradkcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/_incrementalpls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/_pls_als.py
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/_pmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/_scca_admm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/_scca_hsic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/_scca_parkhomenko.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/_scca_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/_stochasticpls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_iterative/_swcca.py
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_kcca.py
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_mcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_ncca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_partialcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_pcacca.py
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_pls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_prcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/classical/_tcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:16:00.000000 cca_zoo-2.0.5/cca_zoo/data/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/data/deep.py
--rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/data/simulated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:16:00.000000 cca_zoo-2.0.5/cca_zoo/deep/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:16:00.000000 cca_zoo-2.0.5/cca_zoo/deep/_discriminative/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/_discriminative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/_discriminative/_dcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/_discriminative/_dcca_ey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/_discriminative/_dcca_gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/_discriminative/_dcca_noi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/_discriminative/_dcca_sdl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/_discriminative/_dcca_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/_discriminative/_dgcca.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/_discriminative/_dtcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:16:00.000000 cca_zoo-2.0.5/cca_zoo/deep/_generative/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/_generative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/_generative/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/_generative/_dccae.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/_generative/_dvcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/_generative/_splitae.py
--rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/deep/objectives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:16:00.000000 cca_zoo-2.0.5/cca_zoo/model_selection/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/model_selection/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/model_selection/_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:16:00.000000 cca_zoo-2.0.5/cca_zoo/probabilistic/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/probabilistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/probabilistic/_probabilisticcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:16:00.000000 cca_zoo-2.0.5/cca_zoo/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/test/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/test/test_deepmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/test/test_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/test/test_probabilistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/test/test_regularised.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/test/test_stochastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/test/test_unregularized.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/test/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:16:00.000000 cca_zoo-2.0.5/cca_zoo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/utils/check_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:16:00.000000 cca_zoo-2.0.5/cca_zoo/visualisation/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/cca_zoo/visualisation/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:16:00.000000 cca_zoo-2.0.5/cca_zoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-22 16:15:59.000000 cca_zoo-2.0.5/cca_zoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-22 16:16:00.000000 cca_zoo-2.0.5/cca_zoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:15:59.000000 cca_zoo-2.0.5/cca_zoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-22 16:15:59.000000 cca_zoo-2.0.5/cca_zoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-22 16:15:59.000000 cca_zoo-2.0.5/cca_zoo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:16:00.000000 cca_zoo-2.0.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/examples/plot_dcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/examples/plot_dcca_custom_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/examples/plot_dcca_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/examples/plot_dvcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/examples/plot_hyperparameter_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/examples/plot_kernel_cca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/examples/plot_many_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/examples/plot_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/examples/plot_sparse_cca.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-06-22 16:15:43.000000 cca_zoo-2.0.5/examples/plot_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 16:16:00.000000 cca_zoo-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-22 16:15:58.000000 cca_zoo-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/cca_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/cca_zoo/classical/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_gcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_grcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/_altmaxvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/_deflation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/_elasticnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/_ey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/_gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/_gradkcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/_incrementalpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/_pls_als.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/_pmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/_scca_admm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/_scca_hsic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/_scca_parkhomenko.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/_scca_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/_stochasticpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_iterative/_swcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_kcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_mcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_ncca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_partialcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_pcacca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_pls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_prcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/classical/_tcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/cca_zoo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/data/deep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/data/simulated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/cca_zoo/deep/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/cca_zoo/deep/_discriminative/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/_discriminative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/_discriminative/_dcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/_discriminative/_dcca_ey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/_discriminative/_dcca_gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/_discriminative/_dcca_noi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/_discriminative/_dcca_sdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/_discriminative/_dcca_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/_discriminative/_dgcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/_discriminative/_dtcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/cca_zoo/deep/_generative/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/_generative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/_generative/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/_generative/_dccae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/_generative/_dvcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/_generative/_splitae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/deep/objectives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/cca_zoo/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/model_selection/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/model_selection/_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/cca_zoo/probabilistic/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/probabilistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/probabilistic/_probabilisticcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/cca_zoo/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/test/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/test/test_deepmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/test/test_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/test/test_probabilistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/test/test_regularised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/test/test_stochastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/test/test_unregularized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/cca_zoo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/utils/check_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/cca_zoo/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/cca_zoo/visualisation/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/cca_zoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/cca_zoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/cca_zoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/cca_zoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/cca_zoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/cca_zoo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/examples/plot_dcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/examples/plot_dcca_custom_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/examples/plot_dcca_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/examples/plot_dvcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/examples/plot_hyperparameter_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/examples/plot_kernel_cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/examples/plot_many_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/examples/plot_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/examples/plot_sparse_cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-06-26 11:32:34.000000 cca_zoo-2.0.6/examples/plot_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 11:32:50.000000 cca_zoo-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-26 11:32:49.000000 cca_zoo-2.0.6/setup.py
```

### Comparing `cca_zoo-2.0.5/PKG-INFO` & `cca_zoo-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cca_zoo
-Version: 2.0.5
+Version: 2.0.6
 Summary: Canonical Correlation Analysis Zoo: A collection of Regularized, Deep Learning based, Kernel, and Probabilistic methods in a scikit-learn style framework
 Home-page: https://github.com/jameschapman19/cca_zoo
 Author: jameschapman
 Author-email: james.chapman.19@ucl.ac.uk
 License: MIT
 Description: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5748062.svg)](https://doi.org/10.5281/zenodo.4382739)
         [![codecov](https://codecov.io/gh/jameschapman19/cca_zoo/branch/main/graph/badge.svg?token=JHG9VUB0L8)](https://codecov.io/gh/jameschapman19/cca_zoo)
```

### Comparing `cca_zoo-2.0.5/README.md` & `cca_zoo-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/__init__.py` & `cca_zoo-2.0.6/cca_zoo/classical/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_base.py` & `cca_zoo-2.0.6/cca_zoo/classical/_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_dummy.py` & `cca_zoo-2.0.6/cca_zoo/classical/_dummy.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_gcca.py` & `cca_zoo-2.0.6/cca_zoo/classical/_gcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_grcca.py` & `cca_zoo-2.0.6/cca_zoo/classical/_grcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_iterative/__init__.py` & `cca_zoo-2.0.6/cca_zoo/classical/_iterative/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_iterative/_altmaxvar.py` & `cca_zoo-2.0.6/cca_zoo/classical/_iterative/_altmaxvar.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
             copy_data=copy_data,
             random_state=random_state,
             tol=tol,
             epochs=epochs,
             convergence_checking=convergence_checking,
             track=track,
             verbose=verbose,
+            trainer_kwargs={"accelerator": "cpu"}
         )
         self.tau = tau
         self.proximal = proximal
         self.proximal_params = proximal_params
         self.gamma = gamma
         self.learning_rate = learning_rate
         self.T = T
```

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_iterative/_base.py` & `cca_zoo-2.0.6/cca_zoo/classical/_iterative/_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_iterative/_deflation.py` & `cca_zoo-2.0.6/cca_zoo/classical/_iterative/_deflation.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_iterative/_elasticnet.py` & `cca_zoo-2.0.6/cca_zoo/classical/_iterative/_elasticnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,15 @@
             initialization=initialization,
             tol=tol,
             random_state=random_state,
             convergence_checking=convergence_checking,
             patience=0,
             track=track,
             verbose=verbose,
+            trainer_kwargs={"accelerator": "cpu"}
         )
 
     def _check_params(self):
         self.alpha = _process_parameter("alpha", self.alpha, 0, self.n_views_)
         self.l1_ratio = _process_parameter("l1_ratio", self.l1_ratio, 0, self.n_views_)
         self.positive = _process_parameter(
             "positive", self.positive, False, self.n_views_
```

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_iterative/_ey.py` & `cca_zoo-2.0.6/cca_zoo/classical/_iterative/_ey.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_iterative/_gh.py` & `cca_zoo-2.0.6/cca_zoo/classical/_iterative/_gh.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_iterative/_gradient.py` & `cca_zoo-2.0.6/cca_zoo/classical/_iterative/_gradient.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_iterative/_gradkcca.py` & `cca_zoo-2.0.6/cca_zoo/classical/_iterative/_gradkcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_iterative/_incrementalpls.py` & `cca_zoo-2.0.6/cca_zoo/classical/_iterative/_incrementalpls.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_iterative/_pls_als.py` & `cca_zoo-2.0.6/cca_zoo/classical/_iterative/_pls_als.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,14 @@
         batch_size=None,
         dataloader_kwargs=None,
         epochs=100,
         val_split=None,
         learning_rate=1,
         initialization: Union[str, callable] = "random",
         callbacks=None,
-        trainer_kwargs=None,
     ):
         super().__init__(
             latent_dimensions,
             copy_data,
             random_state,
             tol,
             deflation=deflation,
@@ -71,15 +70,15 @@
             batch_size=batch_size,
             dataloader_kwargs=dataloader_kwargs,
             epochs=epochs,
             val_split=val_split,
             learning_rate=learning_rate,
             initialization=initialization,
             callbacks=callbacks,
-            trainer_kwargs=trainer_kwargs,
+            trainer_kwargs={"accelerator": "cpu"}
         )
 
     def _get_module(self, weights=None, k=None):
         return PlsAlsLoop(
             weights=weights,
             k=k,
         )
```

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_iterative/_pmd.py` & `cca_zoo-2.0.6/cca_zoo/classical/_iterative/_pmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,15 @@
             deflation=deflation,
             initialization=initialization,
             tol=tol,
             convergence_checking=convergence_checking,
             patience=0,
             track=track,
             verbose=verbose,
+            trainer_kwargs={"accelerator": "cpu"}
         )
         self.tau = tau
         self.positive = positive
 
     def _check_params(self):
         if self.tau is None:
             warnings.warn(
@@ -109,36 +110,36 @@
 
     def _get_module(self, weights=None, k=None):
         return PMDLoop(
             weights=weights,
             k=k,
             tau=self.tau,
             tol=self.tol,
-            track=self.track,
+            tracking=self.track,
             convergence_checking=self.convergence_checking,
         )
 
     def _more_tags(self):
         return {"multiview": True}
 
 
 class PMDLoop(BaseLoop):
     def __init__(
         self,
         weights,
         k=None,
         tau=None,
         tol=1e-3,
-        track=False,
+        tracking=False,
         convergence_checking=False,
     ):
         super().__init__(
             weights=weights,
             k=k,
-            tracking=track,
+            tracking=tracking,
             convergence_checking=convergence_checking,
         )
         self.tau = tau
         self.tol = tol
         shape_sqrts = [np.sqrt(weight.shape[0]) for weight in self.weights]
         self.t = [max(1, x * y) for x, y in zip(self.tau, shape_sqrts)]
 
@@ -159,15 +160,15 @@
                 tol=self.tol,
             )
             if np.linalg.norm(self.weights[view_index]) <= 0:
                 warnings.warn(
                     f"All result weights are zero in view {view_index}. "
                     "Try less regularisation or another initialisation"
                 )
-        # if track or convergence_checking is enabled, compute the objective function
+        # if tracking or convergence_checking is enabled, compute the objective function
         if self.tracking or self.convergence_checking:
             objective = self.objective(batch["views"])
             # check that the maximum change in weights is smaller than the tolerance times the maximum absolute value of the weights
             weights_change = torch.tensor(
                 np.max(
                     [
                         np.max(np.abs(old_weights[i] - self.weights[i]))
```

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_iterative/_scca_admm.py` & `cca_zoo-2.0.6/cca_zoo/classical/_iterative/_scca_admm.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_iterative/_scca_hsic.py` & `cca_zoo-2.0.6/cca_zoo/classical/_iterative/_scca_hsic.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_iterative/_scca_parkhomenko.py` & `cca_zoo-2.0.6/cca_zoo/classical/_iterative/_scca_parkhomenko.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
             tol=tol,
             random_state=random_state,
             deflation=deflation,
             convergence_checking=convergence_checking,
             patience=patience,
             track=track,
             verbose=verbose,
+            trainer_kwargs={"accelerator": "cpu"}
         )
 
     def _check_params(self):
         self.tau = _process_parameter("tau", self.tau, 0.0001, self.n_views_)
         if any(tau <= 0 for tau in self.tau):
             raise (
                 "All regularisation parameters should be above 0. " f"tau=[{self.tau}]"
```

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_iterative/_scca_span.py` & `cca_zoo-2.0.6/cca_zoo/classical/_iterative/_scca_span.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
             epochs=epochs,
             copy_data=copy_data,
             initialization=initialization,
             tol=tol,
             random_state=random_state,
             deflation=deflation,
             verbose=verbose,
+            trainer_kwargs={"accelerator": "cpu"}
         )
         self.tau = tau
         self.regularisation = regularisation
         self.rank = rank
         self.positive = positive
 
     def _check_params(self):
```

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_iterative/_stochasticpls.py` & `cca_zoo-2.0.6/cca_zoo/classical/_iterative/_stochasticpls.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_iterative/_svd.py` & `cca_zoo-2.0.6/cca_zoo/classical/_iterative/_svd.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_iterative/_swcca.py` & `cca_zoo-2.0.6/cca_zoo/classical/_iterative/_swcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_kcca.py` & `cca_zoo-2.0.6/cca_zoo/classical/_kcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_mcca.py` & `cca_zoo-2.0.6/cca_zoo/classical/_mcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_ncca.py` & `cca_zoo-2.0.6/cca_zoo/classical/_ncca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_partialcca.py` & `cca_zoo-2.0.6/cca_zoo/classical/_partialcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_pcacca.py` & `cca_zoo-2.0.6/cca_zoo/classical/_pcacca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_pls.py` & `cca_zoo-2.0.6/cca_zoo/classical/_pls.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_prcca.py` & `cca_zoo-2.0.6/cca_zoo/classical/_prcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_search.py` & `cca_zoo-2.0.6/cca_zoo/classical/_search.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/classical/_tcca.py` & `cca_zoo-2.0.6/cca_zoo/classical/_tcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/data/deep.py` & `cca_zoo-2.0.6/cca_zoo/data/deep.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/data/simulated.py` & `cca_zoo-2.0.6/cca_zoo/data/simulated.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/deep/__init__.py` & `cca_zoo-2.0.6/cca_zoo/deep/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/deep/_base.py` & `cca_zoo-2.0.6/cca_zoo/deep/_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/deep/_discriminative/_dcca.py` & `cca_zoo-2.0.6/cca_zoo/deep/_discriminative/_dcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py` & `cca_zoo-2.0.6/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/deep/_discriminative/_dcca_ey.py` & `cca_zoo-2.0.6/cca_zoo/deep/_discriminative/_dcca_ey.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/deep/_discriminative/_dcca_gh.py` & `cca_zoo-2.0.6/cca_zoo/deep/_discriminative/_dcca_gh.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/deep/_discriminative/_dcca_noi.py` & `cca_zoo-2.0.6/cca_zoo/deep/_discriminative/_dcca_noi.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/deep/_discriminative/_dcca_sdl.py` & `cca_zoo-2.0.6/cca_zoo/deep/_discriminative/_dcca_sdl.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/deep/_discriminative/_dcca_svd.py` & `cca_zoo-2.0.6/cca_zoo/deep/_discriminative/_dcca_svd.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/deep/_discriminative/_dgcca.py` & `cca_zoo-2.0.6/cca_zoo/deep/_discriminative/_dgcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/deep/_discriminative/_dtcca.py` & `cca_zoo-2.0.6/cca_zoo/deep/_discriminative/_dtcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/deep/_generative/_base.py` & `cca_zoo-2.0.6/cca_zoo/deep/_generative/_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/deep/_generative/_dccae.py` & `cca_zoo-2.0.6/cca_zoo/deep/_generative/_dccae.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/deep/_generative/_dvcca.py` & `cca_zoo-2.0.6/cca_zoo/deep/_generative/_dvcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/deep/_generative/_splitae.py` & `cca_zoo-2.0.6/cca_zoo/deep/_generative/_splitae.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/deep/architectures.py` & `cca_zoo-2.0.6/cca_zoo/deep/architectures.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/deep/metrics.py` & `cca_zoo-2.0.6/cca_zoo/deep/metrics.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/deep/objectives.py` & `cca_zoo-2.0.6/cca_zoo/deep/objectives.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/model_selection/_search.py` & `cca_zoo-2.0.6/cca_zoo/model_selection/_search.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/model_selection/_validation.py` & `cca_zoo-2.0.6/cca_zoo/model_selection/_validation.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/probabilistic/_probabilisticcca.py` & `cca_zoo-2.0.6/cca_zoo/probabilistic/_probabilisticcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/test/test_callbacks.py` & `cca_zoo-2.0.6/cca_zoo/test/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/test/test_data.py` & `cca_zoo-2.0.6/cca_zoo/test/test_data.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/test/test_deepmodels.py` & `cca_zoo-2.0.6/cca_zoo/test/test_deepmodels.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/test/test_kernel.py` & `cca_zoo-2.0.6/cca_zoo/test/test_kernel.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/test/test_probabilistic.py` & `cca_zoo-2.0.6/cca_zoo/test/test_probabilistic.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/test/test_regularised.py` & `cca_zoo-2.0.6/cca_zoo/test/test_regularised.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/test/test_stochastic.py` & `cca_zoo-2.0.6/cca_zoo/test/test_stochastic.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/test/test_unregularized.py` & `cca_zoo-2.0.6/cca_zoo/test/test_unregularized.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/test/test_utils.py` & `cca_zoo-2.0.6/cca_zoo/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/utils/check_values.py` & `cca_zoo-2.0.6/cca_zoo/utils/check_values.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo/visualisation/plotting.py` & `cca_zoo-2.0.6/cca_zoo/visualisation/plotting.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/cca_zoo.egg-info/PKG-INFO` & `cca_zoo-2.0.6/cca_zoo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cca-zoo
-Version: 2.0.5
+Version: 2.0.6
 Summary: Canonical Correlation Analysis Zoo: A collection of Regularized, Deep Learning based, Kernel, and Probabilistic methods in a scikit-learn style framework
 Home-page: https://github.com/jameschapman19/cca_zoo
 Author: jameschapman
 Author-email: james.chapman.19@ucl.ac.uk
 License: MIT
 Description: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5748062.svg)](https://doi.org/10.5281/zenodo.4382739)
         [![codecov](https://codecov.io/gh/jameschapman19/cca_zoo/branch/main/graph/badge.svg?token=JHG9VUB0L8)](https://codecov.io/gh/jameschapman19/cca_zoo)
```

### Comparing `cca_zoo-2.0.5/cca_zoo.egg-info/SOURCES.txt` & `cca_zoo-2.0.6/cca_zoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/examples/__init__.py` & `cca_zoo-2.0.6/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/examples/plot_dcca.py` & `cca_zoo-2.0.6/examples/plot_dcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/examples/plot_dcca_custom_data.py` & `cca_zoo-2.0.6/examples/plot_dcca_custom_data.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/examples/plot_dcca_multi.py` & `cca_zoo-2.0.6/examples/plot_dcca_multi.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/examples/plot_dvcca.py` & `cca_zoo-2.0.6/examples/plot_dvcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/examples/plot_hyperparameter_selection.py` & `cca_zoo-2.0.6/examples/plot_hyperparameter_selection.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/examples/plot_kernel_cca.py` & `cca_zoo-2.0.6/examples/plot_kernel_cca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/examples/plot_many_views.py` & `cca_zoo-2.0.6/examples/plot_many_views.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/examples/plot_plotting.py` & `cca_zoo-2.0.6/examples/plot_plotting.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/examples/plot_sparse_cca.py` & `cca_zoo-2.0.6/examples/plot_sparse_cca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/examples/plot_validation.py` & `cca_zoo-2.0.6/examples/plot_validation.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.5/setup.py` & `cca_zoo-2.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "deep": ["torch", "torchvision", "pytorch-lightning"],
     "probabilistic": ["jax", "numpyro", "arviz"],
 }
 EXTRA_PACKAGES["all"] = EXTRA_PACKAGES["deep"] + EXTRA_PACKAGES["probabilistic"]
 
 setup(
     name="cca_zoo",
-    version="2.0.5",
+    version="2.0.6",
     include_package_data=True,
     keywords="cca",
     packages=find_packages(),
     url="https://github.com/jameschapman19/cca_zoo",
     license="MIT",
     author="jameschapman",
     description=(
```

