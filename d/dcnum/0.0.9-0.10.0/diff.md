# Comparing `tmp/dcnum-0.0.9.tar.gz` & `tmp/dcnum-0.10.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.0.9.tar", last modified: Fri Jun 23 09:35:12 2023, max compression
+gzip compressed data, was "dcnum-0.10.0.tar", last modified: Mon Jun 26 11:50:20 2023, max compression
```

## Comparing `dcnum-0.0.9.tar` & `dcnum-0.10.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:12.006134 dcnum-0.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.994125 dcnum-0.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.994125 dcnum-0.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-23 09:34:54.000000 dcnum-0.0.9/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-23 09:34:54.000000 dcnum-0.0.9/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-23 09:34:54.000000 dcnum-0.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-23 09:34:54.000000 dcnum-0.0.9/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-23 09:34:54.000000 dcnum-0.0.9/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-23 09:34:54.000000 dcnum-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-23 09:35:12.006134 dcnum-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-23 09:34:54.000000 dcnum-0.0.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.994125 dcnum-0.0.9/dcnum/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 09:35:11.000000 dcnum-0.0.9/dcnum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.998128 dcnum-0.0.9/dcnum/feat/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/event_extractor_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.998128 dcnum-0.0.9/dcnum/feat/feat_background/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_background/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_background/bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_background/bg_sparse_median.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.998128 dcnum-0.0.9/dcnum/feat/feat_brightness/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_brightness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_brightness/bright_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_brightness/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.998128 dcnum-0.0.9/dcnum/feat/feat_moments/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_moments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_moments/ct_opencv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_moments/mt_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.998128 dcnum-0.0.9/dcnum/feat/feat_texture/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_texture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_texture/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/feat_texture/tex_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/feat/queue_event_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.998128 dcnum-0.0.9/dcnum/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/meta/ppid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.998128 dcnum-0.0.9/dcnum/read/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/read/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/read/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/read/hdf5_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:12.002131 dcnum-0.0.9/dcnum/segm/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/segm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/segm/segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/segm/segmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/segm/segmenter_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/segm/segmenter_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:12.002131 dcnum-0.0.9/dcnum/write/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/write/deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/write/queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-23 09:34:54.000000 dcnum-0.0.9/dcnum/write/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:11.998128 dcnum-0.0.9/dcnum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-23 09:35:11.000000 dcnum-0.0.9/dcnum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-23 09:35:11.000000 dcnum-0.0.9/dcnum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:35:11.000000 dcnum-0.0.9/dcnum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-23 09:35:11.000000 dcnum-0.0.9/dcnum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 09:35:11.000000 dcnum-0.0.9/dcnum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:12.002131 dcnum-0.0.9/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-23 09:34:54.000000 dcnum-0.0.9/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:12.002131 dcnum-0.0.9/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-23 09:34:54.000000 dcnum-0.0.9/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-23 09:34:54.000000 dcnum-0.0.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-23 09:34:54.000000 dcnum-0.0.9/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-23 09:34:54.000000 dcnum-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:35:12.006134 dcnum-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:12.002131 dcnum-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:35:12.006134 dcnum-0.0.9/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_feat_background_bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_feat_brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_feat_haralick.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_feat_moments_based.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_ppid.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_ppid_segm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_read_concat_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_read_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_write_deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-23 09:34:54.000000 dcnum-0.0.9/tests/test_write_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.968482 dcnum-0.10.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.952481 dcnum-0.10.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.956481 dcnum-0.10.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-26 11:50:06.000000 dcnum-0.10.0/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-26 11:50:06.000000 dcnum-0.10.0/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-26 11:50:06.000000 dcnum-0.10.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-26 11:50:06.000000 dcnum-0.10.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-26 11:50:06.000000 dcnum-0.10.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 11:50:06.000000 dcnum-0.10.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-26 11:50:20.968482 dcnum-0.10.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-26 11:50:06.000000 dcnum-0.10.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.956481 dcnum-0.10.0/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-26 11:50:20.000000 dcnum-0.10.0/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.960482 dcnum-0.10.0/dcnum/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/event_extractor_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.960482 dcnum-0.10.0/dcnum/feat/feat_background/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_background/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_background/bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_background/bg_sparse_median.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.960482 dcnum-0.10.0/dcnum/feat/feat_brightness/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_brightness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_brightness/bright_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_brightness/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.960482 dcnum-0.10.0/dcnum/feat/feat_moments/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_moments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_moments/ct_opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_moments/mt_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.960482 dcnum-0.10.0/dcnum/feat/feat_texture/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_texture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_texture/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/feat_texture/tex_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/feat/queue_event_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.960482 dcnum-0.10.0/dcnum/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/meta/ppid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.964481 dcnum-0.10.0/dcnum/read/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/read/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/read/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/read/hdf5_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.964481 dcnum-0.10.0/dcnum/segm/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/segm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/segm/segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/segm/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/segm/segmenter_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/segm/segmenter_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.964481 dcnum-0.10.0/dcnum/write/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/write/deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/write/queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-26 11:50:06.000000 dcnum-0.10.0/dcnum/write/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.956481 dcnum-0.10.0/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-26 11:50:20.000000 dcnum-0.10.0/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-26 11:50:20.000000 dcnum-0.10.0/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 11:50:20.000000 dcnum-0.10.0/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-26 11:50:20.000000 dcnum-0.10.0/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 11:50:20.000000 dcnum-0.10.0/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.964481 dcnum-0.10.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-26 11:50:06.000000 dcnum-0.10.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.964481 dcnum-0.10.0/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-26 11:50:06.000000 dcnum-0.10.0/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-26 11:50:06.000000 dcnum-0.10.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 11:50:06.000000 dcnum-0.10.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-26 11:50:06.000000 dcnum-0.10.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 11:50:20.968482 dcnum-0.10.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.968482 dcnum-0.10.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:50:20.968482 dcnum-0.10.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_feat_background_bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_feat_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_feat_haralick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_feat_moments_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_ppid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_ppid_segm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_read_concat_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_read_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_write_deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-26 11:50:06.000000 dcnum-0.10.0/tests/test_write_writer.py
```

### Comparing `dcnum-0.0.9/.github/workflows/check.yml` & `dcnum-0.10.0/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/.github/workflows/deploy_pypi.yml` & `dcnum-0.10.0/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/.gitignore` & `dcnum-0.10.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/CHANGELOG` & `dcnum-0.10.0/CHANGELOG`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+0.0.10
+ - enh: some minor improvements in efficiency
+ - ref: increment DCNUM_PPID_GENERATION for the sake of clarity
+ - ref: unify dealing with num_workers and debugging
 0.0.9
  - fix: properly propagate event extraction keyword arguments
  - fix: QueueCollectorThread used uint16 for enumerating indices
  - fix: handle case where number of events is not multiple of chunk_size
  - enh: reduce thread waiting times
  - enh: add bounds check for image cache
 0.0.8
```

