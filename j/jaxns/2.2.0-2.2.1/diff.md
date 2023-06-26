# Comparing `tmp/jaxns-2.2.0.tar.gz` & `tmp/jaxns-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxns-2.2.0.tar", last modified: Thu Jun 15 14:57:59 2023, max compression
+gzip compressed data, was "jaxns-2.2.1.tar", last modified: Mon Jun 26 12:50:15 2023, max compression
```

## Comparing `jaxns-2.2.0.tar` & `jaxns-2.2.1.tar`

### file list

```diff
@@ -1,61 +1,64 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 14:57:59.366724 jaxns-2.2.0/
--rw-rw-r--   0 albert    (1000) albert    (1000)    20138 2022-10-13 02:52:05.000000 jaxns-2.2.0/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)     4810 2023-06-15 14:57:59.366724 jaxns-2.2.0/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     4371 2023-06-15 14:34:45.000000 jaxns-2.2.0/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 14:57:59.362723 jaxns-2.2.0/jaxns/
--rw-rw-r--   0 albert    (1000) albert    (1000)      386 2023-04-20 22:44:04.000000 jaxns-2.2.0/jaxns/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    13247 2023-05-18 21:09:50.000000 jaxns-2.2.0/jaxns/adaptive_refinement.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     6940 2023-04-21 01:26:04.000000 jaxns-2.2.0/jaxns/initial_state.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 14:57:59.362723 jaxns-2.2.0/jaxns/internals/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.2.0/jaxns/internals/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      849 2023-01-03 05:33:37.000000 jaxns-2.2.0/jaxns/internals/linalg.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    12651 2023-06-15 13:49:53.000000 jaxns-2.2.0/jaxns/internals/log_semiring.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     4919 2023-04-21 14:08:43.000000 jaxns-2.2.0/jaxns/internals/maps.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1899 2022-10-13 02:52:05.000000 jaxns-2.2.0/jaxns/internals/shapes.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1853 2023-01-03 05:33:37.000000 jaxns-2.2.0/jaxns/internals/stats.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 14:57:59.362723 jaxns-2.2.0/jaxns/internals/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.2.0/jaxns/internals/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      277 2023-01-03 05:33:37.000000 jaxns-2.2.0/jaxns/internals/tests/test_linalg.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5490 2023-01-03 05:33:37.000000 jaxns-2.2.0/jaxns/internals/tests/test_log_semiring.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2898 2023-06-14 16:43:12.000000 jaxns-2.2.0/jaxns/internals/tests/test_maps.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1110 2022-12-29 07:48:31.000000 jaxns-2.2.0/jaxns/internals/tests/test_shapes.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1186 2023-01-03 05:33:37.000000 jaxns-2.2.0/jaxns/internals/tests/test_stats.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 14:57:59.362723 jaxns-2.2.0/jaxns/likelihood_samplers/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.2.0/jaxns/likelihood_samplers/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3269 2023-06-15 13:57:48.000000 jaxns-2.2.0/jaxns/likelihood_samplers/em_gmm.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    20604 2023-06-15 10:22:16.000000 jaxns-2.2.0/jaxns/likelihood_samplers/multi_ellipsoid_utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 14:57:59.362723 jaxns-2.2.0/jaxns/likelihood_samplers/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.2.0/jaxns/likelihood_samplers/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1304 2023-06-14 20:46:20.000000 jaxns-2.2.0/jaxns/likelihood_samplers/tests/test_em_gmm.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     4836 2023-06-14 21:03:21.000000 jaxns-2.2.0/jaxns/likelihood_samplers/tests/test_multi_ellipsoid.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3103 2023-05-18 20:19:33.000000 jaxns-2.2.0/jaxns/model.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    18103 2023-06-15 13:59:36.000000 jaxns-2.2.0/jaxns/nested_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    16040 2023-01-03 05:33:37.000000 jaxns-2.2.0/jaxns/plotting.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    12554 2023-06-14 10:16:12.000000 jaxns-2.2.0/jaxns/prior.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2787 2023-04-20 15:27:03.000000 jaxns-2.2.0/jaxns/random.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    10153 2023-05-18 20:55:58.000000 jaxns-2.2.0/jaxns/special_priors.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    16184 2023-05-15 09:26:33.000000 jaxns-2.2.0/jaxns/static_nested_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    26201 2023-04-25 10:29:16.000000 jaxns-2.2.0/jaxns/static_slice.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5072 2023-05-12 12:36:05.000000 jaxns-2.2.0/jaxns/static_uniform.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    16841 2023-06-15 13:57:48.000000 jaxns-2.2.0/jaxns/statistics.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     6607 2023-05-12 13:17:17.000000 jaxns-2.2.0/jaxns/termination.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 14:57:59.362723 jaxns-2.2.0/jaxns/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-01-03 05:33:37.000000 jaxns-2.2.0/jaxns/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2821 2023-06-15 14:57:56.000000 jaxns-2.2.0/jaxns/tests/test_adaptive_refinement.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3882 2023-06-15 10:22:16.000000 jaxns-2.2.0/jaxns/tests/test_initial_state.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    16392 2023-05-15 05:52:12.000000 jaxns-2.2.0/jaxns/tests/test_nested_sampler.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     9019 2023-05-18 20:50:55.000000 jaxns-2.2.0/jaxns/tests/test_prior.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     1306 2023-04-15 16:37:14.000000 jaxns-2.2.0/jaxns/tests/test_random.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    24209 2023-06-15 13:59:36.000000 jaxns-2.2.0/jaxns/tests/test_statistics.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      477 2023-01-03 05:33:37.000000 jaxns-2.2.0/jaxns/tests/test_utils.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5118 2023-05-12 12:43:32.000000 jaxns-2.2.0/jaxns/types.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    17668 2023-05-15 05:41:18.000000 jaxns-2.2.0/jaxns/utils.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      716 2023-05-07 18:38:45.000000 jaxns-2.2.0/jaxns/warnings.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-15 14:57:59.362723 jaxns-2.2.0/jaxns.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     4810 2023-06-15 14:57:59.000000 jaxns-2.2.0/jaxns.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     1497 2023-06-15 14:57:59.000000 jaxns-2.2.0/jaxns.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-06-15 14:57:59.000000 jaxns-2.2.0/jaxns.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        6 2023-06-15 14:57:59.000000 jaxns-2.2.0/jaxns.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)      103 2022-10-13 02:52:05.000000 jaxns-2.2.0/pyproject.toml
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-06-15 14:57:59.366724 jaxns-2.2.0/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)      949 2023-06-15 14:09:56.000000 jaxns-2.2.0/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-26 12:50:15.359704 jaxns-2.2.1/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2553 2023-06-19 23:43:03.000000 jaxns-2.2.1/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4810 2023-06-26 12:50:15.359704 jaxns-2.2.1/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4371 2023-06-15 14:34:45.000000 jaxns-2.2.1/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-26 12:50:15.355704 jaxns-2.2.1/jaxns/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      581 2023-06-23 10:30:30.000000 jaxns-2.2.1/jaxns/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    13249 2023-06-23 10:30:30.000000 jaxns-2.2.1/jaxns/adaptive_refinement.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6940 2023-04-21 01:26:04.000000 jaxns-2.2.1/jaxns/initial_state.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-26 12:50:15.359704 jaxns-2.2.1/jaxns/internals/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.2.1/jaxns/internals/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      849 2023-01-03 05:33:37.000000 jaxns-2.2.1/jaxns/internals/linalg.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    12651 2023-06-15 13:49:53.000000 jaxns-2.2.1/jaxns/internals/log_semiring.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4919 2023-04-21 14:08:43.000000 jaxns-2.2.1/jaxns/internals/maps.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1899 2022-10-13 02:52:05.000000 jaxns-2.2.1/jaxns/internals/shapes.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1853 2023-01-03 05:33:37.000000 jaxns-2.2.1/jaxns/internals/stats.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-26 12:50:15.359704 jaxns-2.2.1/jaxns/internals/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.2.1/jaxns/internals/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      277 2023-01-03 05:33:37.000000 jaxns-2.2.1/jaxns/internals/tests/test_linalg.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5490 2023-01-03 05:33:37.000000 jaxns-2.2.1/jaxns/internals/tests/test_log_semiring.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2898 2023-06-14 16:43:12.000000 jaxns-2.2.1/jaxns/internals/tests/test_maps.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1110 2022-12-29 07:48:31.000000 jaxns-2.2.1/jaxns/internals/tests/test_shapes.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1186 2023-01-03 05:33:37.000000 jaxns-2.2.1/jaxns/internals/tests/test_stats.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-26 12:50:15.359704 jaxns-2.2.1/jaxns/likelihood_samplers/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.2.1/jaxns/likelihood_samplers/__init__.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-26 12:50:15.359704 jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3192 2023-06-23 00:05:06.000000 jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/em_gmm.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    29797 2023-06-23 10:35:37.000000 jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/multi_ellipsoid_utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-26 12:50:15.359704 jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1320 2023-06-20 09:16:37.000000 jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_em_gmm.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5263 2023-06-20 09:51:44.000000 jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_multi_ellipsoid.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3103 2023-05-18 20:19:33.000000 jaxns-2.2.1/jaxns/model.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4425 2023-06-23 10:35:53.000000 jaxns-2.2.1/jaxns/multi_ellipsoidal_samplers.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    18526 2023-06-26 12:35:12.000000 jaxns-2.2.1/jaxns/nested_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    16165 2023-06-23 11:05:56.000000 jaxns-2.2.1/jaxns/plotting.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    12554 2023-06-14 10:16:12.000000 jaxns-2.2.1/jaxns/prior.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2787 2023-04-20 15:27:03.000000 jaxns-2.2.1/jaxns/random.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    26263 2023-06-23 08:35:53.000000 jaxns-2.2.1/jaxns/slice_samplers.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    10153 2023-05-18 20:55:58.000000 jaxns-2.2.1/jaxns/special_priors.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    16335 2023-06-26 12:39:04.000000 jaxns-2.2.1/jaxns/static_nested_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    18919 2023-06-23 10:15:39.000000 jaxns-2.2.1/jaxns/statistics.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     6607 2023-05-12 13:17:17.000000 jaxns-2.2.1/jaxns/termination.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-26 12:50:15.359704 jaxns-2.2.1/jaxns/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2023-01-03 05:33:37.000000 jaxns-2.2.1/jaxns/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2198 2023-06-23 10:30:30.000000 jaxns-2.2.1/jaxns/tests/debug_adaptive_refinement.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3884 2023-06-23 10:30:30.000000 jaxns-2.2.1/jaxns/tests/test_initial_state.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    18625 2023-06-23 10:37:16.000000 jaxns-2.2.1/jaxns/tests/test_nested_sampler.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     9019 2023-06-20 23:01:19.000000 jaxns-2.2.1/jaxns/tests/test_prior.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1306 2023-04-15 16:37:14.000000 jaxns-2.2.1/jaxns/tests/test_random.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    24211 2023-06-23 10:30:30.000000 jaxns-2.2.1/jaxns/tests/test_statistics.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      477 2023-01-03 05:33:37.000000 jaxns-2.2.1/jaxns/tests/test_utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5118 2023-05-12 12:43:32.000000 jaxns-2.2.1/jaxns/types.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5122 2023-06-23 08:35:53.000000 jaxns-2.2.1/jaxns/uniform_samplers.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    17668 2023-05-15 05:41:18.000000 jaxns-2.2.1/jaxns/utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      716 2023-05-07 18:38:45.000000 jaxns-2.2.1/jaxns/warnings.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-06-26 12:50:15.355704 jaxns-2.2.1/jaxns.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4810 2023-06-26 12:50:15.000000 jaxns-2.2.1/jaxns.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1676 2023-06-26 12:50:15.000000 jaxns-2.2.1/jaxns.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-06-26 12:50:15.000000 jaxns-2.2.1/jaxns.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        6 2023-06-26 12:50:15.000000 jaxns-2.2.1/jaxns.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)      103 2022-10-13 02:52:05.000000 jaxns-2.2.1/pyproject.toml
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-06-26 12:50:15.359704 jaxns-2.2.1/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)      949 2023-06-26 12:40:43.000000 jaxns-2.2.1/setup.py
```

### Comparing `jaxns-2.2.0/PKG-INFO` & `jaxns-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxns
-Version: 2.2.0
+Version: 2.2.1
 Summary: Nested Sampling in JAX
 Home-page: https://github.com/joshuaalbert/jaxns
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jaxns-2.2.0/README.md` & `jaxns-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/adaptive_refinement.py` & `jaxns-2.2.1/jaxns/adaptive_refinement.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from jax import core, numpy as jnp, tree_map, random, pmap
 from jax._src.lax.control_flow import while_loop, scan
 from jax._src.lax.parallel import all_gather
 
 from jaxns.internals.stats import linear_to_log_stats
 from jaxns.model import Model
 from jaxns.static_nested_sampler import PreProcessType, add_chunk_dim, remove_chunk_dim, SeedPoint
