# Comparing `tmp/XPER-0.0.8.tar.gz` & `tmp/XPER-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XPER-0.0.8.tar", last modified: Fri Jun 23 06:27:25 2023, max compression
+gzip compressed data, was "XPER-0.0.9.tar", last modified: Fri Jun 23 06:38:18 2023, max compression
```

## Comparing `XPER-0.0.8.tar` & `XPER-0.0.9.tar`

### file list

```diff
@@ -1,242 +1,242 @@
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.761688 XPER-0.0.8/
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     8196 2023-06-09 15:56:03.000000 XPER-0.0.8/.DS_Store
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     1799 2023-04-17 07:42:16.000000 XPER-0.0.8/.gitignore
--rw-r--r--   0 gaetanbrison   (501) staff       (20)        0 2023-05-30 07:41:57.000000 XPER-0.0.8/History.rst
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     1249 2023-06-21 12:05:00.000000 XPER-0.0.8/LICENSE
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     1208 2023-06-23 06:27:25.761122 XPER-0.0.8/PKG-INFO
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    23816 2023-06-13 09:26:29.000000 XPER-0.0.8/README.html
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     3513 2023-06-21 12:05:00.000000 XPER-0.0.8/README.md
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.379372 XPER-0.0.8/XPER/
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      120 2023-06-22 08:23:17.000000 XPER-0.0.8/XPER/__init__.py
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.392613 XPER-0.0.8/XPER/compute/
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    15236 2023-06-22 08:23:17.000000 XPER-0.0.8/XPER/compute/EM.py
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    21359 2023-06-15 11:52:56.000000 XPER-0.0.8/XPER/compute/Optimisation.py
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     8208 2023-06-22 12:13:54.000000 XPER-0.0.8/XPER/compute/Performance.py
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     5176 2023-06-22 06:08:21.000000 XPER-0.0.8/XPER/compute/XGBoost_model.py
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      165 2023-06-22 08:23:17.000000 XPER-0.0.8/XPER/compute/__init__.py
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.479613 XPER-0.0.8/XPER/datasets/
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    35735 2023-06-10 09:03:03.000000 XPER-0.0.8/XPER/datasets/BostonHousing.csv
--rw-r--r--   0 gaetanbrison   (501) staff       (20)       72 2023-06-09 13:57:09.000000 XPER-0.0.8/XPER/datasets/__init__.py
--rw-r--r--   0 gaetanbrison   (501) staff       (20)  3974305 2023-06-13 08:34:01.000000 XPER-0.0.8/XPER/datasets/adult.data
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      315 2023-06-13 08:34:01.000000 XPER-0.0.8/XPER/datasets/load_data.py
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2772 2023-06-21 12:36:00.000000 XPER-0.0.8/XPER/datasets/sample.py
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.482375 XPER-0.0.8/XPER/viz/
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    24995 2023-06-23 06:23:46.000000 XPER-0.0.8/XPER/viz/Visualisation.py
--rw-r--r--   0 gaetanbrison   (501) staff       (20)       36 2023-06-13 08:44:48.000000 XPER-0.0.8/XPER/viz/__init__.py
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.483202 XPER-0.0.8/XPER/viz/figures/
--rw-rw-r--   0 gaetanbrison   (501) staff       (20)    57106 2023-06-08 14:29:51.000000 XPER-0.0.8/XPER/viz/figures/force_plot.pdf
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.385557 XPER-0.0.8/XPER.egg-info/
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     1208 2023-06-23 06:27:25.000000 XPER-0.0.8/XPER.egg-info/PKG-INFO
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     6751 2023-06-23 06:27:25.000000 XPER-0.0.8/XPER.egg-info/SOURCES.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)        1 2023-06-23 06:27:25.000000 XPER-0.0.8/XPER.egg-info/dependency_links.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)        1 2023-06-05 11:34:15.000000 XPER-0.0.8/XPER.egg-info/not-zip-safe
--rw-r--r--   0 gaetanbrison   (501) staff       (20)       88 2023-06-23 06:27:25.000000 XPER-0.0.8/XPER.egg-info/requires.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)        5 2023-06-23 06:27:25.000000 XPER-0.0.8/XPER.egg-info/top_level.txt
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.502920 XPER-0.0.8/docs/
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      100 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/Beta.rst
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      120 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/Beta_model.rst
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      146 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/Beta_not_optimized.rst
--rw-r--r--   0 gaetanbrison   (501) staff       (20)       94 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/EM.rst
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      634 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/Makefile
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      117 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/OLS_model.rst
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      124 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/Optimisation.rst
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      106 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/Probit.rst
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      126 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/Probit_model.rst
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      127 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/Visualisation.rst
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      109 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/XGBoost.rst
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      129 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/XGBoost_model.rst
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      100 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/XPER.rst
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      114 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/XPER_OLS.rst
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      126 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/XPER_XGBoost.rst
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      146 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/XPER_empirical_app.rst
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.355153 XPER-0.0.8/docs/_build/
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.538145 XPER-0.0.8/docs/_build/doctrees/
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2379 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/doctrees/Beta.doctree
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2411 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/doctrees/Beta_model.doctree
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2453 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/doctrees/Beta_not_optimized.doctree
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2369 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/doctrees/EM.doctree
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2406 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/doctrees/OLS_model.doctree
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2419 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/doctrees/Optimisation.doctree
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2389 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/doctrees/Probit.doctree
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2421 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/doctrees/Probit_model.doctree
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2424 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/doctrees/Visualisation.doctree
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2394 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/doctrees/XGBoost.doctree
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2426 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/doctrees/XGBoost_model.doctree
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2379 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/doctrees/XPER.doctree
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2401 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/doctrees/XPER_OLS.doctree
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2421 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/doctrees/XPER_XGBoost.doctree
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2453 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/doctrees/XPER_empirical_app.doctree
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    49197 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/doctrees/environment.pickle
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     4926 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/doctrees/index.doctree
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2937 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/doctrees/modules.doctree
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.561209 XPER-0.0.8/docs/_build/html/
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     3678 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/Beta.html
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     3720 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/Beta_model.html
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     3776 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/Beta_not_optimized.html
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     3664 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/EM.html
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     3713 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/OLS_model.html
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     3734 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/Optimisation.html
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     3692 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/Probit.html
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     3734 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/Probit_model.html
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     3741 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/Visualisation.html
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     3699 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/XGBoost.html
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     3741 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/XGBoost_model.html
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     3678 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/XPER.html
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     3706 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/XPER_OLS.html
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     3734 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/XPER_XGBoost.html
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     3776 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/XPER_empirical_app.html
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.579530 XPER-0.0.8/docs/_build/html/_sources/
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      100 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_sources/Beta.rst.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      120 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_sources/Beta_model.rst.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      146 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_sources/Beta_not_optimized.rst.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)       94 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_sources/EM.rst.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      117 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_sources/OLS_model.rst.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      124 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_sources/Optimisation.rst.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      106 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_sources/Probit.rst.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      126 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_sources/Probit_model.rst.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      127 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_sources/Visualisation.rst.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      109 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_sources/XGBoost.rst.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      129 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_sources/XGBoost_model.rst.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      100 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_sources/XPER.rst.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      114 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_sources/XPER_OLS.rst.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      126 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_sources/XPER_XGBoost.rst.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      146 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_sources/XPER_empirical_app.rst.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      428 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      249 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_sources/modules.rst.txt
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.600898 XPER-0.0.8/docs/_build/html/_static/
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     4289 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    14813 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.602754 XPER-0.0.8/docs/_build/html/_static/css/
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     3229 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/css/badge_only.css
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.659923 XPER-0.0.8/docs/_build/html/_static/css/fonts/
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    87624 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    67312 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    86288 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    66444 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 gaetanbrison   (501) staff       (20)   165742 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 gaetanbrison   (501) staff       (20)   444379 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 gaetanbrison   (501) staff       (20)   165548 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    98024 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    77160 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 gaetanbrison   (501) staff       (20)   323344 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 gaetanbrison   (501) staff       (20)   193308 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 gaetanbrison   (501) staff       (20)   309728 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 gaetanbrison   (501) staff       (20)   184912 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 gaetanbrison   (501) staff       (20)   328412 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 gaetanbrison   (501) staff       (20)   195704 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 gaetanbrison   (501) staff       (20)   309192 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 gaetanbrison   (501) staff       (20)   182708 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 gaetanbrison   (501) staff       (20)   135235 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/css/theme.css
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     4472 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/doctools.js
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      420 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      286 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/file.png
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    89501 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/jquery.js
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.669141 XPER-0.0.8/docs/_build/html/_static/js/
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      934 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     4370 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2734 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     5023 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/js/theme.js
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     4758 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/language_data.js
--rw-r--r--   0 gaetanbrison   (501) staff       (20)       90 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/minus.png
--rw-r--r--   0 gaetanbrison   (501) staff       (20)       90 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/plus.png
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     4819 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/pygments.css
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    18215 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     4712 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     3336 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/genindex.html
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     4452 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/index.html
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     5237 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/modules.html
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      447 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/objects.inv
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     3735 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/search.html
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2953 2023-06-08 12:17:17.000000 XPER-0.0.8/docs/_build/html/searchindex.js
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     1221 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/conf.py
--rw-r--r--   0 gaetanbrison   (501) staff       (20)        0 2023-05-30 07:25:48.000000 XPER-0.0.8/docs/index.md
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      428 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/index.rst
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      800 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/make.bat
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      249 2023-05-30 07:24:48.000000 XPER-0.0.8/docs/modules.rst
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.669797 XPER-0.0.8/env-xper/
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.733071 XPER-0.0.8/env-xper/bin/
--rw-rw-r--   0 gaetanbrison   (501) staff       (20)     8834 2023-04-17 07:43:40.000000 XPER-0.0.8/env-xper/bin/Activate.ps1
--rw-rw-r--   0 gaetanbrison   (501) staff       (20)     1938 2023-04-17 07:43:40.000000 XPER-0.0.8/env-xper/bin/activate
--rw-rw-r--   0 gaetanbrison   (501) staff       (20)      887 2023-04-17 07:43:40.000000 XPER-0.0.8/env-xper/bin/activate.csh
--rw-rw-r--   0 gaetanbrison   (501) staff       (20)     2027 2023-04-17 07:43:40.000000 XPER-0.0.8/env-xper/bin/activate.fish
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      274 2023-05-02 09:30:01.000000 XPER-0.0.8/env-xper/bin/cygdb
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      295 2023-05-02 09:30:01.000000 XPER-0.0.8/env-xper/bin/cython
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      275 2023-05-02 09:30:01.000000 XPER-0.0.8/env-xper/bin/cythonize
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      270 2023-05-02 09:48:46.000000 XPER-0.0.8/env-xper/bin/f2py
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      270 2023-05-02 09:48:46.000000 XPER-0.0.8/env-xper/bin/f2py3
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      270 2023-05-02 09:48:46.000000 XPER-0.0.8/env-xper/bin/f2py3.9
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      268 2023-06-04 19:30:33.000000 XPER-0.0.8/env-xper/bin/flake8
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      271 2023-05-02 09:36:46.000000 XPER-0.0.8/env-xper/bin/fonttools
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      265 2023-06-04 19:33:08.000000 XPER-0.0.8/env-xper/bin/identify-cli
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      278 2023-05-02 11:57:09.000000 XPER-0.0.8/env-xper/bin/ipython
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      278 2023-05-02 11:57:09.000000 XPER-0.0.8/env-xper/bin/ipython3
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      273 2023-05-02 11:57:07.000000 XPER-0.0.8/env-xper/bin/jupyter
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      277 2023-05-02 11:57:07.000000 XPER-0.0.8/env-xper/bin/jupyter-kernel
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      315 2023-05-02 11:57:07.000000 XPER-0.0.8/env-xper/bin/jupyter-kernelspec
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      273 2023-05-02 11:57:07.000000 XPER-0.0.8/env-xper/bin/jupyter-migrate
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      294 2023-05-02 11:57:07.000000 XPER-0.0.8/env-xper/bin/jupyter-run
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      278 2023-05-02 11:57:07.000000 XPER-0.0.8/env-xper/bin/jupyter-troubleshoot
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      264 2023-05-30 07:45:34.000000 XPER-0.0.8/env-xper/bin/keyring
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      274 2023-05-30 07:45:34.000000 XPER-0.0.8/env-xper/bin/markdown-it
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      260 2023-06-04 19:33:08.000000 XPER-0.0.8/env-xper/bin/nodeenv
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      298 2023-05-30 06:45:49.000000 XPER-0.0.8/env-xper/bin/normalizer
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      242 2023-05-02 09:48:48.000000 XPER-0.0.8/env-xper/bin/numba
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      275 2023-04-17 07:43:40.000000 XPER-0.0.8/env-xper/bin/pip
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      275 2023-04-17 07:43:40.000000 XPER-0.0.8/env-xper/bin/pip3
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      275 2023-04-17 07:43:40.000000 XPER-0.0.8/env-xper/bin/pip3.9
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      272 2023-05-30 07:45:33.000000 XPER-0.0.8/env-xper/bin/pkginfo
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      268 2023-06-04 19:33:09.000000 XPER-0.0.8/env-xper/bin/pre-commit
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      276 2023-05-30 06:45:49.000000 XPER-0.0.8/env-xper/bin/pybabel
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      108 2023-05-02 09:48:48.000000 XPER-0.0.8/env-xper/bin/pycc
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      266 2023-06-04 19:30:33.000000 XPER-0.0.8/env-xper/bin/pycodestyle
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      265 2023-06-04 19:30:33.000000 XPER-0.0.8/env-xper/bin/pyflakes
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      268 2023-05-02 09:36:46.000000 XPER-0.0.8/env-xper/bin/pyftmerge
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      269 2023-05-02 09:36:46.000000 XPER-0.0.8/env-xper/bin/pyftsubset
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      269 2023-05-02 09:30:01.000000 XPER-0.0.8/env-xper/bin/pygmentize
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      648 2023-05-30 06:56:21.000000 XPER-0.0.8/env-xper/bin/rst2html.py
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      768 2023-05-30 06:56:21.000000 XPER-0.0.8/env-xper/bin/rst2html4.py
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)     1136 2023-05-30 06:56:21.000000 XPER-0.0.8/env-xper/bin/rst2html5.py
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      845 2023-05-30 06:56:21.000000 XPER-0.0.8/env-xper/bin/rst2latex.py
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      653 2023-05-30 06:56:21.000000 XPER-0.0.8/env-xper/bin/rst2man.py
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      818 2023-05-30 06:56:21.000000 XPER-0.0.8/env-xper/bin/rst2odt.py
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)     1780 2023-05-30 06:56:21.000000 XPER-0.0.8/env-xper/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      655 2023-05-30 06:56:21.000000 XPER-0.0.8/env-xper/bin/rst2pseudoxml.py
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      691 2023-05-30 06:56:21.000000 XPER-0.0.8/env-xper/bin/rst2s5.py
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      925 2023-05-30 06:56:21.000000 XPER-0.0.8/env-xper/bin/rst2xetex.py
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      656 2023-05-30 06:56:21.000000 XPER-0.0.8/env-xper/bin/rst2xml.py
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      724 2023-05-30 06:56:21.000000 XPER-0.0.8/env-xper/bin/rstpep2html.py
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      270 2023-05-30 06:56:22.000000 XPER-0.0.8/env-xper/bin/sphinx-apidoc
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      284 2023-05-30 06:56:22.000000 XPER-0.0.8/env-xper/bin/sphinx-autogen
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      269 2023-05-30 06:56:22.000000 XPER-0.0.8/env-xper/bin/sphinx-build
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      274 2023-05-30 06:56:22.000000 XPER-0.0.8/env-xper/bin/sphinx-quickstart
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      261 2023-05-02 09:48:42.000000 XPER-0.0.8/env-xper/bin/tqdm
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      266 2023-05-02 09:36:46.000000 XPER-0.0.8/env-xper/bin/ttx
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      267 2023-05-30 07:45:34.000000 XPER-0.0.8/env-xper/bin/twine
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      292 2023-06-04 19:33:08.000000 XPER-0.0.8/env-xper/bin/virtualenv
--rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      262 2023-05-30 07:44:41.000000 XPER-0.0.8/env-xper/bin/wheel
--rw-r--r--   0 gaetanbrison   (501) staff       (20)       99 2023-04-17 07:43:36.000000 XPER-0.0.8/env-xper/pyvenv.cfg
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.358367 XPER-0.0.8/env-xper/share/
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.358029 XPER-0.0.8/env-xper/share/jupyter/
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.358155 XPER-0.0.8/env-xper/share/jupyter/kernels/
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.735865 XPER-0.0.8/env-xper/share/jupyter/kernels/python3/
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      193 2023-05-02 11:57:09.000000 XPER-0.0.8/env-xper/share/jupyter/kernels/python3/kernel.json
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     1084 2023-05-02 11:57:09.000000 XPER-0.0.8/env-xper/share/jupyter/kernels/python3/logo-32x32.png
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2180 2023-05-02 11:57:09.000000 XPER-0.0.8/env-xper/share/jupyter/kernels/python3/logo-64x64.png
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     9605 2023-05-02 11:57:09.000000 XPER-0.0.8/env-xper/share/jupyter/kernels/python3/logo-svg.svg
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.358481 XPER-0.0.8/env-xper/share/man/
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.738553 XPER-0.0.8/env-xper/share/man/man1/
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2058 2023-05-02 11:57:08.000000 XPER-0.0.8/env-xper/share/man/man1/ipython.1
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     5377 2023-05-02 09:36:45.000000 XPER-0.0.8/env-xper/share/man/man1/ttx.1
-drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:27:25.759704 XPER-0.0.8/images/
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    42901 2023-06-09 15:51:49.000000 XPER-0.0.8/images/Boston.png
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     1130 2023-06-13 09:20:19.000000 XPER-0.0.8/images/License-MIT-yellow.svg
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    14514 2023-06-09 15:50:19.000000 XPER-0.0.8/images/Performance-Metrics.png
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    68435 2023-06-09 15:49:49.000000 XPER-0.0.8/images/Sample.png
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    11395 2023-06-21 12:05:00.000000 XPER-0.0.8/images/bar_plot.png
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    60044 2023-06-21 12:05:00.000000 XPER-0.0.8/images/beeswarn.png
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    29507 2023-06-21 12:05:00.000000 XPER-0.0.8/images/force.png
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     2227 2023-06-21 12:05:00.000000 XPER-0.0.8/images/performance.jpg
--rw-r--r--   0 gaetanbrison   (501) staff       (20)      100 2023-06-23 06:02:58.000000 XPER-0.0.8/requirements.txt
--rw-r--r--   0 gaetanbrison   (501) staff       (20)       38 2023-06-23 06:27:25.761825 XPER-0.0.8/setup.cfg
--rw-r--r--   0 gaetanbrison   (501) staff       (20)     1715 2023-06-23 06:03:14.000000 XPER-0.0.8/setup.py
--rw-r--r--   0 gaetanbrison   (501) staff       (20)    68150 2023-06-22 06:06:51.000000 XPER-0.0.8/xgboost_model.joblib
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.563978 XPER-0.0.9/
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     8196 2023-06-09 15:56:03.000000 XPER-0.0.9/.DS_Store
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     1799 2023-04-17 07:42:16.000000 XPER-0.0.9/.gitignore
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)        0 2023-05-30 07:41:57.000000 XPER-0.0.9/History.rst
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     1249 2023-06-21 12:05:00.000000 XPER-0.0.9/LICENSE
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     1208 2023-06-23 06:38:18.563638 XPER-0.0.9/PKG-INFO
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    23816 2023-06-13 09:26:29.000000 XPER-0.0.9/README.html
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     3513 2023-06-21 12:05:00.000000 XPER-0.0.9/README.md
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.285373 XPER-0.0.9/XPER/
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      120 2023-06-22 08:23:17.000000 XPER-0.0.9/XPER/__init__.py
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.296104 XPER-0.0.9/XPER/compute/
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    15236 2023-06-22 08:23:17.000000 XPER-0.0.9/XPER/compute/EM.py
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    21359 2023-06-15 11:52:56.000000 XPER-0.0.9/XPER/compute/Optimisation.py
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     8208 2023-06-22 12:13:54.000000 XPER-0.0.9/XPER/compute/Performance.py
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     5176 2023-06-22 06:08:21.000000 XPER-0.0.9/XPER/compute/XGBoost_model.py
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      165 2023-06-22 08:23:17.000000 XPER-0.0.9/XPER/compute/__init__.py
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.326484 XPER-0.0.9/XPER/datasets/
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    35735 2023-06-10 09:03:03.000000 XPER-0.0.9/XPER/datasets/BostonHousing.csv
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)       72 2023-06-09 13:57:09.000000 XPER-0.0.9/XPER/datasets/__init__.py
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)  3974305 2023-06-13 08:34:01.000000 XPER-0.0.9/XPER/datasets/adult.data
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      315 2023-06-13 08:34:01.000000 XPER-0.0.9/XPER/datasets/load_data.py
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2772 2023-06-21 12:36:00.000000 XPER-0.0.9/XPER/datasets/sample.py
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.329436 XPER-0.0.9/XPER/viz/
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    28086 2023-06-23 06:37:31.000000 XPER-0.0.9/XPER/viz/Visualisation.py
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)       36 2023-06-13 08:44:48.000000 XPER-0.0.9/XPER/viz/__init__.py
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.330402 XPER-0.0.9/XPER/viz/figures/
+-rw-rw-r--   0 gaetanbrison   (501) staff       (20)    57106 2023-06-08 14:29:51.000000 XPER-0.0.9/XPER/viz/figures/force_plot.pdf
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.290379 XPER-0.0.9/XPER.egg-info/
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     1208 2023-06-23 06:38:18.000000 XPER-0.0.9/XPER.egg-info/PKG-INFO
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     6751 2023-06-23 06:38:18.000000 XPER-0.0.9/XPER.egg-info/SOURCES.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)        1 2023-06-23 06:38:18.000000 XPER-0.0.9/XPER.egg-info/dependency_links.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)        1 2023-06-05 11:34:15.000000 XPER-0.0.9/XPER.egg-info/not-zip-safe
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)       88 2023-06-23 06:38:18.000000 XPER-0.0.9/XPER.egg-info/requires.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)        5 2023-06-23 06:38:18.000000 XPER-0.0.9/XPER.egg-info/top_level.txt
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.343944 XPER-0.0.9/docs/
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      100 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/Beta.rst
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      120 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/Beta_model.rst
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      146 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/Beta_not_optimized.rst
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)       94 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/EM.rst
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      634 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/Makefile
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      117 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/OLS_model.rst
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      124 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/Optimisation.rst
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      106 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/Probit.rst
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      126 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/Probit_model.rst
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      127 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/Visualisation.rst
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      109 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/XGBoost.rst
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      129 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/XGBoost_model.rst
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      100 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/XPER.rst
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      114 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/XPER_OLS.rst
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      126 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/XPER_XGBoost.rst
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      146 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/XPER_empirical_app.rst
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.271677 XPER-0.0.9/docs/_build/
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.361107 XPER-0.0.9/docs/_build/doctrees/
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2379 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/doctrees/Beta.doctree
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2411 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/doctrees/Beta_model.doctree
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2453 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/doctrees/Beta_not_optimized.doctree
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2369 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/doctrees/EM.doctree
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2406 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/doctrees/OLS_model.doctree
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2419 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/doctrees/Optimisation.doctree
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2389 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/doctrees/Probit.doctree
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2421 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/doctrees/Probit_model.doctree
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2424 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/doctrees/Visualisation.doctree
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2394 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/doctrees/XGBoost.doctree
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2426 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/doctrees/XGBoost_model.doctree
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2379 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/doctrees/XPER.doctree
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2401 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/doctrees/XPER_OLS.doctree
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2421 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/doctrees/XPER_XGBoost.doctree
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2453 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/doctrees/XPER_empirical_app.doctree
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    49197 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     4926 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/doctrees/index.doctree
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2937 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/doctrees/modules.doctree
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.376568 XPER-0.0.9/docs/_build/html/
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     3678 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/Beta.html
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     3720 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/Beta_model.html
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     3776 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/Beta_not_optimized.html
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     3664 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/EM.html
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     3713 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/OLS_model.html
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     3734 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/Optimisation.html
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     3692 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/Probit.html
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     3734 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/Probit_model.html
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     3741 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/Visualisation.html
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     3699 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/XGBoost.html
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     3741 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/XGBoost_model.html
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     3678 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/XPER.html
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     3706 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/XPER_OLS.html
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     3734 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/XPER_XGBoost.html
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     3776 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/XPER_empirical_app.html
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.390520 XPER-0.0.9/docs/_build/html/_sources/
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      100 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_sources/Beta.rst.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      120 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_sources/Beta_model.rst.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      146 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_sources/Beta_not_optimized.rst.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)       94 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_sources/EM.rst.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      117 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_sources/OLS_model.rst.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      124 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_sources/Optimisation.rst.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      106 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_sources/Probit.rst.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      126 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_sources/Probit_model.rst.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      127 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_sources/Visualisation.rst.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      109 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_sources/XGBoost.rst.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      129 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_sources/XGBoost_model.rst.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      100 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_sources/XPER.rst.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      114 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_sources/XPER_OLS.rst.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      126 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_sources/XPER_XGBoost.rst.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      146 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_sources/XPER_empirical_app.rst.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      428 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      249 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_sources/modules.rst.txt
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.402486 XPER-0.0.9/docs/_build/html/_static/
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     4289 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    14813 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.403493 XPER-0.0.9/docs/_build/html/_static/css/
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     3229 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/css/badge_only.css
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.453645 XPER-0.0.9/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    87624 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    67312 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    86288 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    66444 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)   165742 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)   444379 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)   165548 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    98024 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    77160 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)   323344 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)   193308 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)   309728 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)   184912 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)   328412 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)   195704 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)   309192 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)   182708 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)   135235 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     4472 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      420 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      286 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/file.png
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    89501 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/jquery.js
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.459790 XPER-0.0.9/docs/_build/html/_static/js/
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      934 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     4370 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2734 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     5023 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     4758 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)       90 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/minus.png
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)       90 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/plus.png
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     4819 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    18215 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     4712 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     3336 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/genindex.html
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     4452 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/index.html
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     5237 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/modules.html
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      447 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/objects.inv
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     3735 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/search.html
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2953 2023-06-08 12:17:17.000000 XPER-0.0.9/docs/_build/html/searchindex.js
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     1221 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/conf.py
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)        0 2023-05-30 07:25:48.000000 XPER-0.0.9/docs/index.md
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      428 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/index.rst
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      800 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/make.bat
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      249 2023-05-30 07:24:48.000000 XPER-0.0.9/docs/modules.rst
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.460450 XPER-0.0.9/env-xper/
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.532737 XPER-0.0.9/env-xper/bin/
+-rw-rw-r--   0 gaetanbrison   (501) staff       (20)     8834 2023-04-17 07:43:40.000000 XPER-0.0.9/env-xper/bin/Activate.ps1
+-rw-rw-r--   0 gaetanbrison   (501) staff       (20)     1938 2023-04-17 07:43:40.000000 XPER-0.0.9/env-xper/bin/activate
+-rw-rw-r--   0 gaetanbrison   (501) staff       (20)      887 2023-04-17 07:43:40.000000 XPER-0.0.9/env-xper/bin/activate.csh
+-rw-rw-r--   0 gaetanbrison   (501) staff       (20)     2027 2023-04-17 07:43:40.000000 XPER-0.0.9/env-xper/bin/activate.fish
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      274 2023-05-02 09:30:01.000000 XPER-0.0.9/env-xper/bin/cygdb
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      295 2023-05-02 09:30:01.000000 XPER-0.0.9/env-xper/bin/cython
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      275 2023-05-02 09:30:01.000000 XPER-0.0.9/env-xper/bin/cythonize
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      270 2023-05-02 09:48:46.000000 XPER-0.0.9/env-xper/bin/f2py
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      270 2023-05-02 09:48:46.000000 XPER-0.0.9/env-xper/bin/f2py3
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      270 2023-05-02 09:48:46.000000 XPER-0.0.9/env-xper/bin/f2py3.9
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      268 2023-06-04 19:30:33.000000 XPER-0.0.9/env-xper/bin/flake8
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      271 2023-05-02 09:36:46.000000 XPER-0.0.9/env-xper/bin/fonttools
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      265 2023-06-04 19:33:08.000000 XPER-0.0.9/env-xper/bin/identify-cli
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      278 2023-05-02 11:57:09.000000 XPER-0.0.9/env-xper/bin/ipython
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      278 2023-05-02 11:57:09.000000 XPER-0.0.9/env-xper/bin/ipython3
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      273 2023-05-02 11:57:07.000000 XPER-0.0.9/env-xper/bin/jupyter
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      277 2023-05-02 11:57:07.000000 XPER-0.0.9/env-xper/bin/jupyter-kernel
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      315 2023-05-02 11:57:07.000000 XPER-0.0.9/env-xper/bin/jupyter-kernelspec
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      273 2023-05-02 11:57:07.000000 XPER-0.0.9/env-xper/bin/jupyter-migrate
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      294 2023-05-02 11:57:07.000000 XPER-0.0.9/env-xper/bin/jupyter-run
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      278 2023-05-02 11:57:07.000000 XPER-0.0.9/env-xper/bin/jupyter-troubleshoot
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      264 2023-05-30 07:45:34.000000 XPER-0.0.9/env-xper/bin/keyring
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      274 2023-05-30 07:45:34.000000 XPER-0.0.9/env-xper/bin/markdown-it
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      260 2023-06-04 19:33:08.000000 XPER-0.0.9/env-xper/bin/nodeenv
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      298 2023-05-30 06:45:49.000000 XPER-0.0.9/env-xper/bin/normalizer
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      242 2023-05-02 09:48:48.000000 XPER-0.0.9/env-xper/bin/numba
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      275 2023-04-17 07:43:40.000000 XPER-0.0.9/env-xper/bin/pip
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      275 2023-04-17 07:43:40.000000 XPER-0.0.9/env-xper/bin/pip3
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      275 2023-04-17 07:43:40.000000 XPER-0.0.9/env-xper/bin/pip3.9
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      272 2023-05-30 07:45:33.000000 XPER-0.0.9/env-xper/bin/pkginfo
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      268 2023-06-04 19:33:09.000000 XPER-0.0.9/env-xper/bin/pre-commit
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      276 2023-05-30 06:45:49.000000 XPER-0.0.9/env-xper/bin/pybabel
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      108 2023-05-02 09:48:48.000000 XPER-0.0.9/env-xper/bin/pycc
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      266 2023-06-04 19:30:33.000000 XPER-0.0.9/env-xper/bin/pycodestyle
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      265 2023-06-04 19:30:33.000000 XPER-0.0.9/env-xper/bin/pyflakes
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      268 2023-05-02 09:36:46.000000 XPER-0.0.9/env-xper/bin/pyftmerge
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      269 2023-05-02 09:36:46.000000 XPER-0.0.9/env-xper/bin/pyftsubset
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      269 2023-05-02 09:30:01.000000 XPER-0.0.9/env-xper/bin/pygmentize
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      648 2023-05-30 06:56:21.000000 XPER-0.0.9/env-xper/bin/rst2html.py
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      768 2023-05-30 06:56:21.000000 XPER-0.0.9/env-xper/bin/rst2html4.py
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)     1136 2023-05-30 06:56:21.000000 XPER-0.0.9/env-xper/bin/rst2html5.py
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      845 2023-05-30 06:56:21.000000 XPER-0.0.9/env-xper/bin/rst2latex.py
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      653 2023-05-30 06:56:21.000000 XPER-0.0.9/env-xper/bin/rst2man.py
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      818 2023-05-30 06:56:21.000000 XPER-0.0.9/env-xper/bin/rst2odt.py
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)     1780 2023-05-30 06:56:21.000000 XPER-0.0.9/env-xper/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      655 2023-05-30 06:56:21.000000 XPER-0.0.9/env-xper/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      691 2023-05-30 06:56:21.000000 XPER-0.0.9/env-xper/bin/rst2s5.py
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      925 2023-05-30 06:56:21.000000 XPER-0.0.9/env-xper/bin/rst2xetex.py
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      656 2023-05-30 06:56:21.000000 XPER-0.0.9/env-xper/bin/rst2xml.py
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      724 2023-05-30 06:56:21.000000 XPER-0.0.9/env-xper/bin/rstpep2html.py
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      270 2023-05-30 06:56:22.000000 XPER-0.0.9/env-xper/bin/sphinx-apidoc
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      284 2023-05-30 06:56:22.000000 XPER-0.0.9/env-xper/bin/sphinx-autogen
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      269 2023-05-30 06:56:22.000000 XPER-0.0.9/env-xper/bin/sphinx-build
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      274 2023-05-30 06:56:22.000000 XPER-0.0.9/env-xper/bin/sphinx-quickstart
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      261 2023-05-02 09:48:42.000000 XPER-0.0.9/env-xper/bin/tqdm
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      266 2023-05-02 09:36:46.000000 XPER-0.0.9/env-xper/bin/ttx
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      267 2023-05-30 07:45:34.000000 XPER-0.0.9/env-xper/bin/twine
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      292 2023-06-04 19:33:08.000000 XPER-0.0.9/env-xper/bin/virtualenv
+-rwxr-xr-x   0 gaetanbrison   (501) staff       (20)      262 2023-05-30 07:44:41.000000 XPER-0.0.9/env-xper/bin/wheel
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)       99 2023-04-17 07:43:36.000000 XPER-0.0.9/env-xper/pyvenv.cfg
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.273533 XPER-0.0.9/env-xper/share/
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.273264 XPER-0.0.9/env-xper/share/jupyter/
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.273365 XPER-0.0.9/env-xper/share/jupyter/kernels/
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.545797 XPER-0.0.9/env-xper/share/jupyter/kernels/python3/
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      193 2023-05-02 11:57:09.000000 XPER-0.0.9/env-xper/share/jupyter/kernels/python3/kernel.json
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     1084 2023-05-02 11:57:09.000000 XPER-0.0.9/env-xper/share/jupyter/kernels/python3/logo-32x32.png
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2180 2023-05-02 11:57:09.000000 XPER-0.0.9/env-xper/share/jupyter/kernels/python3/logo-64x64.png
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     9605 2023-05-02 11:57:09.000000 XPER-0.0.9/env-xper/share/jupyter/kernels/python3/logo-svg.svg
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.273646 XPER-0.0.9/env-xper/share/man/
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.548144 XPER-0.0.9/env-xper/share/man/man1/
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2058 2023-05-02 11:57:08.000000 XPER-0.0.9/env-xper/share/man/man1/ipython.1
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     5377 2023-05-02 09:36:45.000000 XPER-0.0.9/env-xper/share/man/man1/ttx.1
+drwxr-xr-x   0 gaetanbrison   (501) staff       (20)        0 2023-06-23 06:38:18.561749 XPER-0.0.9/images/
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    42901 2023-06-09 15:51:49.000000 XPER-0.0.9/images/Boston.png
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     1130 2023-06-13 09:20:19.000000 XPER-0.0.9/images/License-MIT-yellow.svg
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    14514 2023-06-09 15:50:19.000000 XPER-0.0.9/images/Performance-Metrics.png
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    68435 2023-06-09 15:49:49.000000 XPER-0.0.9/images/Sample.png
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    11395 2023-06-21 12:05:00.000000 XPER-0.0.9/images/bar_plot.png
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    60044 2023-06-21 12:05:00.000000 XPER-0.0.9/images/beeswarn.png
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    29507 2023-06-21 12:05:00.000000 XPER-0.0.9/images/force.png
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     2227 2023-06-21 12:05:00.000000 XPER-0.0.9/images/performance.jpg
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)      100 2023-06-23 06:02:58.000000 XPER-0.0.9/requirements.txt
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)       38 2023-06-23 06:38:18.564131 XPER-0.0.9/setup.cfg
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)     1715 2023-06-23 06:31:49.000000 XPER-0.0.9/setup.py
+-rw-r--r--   0 gaetanbrison   (501) staff       (20)    68150 2023-06-22 06:06:51.000000 XPER-0.0.9/xgboost_model.joblib
```

### Comparing `XPER-0.0.8/.DS_Store` & `XPER-0.0.9/.DS_Store`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/.gitignore` & `XPER-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/LICENSE` & `XPER-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/PKG-INFO` & `XPER-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XPER
-Version: 0.0.8
+Version: 0.0.9
 Summary: XPER (eXplainable PERformance) is a methodology designed      to measure the specific contribution of the input features to      the predictive performance of any econometric or machine learning model.
 Home-page: https://github.com/hi-paris/XPER
 Author: Sebastien Saurin, Christophe Hurlin, Christophe Perignon,
      supported by Awais Sani and Gaëtan Brison
 Author-email: engineer.hi.paris@gmail.com
 License: MIT license
 Keywords: XPER
```

