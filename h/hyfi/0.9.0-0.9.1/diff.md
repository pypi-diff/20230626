# Comparing `tmp/hyfi-0.9.0.tar.gz` & `tmp/hyfi-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.9.0.tar", max compression
+gzip compressed data, was "hyfi-0.9.1.tar", max compression
```

## Comparing `hyfi-0.9.0.tar` & `hyfi-0.9.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0     1071 2023-06-20 07:37:38.410794 hyfi-0.9.0/LICENSE
--rw-r--r--   0        0        0     1828 2023-06-20 07:37:38.410794 hyfi-0.9.0/README.md
--rw-r--r--   0        0        0     4652 2023-06-20 07:38:04.170607 hyfi-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3810 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2550 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/__click__.py
--rw-r--r--   0        0        0      653 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/__global__/__init__.py
--rw-r--r--   0        0        0     9835 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/__global__/config.py
--rw-r--r--   0        0        0      733 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-06-20 07:38:04.098607 hyfi-0.9.0/src/hyfi/_version.py
--rw-r--r--   0        0        0      783 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     3353 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1923 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3449 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1244 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0        0 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-06-20 07:38:04.098607 hyfi-0.9.0/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      435 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       49 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      141 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0      320 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      559 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      725 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      291 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      948 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0       61 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       96 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0     1719 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      396 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      806 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0      153 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      195 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0     6414 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     3050 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8363 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     6627 2023-06-20 07:37:38.414794 hyfi-0.9.0/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0    21012 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/hydra/__init__.py
--rw-r--r--   0        0        0     7598 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/hydra/main.py
--rw-r--r--   0        0        0     3526 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     2987 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     2099 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    16595 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0     2642 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/joblib/pipe.py
--rw-r--r--   0        0        0    39697 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      225 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     2379 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0      973 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/path/batch.py
--rw-r--r--   0        0        0     3782 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5351 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/py.typed
--rw-r--r--   0        0        0     4042 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     5140 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0     1314 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    23179 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     6340 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10731 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     3769 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    19766 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     4828 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-06-20 07:37:38.418794 hyfi-0.9.0/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     3252 1970-01-01 00:00:00.000000 hyfi-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-20 09:05:25.739669 hyfi-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1828 2023-06-20 09:05:25.739669 hyfi-0.9.1/README.md
+-rw-r--r--   0        0        0     4652 2023-06-20 09:05:56.174588 hyfi-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3810 2023-06-20 09:05:25.743669 hyfi-0.9.1/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2550 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      653 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/__global__/__init__.py
+-rw-r--r--   0        0        0     9835 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/__global__/config.py
+-rw-r--r--   0        0        0      733 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-20 09:05:56.090579 hyfi-0.9.1/src/hyfi/_version.py
+-rw-r--r--   0        0        0      783 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     3353 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1923 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3449 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1244 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-20 09:05:56.090579 hyfi-0.9.1/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      435 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      141 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0      320 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      559 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      725 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      291 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      948 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/mode/debug.yaml
+-rw-r--r--   0        0        0       61 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       96 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0     1719 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      396 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      806 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      153 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      195 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0     6414 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     3050 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8363 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     6627 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0    21012 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/hydra/__init__.py
+-rw-r--r--   0        0        0     7598 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/hydra/main.py
+-rw-r--r--   0        0        0     3526 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     2987 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     2099 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    16595 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0     2642 2023-06-20 09:05:25.747670 hyfi-0.9.1/src/hyfi/joblib/pipe.py
+-rw-r--r--   0        0        0    39697 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      225 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     2379 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0      973 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0     3782 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5351 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/py.typed
+-rw-r--r--   0        0        0     4042 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     5140 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0     1314 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    23179 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     6358 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10731 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     3769 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    19766 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     4828 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-06-20 09:05:25.751670 hyfi-0.9.1/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     3252 1970-01-01 00:00:00.000000 hyfi-0.9.1/PKG-INFO
```

### Comparing `hyfi-0.9.0/LICENSE` & `hyfi-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/README.md` & `hyfi-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/pyproject.toml` & `hyfi-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.9.0"
+version = "0.9.1"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-0.9.0/src/hyfi/__cli__.py` & `hyfi-0.9.1/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/__click__.py` & `hyfi-0.9.1/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/__global__/__init__.py` & `hyfi-0.9.1/src/hyfi/__global__/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/__global__/config.py` & `hyfi-0.9.1/src/hyfi/__global__/config.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/__init__.py` & `hyfi-0.9.1/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/about/__init__.py` & `hyfi-0.9.1/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/batch/__init__.py` & `hyfi-0.9.1/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/cached_path/__init__.py` & `hyfi-0.9.1/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/cached_path/_cached_path.py` & `hyfi-0.9.1/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/cached_path/cache_file.py` & `hyfi-0.9.1/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/cached_path/common.py` & `hyfi-0.9.1/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/cached_path/file_lock.py` & `hyfi-0.9.1/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/cached_path/meta.py` & `hyfi-0.9.1/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/cached_path/progress.py` & `hyfi-0.9.1/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-0.9.1/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-0.9.1/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/cached_path/schemes/hf.py` & `hyfi-0.9.1/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/cached_path/schemes/http.py` & `hyfi-0.9.1/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-0.9.1/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/cached_path/testing.py` & `hyfi-0.9.1/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/cached_path/util.py` & `hyfi-0.9.1/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/conf/copier/conf.yaml` & `hyfi-0.9.1/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-0.9.1/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-0.9.1/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/conf/mode/__init__.yaml` & `hyfi-0.9.1/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/conf/path/__init__.yaml` & `hyfi-0.9.1/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/conf/project/__init__.yaml` & `hyfi-0.9.1/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/copier/__init__.py` & `hyfi-0.9.1/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/dotenv/__init__.py` & `hyfi-0.9.1/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/graphics/collage.py` & `hyfi-0.9.1/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/graphics/motion.py` & `hyfi-0.9.1/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/graphics/utils.py` & `hyfi-0.9.1/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/hydra/__init__.py` & `hyfi-0.9.1/src/hyfi/hydra/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/hydra/main.py` & `hyfi-0.9.1/src/hyfi/hydra/main.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/joblib/__init__.py` & `hyfi-0.9.1/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/joblib/batch/apply.py` & `hyfi-0.9.1/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-0.9.1/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/joblib/batch/batcher.py` & `hyfi-0.9.1/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/joblib/pipe.py` & `hyfi-0.9.1/src/hyfi/joblib/pipe.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/main/__init__.py` & `hyfi-0.9.1/src/hyfi/main/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/path/__init__.py` & `hyfi-0.9.1/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/path/batch.py` & `hyfi-0.9.1/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/path/task.py` & `hyfi-0.9.1/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/project/__init__.py` & `hyfi-0.9.1/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/task/__init__.py` & `hyfi-0.9.1/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/task/batch.py` & `hyfi-0.9.1/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/utils/contexts.py` & `hyfi-0.9.1/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/utils/datasets.py` & `hyfi-0.9.1/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/utils/envs.py` & `hyfi-0.9.1/src/hyfi/utils/envs.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,15 @@
             value = os.path.abspath(value)
         if pre_val := os.environ.get(key):
             logger.info("Overwriting %s=%s with %s", key, pre_val, value)
         else:
             logger.info("Setting %s=%s", key, value)
         os.environ[key] = value
 
+    @staticmethod
     def check_and_set_osenv(key: str, value: Any) -> Any:
         """Check and set value to environment variable"""
         env_key = key.upper()
         if value is not None:
             old_value = os.getenv(env_key, "")
             if str(old_value).lower() != str(value).lower():
                 os.environ[env_key] = str(value)
```

### Comparing `hyfi-0.9.0/src/hyfi/utils/funcs.py` & `hyfi-0.9.1/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/utils/gpumon.py` & `hyfi-0.9.1/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/utils/iolibs.py` & `hyfi-0.9.1/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/utils/logging.py` & `hyfi-0.9.1/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/utils/notebooks.py` & `hyfi-0.9.1/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/src/hyfi/utils/packages.py` & `hyfi-0.9.1/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.9.0/PKG-INFO` & `hyfi-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.9.0
+Version: 0.9.1
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