-from jaxns.static_slice import UniDimSliceSampler
+from jaxns.slice_samplers import UniDimSliceSampler
 from jaxns.statistics import analyse_sample_collection
 from jaxns.types import NestedSamplerState, Reservoir, int_type, float_type
 from jaxns.utils import sort_samples
 
 __all__ = ['AdaptiveRefinement']
 
 logger = logging.getLogger('jaxns')
```

### Comparing `jaxns-2.2.0/jaxns/initial_state.py` & `jaxns-2.2.1/jaxns/initial_state.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/internals/linalg.py` & `jaxns-2.2.1/jaxns/internals/linalg.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/internals/log_semiring.py` & `jaxns-2.2.1/jaxns/internals/log_semiring.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/internals/maps.py` & `jaxns-2.2.1/jaxns/internals/maps.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/internals/shapes.py` & `jaxns-2.2.1/jaxns/internals/shapes.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/internals/stats.py` & `jaxns-2.2.1/jaxns/internals/stats.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/internals/tests/test_log_semiring.py` & `jaxns-2.2.1/jaxns/internals/tests/test_log_semiring.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/internals/tests/test_maps.py` & `jaxns-2.2.1/jaxns/internals/tests/test_maps.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/internals/tests/test_shapes.py` & `jaxns-2.2.1/jaxns/internals/tests/test_shapes.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/internals/tests/test_stats.py` & `jaxns-2.2.1/jaxns/internals/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/likelihood_samplers/em_gmm.py` & `jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/em_gmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,11 +80,7 @@
         cond,
         body,
         (jnp.asarray(False), jnp.asarray(0), params)
     )
 
     cluster_id = jnp.argmax(e_step(data, *params, mask=mask), axis=0)
     return cluster_id, params, total_iters
-
-
-def recursive_gmm(key, data, n_components, n_iters=10, tol=1e-6):
-    pass
```

### Comparing `jaxns-2.2.0/jaxns/likelihood_samplers/multi_ellipsoid_utils.py` & `jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/multi_ellipsoid_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-from typing import NamedTuple, Tuple
+from typing import NamedTuple, Tuple, Literal
 
 import numpy as np
 import pylab as plt
 from etils.array_types import IntArray, FloatArray, PRNGKey, BoolArray
 from jax import numpy as jnp, vmap, random, tree_map
 from jax._src.lax.control_flow import while_loop
 from jax._src.scipy.special import gammaln
 
 from jaxns.internals.log_semiring import LogSpace
-from jaxns.likelihood_samplers.em_gmm import em_gmm
+from jaxns.likelihood_samplers.multi_ellipsoid.em_gmm import em_gmm
 from jaxns.types import UType, int_type, float_type
 
-__all__ = ['ellipsoid_clustering',
-           'sample_multi_ellipsoid',
-           'MultEllipsoidState']
+__all__ = [
+    'ellipsoid_clustering',
+    'sample_multi_ellipsoid',
+    'MultEllipsoidState',
+]
 
 
-class MultiEllipsoidParams(NamedTuple):
+class EllipsoidParams(NamedTuple):
     mu: FloatArray  # [K, D] Ellipsoids centres
     radii: FloatArray  # [K, D] Ellsipoids radii
     rotation: FloatArray  # [K, D, D] Ellipsoids rotation matrices
 
 
 class MultEllipsoidState(NamedTuple):
-    params: MultiEllipsoidParams
+    params: EllipsoidParams
     cluster_id: IntArray  # [N] the cluster index of each point
 
 
 def log_ellipsoid_volume(radii):
     D = radii.shape[0]
     return jnp.log(2.) - jnp.log(D) + 0.5 * D * jnp.log(jnp.pi) - gammaln(0.5 * D) + jnp.sum(jnp.log(radii))
 
@@ -73,21 +75,21 @@
     u, s, vh = jnp.linalg.svd(cov)
     radii_min = jnp.finfo(s.dtype).eps
     radii = jnp.maximum(jnp.sqrt(s), radii_min)
     rotation = u
     return radii, rotation
 
 
-def ellipsoid_params(points: UType, mask: FloatArray) -> Tuple[FloatArray, FloatArray, FloatArray]:
+def ellipsoid_params(points: UType, mask: FloatArray) -> EllipsoidParams:
     """
     If the ellipsoid is defined by
 
-    (x - mu)^T cov (x - mu) = 1
+    (x - mu)^T C (x - mu) = 1
 
-    where cov = L @ L.T and L = diag(1/radii) @ rotation.T
+    where C = L @ L.T and L = diag(1/radii) @ rotation.T
 
     then this returns the mu, radius and rotation matrices of the ellipsoid.
 
     Args:
         points: [N, D] points to fit ellipsoids to
         mask: [N] mask of which points to consider
 
@@ -102,15 +104,15 @@
     # for all i (points[i] - mu) @ inv(Sigma) / scale**2 @ (points[i] - mu) <= 1
     # for all i (points[i] - mu) @ (L @ L.T) @ (points[i] - mu) <= scale**2
     rho = vmap(lambda x: maha_ellipsoid(x=x, mu=mu, radii=radii, rotation=rotation))(points)
 
     rho_max = jnp.max(jnp.where(mask, rho, 0.))
     radii *= jnp.sqrt(rho_max)
 
-    return mu, radii, rotation
+    return EllipsoidParams(mu=mu, radii=radii, rotation=rotation)
 
 
 def ellipsoid_to_circle(point: FloatArray, mu: FloatArray, radii: FloatArray, rotation: FloatArray) -> FloatArray:
     """
     Apply a linear map that would turn an ellipsoid into a sphere.
     Args:
         point: [D] point to transform
@@ -237,27 +239,27 @@
         # outside cube
         outside_unit_cube = jnp.any(point < 0.) | jnp.any(point > 1.)
         depth = jnp.where(outside_unit_cube, jnp.iinfo(depth.dtype).max, depth)
     return depth
 
 
 def sample_multi_ellipsoid(key: PRNGKey, mu: FloatArray, radii: FloatArray, rotation: FloatArray,
-                           unit_cube_constraint: bool = True) -> FloatArray:
+                           unit_cube_constraint: bool = True) -> Tuple[IntArray, FloatArray]:
     """
     Sample from a set of intersecting ellipsoids.
     When unit_cube_constraint=True then reject points outside the closed unit-cube.
 
     Args:
         key: PRNGKey
         mu: [K, D] centres of ellipses
         radii: [K, D] radii of ellipses
         rotation: [K,D,D] rotation matrices of ellipses
 
     Returns:
-        a sample point i.i.d. sampled from union of ellipsoids, of shape [D]
+        ellipsoid selected, and a sample point i.i.d. sampled from union of ellipsoids, of shape [D]
     """
     # u(t) = R @ (x + t * num_options) + c
     #     u(t) == 1
     #     1-c = R@x + t * R@num_options
     #     t = ((1 - c) - R@x)/R@num_options
     K, D = radii.shape
     log_VE = vmap(log_ellipsoid_volume)(radii)
@@ -281,171 +283,358 @@
     return k, u_accept
 
 
 def log_coverage_scale(log_VE, log_VS, D):
     """
     Computes the required scaling relation such that
     V(E) = max(V(E), V(S))
-    where the scaling is applied to each radius.
+    where the scaling is to be applied to each radius.
     Args:
         log_VE:
         log_VS:
         D:
     Returns:
     """
     return jnp.maximum(0., (log_VS - log_VE) / D)
 
 
-def cluster_split(key: PRNGKey, points: FloatArray, mask: BoolArray, log_VS: FloatArray, log_VE: FloatArray,
-                  kmeans_init: bool = True) \
-        -> Tuple[IntArray, FloatArray, MultiEllipsoidParams, FloatArray, MultiEllipsoidParams, BoolArray]:
+class ClusterSplitResult(NamedTuple):
+    unsorted_cluster_id: IntArray  # unsorted cluster id, using 0/1 to indicate the child.
+    log_VS0: FloatArray
+    params0: EllipsoidParams
+    log_VS1: FloatArray
+    params1: EllipsoidParams
+    successful_split: BoolArray
+
+
+def _multinest_split(key: PRNGKey, params: EllipsoidParams, points: FloatArray, mask: BoolArray, log_VS: FloatArray,
+                     em_init: bool = False,
+                     patience: int = 1):
     """
-    Splits a set of points into two ellipsoids such that the enclosed volume is as close to V(S) without being less.
-    V(S) should be an estimate of the true volume contained by the points.
+    Use's Multinest's method to partition points
 
     Args:
         key: PRNGKey
+        params: ellipsoid params of points that are being split (same as used for log VE)
         points: [N, D] points to split
         mask: [N] mask only those points which should be split
         log_VS: estimate of logV(S) of the set of points
-        log_VE: logV(E) of the minimum volume enclosing ellipsoid of masked points
-        kmeans_init: whether to use kmeans to initialise the clustering
+        em_init: whether to use kmeans to initialise the clustering
+        patience: how long to wait before seeing improvement
 
     Returns:
-        cluster indices of points (0 | 1),
-        logV(S1),
-        params of ellipsoid 1
-        logV(S2),
-        params of ellipsoid 2,
-        whether split occured -- If False then above return values are undefined
+        cluster_id, log_VS0, params0, log_VS1, params1
     """