### Comparing `XPER-0.0.8/README.html` & `XPER-0.0.9/README.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/README.md` & `XPER-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/XPER/compute/EM.py` & `XPER-0.0.9/XPER/compute/EM.py`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/XPER/compute/Optimisation.py` & `XPER-0.0.9/XPER/compute/Optimisation.py`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/XPER/compute/Performance.py` & `XPER-0.0.9/XPER/compute/Performance.py`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/XPER/compute/XGBoost_model.py` & `XPER-0.0.9/XPER/compute/XGBoost_model.py`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/XPER/datasets/BostonHousing.csv` & `XPER-0.0.9/XPER/datasets/BostonHousing.csv`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/XPER/datasets/adult.data` & `XPER-0.0.9/XPER/datasets/adult.data`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/XPER/datasets/sample.py` & `XPER-0.0.9/XPER/datasets/sample.py`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/XPER/viz/Visualisation.py` & `XPER-0.0.9/XPER/viz/Visualisation.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,131 +35,195 @@
         self.benchmark_v_ind = pd.DataFrame(XPER_values[1][:,0],columns=["Individual Benchmark"])
         self.p = p # Number of features
 
     # =============================================================================
     #       Bar plot: X-axis = phi_j value or pct // y-axis = Feature names
     # =============================================================================
     
