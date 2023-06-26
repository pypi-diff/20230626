# Comparing `tmp/dcnum-0.10.0.tar.gz` & `tmp/dcnum-0.11.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.10.0.tar", last modified: Mon Jun 26 11:50:20 2023, max compression
+gzip compressed data, was "dcnum-0.11.0.tar", last modified: Mon Jun 26 15:14:13 2023, max compression
```

## Comparing `dcnum-0.10.0.tar` & `dcnum-0.11.0.tar`

### file list

```diff
@@ -1,88 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.968482 dcnum-0.10.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.952481 dcnum-0.10.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.956481 dcnum-0.10.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-26 11:50:06.000000 dcnum-0.10.0/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-26 11:50:06.000000 dcnum-0.10.0/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-26 11:50:06.000000 dcnum-0.10.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-26 11:50:06.000000 dcnum-0.10.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-26 11:50:06.000000 dcnum-0.10.0/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 11:50:06.000000 dcnum-0.10.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-26 11:50:20.968482 dcnum-0.10.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-26 11:50:06.000000 dcnum-0.10.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.956481 dcnum-0.10.0/dcnum/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-26 11:50:20.000000 dcnum-0.10.0/dcnum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.960482 dcnum-0.10.0/dcnum/feat/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/event_extractor_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.960482 dcnum-0.10.0/dcnum/feat/feat_background/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_background/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_background/bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_background/bg_sparse_median.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.960482 dcnum-0.10.0/dcnum/feat/feat_brightness/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_brightness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_brightness/bright_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_brightness/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.960482 dcnum-0.10.0/dcnum/feat/feat_moments/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_moments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_moments/ct_opencv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_moments/mt_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.960482 dcnum-0.10.0/dcnum/feat/feat_texture/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_texture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_texture/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_texture/tex_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/queue_event_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.960482 dcnum-0.10.0/dcnum/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/meta/ppid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.964481 dcnum-0.10.0/dcnum/read/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/read/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/read/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/read/hdf5_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.964481 dcnum-0.10.0/dcnum/segm/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/segm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/segm/segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/segm/segmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/segm/segmenter_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/segm/segmenter_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.964481 dcnum-0.10.0/dcnum/write/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/write/deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/write/queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/write/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.956481 dcnum-0.10.0/dcnum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-26 11:50:20.000000 dcnum-0.10.0/dcnum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-26 11:50:20.000000 dcnum-0.10.0/dcnum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 11:50:20.000000 dcnum-0.10.0/dcnum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-26 11:50:20.000000 dcnum-0.10.0/dcnum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 11:50:20.000000 dcnum-0.10.0/dcnum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.964481 dcnum-0.10.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-26 11:50:06.000000 dcnum-0.10.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.964481 dcnum-0.10.0/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-26 11:50:06.000000 dcnum-0.10.0/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-26 11:50:06.000000 dcnum-0.10.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 11:50:06.000000 dcnum-0.10.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-26 11:50:06.000000 dcnum-0.10.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 11:50:20.968482 dcnum-0.10.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.968482 dcnum-0.10.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.968482 dcnum-0.10.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_feat_background_bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_feat_brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_feat_haralick.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_feat_moments_based.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_ppid.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_ppid_segm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_read_concat_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_read_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_write_deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_write_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.142020 dcnum-0.11.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.130020 dcnum-0.11.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.134020 dcnum-0.11.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-26 15:14:04.000000 dcnum-0.11.0/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-26 15:14:04.000000 dcnum-0.11.0/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-26 15:14:04.000000 dcnum-0.11.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-26 15:14:04.000000 dcnum-0.11.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-26 15:14:04.000000 dcnum-0.11.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 15:14:04.000000 dcnum-0.11.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-26 15:14:13.142020 dcnum-0.11.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-26 15:14:04.000000 dcnum-0.11.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.134020 dcnum-0.11.0/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-26 15:14:13.000000 dcnum-0.11.0/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.134020 dcnum-0.11.0/dcnum/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/event_extractor_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.134020 dcnum-0.11.0/dcnum/feat/feat_background/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_background/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_background/bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_background/bg_sparse_median.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.134020 dcnum-0.11.0/dcnum/feat/feat_brightness/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_brightness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_brightness/bright_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_brightness/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.134020 dcnum-0.11.0/dcnum/feat/feat_moments/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_moments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_moments/ct_opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_moments/mt_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.134020 dcnum-0.11.0/dcnum/feat/feat_texture/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_texture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_texture/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/feat_texture/tex_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/feat/queue_event_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.134020 dcnum-0.11.0/dcnum/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/meta/ppid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.138020 dcnum-0.11.0/dcnum/read/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/read/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/read/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11702 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/read/hdf5_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.138020 dcnum-0.11.0/dcnum/segm/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/segm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/segm/segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/segm/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/segm/segmenter_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/segm/segmenter_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/segm/segmenter_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.138020 dcnum-0.11.0/dcnum/write/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/write/deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/write/queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-26 15:14:04.000000 dcnum-0.11.0/dcnum/write/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.134020 dcnum-0.11.0/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-26 15:14:13.000000 dcnum-0.11.0/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-26 15:14:13.000000 dcnum-0.11.0/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:14:13.000000 dcnum-0.11.0/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-26 15:14:13.000000 dcnum-0.11.0/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 15:14:13.000000 dcnum-0.11.0/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.138020 dcnum-0.11.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-26 15:14:04.000000 dcnum-0.11.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.138020 dcnum-0.11.0/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-26 15:14:04.000000 dcnum-0.11.0/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-26 15:14:04.000000 dcnum-0.11.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 15:14:04.000000 dcnum-0.11.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-26 15:14:04.000000 dcnum-0.11.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:14:13.142020 dcnum-0.11.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.138020 dcnum-0.11.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:14:13.142020 dcnum-0.11.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_feat_background_bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_feat_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_feat_haralick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_feat_moments_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_ppid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_ppid_segm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_read_concat_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_read_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_write_deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-26 15:14:04.000000 dcnum-0.11.0/tests/test_write_writer.py
```

### Comparing `dcnum-0.10.0/.github/workflows/check.yml` & `dcnum-0.11.0/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/.github/workflows/deploy_pypi.yml` & `dcnum-0.11.0/.github/workflows/deploy_pypi.yml`

 * *Files 25% similar despite different names*

```diff
@@ -2,48 +2,43 @@
 
 on:
   push:
     tags:
       - '*'
 
 jobs:
-  build_wheels:
-    name: Build wheels on ${{ matrix.os }}
-    runs-on: ${{ matrix.os }}
-    strategy:
-      matrix:
-        python-version: ['3.10', '3.11']
-        os: [ubuntu-20.04, windows-2019, macos-11]
-
+  build_sdist:
+    name: Build source distribution
+    runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
-      - name: Build wheels
-        uses: pypa/cibuildwheel@v2.12.1
+      - name: Build sdist
+        run: pipx run build --sdist
 
       - name: publish
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.PYPI_PWD }}
         run: |
           pipx install twine
-          twine upload --skip-existing wheelhouse/*
+          twine upload --skip-existing dist/*
 
-  build_sdist:
+  build_wheels:
     name: Build source distribution
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Build sdist
-        run: pipx run build --sdist
+        run: pipx run build --wheel
 
       - name: publish
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.PYPI_PWD }}
         run: |
           pipx install twine
```

### Comparing `dcnum-0.10.0/.gitignore` & `dcnum-0.11.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/CHANGELOG` & `dcnum-0.11.0/CHANGELOG`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-0.0.10
+0.11.0
+ - feat: introduce GPUSegmenter base class
+ - fix: handle bytes-values in HDF5 attributes
+ - ref: correctly introduce `requires_background_correction` for segmenters
+ - setup: don't requrie cibuildwheel
+0.10.0
  - enh: some minor improvements in efficiency
  - ref: increment DCNUM_PPID_GENERATION for the sake of clarity
  - ref: unify dealing with num_workers and debugging
 0.0.9
  - fix: properly propagate event extraction keyword arguments
  - fix: QueueCollectorThread used uint16 for enumerating indices
  - fix: handle case where number of events is not multiple of chunk_size
```

### Comparing `dcnum-0.10.0/LICENSE` & `dcnum-0.11.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/PKG-INFO` & `dcnum-0.11.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.10.0
+Version: 0.11.0
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.10.0/README.rst` & `dcnum-0.11.0/README.rst`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/dcnum/feat/event_extractor_manager_thread.py` & `dcnum-0.11.0/dcnum/feat/event_extractor_manager_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/dcnum/feat/feat_background/base.py` & `dcnum-0.11.0/dcnum/feat/feat_background/base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/dcnum/feat/feat_background/bg_roll_median.py` & `dcnum-0.11.0/dcnum/feat/feat_background/bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/dcnum/feat/feat_background/bg_sparse_median.py` & `dcnum-0.11.0/dcnum/feat/feat_background/bg_sparse_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/dcnum/feat/feat_brightness/bright_all.py` & `dcnum-0.11.0/dcnum/feat/feat_brightness/bright_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/dcnum/feat/feat_moments/mt_legacy.py` & `dcnum-0.11.0/dcnum/feat/feat_moments/mt_legacy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/dcnum/feat/feat_texture/tex_all.py` & `dcnum-0.11.0/dcnum/feat/feat_texture/tex_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/dcnum/feat/gate.py` & `dcnum-0.11.0/dcnum/feat/gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/dcnum/feat/queue_event_extractor.py` & `dcnum-0.11.0/dcnum/feat/queue_event_extractor.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/dcnum/meta/ppid.py` & `dcnum-0.11.0/dcnum/meta/ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/dcnum/read/cache.py` & `dcnum-0.11.0/dcnum/read/cache.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/dcnum/read/hdf5_data.py` & `dcnum-0.11.0/dcnum/read/hdf5_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,17 @@
             self.tables = {}
             # get dataset configuration
             with h5py.File(self.path,
                            libver="latest",
                            locking=False,
                            ) as h5:
                 self.meta = dict(h5.attrs)
+                for key in self.meta:
+                    if isinstance(self.meta[key], bytes):
+                        self.meta[key] = self.meta[key].decode("utf-8")
                 for key in h5.get("logs", []):
                     alog = list(h5["logs"][key])
                     if isinstance(alog[0], bytes):
                         alog = [ll.decode("utf") for ll in alog]
                     self.logs[key] = alog
                 for tab in h5.get("tables", []):
                     self.tables[tab] = h5["tables"][key][:]
```

### Comparing `dcnum-0.10.0/dcnum/segm/segm_thresh.py` & `dcnum-0.11.0/dcnum/segm/segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/dcnum/segm/segmenter.py` & `dcnum-0.11.0/dcnum/segm/segmenter.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     #: Whether to enable mask post-processing. If disabled, you should
     #: make sure that your mask is properly defined and cleaned or you
     #: have to call `process_mask` in your `segment_approach` implementation.
     mask_postprocessing = False
     #: Default keyword arguments for mask post-processing. See `process_mask`
     #: for available options.
     mask_default_kwargs = {}
-    #: If the segmenter requires a background image, set this to True
-    requires_background = False
+    #: If the segmenter requires a background-corrected image, set this to True
+    requires_background_correction = False
 
     def __init__(self, kwargs_mask=None, debug=False, **kwargs):
         """Base segemnter
 
         Parameters
         ----------
         data: HDF5Data
@@ -228,13 +228,13 @@
         return segm_wrap
 
     @staticmethod
     @abc.abstractmethod
     def segment_approach(image):
         """Perform segmentation and return integer label or binary mask image
 
-        This is the approach the subclasses implements.
+        This is the approach the subclasses implement.
         """
 
     @abc.abstractmethod
     def segment_batch(self, data, start=None, stop=None):
         """Return the integer labels for an entire batch"""
```

### Comparing `dcnum-0.10.0/dcnum/segm/segmenter_cpu.py` & `dcnum-0.11.0/dcnum/segm/segmenter_cpu.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/dcnum/segm/segmenter_manager_thread.py` & `dcnum-0.11.0/dcnum/segm/segmenter_manager_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/dcnum/write/deque_writer_thread.py` & `dcnum-0.11.0/dcnum/write/deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/dcnum/write/queue_collector_thread.py` & `dcnum-0.11.0/dcnum/write/queue_collector_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/dcnum/write/writer.py` & `dcnum-0.11.0/dcnum/write/writer.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/dcnum.egg-info/PKG-INFO` & `dcnum-0.11.0/dcnum.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.10.0
+Version: 0.11.0
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.10.0/dcnum.egg-info/SOURCES.txt` & `dcnum-0.11.0/dcnum.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 dcnum/read/cache.py
 dcnum/read/const.py
 dcnum/read/hdf5_data.py
 dcnum/segm/__init__.py
 dcnum/segm/segm_thresh.py
 dcnum/segm/segmenter.py
 dcnum/segm/segmenter_cpu.py
+dcnum/segm/segmenter_gpu.py
 dcnum/segm/segmenter_manager_thread.py
 dcnum/write/__init__.py
 dcnum/write/deque_writer_thread.py
 dcnum/write/queue_collector_thread.py
 dcnum/write/writer.py
 docs/conf.py
 docs/index.rst
```

### Comparing `dcnum-0.10.0/docs/conf.py` & `dcnum-0.11.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/docs/extensions/github_changelog.py` & `dcnum-0.11.0/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/pyproject.toml` & `dcnum-0.11.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,9 @@
 [build-system]
-# Defined by PEP 518:
-# use oldest-supported-numpy (https://github.com/pypa/pip/issues/9542#issuecomment-771200755)
-requires = [
-    # for building Cython extensions
-    "cython", "oldest-supported-numpy", "setuptools", "wheel",
-    # for version management
-    "setuptools>=45", "setuptools_scm[toml]>=6.2"
-]
+requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dcnum"
 authors = [
     # In alphabetical order.
     {name = "Paul Müller"},
```

### Comparing `dcnum-0.10.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip` & `dcnum-0.11.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `dcnum-0.11.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/tests/helper_methods.py` & `dcnum-0.11.0/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/tests/test_feat_background_bg_roll_median.py` & `dcnum-0.11.0/tests/test_feat_background_bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/tests/test_feat_brightness.py` & `dcnum-0.11.0/tests/test_feat_brightness.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/tests/test_feat_haralick.py` & `dcnum-0.11.0/tests/test_feat_haralick.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/tests/test_feat_moments_based.py` & `dcnum-0.11.0/tests/test_feat_moments_based.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/tests/test_ppid.py` & `dcnum-0.11.0/tests/test_ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/tests/test_read_concat_hdf5.py` & `dcnum-0.11.0/tests/test_read_concat_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/tests/test_read_hdf5.py` & `dcnum-0.11.0/tests/test_read_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/tests/test_segm_thresh.py` & `dcnum-0.11.0/tests/test_segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/tests/test_write_deque_writer_thread.py` & `dcnum-0.11.0/tests/test_write_deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.10.0/tests/test_write_writer.py` & `dcnum-0.11.0/tests/test_write_writer.py`

 * *Files identical despite different names*