-
     init_key, volume_key = random.split(key, 2)
+
     N, D = points.shape
     n_S = jnp.sum(mask)
     # calculate bounding ellipsoid
+
     ###
     # input is essentially log_VS
-    if kmeans_init:
+    if em_init:
         # do Euclidean kmean clustering
-        cluster_id, (centers, covariances, log_weight), total_iters = em_gmm(key=init_key, data=points, mask=mask,
-                                                                             n_components=2, n_iters=100)
+        cluster_id, (_, _, _), _ = em_gmm(
+            key=init_key,
+            data=points,
+            mask=mask,
+            n_components=2,
+            n_iters=100
+        )
     else:
-        # assign to random clusters: child0 or child1
-        cluster_id = random.randint(init_key, shape=(N,), minval=0, maxval=2)
-
-    def body(state):
-        (i, done, old_cluster_id, _, _, _, _, _, _, _, _, min_loss, delay) = state
-        mask1 = mask & (old_cluster_id == 0)
-        mask2 = mask & (old_cluster_id == 1)
+        # Split the ellipsoid in half
+        j_max = jnp.argmax(params.radii)
+        n = jnp.where(jnp.arange(params.radii.size) == j_max,
+                      jnp.asarray(1., float_type),
+                      jnp.asarray(0., float_type)
+                      )
+        p = params.rotation @ (jnp.diag(params.radii) @ n)
+        q = points - params.mu
+        proj = q @ p
+        cluster_id = jnp.where(proj >= jnp.asarray(0., float_type),
+                               jnp.asarray(0, int_type),
+                               jnp.asarray(1, int_type))
+        # # assign to random clusters: child0 or child1
+        # cluster_id = random.randint(init_key, shape=(N,), minval=0, maxval=2)
+
+    class CarryState(NamedTuple):
+        iter: IntArray
+        done: BoolArray
+        cluster_id: IntArray
+        log_VS0: FloatArray
+        params0: EllipsoidParams
+        log_VS1: FloatArray
+        params1: EllipsoidParams
+        min_loss: FloatArray
+        iters_no_improvement: IntArray
+
+    def body(body_state: CarryState):
+        mask0 = mask & (body_state.cluster_id == 0)
+        mask1 = mask & (body_state.cluster_id == 1)
         # estimate volumes of current clustering
+        n0 = jnp.sum(mask0)
         n1 = jnp.sum(mask1)
-        n2 = jnp.sum(mask2)
+        log_VS0 = log_VS + jnp.log(n0) - jnp.log(n_S)
         log_VS1 = log_VS + jnp.log(n1) - jnp.log(n_S)
-        log_VS2 = log_VS + jnp.log(n2) - jnp.log(n_S)
         # construct E_1, E_2 and compute volumes
-        mu1, radii1, rotation1 = ellipsoid_params(points=points, mask=mask1)
-        log_VE1 = log_ellipsoid_volume(radii1)
-        mu2, radii2, rotation2 = ellipsoid_params(points=points, mask=mask2)
-        log_VE2 = log_ellipsoid_volume(radii2)
+        params0 = ellipsoid_params(points=points, mask=mask0)
+        log_VE0 = log_ellipsoid_volume(params0.radii)
+        params1 = ellipsoid_params(points=points, mask=mask1)
+        log_VE1 = log_ellipsoid_volume(params1.radii)
         # enlarge to at least cover V(S1) and V(S2)
+        log_scale0 = log_coverage_scale(log_VE0, log_VS0, D)
         log_scale1 = log_coverage_scale(log_VE1, log_VS1, D)
-        log_scale2 = log_coverage_scale(log_VE2, log_VS2, D)
-        radii1 = jnp.exp(jnp.log(radii1) + log_scale1)
-        radii2 = jnp.exp(jnp.log(radii2) + log_scale2)
+        radii0 = jnp.exp(jnp.log(params0.radii) + log_scale0)
+        radii1 = jnp.exp(jnp.log(params1.radii) + log_scale1)
+        log_VE0 = log_VE0 + log_scale0 * D
         log_VE1 = log_VE1 + log_scale1 * D
-        log_VE2 = log_VE2 + log_scale2 * D
+        params0 = params0._replace(radii=radii0)
+        params1 = params1._replace(radii=radii1)
+
         # compute reassignment metrics
-        maha1 = vmap(lambda point: maha_ellipsoid(point, mu=mu1, radii=radii1, rotation=rotation1))(points)
-        maha2 = vmap(lambda point: maha_ellipsoid(point, mu=mu2, radii=radii2, rotation=rotation2))(points)
-        log_h1 = log_VE1 - log_VS1 + jnp.log(maha1)
-        log_h2 = log_VE2 - log_VS2 + jnp.log(maha2)
-        # reassign
-        delta_F = LogSpace(log_h1) - LogSpace(log_h2)
-        reassign_idx = jnp.argmax(delta_F.abs().log_abs_val)
-        new_id = jnp.asarray(delta_F[reassign_idx] > LogSpace(-jnp.inf), int_type)
+        maha0 = vmap(lambda point: maha_ellipsoid(point,
+                                                  mu=params0.mu,
+                                                  radii=params0.radii,
+                                                  rotation=params0.radii))(points)
+        maha1 = vmap(lambda point: maha_ellipsoid(point, mu=params1.mu,
+                                                  radii=params1.radii,
+                                                  rotation=params1.radii))(points)
+        h0 = LogSpace(log_VE0) * LogSpace(jnp.log(maha0)) / LogSpace(log_VS0)
+        h1 = LogSpace(log_VE1) * LogSpace(jnp.log(maha1)) / LogSpace(log_VS1)
+        # reassign biggest violator
+        abs_delta_F = (h0 - h1).abs()  # N
+        masked_log_abs_delta_F = jnp.where(mask, abs_delta_F.log_abs_val, -jnp.inf)
+        reassign_idx = jnp.argmax(masked_log_abs_delta_F)
+        new_id = jnp.where(masked_log_abs_delta_F[reassign_idx] > -jnp.inf,
+                           jnp.asarray(1, int_type) - cluster_id[reassign_idx],
+                           cluster_id[reassign_idx])
         new_cluster_id = cluster_id.at[reassign_idx].set(new_id)
 
+        # new_cluster_id = jnp.where(mask & (h0.log_abs_val < h1.log_abs_val),
+        #                            jnp.asarray(0., int_type),
+        #                            jnp.asarray(1., int_type))
+
         # new_cluster_k = jnp.where(log_h1 < log_h2, 0, 1)
-        log_V_sum = jnp.logaddexp(log_VE1, log_VE2)
-        new_loss = log_V_sum - log_VS
-        loss_decreased = new_loss < min_loss
-        delay = jnp.where(loss_decreased, 0, delay + 1)
-        min_loss = jnp.where(loss_decreased, new_loss, min_loss)
+        log_V_sum = jnp.logaddexp(log_VE0, log_VE1)
+        new_loss = log_V_sum - log_VS  # If scaling happened, then this will be zero
+        loss_decreased = new_loss < body_state.min_loss
+        iters_no_improvement = jnp.where(loss_decreased, 0, body_state.iters_no_improvement + 1)
+        min_loss = jnp.where(loss_decreased, new_loss, body_state.min_loss)
         ###
         # i / delay / loss_decreased / new_loss / min_loss
         # 0 / 0 / True / a / a
         # 1 / 1 / False / b / a
         # 2 / 2 / False / a / a
         # 3 / 3 / False / b / a
         # 4 / 4 / False / a / a
-        done = jnp.all(new_cluster_id == old_cluster_id) \
-               | (delay >= 10) \
+        cluster_mapping_unchanged = jnp.all((new_cluster_id == body_state.cluster_id) | jnp.bitwise_not(mask))
+        done = cluster_mapping_unchanged \
+               | (iters_no_improvement >= patience) \
+               | (n0 < D + 1) \
                | (n1 < D + 1) \
-               | (n2 < D + 1) \
                | jnp.isnan(log_V_sum)
-        return (
-            i + jnp.asarray(1, int_type), done, new_cluster_id, log_VS1, mu1, radii1, rotation1, log_VS2, mu2, radii2,
-            rotation2,
-            min_loss, delay)
-
-    done = (jnp.sum(mask) < 2 * (D + 1))
-    (i, _, cluster_id, log_VS1, mu1, radii1, rotation1, log_VS2, mu2, radii2, rotation2, min_loss, delay) = \
-        while_loop(lambda state: ~state[1],
-                   body,
-                   (jnp.array(0), done, cluster_id,
-                    jnp.array(-jnp.inf), jnp.zeros(D), jnp.zeros(D), jnp.eye(D),
-                    jnp.array(-jnp.inf), jnp.zeros(D), jnp.zeros(D), jnp.eye(D),
-                    jnp.asarray(jnp.inf), jnp.asarray(0, int_type)))
-    mask1 = mask & (cluster_id == 0)
-    mask2 = mask & (cluster_id == 1)
-    log_V_sum = jnp.logaddexp(log_ellipsoid_volume(radii1), log_ellipsoid_volume(radii2))
-
-    # V(A v B) = V(A) + V(B) - V(A ^ B) <= V(A) + V(B)
-    # V(A v B) / (V(A) + V(B)) = 1 - V(A ^ B)/(V(A) + V(B))
-    # (1 - V(A v B) / (V(A) + V(B))) = V(A ^ B)/(V(A) + V(B))
-    # V(A ^ B) / V(A v B) = (1 - V(A v B) / (V(A) + V(B))) (V(A) + V(B)) / V(A v B)
-    # intersection_ratio = jnp.log(1. - jnp.exp(log_V_union - log_V_sum)) + log_V_sum - log_V_union
-    # no_intersection = jnp.exp(intersection_ratio) < 0.05
-    no_intersection = (log_V_sum < log_VE)
-
-    do_split = (no_intersection | (log_VE > log_VS + jnp.log(2.))) \
-               & (~jnp.any(jnp.isnan(radii1))) \
-               & (~jnp.any(jnp.isnan(radii2))) \
-               & (jnp.sum(mask1) >= (D + 1)) \
-               & (jnp.sum(mask2) >= (D + 1))
-
-    # do_split = (log_VE > log_VS + jnp.log(2.)) \
-    #            | ((~jnp.any(jnp.isnan(radii1)))
-    #               & (~jnp.any(jnp.isnan(radii2)))
-    #               & (jnp.sum(mask1) >= (D + 1))
-    #               & (jnp.sum(mask2) >= (D + 1)))
-    # & (cond1 < 50.) \
-    # & (cond2 < 50.)
-
-    params1 = MultiEllipsoidParams(mu=mu1,
-                                   radii=radii1,
-                                   rotation=rotation1)
 