-def bar_plot(XPER_values, X_test, labels, p, percentage=True):
-    """
-    Create a bar plot to visualize contributions.
-
-    Parameters
-    ----------
-    XPER_values : numpy.ndarray
-        Array of contributions.
-    X_test : pandas.DataFrame
-        Test data used for labeling the plot.
-    labels : list
-        List of labels for the contributions.
-    p : int
-        Number of top contributions to display.
-    percentage : bool, optional
-        If True, contributions are shown as percentages. Default is True.
-
-    Returns
-    -------
-    None
-
-    Examples
-    --------
-    >>> import numpy as np
-    >>> import pandas as pd
-    >>> import plotly.graph_objects as go
-    >>> import plotly.express as px
-    >>> XPER_values = np.array([0.2, 0.3, 0.5])
-    >>> X_test = pd.DataFrame({'A': [1, 2, 3], 'B': [4, 5, 6], 'C': [7, 8, 9]})
-    >>> labels = ['Label 1', 'Label 2', 'Label 3']
-    >>> p = 2
-    >>> bar_plot(XPER_values, X_test, labels, p)
-
-    Notes
-    -----
-    This function creates a horizontal bar plot to visualize contributions. The contributions are provided as an array
-    in `XPER_values`, which represents the contributions of each feature or metric. The `X_test` DataFrame is used to
-    label the plot based on the column names. The `labels` list provides additional labels for the contributions.
-    The `p` parameter determines the number of top contributions to display.
-
-    If `percentage` is True, the contributions are shown as percentages of the total contribution. Otherwise, the
-    contributions are displayed as absolute values.
-
-    The plot is created using plotly.graph_objects and plotly.express libraries. The bars are colored using a gradient
-    from RGB(249, 218, 37) to RGB(99, 2, 164). The y-axis displays the labels and the x-axis represents the contribution
-    values. The plot is displayed using fig.show().
-    """
-    Contribution = XPER_values[0].copy()
-
-    ecart_contrib = sum(Contribution) - Contribution[0]
-
-    if percentage == True:
-        Contribution = (Contribution / ecart_contrib) * 100
-
-        print("Contribution (%) sum: ", sum(Contribution[1:]))
-
-    selection = pd.DataFrame(Contribution[1:], index=X_test.columns, columns=["Metric"])
-
-    selection["Labels"] = labels
-
-    selection["absolute"] = abs(selection["Metric"])
-
-    testons = selection.sort_values(by="absolute", ascending=False)[:p].index
-
-    final_selection_values = selection.loc[testons, "Metric"].values
-    final_selection_labels = selection.loc[testons, "Labels"]
-
-    colorscale = [[0, 'rgb(174, 20, 166)'], [1, 'rgb(4, 123, 244)']]
-
-    fig = go.Figure()
-    fig.add_trace(go.Bar(
-        x=final_selection_values,
-        y=final_selection_labels,
-        orientation='h',
-        marker=dict(color=final_selection_values, colorscale=colorscale)
-    ))
-
-    if percentage == True:
-        fig.update_layout(xaxis_title='Contribution (%)')
-    else:
-        fig.update_layout(xaxis_title='Contribution')
-
-    fig.update_layout(
-        yaxis=dict(autorange="reversed"),
-        showlegend=False,
-        plot_bgcolor='white'
-    )
+    def bar_plot(XPER_values, X_test, labels, p, percentage=True):
+        """
+        Create a bar plot to visualize contributions.
 
-    fig.show()
+        Parameters
+        ----------
+        XPER_values : numpy.ndarray
+            Array of contributions.
+        X_test : pandas.DataFrame
+            Test data used for labeling the plot.
+        labels : list
+            List of labels for the contributions.
+        p : int
+            Number of top contributions to display.
+        percentage : bool, optional
+            If True, contributions are shown as percentages. Default is True.
 
+        Returns
+        -------
+        None
+
+        Examples
+        --------
+        >>> import numpy as np
+        >>> import pandas as pd
+        >>> import plotly.graph_objects as go
+        >>> import plotly.express as px
+        >>> XPER_values = np.array([0.2, 0.3, 0.5])
+        >>> X_test = pd.DataFrame({'A': [1, 2, 3], 'B': [4, 5, 6], 'C': [7, 8, 9]})
+        >>> labels = ['Label 1', 'Label 2', 'Label 3']
+        >>> p = 2
+        >>> bar_plot(XPER_values, X_test, labels, p)
+
+        Notes
+        -----
+        This function creates a horizontal bar plot to visualize contributions. The contributions are provided as an array
+        in `XPER_values`, which represents the contributions of each feature or metric. The `X_test` DataFrame is used to
+        label the plot based on the column names. The `labels` list provides additional labels for the contributions.
+        The `p` parameter determines the number of top contributions to display.
+
+        If `percentage` is True, the contributions are shown as percentages of the total contribution. Otherwise, the
+        contributions are displayed as absolute values.
+
+        The plot is created using plotly.graph_objects and plotly.express libraries. The bars are colored using a gradient
+        from RGB(249, 218, 37) to RGB(99, 2, 164). The y-axis displays the labels and the x-axis represents the contribution
+        values. The plot is displayed using fig.show().
+        """
+        Contribution = XPER_values[0].copy()
+
+        ecart_contrib = sum(Contribution) - Contribution[0]
+
+        if percentage == True:
+            Contribution = (Contribution / ecart_contrib) * 100
+
+            print("Contribution (%) sum: ", sum(Contribution[1:]))
+
+        selection = pd.DataFrame(Contribution[1:], index=X_test.columns, columns=["Metric"])
+
+        selection["Labels"] = labels
+
+        selection["absolute"] = abs(selection["Metric"])
+
+        testons = selection.sort_values(by="absolute", ascending=False)[:p].index
+
+        final_selection_values = selection.loc[testons, "Metric"].values
+        final_selection_labels = selection.loc[testons, "Labels"]
+
+        colorscale = [[0, 'rgb(174, 20, 166)'], [1, 'rgb(4, 123, 244)']]
+
+        fig = go.Figure()
+        fig.add_trace(go.Bar(
+            x=final_selection_values,
+            y=final_selection_labels,
+            orientation='h',
+            marker=dict(color=final_selection_values, colorscale=colorscale)
+        ))
+
+        if percentage == True:
+            fig.update_layout(xaxis_title='Contribution (%)')
+        else:
+            fig.update_layout(xaxis_title='Contribution')
+
+        fig.update_layout(
+            yaxis=dict(autorange="reversed"),
+            showlegend=False,
+            plot_bgcolor='white'
+        )
+
+        fig.show()
+
+
+    def beeswarn_plot(XPER_values,X_test,labels):
+        
+        XPER_v_ind = pd.DataFrame(XPER_values[1][:,1:])
+        
+        benchmark_v_ind = pd.DataFrame(XPER_values[1][:,0],columns=["Individual Benchmark"])
+        
+        # =============================================================================
+        #                       Prerequisites for the use of SHAP plots 
+        # =============================================================================
+
+        import xgboost
+        import shap
+
+        ### Idea: We use SHAP on a given model and then we change the values, data, 
+        ### feature_names, base_values to the one obtained with XPER. Therefore, we
+        ### are able to use the shap plots from the shap package on our results from XPER.
+
+        # train XGBoost model
+        X_useless,y_useless = shap.datasets.adult()
+
+        X_useless = X_useless.iloc[:100,:]
+        y_useless = y_useless[:100]
+
+        model = xgboost.XGBClassifier().fit(X_useless, y_useless)
+
+        # compute SHAP values
+        explainer = shap.Explainer(model, X_useless)
+        shap_values = explainer(X_useless)   # This is the object of interests for which
+                                              # we are going to the change the values to 
+                                              # those of XPER.
+                                              
+        # ########################## phi_i_j contributions ##############################
+        # ##########################     Beeswarn plot     ##############################
+
+
+        #### Now we change the values of "shap_values" to those of XPER
+
+        df_phi_i_j = XPER_v_ind.copy()
+
+        shap_values.values = df_phi_i_j.to_numpy()  # XPER values for each observation
+                                                    # and for each feature 
+        shap_values.base_values = np.reshape(benchmark_v_ind.to_numpy(),benchmark_v_ind.shape[0])
+                                                    # Base_value = benchmark values
+        shap_values.data = X_test                   # Data/Inputs
+
+        shap_values.feature_names = labels   # Label of the features displayed on
+                                                    # the y-axis
+
+
+        # ##### Summary plots
+
+        ordering = shap_values.mean(0)              # By default the features are ordered
+                                                    # using shap_values.abs.mean(0). We
+                                                    # change it to the mean value of the
+                                                    # XPER values = phi_j (global ones)
+
+        shap.plots.beeswarm(shap_values, order=ordering,show=False)
+        plt.xlabel("Contribution")
+        plt.show()
 
     
-  
-    
+
+
+
+
+
+
     # =============================================================================
     #                                   Force plots
     # =============================================================================
         
     plt.rcParams["figure.figsize"] = [7.00, 3.50]
     plt.rcParams["figure.autolayout"] = True
     
     
     def draw_higher_lower_element(out_value, offset_text):
         plt.text(out_value - offset_text, 0.495, 'higher',
-                 fontsize=13, color='#FF0D57',
+                 fontsize=13, color='#AEA6A6',
                  horizontalalignment='right')
     
         plt.text(out_value + offset_text, 0.495, 'lower',
-                 fontsize=13, color='#1E88E5',
+                 fontsize=13, color='#047BF4',
                  horizontalalignment='left')
         
         plt.text(out_value, 0.49, r'$\leftarrow$',
-                 fontsize=13, color='#1E88E5',
+                 fontsize=13, color='#047BF4',
                  horizontalalignment='center')
         
         plt.text(out_value, 0.515, r'$\rightarrow$',
-                 fontsize=13, color='#FF0D57',
+                 fontsize=13, color='#AEA6A6',
                  horizontalalignment='center')
         
     def force_plot(XPER_values,instance, X_test, variable_name,figsize=(8,4),min_perc=0.00001):
         
         
         ind_i = instance
