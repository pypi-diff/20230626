# Comparing `tmp/fasttreeshap-0.1.5.tar.gz` & `tmp/fasttreeshap-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasttreeshap-0.1.5.tar", last modified: Wed Jun 14 06:36:21 2023, max compression
+gzip compressed data, was "fasttreeshap-0.1.6.tar", last modified: Mon Jun 26 03:54:55 2023, max compression
```

## Comparing `fasttreeshap-0.1.5.tar` & `fasttreeshap-0.1.6.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.727641 fasttreeshap-0.1.5/
--rw-r--r--   0 jlyang   (26356) staff       (20)     1315 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/LICENSE
--rw-r--r--   0 jlyang   (26356) staff       (20)       31 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/MANIFEST.in
--rw-r--r--   0 jlyang   (26356) staff       (20)      301 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/NOTICE
--rw-r--r--   0 jlyang   (26356) staff       (20)     1149 2023-06-14 06:36:21.726746 fasttreeshap-0.1.5/PKG-INFO
--rw-r--r--   0 jlyang   (26356) staff       (20)    12973 2022-10-20 10:28:10.000000 fasttreeshap-0.1.5/README.md
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.643332 fasttreeshap-0.1.5/fasttreeshap/
--rw-r--r--   0 jlyang   (26356) staff       (20)     2154 2023-06-14 06:34:38.000000 fasttreeshap-0.1.5/fasttreeshap/__init__.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    31324 2023-05-18 05:47:46.000000 fasttreeshap-0.1.5/fasttreeshap/_explanation.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     8702 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/_serializable.py
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.650435 fasttreeshap-0.1.5/fasttreeshap/cext/
--rw-r--r--   0 jlyang   (26356) staff       (20)    25950 2021-12-22 23:39:22.000000 fasttreeshap-0.1.5/fasttreeshap/cext/_cext.cc
--rw-r--r--   0 jlyang   (26356) staff       (20)    96965 2022-01-26 19:51:12.000000 fasttreeshap-0.1.5/fasttreeshap/cext/tree_shap.h
--rw-r--r--   0 jlyang   (26356) staff       (20)     9105 2023-05-18 05:47:46.000000 fasttreeshap-0.1.5/fasttreeshap/datasets.py
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.654719 fasttreeshap-0.1.5/fasttreeshap/explainers/
--rw-r--r--   0 jlyang   (26356) staff       (20)       23 2022-01-26 19:51:12.000000 fasttreeshap-0.1.5/fasttreeshap/explainers/__init__.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    16708 2023-05-18 05:47:46.000000 fasttreeshap-0.1.5/fasttreeshap/explainers/_explainer.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    98158 2023-05-18 05:47:46.000000 fasttreeshap-0.1.5/fasttreeshap/explainers/_tree.py
--rw-r--r--   0 jlyang   (26356) staff       (20)      433 2023-06-14 06:34:15.000000 fasttreeshap-0.1.5/fasttreeshap/links.py
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.665366 fasttreeshap-0.1.5/fasttreeshap/maskers/
--rw-r--r--   0 jlyang   (26356) staff       (20)      283 2021-12-22 23:04:49.000000 fasttreeshap-0.1.5/fasttreeshap/maskers/__init__.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     5144 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/maskers/_composite.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     1008 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/maskers/_fixed.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     2401 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/maskers/_fixed_composite.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     8218 2023-05-18 05:47:46.000000 fasttreeshap-0.1.5/fasttreeshap/maskers/_image.py
--rw-r--r--   0 jlyang   (26356) staff       (20)      753 2023-05-18 05:47:46.000000 fasttreeshap-0.1.5/fasttreeshap/maskers/_masker.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     2672 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/maskers/_output_composite.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    14014 2023-06-14 06:34:15.000000 fasttreeshap-0.1.5/fasttreeshap/maskers/_tabular.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    21420 2023-05-18 05:47:46.000000 fasttreeshap-0.1.5/fasttreeshap/maskers/_text.py
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.668428 fasttreeshap-0.1.5/fasttreeshap/models/
--rw-r--r--   0 jlyang   (26356) staff       (20)       26 2022-01-26 19:51:12.000000 fasttreeshap-0.1.5/fasttreeshap/models/__init__.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     1178 2021-12-21 08:43:12.000000 fasttreeshap-0.1.5/fasttreeshap/models/_model.py
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.695413 fasttreeshap-0.1.5/fasttreeshap/plots/
--rw-r--r--   0 jlyang   (26356) staff       (20)      512 2021-12-20 22:31:41.000000 fasttreeshap-0.1.5/fasttreeshap/plots/__init__.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    17284 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_bar.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    41053 2023-05-18 06:03:46.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_beeswarm.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     8827 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_benchmark.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    25998 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_decision.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     2813 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_embedding.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    19403 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_force.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    14787 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_force_matplotlib.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     3121 2023-05-18 05:47:46.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_group_difference.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     6392 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_heatmap.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    24258 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_image.py
--rw-r--r--   0 jlyang   (26356) staff       (20)      608 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_labels.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     2825 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_monitoring.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     9521 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_partial_dependence.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    32609 2023-05-18 06:04:06.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_scatter.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    58223 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_text.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     7616 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_utils.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    23938 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_violin.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    26292 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/_waterfall.py
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.701339 fasttreeshap-0.1.5/fasttreeshap/plots/colors/
--rw-r--r--   0 jlyang   (26356) staff       (20)      262 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/colors/__init__.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    36759 2023-05-30 19:28:57.000000 fasttreeshap-0.1.5/fasttreeshap/plots/colors/_colorconv.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     5096 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/colors/_colors.py
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.709052 fasttreeshap-0.1.5/fasttreeshap/plots/resources/
--rw-r--r--   0 jlyang   (26356) staff       (20)   370829 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/resources/bundle.js
--rw-r--r--   0 jlyang   (26356) staff       (20)      570 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/plots/resources/logoSmallGray.png
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.725118 fasttreeshap-0.1.5/fasttreeshap/utils/
--rw-r--r--   0 jlyang   (26356) staff       (20)      449 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/utils/__init__.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     8514 2023-06-14 06:34:15.000000 fasttreeshap-0.1.5/fasttreeshap/utils/_clustering.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    10640 2023-05-18 05:47:46.000000 fasttreeshap-0.1.5/fasttreeshap/utils/_general.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     2576 2021-12-22 23:06:09.000000 fasttreeshap-0.1.5/fasttreeshap/utils/_keras.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     7329 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/utils/_legacy.py
--rw-r--r--   0 jlyang   (26356) staff       (20)    20513 2023-06-14 06:34:15.000000 fasttreeshap-0.1.5/fasttreeshap/utils/_masked_model.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     1227 2021-11-05 18:22:53.000000 fasttreeshap-0.1.5/fasttreeshap/utils/_show_progress.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     5552 2021-12-22 23:06:09.000000 fasttreeshap-0.1.5/fasttreeshap/utils/image.py
--rw-r--r--   0 jlyang   (26356) staff       (20)     6494 2021-12-22 23:06:09.000000 fasttreeshap-0.1.5/fasttreeshap/utils/transformers.py
-drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-14 06:36:21.647973 fasttreeshap-0.1.5/fasttreeshap.egg-info/
--rwx------   0 jlyang   (26356) staff       (20)     1149 2023-06-14 06:36:21.000000 fasttreeshap-0.1.5/fasttreeshap.egg-info/PKG-INFO
--rwx------   0 jlyang   (26356) staff       (20)     2045 2023-06-14 06:36:21.000000 fasttreeshap-0.1.5/fasttreeshap.egg-info/SOURCES.txt
--rwx------   0 jlyang   (26356) staff       (20)        1 2023-06-14 06:36:21.000000 fasttreeshap-0.1.5/fasttreeshap.egg-info/dependency_links.txt
--rwx------   0 jlyang   (26356) staff       (20)        1 2021-11-04 04:21:15.000000 fasttreeshap-0.1.5/fasttreeshap.egg-info/not-zip-safe
--rwx------   0 jlyang   (26356) staff       (20)      526 2023-06-14 06:36:21.000000 fasttreeshap-0.1.5/fasttreeshap.egg-info/requires.txt
--rwx------   0 jlyang   (26356) staff       (20)       13 2023-06-14 06:36:21.000000 fasttreeshap-0.1.5/fasttreeshap.egg-info/top_level.txt
--rw-r--r--   0 jlyang   (26356) staff       (20)      115 2023-05-18 18:21:26.000000 fasttreeshap-0.1.5/pyproject.toml
--rw-r--r--   0 jlyang   (26356) staff       (20)       38 2023-06-14 06:36:21.727887 fasttreeshap-0.1.5/setup.cfg
--rw-r--r--   0 jlyang   (26356) staff       (20)     8524 2023-05-18 18:27:08.000000 fasttreeshap-0.1.5/setup.py
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-26 03:54:55.478835 fasttreeshap-0.1.6/
+-rw-r--r--   0 jlyang   (26356) staff       (20)     1315 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/LICENSE
+-rw-r--r--   0 jlyang   (26356) staff       (20)       31 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/MANIFEST.in
+-rw-r--r--   0 jlyang   (26356) staff       (20)      301 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/NOTICE
+-rw-r--r--   0 jlyang   (26356) staff       (20)     1149 2023-06-26 03:54:55.478102 fasttreeshap-0.1.6/PKG-INFO
+-rw-r--r--   0 jlyang   (26356) staff       (20)    12973 2022-10-20 10:28:10.000000 fasttreeshap-0.1.6/README.md
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-26 03:54:55.401494 fasttreeshap-0.1.6/fasttreeshap/
+-rw-r--r--   0 jlyang   (26356) staff       (20)     2154 2023-06-26 03:40:16.000000 fasttreeshap-0.1.6/fasttreeshap/__init__.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    31324 2023-05-18 05:47:46.000000 fasttreeshap-0.1.6/fasttreeshap/_explanation.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     8702 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/_serializable.py
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-26 03:54:55.408619 fasttreeshap-0.1.6/fasttreeshap/cext/
+-rw-r--r--   0 jlyang   (26356) staff       (20)    25950 2021-12-22 23:39:22.000000 fasttreeshap-0.1.6/fasttreeshap/cext/_cext.cc
+-rw-r--r--   0 jlyang   (26356) staff       (20)    96965 2022-01-26 19:51:12.000000 fasttreeshap-0.1.6/fasttreeshap/cext/tree_shap.h
+-rw-r--r--   0 jlyang   (26356) staff       (20)     9105 2023-05-18 05:47:46.000000 fasttreeshap-0.1.6/fasttreeshap/datasets.py
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-26 03:54:55.412358 fasttreeshap-0.1.6/fasttreeshap/explainers/
+-rw-r--r--   0 jlyang   (26356) staff       (20)       23 2022-01-26 19:51:12.000000 fasttreeshap-0.1.6/fasttreeshap/explainers/__init__.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    16708 2023-05-18 05:47:46.000000 fasttreeshap-0.1.6/fasttreeshap/explainers/_explainer.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    98155 2023-06-26 03:39:39.000000 fasttreeshap-0.1.6/fasttreeshap/explainers/_tree.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)      433 2023-06-14 06:34:15.000000 fasttreeshap-0.1.6/fasttreeshap/links.py
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-26 03:54:55.425387 fasttreeshap-0.1.6/fasttreeshap/maskers/
+-rw-r--r--   0 jlyang   (26356) staff       (20)      283 2021-12-22 23:04:49.000000 fasttreeshap-0.1.6/fasttreeshap/maskers/__init__.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     5144 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/maskers/_composite.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     1008 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/maskers/_fixed.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     2401 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/maskers/_fixed_composite.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     8218 2023-05-18 05:47:46.000000 fasttreeshap-0.1.6/fasttreeshap/maskers/_image.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)      753 2023-05-18 05:47:46.000000 fasttreeshap-0.1.6/fasttreeshap/maskers/_masker.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     2672 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/maskers/_output_composite.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    14014 2023-06-14 06:34:15.000000 fasttreeshap-0.1.6/fasttreeshap/maskers/_tabular.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    21420 2023-05-18 05:47:46.000000 fasttreeshap-0.1.6/fasttreeshap/maskers/_text.py
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-26 03:54:55.429408 fasttreeshap-0.1.6/fasttreeshap/models/
+-rw-r--r--   0 jlyang   (26356) staff       (20)       26 2022-01-26 19:51:12.000000 fasttreeshap-0.1.6/fasttreeshap/models/__init__.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     1178 2021-12-21 08:43:12.000000 fasttreeshap-0.1.6/fasttreeshap/models/_model.py
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-26 03:54:55.455335 fasttreeshap-0.1.6/fasttreeshap/plots/
+-rw-r--r--   0 jlyang   (26356) staff       (20)      512 2021-12-20 22:31:41.000000 fasttreeshap-0.1.6/fasttreeshap/plots/__init__.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    17284 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/plots/_bar.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    41053 2023-05-18 06:03:46.000000 fasttreeshap-0.1.6/fasttreeshap/plots/_beeswarm.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     8827 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/plots/_benchmark.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    25998 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/plots/_decision.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     2813 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/plots/_embedding.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    19403 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/plots/_force.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    14787 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/plots/_force_matplotlib.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     3121 2023-05-18 05:47:46.000000 fasttreeshap-0.1.6/fasttreeshap/plots/_group_difference.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     6392 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/plots/_heatmap.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    24258 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/plots/_image.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)      608 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/plots/_labels.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     2825 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/plots/_monitoring.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     9521 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/plots/_partial_dependence.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    32609 2023-05-18 06:04:06.000000 fasttreeshap-0.1.6/fasttreeshap/plots/_scatter.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    58223 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/plots/_text.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     7616 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/plots/_utils.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    23938 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/plots/_violin.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    26292 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/plots/_waterfall.py
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-26 03:54:55.459589 fasttreeshap-0.1.6/fasttreeshap/plots/colors/
+-rw-r--r--   0 jlyang   (26356) staff       (20)      262 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/plots/colors/__init__.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    36759 2023-05-30 19:28:57.000000 fasttreeshap-0.1.6/fasttreeshap/plots/colors/_colorconv.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     5096 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/plots/colors/_colors.py
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-26 03:54:55.464496 fasttreeshap-0.1.6/fasttreeshap/plots/resources/
+-rw-r--r--   0 jlyang   (26356) staff       (20)   370829 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/plots/resources/bundle.js
+-rw-r--r--   0 jlyang   (26356) staff       (20)      570 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/plots/resources/logoSmallGray.png
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-26 03:54:55.476775 fasttreeshap-0.1.6/fasttreeshap/utils/
+-rw-r--r--   0 jlyang   (26356) staff       (20)      449 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/utils/__init__.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     8514 2023-06-14 06:34:15.000000 fasttreeshap-0.1.6/fasttreeshap/utils/_clustering.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    10640 2023-05-18 05:47:46.000000 fasttreeshap-0.1.6/fasttreeshap/utils/_general.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     2576 2021-12-22 23:06:09.000000 fasttreeshap-0.1.6/fasttreeshap/utils/_keras.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     7329 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/utils/_legacy.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)    20513 2023-06-14 06:34:15.000000 fasttreeshap-0.1.6/fasttreeshap/utils/_masked_model.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     1227 2021-11-05 18:22:53.000000 fasttreeshap-0.1.6/fasttreeshap/utils/_show_progress.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     5552 2021-12-22 23:06:09.000000 fasttreeshap-0.1.6/fasttreeshap/utils/image.py
+-rw-r--r--   0 jlyang   (26356) staff       (20)     6494 2021-12-22 23:06:09.000000 fasttreeshap-0.1.6/fasttreeshap/utils/transformers.py
+drwxr-xr-x   0 jlyang   (26356) staff       (20)        0 2023-06-26 03:54:55.406334 fasttreeshap-0.1.6/fasttreeshap.egg-info/
+-rwx------   0 jlyang   (26356) staff       (20)     1149 2023-06-26 03:54:55.000000 fasttreeshap-0.1.6/fasttreeshap.egg-info/PKG-INFO
+-rwx------   0 jlyang   (26356) staff       (20)     2045 2023-06-26 03:54:55.000000 fasttreeshap-0.1.6/fasttreeshap.egg-info/SOURCES.txt
+-rwx------   0 jlyang   (26356) staff       (20)        1 2023-06-26 03:54:55.000000 fasttreeshap-0.1.6/fasttreeshap.egg-info/dependency_links.txt
+-rwx------   0 jlyang   (26356) staff       (20)        1 2021-11-04 04:21:15.000000 fasttreeshap-0.1.6/fasttreeshap.egg-info/not-zip-safe
+-rwx------   0 jlyang   (26356) staff       (20)      526 2023-06-26 03:54:55.000000 fasttreeshap-0.1.6/fasttreeshap.egg-info/requires.txt
+-rwx------   0 jlyang   (26356) staff       (20)       13 2023-06-26 03:54:55.000000 fasttreeshap-0.1.6/fasttreeshap.egg-info/top_level.txt
+-rw-r--r--   0 jlyang   (26356) staff       (20)      115 2023-05-18 18:21:26.000000 fasttreeshap-0.1.6/pyproject.toml
+-rw-r--r--   0 jlyang   (26356) staff       (20)       38 2023-06-26 03:54:55.479088 fasttreeshap-0.1.6/setup.cfg
+-rw-r--r--   0 jlyang   (26356) staff       (20)     8524 2023-05-18 18:27:08.000000 fasttreeshap-0.1.6/setup.py
```

### Comparing `fasttreeshap-0.1.5/LICENSE` & `fasttreeshap-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/PKG-INFO` & `fasttreeshap-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasttreeshap
-Version: 0.1.5
+Version: 0.1.6
 Summary: A fast implementation of TreeSHAP algorithm.
 Home-page: http://github.com/linkedin/fasttreeshap
 Author: Jilei Yang
 Author-email: jlyang0712@gmail.com
 License: BSD 2-CLAUSE
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
```

### Comparing `fasttreeshap-0.1.5/README.md` & `fasttreeshap-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/__init__.py` & `fasttreeshap-0.1.6/fasttreeshap/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # flake8: noqa
 
 import warnings
 import sys
 