### Comparing `dcnum-0.0.9/LICENSE` & `dcnum-0.10.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/PKG-INFO` & `dcnum-0.10.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.0.9
+Version: 0.10.0
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.0.9/README.rst` & `dcnum-0.10.0/README.rst`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/dcnum/feat/event_extractor_manager_thread.py` & `dcnum-0.10.0/dcnum/feat/event_extractor_manager_thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                     break
                 else:
                     unavailable_slots += 1
                     cur_slot = (cur_slot + 1) % num_slots
                 if unavailable_slots >= num_slots:
                     # There is nothing to do, try to avoid 100% CPU
                     unavailable_slots = 0
-                    time.sleep(.01)
+                    time.sleep(.1)
 
             # We have a chunk, process it!
             chunk = self.slot_chunks[cur_slot]
             # Populate the labeling array for the workers
             new_labels = self.labels_list[cur_slot]
             if len(new_labels) == self.label_array.shape[0]:
                 self.label_array[:] = new_labels
@@ -113,15 +113,15 @@
                 raise ValueError("labels_list contains bad size data!")
             # Let the workers know there is work
             for ii in range(self.data.image.get_chunk_size(chunk)):
                 self.raw_queue.put((chunk, ii))
 
             # Make sure the entire chunk has been processed.
             while self.raw_queue.qsize():
-                time.sleep(.01)
+                time.sleep(.1)
 
             # We are done here. The segmenter may continue its deed.
             self.slot_states[cur_slot] = "w"
 
             self.logger.debug(f"Extracted one chunk: {chunk}")
 
             chunks_processed += 1
```