-    params2 = MultiEllipsoidParams(mu=mu2, radii=radii2, rotation=rotation2)
+        return CarryState(
+            iter=body_state.iter + jnp.asarray(1, int_type),
+            done=done,
+            cluster_id=new_cluster_id,
+            log_VS0=log_VS0,
+            params0=params0,
+            log_VS1=log_VS1,
+            params1=params1,
+            min_loss=min_loss,
+            iters_no_improvement=iters_no_improvement
+        )
+
+    # Done to start with if not at least D+1 points per ellipsoid possible
+    done = (n_S < 2 * (D + 1))
+
+    init_state = CarryState(
+        iter=jnp.array(0),
+        done=done,
+        cluster_id=cluster_id,
+        log_VS0=jnp.array(-jnp.inf),
+        params0=EllipsoidParams(mu=jnp.zeros(D), radii=jnp.zeros(D), rotation=jnp.eye(D)),
+        log_VS1=jnp.array(-jnp.inf),
+        params1=EllipsoidParams(mu=jnp.zeros(D), radii=jnp.zeros(D), rotation=jnp.eye(D)),
+        min_loss=jnp.asarray(jnp.inf),
+        iters_no_improvement=jnp.asarray(0, int_type)
+    )
+
+    output_state: CarryState = while_loop(lambda state: ~state.done,
+                                          body,
+                                          init_state)
+    return output_state.cluster_id, output_state.log_VS0, output_state.params0, output_state.log_VS1, output_state.params1
+
+
+def _em_gmm_split(key: PRNGKey, points: FloatArray, mask: BoolArray, log_VS: FloatArray):
+    """
+    Use's EM Gaussian mixture model to partition points.
+
+    Args:
+        key: PRNGKey
+        points: [N, D] points to split
+        mask: [N] mask only those points which should be split
+        log_VS: estimate of logV(S) of the set of points
+
+    Returns:
+        cluster_id, log_VS0, params0, log_VS1, params1
+    """
+    N, D = points.shape
+    n_S = jnp.sum(mask)
+
+    # do Euclidean kmean clustering
+    cluster_id, (_, _, _), _ = em_gmm(
+        key=key,
+        data=points,
+        mask=mask,
+        n_components=2,
+        n_iters=100
+    )
+
+    mask0 = mask & (cluster_id == 0)
+    mask1 = mask & (cluster_id == 1)
+    # estimate volumes of current clustering
+    n0 = jnp.sum(mask0)
+    n1 = jnp.sum(mask1)
+    log_VS0 = log_VS + jnp.log(n0) - jnp.log(n_S)
+    log_VS1 = log_VS + jnp.log(n1) - jnp.log(n_S)
+    # construct E_1, E_2 and compute volumes
+    params0 = ellipsoid_params(points=points, mask=mask0)
+    log_VE0 = log_ellipsoid_volume(params0.radii)
+    params1 = ellipsoid_params(points=points, mask=mask1)
+    log_VE1 = log_ellipsoid_volume(params1.radii)
+    # enlarge to at least cover V(S1) and V(S2)
+    log_scale0 = log_coverage_scale(log_VE0, log_VS0, D)
+    log_scale1 = log_coverage_scale(log_VE1, log_VS1, D)
+    radii0 = jnp.exp(jnp.log(params0.radii) + log_scale0)
+    radii1 = jnp.exp(jnp.log(params1.radii) + log_scale1)
+    params0 = params0._replace(radii=radii0)
+    params1 = params1._replace(radii=radii1)
+
+    return cluster_id, log_VS0, params0, log_VS1, params1
+
+
+def cluster_split(key: PRNGKey, params: EllipsoidParams, points: FloatArray, mask: BoolArray, log_VS: FloatArray,
+                  method: Literal['multinest', 'em_gmm']) -> ClusterSplitResult:
+    """
+    Splits a set of points into two ellipsoids such that the enclosed volume is as close to V(S) without being less.
+    V(S) should be an estimate of the true volume contained by the points.
+
+    Args:
+        key: PRNGKey
+        params: ellipsoid params of points that are being split (same as used for log VE)
+        points: [N, D] points to split
+        mask: [N] mask only those points which should be split
+        log_VS: estimate of logV(S) of the set of points
+        method: what method to use for splitting. Available are: 'multinest','em_gmm'
+
+    Returns:
+        cluster split results
+    """
+
+    N, D = points.shape
+    # calculate bounding ellipsoid
+    # volume of ellipsoid, already have E scaled so that V(E) >= V(S)
+    log_VE = log_ellipsoid_volume(params.radii)
+
+    # We always have
+    if method == 'em_gmm':
+        cluster_id, log_VS0, params0, log_VS1, params1 = _em_gmm_split(key=key, points=points, mask=mask,
+                                                                       log_VS=log_VS)
+    elif method == 'multinest':
+        cluster_id, log_VS0, params0, log_VS1, params1 = _multinest_split(key=key, params=params, points=points,
+                                                                          mask=mask,
+                                                                          log_VS=log_VS,
+                                                                          em_init=False,
+                                                                          patience=1)
+    else:
+        raise ValueError(f"Invalid method {method}")
+
+    # Imperfect sampling condition
+    # (0)       V(A) <= V(S1), and V(B) <= V(S2)
+
+    # V(A) <= V(S1) = V(S) V(A) / (V(A) + V(B))
+    # V(A) (V(A) + V(B)) <= V(S) V(A)
+    # V(A)^2 + V(A)V(B) - V(S) V(A) <= 0
+    # V(B)^2 + V(A)V(B) - V(S) V(B) <= 0
+    # V(A)^2 - V(B)^2 - V(S) (V(A) - V(B)) <= 0
+    # (V(A) + V(B)) (V(A) - V(B)) - V(S) (V(A) - V(B)) <= 0
+    # (V(A) + V(B)) - V(S) <= 0, (V(A) - V(B)) != 0
+    #
+    # Bounding ellipsoid condition
+    # (1)       V(S1) <= V(E_A), and V(S2) <= V(E_B)
+    # (1.1)     from (0) => V(A) + V(B) <= V(S1) + V(S2) <= V(E_A) + V(E_B)
+
+    # Disjoint partitioning condition
+    # (2)       V(S1) + V(S2) = V(S)
+    # (2.1)     from (1.1) => V(A) + V(B) <= V(S1) + V(S2) = V(S) <= V(E_A) + V(E_B)
+    # (2.2)     from (2) => V(S1 ^ S2) = 0
+
+    # Disjoint partitioning condition
+    # (3)       V(A) + V(B) = V(A v B)
+    # (3.1)     from (2) => V(A ^ B) = 0
+
+    # Bounding ellipsoid condition
+    # (4)       V(S) <= V(E)
+    # (4.1)     with (2.1) => V(A) + V(B) <= V(S1) + V(S2) = V(S) <= V(E)
+
+    # (5)       Good split <=> V(S1) ~ V(E_A), and V(S2) ~ V(E_B)
+    # (5.1)     from (4.1) Good split <=> V(A) + V(B) <= V(S1) + V(S2) = V(S) <~ V(E_B) + V(E_B)  <= V(E)
+
+    # (6)       Good sampling <=> V(A) ~ V(S1), and V(B) ~ V(S2)
+    # (6.1)     from (5.1) Good sampling <=> V(A) + V(B) <~ V(S1) + V(S2) = V(S) <= V(E)
 
-    return cluster_id, log_VS1, params1, log_VS2, params2, do_split
+    # (7)       Good split and Good sampling <=> V(A) + V(B) <~ V(S1) + V(S2) = V(S) <~ V(E_B) + V(E_B) <= V(E)
 
+    # We take the condition for success:
+    #  V(E_B) + V(E_B) is closer to V(S) than V(E) (from 5.1)
 
-def plot_ellipses(params: MultiEllipsoidParams):
+    mask0 = mask & (cluster_id == 0)
+    mask1 = mask & (cluster_id == 1)
+
+    log_VE_A = log_ellipsoid_volume(params0.radii)
+    log_VE_B = log_ellipsoid_volume(params1.radii)
+
+    V_sum = LogSpace(log_VE_A) + LogSpace(log_VE_B)
+
+    good_split = (V_sum.log_abs_val < log_VE)
+
+    successful_split = good_split \
+                       & jnp.bitwise_not(jnp.isnan(log_VE_A)) \
+                       & jnp.bitwise_not(jnp.isnan(log_VE_A)) \
+                       & (jnp.sum(mask0) >= (D + 1)) \
+                       & (jnp.sum(mask1) >= (D + 1))
+
+    return ClusterSplitResult(unsorted_cluster_id=cluster_id, log_VS0=log_VS0,
+                              params0=params0, log_VS1=log_VS1,
+                              params1=params1, successful_split=successful_split)
+
+
+def plot_ellipses(params: EllipsoidParams, show: bool = True):
+    """
+    Plots ellipses.
+
+    Args:
+        params: ellipsoid parameters to plot
+        show: whether to show figure
+    """
     theta = jnp.linspace(0., 2 * jnp.pi, 100)
     circle = jnp.stack([jnp.cos(theta), jnp.sin(theta)], axis=1)
     for mu, radii, rotation in zip(params.mu, params.radii, params.rotation):
         ellipse = vmap(lambda point: circle_to_ellipsoid(point, mu, radii, rotation))(circle)
         plt.plot(ellipse[:, 0], ellipse[:, 1], c=np.random.uniform(size=3))
-    plt.show()
+    if show:
+        plt.show()
 
 
 def ellipsoid_clustering(key: PRNGKey, points: FloatArray, log_VS: FloatArray,
-                         max_num_ellipsoids: int) -> MultEllipsoidState:
+                         max_num_ellipsoids: int,
+                         method: Literal['multinest', 'em_gmm'] = 'em_gmm') -> MultEllipsoidState:
     """
     Partition live_points into 2^depth ellipsoids in depth-first order.
 
     Args:
         key:PRNGKey
         points: [N, D] points to partition
         log_VS: expected true volume of points
@@ -456,87 +645,137 @@
     """
 
     N, D = points.shape
     if max_num_ellipsoids < 1:
         raise ValueError(f"max_num_ellipsoids should be >= 1, got {max_num_ellipsoids}.")
     K = max_num_ellipsoids
 