-__version__ = '0.1.5'
+__version__ = '0.1.6'
 
 # check python version
 if (sys.version_info < (3, 0)):
     warnings.warn("fasttreeshap only supports Python 3 (not 2)!")
 
 from ._explanation import Explanation, Cohorts
```

### Comparing `fasttreeshap-0.1.5/fasttreeshap/_explanation.py` & `fasttreeshap-0.1.6/fasttreeshap/_explanation.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/_serializable.py` & `fasttreeshap-0.1.6/fasttreeshap/_serializable.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/cext/_cext.cc` & `fasttreeshap-0.1.6/fasttreeshap/cext/_cext.cc`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/cext/tree_shap.h` & `fasttreeshap-0.1.6/fasttreeshap/cext/tree_shap.h`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/datasets.py` & `fasttreeshap-0.1.6/fasttreeshap/datasets.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/explainers/_explainer.py` & `fasttreeshap-0.1.6/fasttreeshap/explainers/_explainer.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/explainers/_tree.py` & `fasttreeshap-0.1.6/fasttreeshap/explainers/_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1589,15 +1589,15 @@
                 self.node_sindex[-1][j] = self.read('I')
                 self.node_info[-1][j] = self.read('f')
 
             # load the stat nodes
             self.loss_chg.append(np.zeros(self.num_nodes[i], dtype=np.float32))
             self.sum_hess.append(np.zeros(self.num_nodes[i], dtype=np.float32))
             self.base_weight.append(np.zeros(self.num_nodes[i], dtype=np.float32))