### Comparing `dcnum-0.0.9/dcnum/feat/feat_background/base.py` & `dcnum-0.10.0/dcnum/feat/feat_background/base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/dcnum/feat/feat_background/bg_roll_median.py` & `dcnum-0.10.0/dcnum/feat/feat_background/bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/dcnum/feat/feat_background/bg_sparse_median.py` & `dcnum-0.10.0/dcnum/feat/feat_background/bg_sparse_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/dcnum/feat/feat_brightness/bright_all.py` & `dcnum-0.10.0/dcnum/feat/feat_brightness/bright_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/dcnum/feat/feat_moments/mt_legacy.py` & `dcnum-0.10.0/dcnum/feat/feat_moments/mt_legacy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/dcnum/feat/feat_texture/tex_all.py` & `dcnum-0.10.0/dcnum/feat/feat_texture/tex_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,17 @@
     # compute features if necessary
     if image_bg is not None or image_corr is not None:
         # Background-corrected brightness values
         if image_corr is None:
             image_corr = np.array(image, dtype=np.int16) - image_bg
 
     tex_dict = {}
+    empty = np.full(size, np.nan, dtype=np.float64)
     for key in haralick_names:
-        tex_dict[key] = np.full(size, np.nan, dtype=np.float64)
+        tex_dict[key] = np.copy(empty)
 
     for ii in range(size):
         # Haralick texture features
         # https://gitlab.gwdg.de/blood_data_analysis/dcevent/-/issues/20
         # Preprocessing:
         # - create a copy of the array (don't edit `image_corr`)
         # - add grayscale values (negative values not supported)
```

### Comparing `dcnum-0.0.9/dcnum/feat/gate.py` & `dcnum-0.10.0/dcnum/feat/gate.py`

 * *Files 7% similar despite different names*

```diff
@@ -153,10 +153,20 @@
                 valid = np.logical_and(valid,
                                        self.gate_feature(feat, events[feat])
                                        )
         else:
             raise ValueError("Empty events provided!")
         return valid
 
-    def gate_mask(self, mask):
-        """Gate the mask, return False if the mask should not be used"""
-        return np.sum(mask) > self.kwargs["size_thresh_mask"]
+    def gate_mask(self, mask, mask_sum=None):
+        """Gate the mask, return False if the mask should not be used
+
+        Parameters
+        ----------
+        mask: 2d ndarray
+            The boolean mask image for the event.
+        mask_sum: int
+            The sum of the mask (if not specified, it is computed)
+        """
+        if mask_sum is None:
+            mask_sum = np.sum(mask)
+        return mask_sum > self.kwargs["size_thresh_mask"]
```

### Comparing `dcnum-0.0.9/dcnum/feat/queue_event_extractor.py` & `dcnum-0.10.0/dcnum/feat/queue_event_extractor.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,20 +176,22 @@
         else:
             gated_events = events
 
         return gated_events
 
     def get_masks_from_label(self, label):
         """Get masks, performing mask-based gating"""
-        unu = np.unique(label)  # background is 0
+        # Using np.unique is a little slower than iterating over lmax
+        # unu = np.unique(label)  # background is 0
+        lmax = np.max(label)
         masks = []
-        for jj in unu[1:]:  # first item is 0
+        for jj in range(1, lmax+1):  # first item is 0
             mask_jj = label == jj