```

### Comparing `XPER-0.0.8/XPER/viz/figures/force_plot.pdf` & `XPER-0.0.9/XPER/viz/figures/force_plot.pdf`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/XPER.egg-info/PKG-INFO` & `XPER-0.0.9/XPER.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XPER
-Version: 0.0.8
+Version: 0.0.9
 Summary: XPER (eXplainable PERformance) is a methodology designed      to measure the specific contribution of the input features to      the predictive performance of any econometric or machine learning model.
 Home-page: https://github.com/hi-paris/XPER
 Author: Sebastien Saurin, Christophe Hurlin, Christophe Perignon,
      supported by Awais Sani and Gaëtan Brison
 Author-email: engineer.hi.paris@gmail.com
 License: MIT license
 Keywords: XPER
```

### Comparing `XPER-0.0.8/XPER.egg-info/SOURCES.txt` & `XPER-0.0.9/XPER.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/Makefile` & `XPER-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/doctrees/Beta.doctree` & `XPER-0.0.9/docs/_build/doctrees/Beta.doctree`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/doctrees/Beta_model.doctree` & `XPER-0.0.9/docs/_build/doctrees/Beta_model.doctree`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/doctrees/Beta_not_optimized.doctree` & `XPER-0.0.9/docs/_build/doctrees/Beta_not_optimized.doctree`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/doctrees/EM.doctree` & `XPER-0.0.9/docs/_build/doctrees/EM.doctree`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/doctrees/OLS_model.doctree` & `XPER-0.0.9/docs/_build/doctrees/OLS_model.doctree`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/doctrees/Optimisation.doctree` & `XPER-0.0.9/docs/_build/doctrees/Optimisation.doctree`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/doctrees/Probit.doctree` & `XPER-0.0.9/docs/_build/doctrees/Probit.doctree`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/doctrees/Probit_model.doctree` & `XPER-0.0.9/docs/_build/doctrees/Probit_model.doctree`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/doctrees/Visualisation.doctree` & `XPER-0.0.9/docs/_build/doctrees/Visualisation.doctree`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/doctrees/XGBoost.doctree` & `XPER-0.0.9/docs/_build/doctrees/XGBoost.doctree`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/doctrees/XGBoost_model.doctree` & `XPER-0.0.9/docs/_build/doctrees/XGBoost_model.doctree`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/doctrees/XPER.doctree` & `XPER-0.0.9/docs/_build/doctrees/XPER.doctree`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/doctrees/XPER_OLS.doctree` & `XPER-0.0.9/docs/_build/doctrees/XPER_OLS.doctree`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/doctrees/XPER_XGBoost.doctree` & `XPER-0.0.9/docs/_build/doctrees/XPER_XGBoost.doctree`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/doctrees/XPER_empirical_app.doctree` & `XPER-0.0.9/docs/_build/doctrees/XPER_empirical_app.doctree`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/doctrees/environment.pickle` & `XPER-0.0.9/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/doctrees/index.doctree` & `XPER-0.0.9/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/doctrees/modules.doctree` & `XPER-0.0.9/docs/_build/doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/Beta.html` & `XPER-0.0.9/docs/_build/html/Beta.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/Beta_model.html` & `XPER-0.0.9/docs/_build/html/Beta_model.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/Beta_not_optimized.html` & `XPER-0.0.9/docs/_build/html/Beta_not_optimized.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/EM.html` & `XPER-0.0.9/docs/_build/html/EM.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/OLS_model.html` & `XPER-0.0.9/docs/_build/html/OLS_model.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/Optimisation.html` & `XPER-0.0.9/docs/_build/html/Optimisation.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/Probit.html` & `XPER-0.0.9/docs/_build/html/Probit.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/Probit_model.html` & `XPER-0.0.9/docs/_build/html/Probit_model.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/Visualisation.html` & `XPER-0.0.9/docs/_build/html/Visualisation.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/XGBoost.html` & `XPER-0.0.9/docs/_build/html/XGBoost.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/XGBoost_model.html` & `XPER-0.0.9/docs/_build/html/XGBoost_model.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/XPER.html` & `XPER-0.0.9/docs/_build/html/XPER.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/XPER_OLS.html` & `XPER-0.0.9/docs/_build/html/XPER_OLS.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/XPER_XGBoost.html` & `XPER-0.0.9/docs/_build/html/XPER_XGBoost.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/XPER_empirical_app.html` & `XPER-0.0.9/docs/_build/html/XPER_empirical_app.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `XPER-0.0.9/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/basic.css` & `XPER-0.0.9/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/css/badge_only.css` & `XPER-0.0.9/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `XPER-0.0.9/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `XPER-0.0.9/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `XPER-0.0.9/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `XPER-0.0.9/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `XPER-0.0.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `XPER-0.0.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `XPER-0.0.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `XPER-0.0.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `XPER-0.0.9/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/css/fonts/lato-bold-italic.woff` & `XPER-0.0.9/docs/_build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2` & `XPER-0.0.9/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/css/fonts/lato-bold.woff` & `XPER-0.0.9/docs/_build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/css/fonts/lato-bold.woff2` & `XPER-0.0.9/docs/_build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/css/fonts/lato-normal-italic.woff` & `XPER-0.0.9/docs/_build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2` & `XPER-0.0.9/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/css/fonts/lato-normal.woff` & `XPER-0.0.9/docs/_build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/css/fonts/lato-normal.woff2` & `XPER-0.0.9/docs/_build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/css/theme.css` & `XPER-0.0.9/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/doctools.js` & `XPER-0.0.9/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/jquery.js` & `XPER-0.0.9/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/js/badge_only.js` & `XPER-0.0.9/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/js/html5shiv-printshiv.min.js` & `XPER-0.0.9/docs/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/js/html5shiv.min.js` & `XPER-0.0.9/docs/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/js/theme.js` & `XPER-0.0.9/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/language_data.js` & `XPER-0.0.9/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/pygments.css` & `XPER-0.0.9/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/searchtools.js` & `XPER-0.0.9/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/_static/sphinx_highlight.js` & `XPER-0.0.9/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/genindex.html` & `XPER-0.0.9/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/index.html` & `XPER-0.0.9/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/modules.html` & `XPER-0.0.9/docs/_build/html/modules.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/search.html` & `XPER-0.0.9/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/_build/html/searchindex.js` & `XPER-0.0.9/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/conf.py` & `XPER-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/docs/make.bat` & `XPER-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/bin/Activate.ps1` & `XPER-0.0.9/env-xper/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/bin/activate` & `XPER-0.0.9/env-xper/bin/activate`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/bin/activate.csh` & `XPER-0.0.9/env-xper/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/bin/activate.fish` & `XPER-0.0.9/env-xper/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/bin/rst2html.py` & `XPER-0.0.9/env-xper/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/bin/rst2html4.py` & `XPER-0.0.9/env-xper/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/bin/rst2html5.py` & `XPER-0.0.9/env-xper/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/bin/rst2latex.py` & `XPER-0.0.9/env-xper/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/bin/rst2man.py` & `XPER-0.0.9/env-xper/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/bin/rst2odt.py` & `XPER-0.0.9/env-xper/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/bin/rst2odt_prepstyles.py` & `XPER-0.0.9/env-xper/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/bin/rst2pseudoxml.py` & `XPER-0.0.9/env-xper/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/bin/rst2s5.py` & `XPER-0.0.9/env-xper/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/bin/rst2xetex.py` & `XPER-0.0.9/env-xper/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/bin/rst2xml.py` & `XPER-0.0.9/env-xper/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/bin/rstpep2html.py` & `XPER-0.0.9/env-xper/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/share/jupyter/kernels/python3/logo-32x32.png` & `XPER-0.0.9/env-xper/share/jupyter/kernels/python3/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/share/jupyter/kernels/python3/logo-64x64.png` & `XPER-0.0.9/env-xper/share/jupyter/kernels/python3/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/share/jupyter/kernels/python3/logo-svg.svg` & `XPER-0.0.9/env-xper/share/jupyter/kernels/python3/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/share/man/man1/ipython.1` & `XPER-0.0.9/env-xper/share/man/man1/ipython.1`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/env-xper/share/man/man1/ttx.1` & `XPER-0.0.9/env-xper/share/man/man1/ttx.1`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/images/Boston.png` & `XPER-0.0.9/images/Boston.png`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/images/License-MIT-yellow.svg` & `XPER-0.0.9/images/License-MIT-yellow.svg`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/images/Performance-Metrics.png` & `XPER-0.0.9/images/Performance-Metrics.png`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/images/Sample.png` & `XPER-0.0.9/images/Sample.png`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/images/bar_plot.png` & `XPER-0.0.9/images/bar_plot.png`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/images/beeswarn.png` & `XPER-0.0.9/images/beeswarn.png`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/images/force.png` & `XPER-0.0.9/images/force.png`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/images/performance.jpg` & `XPER-0.0.9/images/performance.jpg`

 * *Files identical despite different names*

### Comparing `XPER-0.0.8/setup.py` & `XPER-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,10 +37,10 @@
     include_package_data=True,
     keywords='XPER',
     name='XPER',
     packages=find_packages(include=['XPER', 'XPER.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/hi-paris/XPER',
-    version='0.0.8',
+    version='0.0.9',
     zip_safe=False,
 )
```

### Comparing `XPER-0.0.8/xgboost_model.joblib` & `XPER-0.0.9/xgboost_model.joblib`

 * *Files identical despite different names*