-            self.leaf_child_cnt.append(np.zeros(self.num_nodes[i], dtype=np.int))
+            self.leaf_child_cnt.append(np.zeros(self.num_nodes[i], dtype=int))
             for j in range(self.num_nodes[i]):
                 self.loss_chg[-1][j] = self.read('f')
                 self.sum_hess[-1][j] = self.read('f')
                 self.base_weight[-1][j] = self.read('f')
                 self.leaf_child_cnt[-1][j] = self.read('i')
 
     def get_trees(self, data=None, data_missing=None):
```

### Comparing `fasttreeshap-0.1.5/fasttreeshap/maskers/_composite.py` & `fasttreeshap-0.1.6/fasttreeshap/maskers/_composite.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/maskers/_fixed.py` & `fasttreeshap-0.1.6/fasttreeshap/maskers/_fixed.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/maskers/_fixed_composite.py` & `fasttreeshap-0.1.6/fasttreeshap/maskers/_fixed_composite.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/maskers/_image.py` & `fasttreeshap-0.1.6/fasttreeshap/maskers/_image.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/maskers/_masker.py` & `fasttreeshap-0.1.6/fasttreeshap/maskers/_masker.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/maskers/_output_composite.py` & `fasttreeshap-0.1.6/fasttreeshap/maskers/_output_composite.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/maskers/_tabular.py` & `fasttreeshap-0.1.6/fasttreeshap/maskers/_tabular.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/maskers/_text.py` & `fasttreeshap-0.1.6/fasttreeshap/maskers/_text.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/models/_model.py` & `fasttreeshap-0.1.6/fasttreeshap/models/_model.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/__init__.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/_bar.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/_bar.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/_beeswarm.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/_beeswarm.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/_benchmark.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/_benchmark.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/_decision.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/_decision.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/_embedding.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/_embedding.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/_force.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/_force.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/_force_matplotlib.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/_force_matplotlib.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/_group_difference.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/_group_difference.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/_heatmap.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/_heatmap.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/_image.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/_image.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/_labels.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/_labels.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/_monitoring.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/_monitoring.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/_partial_dependence.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/_partial_dependence.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/_scatter.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/_scatter.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/_text.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/_text.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/_utils.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/_utils.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/_violin.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/_violin.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/_waterfall.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/_waterfall.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/colors/_colorconv.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/colors/_colorconv.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/colors/_colors.py` & `fasttreeshap-0.1.6/fasttreeshap/plots/colors/_colors.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/resources/bundle.js` & `fasttreeshap-0.1.6/fasttreeshap/plots/resources/bundle.js`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/plots/resources/logoSmallGray.png` & `fasttreeshap-0.1.6/fasttreeshap/plots/resources/logoSmallGray.png`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/utils/_clustering.py` & `fasttreeshap-0.1.6/fasttreeshap/utils/_clustering.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/utils/_general.py` & `fasttreeshap-0.1.6/fasttreeshap/utils/_general.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/utils/_keras.py` & `fasttreeshap-0.1.6/fasttreeshap/utils/_keras.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/utils/_legacy.py` & `fasttreeshap-0.1.6/fasttreeshap/utils/_legacy.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/utils/_masked_model.py` & `fasttreeshap-0.1.6/fasttreeshap/utils/_masked_model.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/utils/_show_progress.py` & `fasttreeshap-0.1.6/fasttreeshap/utils/_show_progress.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/utils/image.py` & `fasttreeshap-0.1.6/fasttreeshap/utils/image.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap/utils/transformers.py` & `fasttreeshap-0.1.6/fasttreeshap/utils/transformers.py`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap.egg-info/PKG-INFO` & `fasttreeshap-0.1.6/fasttreeshap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasttreeshap
-Version: 0.1.5
+Version: 0.1.6
 Summary: A fast implementation of TreeSHAP algorithm.
 Home-page: http://github.com/linkedin/fasttreeshap
 Author: Jilei Yang
 Author-email: jlyang0712@gmail.com
 License: BSD 2-CLAUSE
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
```

### Comparing `fasttreeshap-0.1.5/fasttreeshap.egg-info/SOURCES.txt` & `fasttreeshap-0.1.6/fasttreeshap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fasttreeshap-0.1.5/fasttreeshap.egg-info/requires.txt` & `fasttreeshap-0.1.6/fasttreeshap.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -7,33 +7,33 @@
 slicer==0.0.7
 numba
 cloudpickle
 psutil
 shap
 
 [all]
-xgboost
 pyspark
+sentencepiece
 transformers
-sphinx_rtd_theme
-catboost
+torch
+lime
+pytest-cov
+pytest-mpl
+opencv-python
 nbsphinx
 ipython
-numpydoc
-pytest-mpl
-matplotlib
 pyod
+matplotlib
+catboost
+xgboost
 sphinx
-lime
-opencv-python
-pytest-cov
-sentencepiece
-lightgbm
+numpydoc
 pytest
-torch
+lightgbm
+sphinx_rtd_theme
 
 [docs]
 matplotlib
 ipython
 numpydoc
 sphinx_rtd_theme
 sphinx
```

### Comparing `fasttreeshap-0.1.5/setup.py` & `fasttreeshap-0.1.6/setup.py`

 * *Files identical despite different names*