-    cluster_id = jnp.zeros(N, dtype=int_type)
+    # Construct the initial state
+    init_ellipsoid = ellipsoid_params(points=points, mask=jnp.ones(N, jnp.bool_))
+
+    log_VE = log_ellipsoid_volume(init_ellipsoid.radii)
+    log_scale = log_coverage_scale(log_VE, log_VS, D)
+    radii = jnp.exp(jnp.log(init_ellipsoid.radii) + log_scale)
+    # log_VE = log_VE + log_scale * D
+    init_ellipsoid = init_ellipsoid._replace(radii=radii)
 
-    params = MultiEllipsoidParams(
+    # state is zeros except first ellipsoid
+    cluster_id = jnp.zeros(N, dtype=int_type)
+    params = EllipsoidParams(
         mu=jnp.zeros((K, D), float_type),
         radii=jnp.zeros((K, D), float_type),
         rotation=jnp.zeros((K, D, D), float_type)
     )
-
-    mu, radii, rotation = ellipsoid_params(points=points, mask=jnp.ones(N, jnp.bool_))
-
-    params = params._replace(
-        mu=params.mu.at[0].set(mu),
-        radii=params.radii.at[0].set(radii),
-        rotation=params.rotation.at[0].set(rotation)
+    params: EllipsoidParams = tree_map(lambda x, y: x.at[0].set(y), params, init_ellipsoid)
+    state = MultEllipsoidState(
+        cluster_id=cluster_id,
+        params=params
     )
 
-    state = MultEllipsoidState(cluster_id=cluster_id,
-                               params=params)
-
-    log_VS_subclusters = jnp.array([log_VS] + [-jnp.inf] * (K - 1))
-    done_splitting = jnp.asarray([False] + [True] * (K - 1), jnp.bool_)
+    # Initial tracking parameters
+    log_VS_subclusters = jnp.asarray([log_VS] + [-jnp.inf] * (K - 1))
+    done_splitting = jnp.isneginf(log_VS_subclusters)
     split_depth = jnp.zeros([K], int_type)
 
-    CarryType = Tuple[PRNGKey, IntArray, MultEllipsoidState, BoolArray, IntArray, FloatArray]
-
-    def body(body_state: CarryType) -> CarryType:
-        (key, next_k, state, done_splitting, split_depth, log_VS_subclusters) = body_state
-
-        key, split_key = random.split(key, 2)
-        # bread first selection
-        select_split = jnp.argmin(jnp.where(done_splitting, jnp.iinfo(split_depth.dtype).max, split_depth))
-
-        mask = state.cluster_id == select_split
-        log_VS_subcluster = log_VS_subclusters[select_split]
-        log_VE_parent = log_ellipsoid_volume(state.params.radii[select_split])
-
-        unsorted_cluster_id, log_VS1, params1, log_VS2, params2, do_split = cluster_split(
-            split_key, points, mask, log_VS_subcluster, log_VE_parent, kmeans_init=True)
+    # TODO: compare performance with scan
 
-        params = tree_map(lambda x, y: jnp.where(do_split, x.at[select_split].set(y), x),
-                          state.params,
-                          params1)
-        params = tree_map(lambda x, y: jnp.where(do_split, x.at[next_k].set(y), x),
-                          params,
-                          params2)
-
-        # update those points where mask is true, unsorted id is 1, and do_split is true
-        cluster_id = jnp.where(do_split & (unsorted_cluster_id == 1) & mask, next_k, state.cluster_id)
-
-        state = state._replace(params=params, cluster_id=cluster_id)
-
-        done_splitting = jnp.where(do_split,
-                                   done_splitting.at[next_k].set(False),
-                                   done_splitting.at[select_split].set(True))
-
-        new_depth = split_depth[select_split] + jnp.asarray(1, int_type)
-        split_depth = jnp.where(do_split, split_depth.at[select_split].set(new_depth), split_depth)
-        split_depth = jnp.where(do_split, split_depth.at[next_k].set(new_depth), split_depth)
-
-        log_VS_subclusters = jnp.where(do_split, log_VS_subclusters.at[select_split].set(log_VS1), log_VS_subclusters)
-        log_VS_subclusters = jnp.where(do_split, log_VS_subclusters.at[next_k].set(log_VS2), log_VS_subclusters)
-
-        # if no split we replace child0 with parent and child1 gets zero-size ellipsoid that has no members.
-
-        next_k = next_k + jnp.asarray(1, int_type)
+    class CarryType(NamedTuple):
+        key: PRNGKey
+        next_k: IntArray
+        state: MultEllipsoidState
+        done_splitting: BoolArray
+        split_depth: IntArray
+        log_VS_subclusters: FloatArray
 
-        return (key, next_k, state, done_splitting, split_depth, log_VS_subclusters)
+    def body(body_state: CarryType) -> CarryType:
+        key, split_key = random.split(body_state.key, 2)
+        # Select the depth we work on now: bread first selection ==> min depth first (excluding done splits)
+        select_split = jnp.argmin(
+            jnp.where(body_state.done_splitting, jnp.iinfo(body_state.split_depth.dtype).max, body_state.split_depth)
+        )
+        mask = body_state.state.cluster_id == select_split
+        # estimated volume in sub-cluster
+        log_VS = body_state.log_VS_subclusters[select_split]
+
+        # params of ellipsoid
+        params = tree_map(lambda x: x[select_split], body_state.state.params)
+
+        # Perform a split on points in the given mask
+        # Strategy: if no split we replace child0 with parent and child1 gets zero-size ellipsoid that has no members.
+        cluster_split_result: ClusterSplitResult = cluster_split(
+            key=split_key,
+            params=params,
+            points=points,
+            mask=mask,
+            log_VS=log_VS,
+            method=method
+        )
+
+        # Update the parameters in given component that is being split with child 0
+        params = tree_map(lambda x, y: jnp.where(cluster_split_result.successful_split, x.at[select_split].set(y), x),
+                          body_state.state.params,
+                          cluster_split_result.params0)
+        # Update the parameters in `next_k` with child 1
+        params = tree_map(
+            lambda x, y: jnp.where(cluster_split_result.successful_split, x.at[body_state.next_k].set(y), x),
+            params,
+            cluster_split_result.params1)
+        # select_split stays the same cluster_id taking on child 0, but next_k gets child 1
+        cluster_id = jnp.where(
+            cluster_split_result.successful_split & (cluster_split_result.unsorted_cluster_id == 1) & mask,
+            body_state.next_k,
+            body_state.state.cluster_id)
+        state = body_state.state._replace(params=params, cluster_id=cluster_id)
+
+        # If success => next_k is not done, (and select_k is not done, as previously set)
+        # Else select_k is done (next_k stays done, as previously set)
+        done_splitting = jnp.where(cluster_split_result.successful_split,
+                                   body_state.done_splitting.at[body_state.next_k].set(False),
+                                   body_state.done_splitting.at[select_split].set(True))
+
+        # If success => update split depth
+        new_depth = body_state.split_depth[select_split] + jnp.asarray(1, int_type)
+        split_depth = jnp.where(cluster_split_result.successful_split,
+                                body_state.split_depth.at[select_split].set(new_depth),
+                                body_state.split_depth)
+        split_depth = jnp.where(cluster_split_result.successful_split,
+                                split_depth.at[body_state.next_k].set(new_depth),
+                                split_depth)
+
+        # If success => update estimated subcluster volumes
+        log_VS_subclusters = jnp.where(cluster_split_result.successful_split,
+                                       body_state.log_VS_subclusters.at[select_split].set(cluster_split_result.log_VS0),
+                                       body_state.log_VS_subclusters)
+        log_VS_subclusters = jnp.where(cluster_split_result.successful_split,
+                                       log_VS_subclusters.at[body_state.next_k].set(cluster_split_result.log_VS1),
+                                       log_VS_subclusters)
+
+        # TODO: (verify) I think next_k should only increment if successful split, as otherwise it uses up space.
+        next_k = jnp.where(cluster_split_result.successful_split,
+                           body_state.next_k + jnp.asarray(1, int_type),
+                           body_state.next_k)
+
+        return CarryType(
+            key=key,
+            next_k=next_k,
+            state=state,
+            done_splitting=done_splitting,
+            split_depth=split_depth,
+            log_VS_subclusters=log_VS_subclusters
+        )
 
     def cond(body_state: CarryType) -> BoolArray:
-        (key, next_k, state, done_splitting, split_depth, log_VS_subclusters) = body_state
-        done = jnp.all(done_splitting) | (next_k == K)
+        done = jnp.all(body_state.done_splitting) | (body_state.next_k == K)
         return jnp.bitwise_not(done)
 
-    init_body_state = (key, jnp.asarray(1, int_type), state, done_splitting, split_depth, log_VS_subclusters)
-    (key, next_k, state, done_splitting, split_depth, log_VS_subclusters) = \
-        while_loop(cond,
-                   body,
-                   init_body_state)
+    init_body_state = CarryType(
+        key=key,
+        next_k=jnp.asarray(1, int_type),
+        state=state,
+        done_splitting=done_splitting,
+        split_depth=split_depth,
+        log_VS_subclusters=log_VS_subclusters
+    )
+
+    output_state = while_loop(cond, body, init_body_state)
 
-    return state
+    return output_state.state
```

### Comparing `jaxns-2.2.0/jaxns/likelihood_samplers/tests/test_em_gmm.py` & `jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_em_gmm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pylab as plt
 from jax import numpy as jnp, random, jit
 from sklearn.datasets import make_blobs
 from sklearn.metrics import adjusted_rand_score
 
-from jaxns.likelihood_samplers.em_gmm import em_gmm
+from jaxns.likelihood_samplers.multi_ellipsoid.em_gmm import em_gmm
 
 
 def test_em_gmm():
     data = jnp.array([[1.0, 1.0], [1.1, 1.1], [1.2, 1.2], [4.0, 4.0], [4.1, 4.1], [4.2, 4.2]])
     n_components = 2
     key = random.PRNGKey(42)
```

### Comparing `jaxns-2.2.0/jaxns/likelihood_samplers/tests/test_multi_ellipsoid.py` & `jaxns-2.2.1/jaxns/likelihood_samplers/multi_ellipsoid/tests/test_multi_ellipsoid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 import pylab as plt
 import tensorflow_probability.substrates.jax as tfp
 from jax import numpy as jnp, random, tree_map, disable_jit, vmap
 
 from jaxns import PriorModelGen, Prior, Model
 from jaxns.initial_state import get_uniform_init_live_points
-from jaxns.likelihood_samplers.multi_ellipsoid_utils import log_ellipsoid_volume, ellipsoid_clustering, \
+from jaxns.likelihood_samplers.multi_ellipsoid.multi_ellipsoid_utils import log_ellipsoid_volume, ellipsoid_clustering, \
     bounding_ellipsoid, covariance_to_rotational, ellipsoid_params, point_in_ellipsoid, plot_ellipses, \
-    MultiEllipsoidParams, maha_ellipsoid, circle_to_ellipsoid, ellipsoid_to_circle
+    EllipsoidParams, maha_ellipsoid, circle_to_ellipsoid, ellipsoid_to_circle
 from jaxns.random import random_ortho_matrix
 from jaxns.types import float_type
 
 tfpd = tfp.distributions
 
 
 def test_ellipsoid_clustering():
@@ -93,21 +93,33 @@
                                    mean=jnp.zeros(N),
                                    cov=cov,
                                    shape=(n,))
 
     mu, radii, rotation = ellipsoid_params(points=X, mask=jnp.ones(n, jnp.bool_))
     inside = vmap(lambda x: point_in_ellipsoid(x, mu, radii, rotation))(X)
     plt.scatter(X[:, 0], X[:, 1], c=inside)
-    plot_ellipses(tree_map(lambda x: x[None], MultiEllipsoidParams(mu, radii, rotation)))
+    plot_ellipses(tree_map(lambda x: x[None], EllipsoidParams(mu, radii, rotation)))
 
     assert np.all(inside)
 
     rho_max = jnp.max(vmap(lambda x: maha_ellipsoid(x, mu, radii, rotation))(X))
     assert jnp.isclose(rho_max, 1.)
 
+    points = jnp.asarray([[0., 1.], [0., -1.], [1.5, 0.], [-1.5, 0.]])
+    mu, radii, rotation = ellipsoid_params(points=points, mask=jnp.ones(4, jnp.bool_))
+    # print(mu, radii, rotation)
+    mu_true = jnp.zeros(2)
+    radii_true = jnp.asarray([1.5, 1.])
+    rotation_true = jnp.eye(2)
+    assert jnp.allclose(mu, mu_true)
+    assert jnp.allclose(radii, radii_true)
+    assert jnp.allclose(rotation, rotation_true)
+
+
+
 
 def test_ellipsoid_transforms():
     n = 1000
 
     N = 2
     random_rotation = random_ortho_matrix(random.PRNGKey(0), n=N, special_orthogonal=True)
     random_radii = random.uniform(random.PRNGKey(1), shape=(N,))
```

### Comparing `jaxns-2.2.0/jaxns/model.py` & `jaxns-2.2.1/jaxns/model.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/nested_sampler.py` & `jaxns-2.2.1/jaxns/nested_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 from jaxns.adaptive_refinement import AdaptiveRefinement
 from jaxns.initial_state import init_sample_collection, get_uniform_init_live_points
 from jaxns.internals.log_semiring import LogSpace, normalise_log_space
 from jaxns.internals.stats import linear_to_log_stats, effective_sample_size
 from jaxns.model import Model
 from jaxns.plotting import plot_cornerplot, plot_diagnostics
+from jaxns.slice_samplers import UniDimSliceSampler
 from jaxns.static_nested_sampler import StaticNestedSampler, AbstractSampler
-from jaxns.static_slice import UniDimSliceSampler
-from jaxns.static_uniform import UniformSampler
 from jaxns.statistics import analyse_sample_collection
 from jaxns.types import TerminationCondition, NestedSamplerState, NestedSamplerResults, LivePoints
+from jaxns.uniform_samplers import UniformSampler
 from jaxns.utils import collect_samples
 from jaxns.utils import summary, save_results, load_results
 
 tfpd = tfp.distributions
 
 logger = logging.getLogger('jaxns')
 
@@ -372,15 +372,19 @@
         """
         super(ExactNestedSampler, self).__init__(model=model, max_samples=max_samples)
 
         self.approximate_sampler = ApproximateNestedSampler(
             model=model,
             num_live_points=num_live_points,
             num_parallel_samplers=num_parallel_samplers,
-            max_samples=max_samples
+            max_samples=max_samples,
+            sampler_chain=[
+                UniformSampler(model=model, efficiency_threshold=0.1),
+                UniDimSliceSampler(model=model, num_slices=model.U_ndims * 3, midpoint_shrink=True, perfect=True)
+            ]
         )
 
         self.adaptive_refinement = AdaptiveRefinement(
             model=self.model,
             patience=patience
         )
 
@@ -397,10 +401,12 @@
         Returns:
             termination reason, and exact state
         """
         if isinstance(key, core.Tracer):
             raise RuntimeError("Tracer detected, but expected imperative context.")
 
         termination_reason, state = self.approximate_sampler(key=key, term_cond=term_cond, init_state=init_state)
-        state = self.adaptive_refinement(state=state)
+        # TODO: Turn on adaptive refinement after fixing bias issue
+        # Note: for now exact here means that we ensure i.i.d. samples by choosing strong hyper parameters for samplers.
+        # state = self.adaptive_refinement(state=state)
 
         return termination_reason, state
```

### Comparing `jaxns-2.2.0/jaxns/plotting.py` & `jaxns-2.2.1/jaxns/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,46 +24,47 @@
 
     Args:
         results: NestedSamplerResult
         save_name: file to save figure to.
     """
     fig, axs = plt.subplots(5, 1, sharex=True, figsize=(8, 12))
     log_X = results.log_X_mean
-    axs[0].plot(-log_X, results.num_live_points_per_sample)
+    axs[0].plot(-log_X, results.num_live_points_per_sample, c='black')
     axs[0].set_ylabel(r'$n_{\rm live}(U)$')
     # detect if too small log likelihood
     log_likelihood = results.log_L_samples
     max_log_likelihood = jnp.max(log_likelihood)
-    likelihood = jnp.exp(log_likelihood - max_log_likelihood)
-    axs[1].plot(-log_X, likelihood)
-    axs[1].hlines(1., jnp.min(-log_X),
+    rel_log_likelihood = log_likelihood - max_log_likelihood
+    axs[1].plot(-log_X, rel_log_likelihood, c='black')
+    axs[1].hlines(0., jnp.min(-log_X),
                   jnp.max(-log_X), colors='black', ls='dashed',
                   label=r"$\log L_{{\rm max}}={:.1f}$".format(max_log_likelihood))
-    axs[1].set_ylabel(r'$L(U)/L_{\rm max}$')
+    axs[1].set_ylabel(r'$\log \left(L(X)/L_{\rm max}\right)$')
     axs[1].legend()
-    axs[2].plot(-log_X, jnp.exp(results.log_dp_mean))
+    axs[2].plot(-log_X, jnp.exp(results.log_dp_mean), c='black')
     # axs[2].vlines(-results.H_mean, 0., jnp.exp(jnp.max(results.log_dp_mean)), colors='black', ls='dashed',
     #               label='-logX=-H={:.1f}'.format(-results.H_mean))
     axs[2].set_ylabel(r'$Z^{-1}L(U) dX$')
     axs[2].legend()
     log_cum_evidence = cumulative_logsumexp(results.log_dp_mean)
     cum_evidence = jnp.exp(log_cum_evidence)
-    axs[3].plot(-log_X, cum_evidence)
+    axs[3].plot(-log_X, cum_evidence, c='black')
     axs[3].hlines(1., jnp.min(-log_X),
                   jnp.max(-log_X), colors='black', ls='dashed',
                   label=r"$\log Z={:.1f}$".format(results.log_Z_mean))
     axs[3].set_ylabel(r'$Z(x > U)/Z$')
     axs[3].legend()
-    axs[4].plot(-log_X, 1./results.num_likelihood_evaluations_per_sample)
+    axs[4].scatter(-log_X, 1./results.num_likelihood_evaluations_per_sample, s=2, c='black')
     axs[4].hlines(jnp.exp(results.log_efficiency), jnp.min(-log_X),
                   jnp.max(-log_X), colors='black', ls='dashed',
                   label='avg. eff.={:.3f}'.format(jnp.exp(results.log_efficiency)))
     axs[4].set_ylabel("sampler efficiency")
     axs[4].set_ylim(0., 1.05)
     axs[4].legend()
+    axs[4].set_xlabel(r'$- \log X$')
     if save_name is not None:
         fig.savefig(save_name)
     plt.show()
 
 
 def plot_cornerplot(results: NestedSamplerResults, vars=None, save_name=None):
     """
```

### Comparing `jaxns-2.2.0/jaxns/prior.py` & `jaxns-2.2.1/jaxns/prior.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/random.py` & `jaxns-2.2.1/jaxns/random.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/special_priors.py` & `jaxns-2.2.1/jaxns/special_priors.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/static_nested_sampler.py` & `jaxns-2.2.1/jaxns/static_nested_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Tuple, NamedTuple, TypeVar, Optional, List
+from typing import Tuple, NamedTuple, TypeVar, Optional, List, Union
 
 from etils.array_types import PRNGKey, IntArray, BoolArray, FloatArray
 from jax import tree_map, numpy as jnp, random, pmap
 from jax._src.lax.control_flow import while_loop, scan
 from jax._src.lax.parallel import all_gather
 
 from jaxns.model import Model
@@ -54,15 +54,15 @@
             raise ValueError(f"{efficiency_threshold} must be in [0., 1.), got {efficiency_threshold}.")
         efficiency_threshold = jnp.asarray(efficiency_threshold, float_type)
         self.efficiency_threshold = efficiency_threshold
 
     def __repr__(self):
         return self.__class__.__name__
 
-    def preprocess(self, state: NestedSamplerState) -> PreProcessType:
+    def preprocess(self, state: NestedSamplerState, live_points: Union[LivePoints, None] = None) -> PreProcessType:
         """
         Produces a data structure that is necessary for sampling to run.
         Typically this is where clustering happens.
 
         Args:
             state: nested sampler state
 
@@ -295,29 +295,30 @@
             return done, termination_reason
 
         def build_body(sampler: AbstractSampler, term_cond: TerminationCondition):
             def body(body_state: CarryType) -> CarryType:
                 key, sample_key = random.split(body_state.state.key, 2)
                 state = body_state.state._replace(key=key)
 
-                preprocess_data = sampler.preprocess(state)
+                preprocess_data = sampler.preprocess(state=state, live_points=body_state.live_points)
 
                 (dead_reservoir, live_points, log_L_contour) = self._single_live_point_shrink(
                     key=sample_key,
                     live_points=body_state.live_points,
                     log_L_contour=body_state.log_L_contour,
                     preprocess_data=preprocess_data,
                     sampler=sampler
                 )
                 # Collect dead reservoirs from all devices, and merge into state
                 all_dead_reservoir: Reservoir = remove_chunk_dim(all_gather(dead_reservoir, 'i'))
                 all_live_points: LivePoints = remove_chunk_dim(all_gather(live_points, 'i'))
                 new_state = collect_samples(state, all_dead_reservoir)
 
-                done, termination_reason = stopping_cond(state=new_state, live_points=all_live_points, term_cond=term_cond)
+                done, termination_reason = stopping_cond(state=new_state, live_points=all_live_points,
+                                                         term_cond=term_cond)
 
                 return CarryType(done=done, termination_reason=termination_reason, state=new_state,
                                  live_points=live_points, log_L_contour=log_L_contour)
 
             return body
 
         # We start with live points sorted. The starting contour is the constraint of the minimal sample.
```

### Comparing `jaxns-2.2.0/jaxns/static_slice.py` & `jaxns-2.2.1/jaxns/slice_samplers.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from etils.array_types import PRNGKey, FloatArray, BoolArray
 from jax import numpy as jnp, random, tree_map
 from jax._src.lax.control_flow import while_loop
 
 from jaxns.model import Model
 from jaxns.static_nested_sampler import MarkovSampler, PreProcessType, SeedPoint
-from jaxns.types import Sample, NestedSamplerState
+from jaxns.types import Sample, NestedSamplerState, LivePoints
 from jaxns.types import float_type, int_type
 
 logger = logging.getLogger('jaxns')
 
 __all__ = ['UniDimSliceSampler', 'MultiDimSliceSampler']
 
 T = TypeVar('T')
@@ -54,15 +54,15 @@
         super().__init__(model=model, efficiency_threshold=efficiency_threshold)
         if num_slices < 1:
             raise ValueError(f"num_slices should be > 0, got {num_slices}.")
         self.num_slices = num_slices
         self.midpoint_shrink = midpoint_shrink
         self.perfect = perfect
 
-    def preprocess(self, state: NestedSamplerState) -> PreProcessType:
+    def preprocess(self, state: NestedSamplerState, live_points: LivePoints) -> PreProcessType:
         if self.perfect: # nothing needed
             return ()
         # else: # step out with doubling
         #     return multi_ellipsoidal_params()
 
     def _sample_direction(self, n_key: PRNGKey, ndim: int) -> FloatArray:
         """
@@ -348,15 +348,15 @@
         if num_restrict_dims is not None:
             if num_restrict_dims == 1:
                 raise ValueError(f"If restricting to 1 dimension, then you should use UniDimSliceSampler.")
             if not (1 < num_restrict_dims <= model.U_ndims):
                 raise ValueError(f"Expected num_restriction dim in (1, {model.U_ndims}], got {num_restrict_dims}.")
         self.num_restrict_dims = num_restrict_dims
 
-    def preprocess(self, state: NestedSamplerState) -> PreProcessType:
+    def preprocess(self, state: NestedSamplerState, live_points: LivePoints) -> PreProcessType:
         return ()
 
     def _slice_bounds(self, key: PRNGKey, point_U0: FloatArray) -> Tuple[FloatArray, FloatArray]:
         """
         Get the slice bounds, randomly selecting which dimensions to slice in.
 
         Args:
```

### Comparing `jaxns-2.2.0/jaxns/static_uniform.py` & `jaxns-2.2.1/jaxns/uniform_samplers.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from jaxns.static_nested_sampler import PreProcessType, RejectionSampler
 from jaxns.types import NestedSamplerState, LivePoints, Sample, int_type
 
 __all__ = ['UniformSampler']
 
 
 class UniformSampler(RejectionSampler):
-    def preprocess(self, state: NestedSamplerState) -> PreProcessType:
+    def preprocess(self, state: NestedSamplerState, live_points: LivePoints) -> PreProcessType:
         return ()
 
     def get_sample(self, key: PRNGKey, log_L_constraint: FloatArray, live_points: LivePoints,
                    preprocess_data: PreProcessType) -> Sample:
         class CarryState(NamedTuple):
             done: BoolArray
             key: PRNGKey
@@ -58,15 +58,15 @@
 
 
 class BadUniformSampler(RejectionSampler):
     def __init__(self, mis_fraction: float, model: Model):
         super().__init__(model=model, efficiency_threshold=None)
         self.mis_fraction = mis_fraction
 
-    def preprocess(self, state: NestedSamplerState) -> PreProcessType:
+    def preprocess(self, state: NestedSamplerState, live_points: LivePoints) -> PreProcessType:
         return ()
 
     def get_sample(self, key: PRNGKey, log_L_constraint: FloatArray, live_points: LivePoints,
                    preprocess_data: PreProcessType) -> Sample:
         class CarryState(NamedTuple):
             done: BoolArray
             key: PRNGKey
```

### Comparing `jaxns-2.2.0/jaxns/statistics.py` & `jaxns-2.2.1/jaxns/statistics.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 from jax import numpy as jnp, tree_map
 from jax._src.lax.control_flow import while_loop
 from jax._src.lax.slicing import dynamic_update_slice
 
 from jaxns.internals.log_semiring import LogSpace
 from jaxns.types import EvidenceCalculation, SampleCollection, SampleStatistics, float_type, int_type, Reservoir
 
-__all__ = ['compute_evidence',
-           'analyse_sample_collection',
-           'compute_num_live_points_from_unit_threads']
+__all__ = [
+    'compute_evidence',
+    'analyse_sample_collection',
+    'compute_num_live_points_from_unit_threads'
+]
 
 
 def _init_evidence_calculation() -> EvidenceCalculation:
     """
     Returns an initial evidence calculation object.
 
     Returns:
@@ -90,14 +92,62 @@
 
     # next_evidence_calculation = tree_map(lambda old, new: jnp.where(jnp.isnan(new), old, new),
     #                                      evidence_calculation, next_evidence_calculation)
 
     return next_evidence_calculation
 
 
+def compute_evidence_no_stats(sample_collection: SampleCollection, num_live_points: FloatArray) \
+        -> EvidenceCalculation:
+    """
+    Compute the evidence by traversing the sample collection.
+
+    Args:
+        sample_collection: the sorted sample collection to use to calculate the evidence
+        num_live_points: the number of live points at each sample (see compute_num_live_points_from_unit_threads)
+
+    Returns:
+        evidence calculation
+    """
+    num_samples = sample_collection.sample_idx
+
+    CarryType = Tuple[EvidenceCalculation, IntArray, FloatArray]
+
+    def thread_cond(body_state: CarryType):
+        (evidence_calculation, idx, log_L_contour) = body_state
+        return idx < num_samples
+
+    def thread_body(body_state: CarryType) -> CarryType:
+        (evidence_calculation, idx, log_L_contour) = body_state
+        next_num_live_points = num_live_points[idx]
+        next_log_L = sample_collection.reservoir.log_L[idx]
+        next_log_L_contour = next_log_L
+        # Get log_dZ_mean, and log_X_mean
+        next_evidence_calculation = _update_evidence_calculation(
+            num_live_points=next_num_live_points,
+            log_L=log_L_contour,
+            next_log_L_contour=next_log_L,
+            evidence_calculation=evidence_calculation
+        )
+
+        next_idx = idx + jnp.ones_like(idx)
+        return (next_evidence_calculation, next_idx, next_log_L_contour)
+
+    initial_evidence_calculation = _init_evidence_calculation()
+    init_log_L_contour = sample_collection.reservoir.log_L_constraint[0]
+
+    (final_evidence_calculation, final_idx, final_log_L_contour) = while_loop(thread_cond,
+                                                                              thread_body,
+                                                                              (initial_evidence_calculation,
+                                                                               jnp.asarray(0, int_type),
+                                                                               init_log_L_contour))
+
+    return final_evidence_calculation
+
+
 def compute_evidence(sample_collection: SampleCollection, num_live_points: FloatArray) \
         -> Tuple[EvidenceCalculation, SampleStatistics]:
     """
     Compute the evidence by traversing the sample collection.
 
     Args:
         sample_collection: the sorted sample collection to use to calculate the evidence
```

### Comparing `jaxns-2.2.0/jaxns/termination.py` & `jaxns-2.2.1/jaxns/termination.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/tests/test_adaptive_refinement.py` & `jaxns-2.2.1/jaxns/tests/debug_adaptive_refinement.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,77 +1,78 @@
-# import tensorflow_probability.substrates.jax as tfp
-# from jax import random, numpy as jnp
-#
-# from jaxns import collect_samples
-# from jaxns.internals.log_semiring import LogSpace
-# from jaxns.model import Model
-# from jaxns.nested_sampler import ApproximateNestedSampler
-# from jaxns.prior import PriorModelGen, Prior
-# from jaxns.static_uniform import BadUniformSampler
-# from jaxns.tests.test_nested_sampler import compute_shrinkage_stats
-# from jaxns.types import TerminationCondition
-#
-# tfpd = tfp.distributions
-#
-#
-# def test_adaptive_refinement():
-#     n = 2
-#
-#     # Prior is uniform in U[0,1]
-#     # Likelihood is 1 - x**n
-#     # Z = 1 - 1/n+1
-#
-#     log_Z_true = jnp.log(1. - 1. / (n + 1))
-#     print(f"True log(Z): {log_Z_true}")
-#
-#     def prior_model() -> PriorModelGen:
-#         x = yield Prior(tfpd.Uniform(low=0, high=1))
-#         return x
-#
-#     def log_likelihood(x):
-#         return (LogSpace(0.) - LogSpace(n * jnp.log(x))).log_abs_val
-#
-#     def exact_X(L):
-#         return (1. - L) ** (1. / n)
-#
-#     def exact_L(X):
-#         return 1. - X ** n
-#
-#     model = Model(prior_model=prior_model,
-#                   log_likelihood=log_likelihood)
-#     ns = ApproximateNestedSampler(
-#         model=model,
-#         num_live_points=50,
-#         num_parallel_samplers=1,
-#         max_samples=1e6,
-#         sampler_chain=[
-#             BadUniformSampler(mis_fraction=0., model=model)
-#         ]
-#     )
-#
-#     total_state = None
-#     for seed in [42, 43, 44]:
-#         termination_reason, state = ns(random.PRNGKey(seed),
-#                                        term_cond=TerminationCondition(live_evidence_frac=1e-4))
-#         termination_reason.block_until_ready()
-#         if total_state is None:
-#             total_state = state
-#         else:
-#             total_state = collect_samples(state=total_state, new_reservoir=state.sample_collection.reservoir)
-#     results = ns.to_results(total_state, termination_reason)
-#     ns.summary(results)
-#     ns.plot_diagnostics(results)
-#
-#     # ensure there is no bug in control flow. X should be same to controlled evaluation
-#     log_X_mean, log_X_std = compute_shrinkage_stats(results.num_live_points_per_sample)
-#     assert jnp.allclose(results.log_X_mean, log_X_mean)
-#
-#     # ensure the deviation from the exact shrinkage is correct
-#     X_exact = exact_X(jnp.exp(results.log_L_samples))
-#
-#     rel_diff = jnp.abs(jnp.exp(log_X_mean) - X_exact) / jnp.exp(log_X_std)
-#
-#     # ensure log_Z is close to truth
-#     assert jnp.isclose(results.log_Z_mean, log_Z_true, atol=results.log_Z_uncert * 1.75)
-#
-#     print("Relative shrinkage errors", jnp.percentile(rel_diff, jnp.asarray([50, 75, 90, 95])))
-#     assert jnp.all(jnp.percentile(rel_diff, jnp.asarray([50, 75, 90, 95])) < jnp.asarray([0.9, 1.1, 1.4, 1.5]))
+import os
+
+os.environ["XLA_FLAGS"] = "--xla_force_host_platform_device_count=6"
+
+import jax
+import tensorflow_probability.substrates.jax as tfp
+from jax import random, numpy as jnp
+
+from jaxns.internals.log_semiring import LogSpace
+from jaxns.model import Model
+from jaxns.nested_sampler import ApproximateNestedSampler
+from jaxns.prior import PriorModelGen, Prior
+from jaxns.uniform_samplers import BadUniformSampler
+from jaxns.tests.test_nested_sampler import compute_shrinkage_stats
+from jaxns.types import TerminationCondition
+
+tfpd = tfp.distributions
+
+if __name__ == '__main__':
+    n = 2
+
+    # Prior is uniform in U[0,1]
+    # Likelihood is 1 - x**n
+    # Z = 1 - 1/n+1
+
+    log_Z_true = jnp.log(1. - 1. / (n + 1))
+    print(f"True log(Z): {log_Z_true}")
+
+
+    def prior_model() -> PriorModelGen:
+        x = yield Prior(tfpd.Uniform(low=0, high=1))
+        return x
+
+
+    def log_likelihood(x):
+        return (LogSpace(0.) - LogSpace(n * jnp.log(x))).log_abs_val
+
+
+    def exact_X(L):
+        return (1. - L) ** (1. / n)
+
+
+    def exact_L(X):
+        return 1. - X ** n
+
+
+    model = Model(
+        prior_model=prior_model,
+        log_likelihood=log_likelihood
+    )
+    ns = ApproximateNestedSampler(
+        model=model,
+        num_live_points=50,
+        num_parallel_samplers=len(jax.devices()),
+        max_samples=1e6,
+        sampler_chain=[
+            BadUniformSampler(mis_fraction=0.0, model=model)
+        ]
+    )
+
+
+
+    termination_reason, state = ns(random.PRNGKey(42),
+                                   term_cond=TerminationCondition(live_evidence_frac=1e-4))
+    results = ns.to_results(state, termination_reason)
+    ns.summary(results)
+    ns.plot_diagnostics(results)
+
+    # ensure there is no bug in control flow. X should be same to controlled evaluation
+    log_X_mean, log_X_std = compute_shrinkage_stats(results.num_live_points_per_sample)
+
+    # ensure the deviation from the exact shrinkage is correct
+    X_exact = exact_X(jnp.exp(results.log_L_samples))
+
+    rel_diff = jnp.abs(jnp.exp(log_X_mean) - X_exact) / jnp.exp(log_X_std)
+
+    # ensure log_Z is close to truth
+    assert jnp.isclose(results.log_Z_mean, log_Z_true, atol=results.log_Z_uncert * 1.75)
```

### Comparing `jaxns-2.2.0/jaxns/tests/test_initial_state.py` & `jaxns-2.2.1/jaxns/tests/test_initial_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from jax import numpy as jnp, vmap, random
 
 from jaxns import StaticNestedSampler, collect_samples
 from jaxns.initial_state import init_sample_collection, get_uniform_init_live_points, \
     get_live_points_from_samples
 from jaxns.model import Model
 from jaxns.prior import PriorModelGen, Prior
-from jaxns.static_uniform import UniformSampler
+from jaxns.uniform_samplers import UniformSampler
 from jaxns.types import NestedSamplerState, SampleCollection, TerminationCondition
 
 tfpd = tfp.distributions
 
 
 def test_init_sample_collection():
     def prior_model() -> PriorModelGen:
```

### Comparing `jaxns-2.2.0/jaxns/tests/test_nested_sampler.py` & `jaxns-2.2.1/jaxns/tests/test_nested_sampler.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 import pylab as plt
 import tensorflow_probability.substrates.jax as tfp
 from jax import random, numpy as jnp
 from jax._src.lax.control_flow import scan
 from jax._src.scipy.linalg import solve_triangular
 
+from jaxns import MultiellipsoidalSampler
 from jaxns.internals.log_semiring import LogSpace
 from jaxns.model import Model
 from jaxns.nested_sampler import ApproximateNestedSampler, ExactNestedSampler
 from jaxns.prior import PriorModelGen, Prior
-from jaxns.static_uniform import BadUniformSampler
 from jaxns.types import TerminationCondition, float_type
+from jaxns.uniform_samplers import BadUniformSampler, UniformSampler
 from jaxns.utils import sample_evidence, bruteforce_evidence
 
 tfpd = tfp.distributions
 
 
 class Timer:
     def __enter__(self):
@@ -199,14 +200,72 @@
     exact_ns.plot_diagnostics(results)
     actual_log_Z_mean = results.log_Z_mean
     expected_log_Z_mean = true_logZ
     tol = 1.75 * results.log_Z_uncert
     assert jnp.isclose(actual_log_Z_mean, expected_log_Z_mean, atol=tol)
 
 
+def test_nested_sampling_mvn_static_multiellipsoid_sampler():
+    def log_normal(x, mean, cov):
+        L = jnp.linalg.cholesky(cov)
+        dx = x - mean
+        dx = solve_triangular(L, dx, lower=True)
+        return -0.5 * x.size * jnp.log(2. * jnp.pi) - jnp.sum(jnp.log(jnp.diag(L))) \
+            - 0.5 * dx @ dx
+
+    ndims = 8
+    prior_mu = 15 * jnp.ones(ndims)
+    prior_cov = jnp.diag(jnp.ones(ndims)) ** 2
+
+    data_mu = jnp.zeros(ndims)
+    data_cov = jnp.diag(jnp.ones(ndims)) ** 2
+    data_cov = jnp.where(data_cov == 0., 0.99, data_cov)
+
+    true_logZ = log_normal(data_mu, prior_mu, prior_cov + data_cov)
+    # not super happy with this being 1.58 and being off by like 0.1. Probably related to the ESS.
+    post_mu = prior_cov @ jnp.linalg.inv(prior_cov + data_cov) @ data_mu + data_cov @ jnp.linalg.inv(
+        prior_cov + data_cov) @ prior_mu
+
+    print(f"True post mu:{post_mu}")
+    print(f"True log Z: {true_logZ}")
+
+    def prior_model() -> PriorModelGen:
+        x = yield Prior(
+            tfpd.MultivariateNormalTriL(loc=prior_mu, scale_tril=jnp.linalg.cholesky(prior_cov)),
+            name='x')
+        return x
+
+    def log_likelihood(x):
+        return log_normal(x, data_mu, data_cov)
+
+    model = Model(prior_model=prior_model, log_likelihood=log_likelihood)
+
+    # model.sanity_check(random.PRNGKey(42), S=100)
+    ns = ApproximateNestedSampler(
+        model=model,
+        num_live_points=100,
+        num_parallel_samplers=1,
+        max_samples=40000,
+        sampler_chain=[
+            UniformSampler(model=model, efficiency_threshold=0.1),
+            MultiellipsoidalSampler(model=model, efficiency_threshold=None, depth=0)
+        ]
+    )
+    with Timer():
+        termination_reason, state = ns(random.PRNGKey(41),
+                                             term_cond=TerminationCondition(live_evidence_frac=1e-5))
+        results = ns.to_results(state, termination_reason)
+        ns.summary(results)
+    ns.plot_diagnostics(results)
+    actual_log_Z_mean = results.log_Z_mean
+    expected_log_Z_mean = true_logZ
+    tol = 1.75 * results.log_Z_uncert
+    assert jnp.isclose(actual_log_Z_mean, expected_log_Z_mean, atol=tol)
+
+
 # def test_multi_needs_fewer_slices():
 #     def log_normal(x, mean, cov):
 #         L = jnp.linalg.cholesky(cov)
 #         dx = x - mean
 #         dx = solve_triangular(L, dx, lower=True)
 #         return -0.5 * x.size * jnp.log(2. * jnp.pi) - jnp.sum(jnp.log(jnp.diag(L))) - 0.5 * dx @ dx
 #
```

### Comparing `jaxns-2.2.0/jaxns/tests/test_prior.py` & `jaxns-2.2.1/jaxns/tests/test_prior.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/tests/test_random.py` & `jaxns-2.2.1/jaxns/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/tests/test_statistics.py` & `jaxns-2.2.1/jaxns/tests/test_statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from jax import numpy as jnp, random, tree_map
 from jax import vmap
 from jax.lax import dynamic_update_slice
 
 from jaxns import TerminationCondition, Reservoir, ApproximateNestedSampler, Model, Prior, PriorModelGen
 from jaxns.internals.log_semiring import LogSpace
 from jaxns.internals.maps import replace_index
-from jaxns.static_uniform import BadUniformSampler
+from jaxns.uniform_samplers import BadUniformSampler
 from jaxns.statistics import compute_num_live_points_from_unit_threads, compute_remaining_evidence, \
     perfect_live_point_computation_jax, fast_perfect_live_point_computation_jax, fast_triu_rowsum, combine_reservoirs
 
 tfpd = tfp.distributions
 
 
 def _sure_compute_num_live_points_from_unit_threads(log_L_constraints, log_L_samples, num_samples=None, debug=False):
```

### Comparing `jaxns-2.2.0/jaxns/types.py` & `jaxns-2.2.1/jaxns/types.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/utils.py` & `jaxns-2.2.1/jaxns/utils.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns/warnings.py` & `jaxns-2.2.1/jaxns/warnings.py`

 * *Files identical despite different names*

### Comparing `jaxns-2.2.0/jaxns.egg-info/PKG-INFO` & `jaxns-2.2.1/jaxns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxns
-Version: 2.2.0
+Version: 2.2.1
 Summary: Nested Sampling in JAX
 Home-page: https://github.com/joshuaalbert/jaxns
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jaxns-2.2.0/setup.py` & `jaxns-2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 setup_requires = ['jax>=' + __minimum_jax_version__]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='jaxns',
-      version='2.2.0',
+      version='2.2.1',
       description='Nested Sampling in JAX',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/joshuaalbert/jaxns",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=setup_requires,
```