-            # mask-based gating
-            if self.gate.gate_mask(mask_jj):
+            mask_sum = np.sum(mask_jj)
+            if mask_sum and self.gate.gate_mask(mask_jj, mask_sum=mask_sum):
                 masks.append(mask_jj)
         return np.array(masks)
 
     def get_ppid(self):
         """Return a unique feature extractor pipeline identifier
 
         The pipeline identifier is universally applicable and must
```

### Comparing `dcnum-0.0.9/dcnum/meta/ppid.py` & `dcnum-0.10.0/dcnum/meta/ppid.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import hashlib
 import inspect
 import pathlib
 
 
 #: Increment this string if there are breaking changes that make
 #: previous pipelines unreproducible.
-DCNUM_PPID_GENERATION = "1"
+DCNUM_PPID_GENERATION = "2"
 
 
 def compute_pipeline_hash(bg_id, seg_id, feat_id, gate_id,
                           gen_id=DCNUM_PPID_GENERATION):
     hasher = hashlib.md5()
     hasher.update("|".join([gen_id, bg_id, seg_id, feat_id, gate_id]).encode())
     pph = hasher.hexdigest()
```

### Comparing `dcnum-0.0.9/dcnum/read/cache.py` & `dcnum-0.10.0/dcnum/read/cache.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/dcnum/read/hdf5_data.py` & `dcnum-0.10.0/dcnum/read/hdf5_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,18 @@
         self.logs = state["logs"]
         self.tables = state["tables"]
         self.meta = state["meta"]
         if self.meta is None or self.logs is None or self.tables is None:
             self.logs = {}
             self.tables = {}
             # get dataset configuration
-            with h5py.File(self.path) as h5:
+            with h5py.File(self.path,
+                           libver="latest",
+                           locking=False,
+                           ) as h5:
                 self.meta = dict(h5.attrs)
                 for key in h5.get("logs", []):
                     alog = list(h5["logs"][key])
                     if isinstance(alog[0], bytes):
                         alog = [ll.decode("utf") for ll in alog]
                     self.logs[key] = alog
                 for tab in h5.get("tables", []):
```

### Comparing `dcnum-0.0.9/dcnum/segm/segm_thresh.py` & `dcnum-0.10.0/dcnum/segm/segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/dcnum/segm/segmenter.py` & `dcnum-0.10.0/dcnum/segm/segmenter.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,18 +190,18 @@
             mask = labels != 2147483647
             labels, _ = ndi.label(
                 input=mask,
                 structure=ndi.generate_binary_structure(2, 2))
 
         return labels
 
-    def segment_chunk(self, image_data, chunk, debug=False):
+    def segment_chunk(self, image_data, chunk):
         """Return the integer labels for one `image_data` chunk"""
         data = image_data.get_chunk(chunk)
-        return self.segment_batch(data, debug=debug)
+        return self.segment_batch(data)
 
     def segment_frame(self, image):
         """Return the integer label image for `index`"""
         segm_wrap = self.segment_frame_wrapper()
         # obtain mask or label
         mol = segm_wrap(image)
         if mol.dtype == bool:
@@ -232,9 +232,9 @@
     def segment_approach(image):
         """Perform segmentation and return integer label or binary mask image
 
         This is the approach the subclasses implements.
         """
 
     @abc.abstractmethod
-    def segment_batch(self, data, start=None, stop=None, debug=False):
+    def segment_batch(self, data, start=None, stop=None):
         """Return the integer labels for an entire batch"""
```

### Comparing `dcnum-0.0.9/dcnum/segm/segmenter_cpu.py` & `dcnum-0.10.0/dcnum/segm/segmenter_cpu.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,17 @@
 
 import numpy as np
 
 from .segmenter import Segmenter
 
 
 class CPUSegmenter(Segmenter, abc.ABC):
-    #: Number of segmenter processes to use.
-    num_processes = None
-
-    def __init__(self, *args, **kwargs):
+    def __init__(self, num_workers=None, *args, **kwargs):
         super(CPUSegmenter, self).__init__(*args, **kwargs)
+        self.num_workers = num_workers or mp.cpu_count()
         self.mp_image_raw = None
         self._mp_image_np = None
         self.mp_labels_raw = None
         self._mp_labels_np = None
         self._mp_workers = []
         # Image shape of the input array
         self.image_shape = None
@@ -92,28 +90,25 @@
         if self._mp_workers:
             self.mp_shutdown.value = 1
             [w.join() for w in self._mp_workers]
 
     def segment_batch(self,
                       image_data: np.ndarray,
                       start: int = None,
-                      stop: int = None,
-                      debug: bool = False):
+                      stop: int = None):
         """Perform batch segmentation of `image_data`
 
         Parameters
         ----------
         image_data: 3d np.ndarray
             The time-series image data. First axis is time.
         start: int
             First index to analyze in `image_data`
         stop: int
             Index after the last index to analyze in `image_data`
-        debug: bool
-            Whether to run this in debug mode (using a single thread)
 
         Notes
         -----
         - If the segmentation algorithm only accepts background-corrected
           images, then `image_data` must already be background-corrected.
         """
         if stop is None or start is None:
@@ -152,21 +147,20 @@
                 dtype=np.ctypeslib.ctypes.c_uint16,
             )
 
         # populate image data
         self._mp_image_np[:] = image_data[start:stop]
 
         # Create the workers
-        if debug:
+        if self.debug:
             worker_cls = CPUSegmenterWorkerThread
             num_workers = 1
         else:
             worker_cls = CPUSegmenterWorkerProcess
-            num_workers = min(self.num_processes or mp.cpu_count(),
-                              image_data.shape[0])
+            num_workers = min(self.num_workers, image_data.shape[0])
 
         if not self._mp_workers:
             step_size = batch_size // num_workers
             rest = batch_size % num_workers
             wstart = 0
             for ii in range(num_workers):
                 # Give every worker the same-sized workload and add one
```

### Comparing `dcnum-0.0.9/dcnum/segm/segmenter_manager_thread.py` & `dcnum-0.10.0/dcnum/segm/segmenter_manager_thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,16 +95,15 @@
                     # There is nothing to do, try to avoid 100% CPU
                     empty_slots = 0
                     time.sleep(.01)
 
             # We have a free slot to compute the segmentation
             labels = self.segmenter.segment_chunk(
                 image_data=self.image_data,
-                chunk=chunk,
-                debug=self.debug)
+                chunk=chunk)
 
             # TODO: make this more memory efficient (pre-shared mp.Arrays?)
             # Store labels in a list accessible by the main thread
             self.labels_list[cur_slot] = np.copy(labels)
             # Remember the chunk index for this slot
             self.slot_chunks[cur_slot] = chunk
             # This must be done last: Let the extractor know that this
```

### Comparing `dcnum-0.0.9/dcnum/write/deque_writer_thread.py` & `dcnum-0.10.0/dcnum/write/deque_writer_thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
         path_out:
             Path to the output HDF5 file
         dq:
             `collections.deque` object from which data are taken
             using `popleft()`.
         """
         super(DequeWriterThread, self).__init__(*args, **kwargs)
+        if mode == "w":
+            path_out.unlink(missing_ok=True)
         self.writer = HDF5Writer(path_out, mode=mode, ds_kwds=ds_kwds)
         self.dq = dq
         self.may_stop_loop = False
         self.must_stop_loop = False
 
     def abort_loop(self):
         """Force aborting the loop as soon as possible"""
```

### Comparing `dcnum-0.0.9/dcnum/write/queue_collector_thread.py` & `dcnum-0.10.0/dcnum/write/queue_collector_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/dcnum/write/writer.py` & `dcnum-0.10.0/dcnum/write/writer.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/dcnum.egg-info/PKG-INFO` & `dcnum-0.10.0/dcnum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.0.9
+Version: 0.10.0
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.0.9/dcnum.egg-info/SOURCES.txt` & `dcnum-0.10.0/dcnum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/docs/conf.py` & `dcnum-0.10.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/docs/extensions/github_changelog.py` & `dcnum-0.10.0/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/pyproject.toml` & `dcnum-0.10.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip` & `dcnum-0.10.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `dcnum-0.10.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/tests/helper_methods.py` & `dcnum-0.10.0/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/tests/test_feat_background_bg_roll_median.py` & `dcnum-0.10.0/tests/test_feat_background_bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/tests/test_feat_brightness.py` & `dcnum-0.10.0/tests/test_feat_brightness.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/tests/test_feat_haralick.py` & `dcnum-0.10.0/tests/test_feat_haralick.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/tests/test_feat_moments_based.py` & `dcnum-0.10.0/tests/test_feat_moments_based.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/tests/test_ppid.py` & `dcnum-0.10.0/tests/test_ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/tests/test_read_concat_hdf5.py` & `dcnum-0.10.0/tests/test_read_concat_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/tests/test_read_hdf5.py` & `dcnum-0.10.0/tests/test_read_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/tests/test_segm_thresh.py` & `dcnum-0.10.0/tests/test_segm_thresh.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,17 +76,18 @@
     for ii, fr in enumerate(frame):
         idx = np.where(frame_u == fr)[0]
         mask_u[idx] = np.logical_or(mask_u[idx], mask[ii])
 
     image_u_c = np.array(image_u, dtype=int) - image_bg_u
 
     sm = segm.segm_thresh.SegmentThresh(thresh=-6,
+                                        debug=debug,
                                         kwargs_mask={"closing_disk": 3})
 
-    labels_seg = sm.segment_batch(image_u_c, start=0, stop=5, debug=debug)
+    labels_seg = sm.segment_batch(image_u_c, start=0, stop=5)
     assert labels_seg is sm.labels_array
     assert np.all(np.array(labels_seg, dtype=bool) == sm.mask_array)
     # tell workers to stop
     sm.join_workers()
 
     for ii in range(len(frame_u)):
         mask_seg = np.array(labels_seg[ii], dtype=bool)
@@ -102,32 +103,33 @@
 
     # Create fake data
     mask = np.zeros((121, 80, 200), dtype=bool)
     mask[:, 10:71, 100:161] = morphology.disk(30).reshape(-1, 61, 61)
     image = -10 * mask
 
     sm = segm.segm_thresh.SegmentThresh(thresh=-6,
-                                        kwargs_mask={"closing_disk": 3})
+                                        kwargs_mask={"closing_disk": 3},
+                                        debug=debug)
 
     labels_seg_1 = np.copy(
-        sm.segment_batch(image, start=0, stop=101, debug=debug))
+        sm.segment_batch(image, start=0, stop=101))
 
     assert labels_seg_1.dtype == np.uint16  # uint8 is not enough
     assert sm.mp_batch_index.value == 0
     if worker_type == "thread":
         assert len(sm._mp_workers) == 1
         assert sm.mp_batch_worker.value == 1
     else:
         # This will fail if you have too many CPUs in your system
         assert len(sm._mp_workers) == mp.cpu_count()
         # Check whether all processes did their deeds
         assert sm.mp_batch_worker.value == mp.cpu_count()
 
     labels_seg_2 = np.copy(
-        sm.segment_batch(image, start=101, stop=121, debug=debug))
+        sm.segment_batch(image, start=101, stop=121))
 
     # tell workers to stop
     sm.join_workers()
 
     for ii in range(101):
         mask_seg = np.array(labels_seg_1[ii], dtype=bool)
         assert np.all(mask_seg == mask[ii]), f"masks not matching at {ii}"
```

### Comparing `dcnum-0.0.9/tests/test_write_deque_writer_thread.py` & `dcnum-0.10.0/tests/test_write_deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.9/tests/test_write_writer.py` & `dcnum-0.10.0/tests/test_write_writer.py`

 * *Files identical despite different names*

