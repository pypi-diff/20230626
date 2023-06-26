# Comparing `tmp/optimum-neuron-0.0.5.tar.gz` & `tmp/optimum-neuron-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-neuron-0.0.5.tar", last modified: Fri Jun 23 16:06:47 2023, max compression
+gzip compressed data, was "optimum-neuron-0.0.6.tar", last modified: Mon Jun 26 16:36:24 2023, max compression
```

## Comparing `optimum-neuron-0.0.5.tar` & `optimum-neuron-0.0.6.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/
--rw-rw-r--   0 michael   (1000) michael   (1000)    11357 2023-02-01 11:11:22.000000 optimum-neuron-0.0.5/LICENSE
--rw-rw-r--   0 michael   (1000) michael   (1000)      651 2023-02-10 14:28:23.000000 optimum-neuron-0.0.5/MANIFEST.in
--rw-rw-r--   0 michael   (1000) michael   (1000)    10761 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     9532 2023-06-15 15:45:47.000000 optimum-neuron-0.0.5/README.md
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.065550 optimum-neuron-0.0.5/optimum/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.065550 optimum-neuron-0.0.5/optimum/commands/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.065550 optimum-neuron-0.0.5/optimum/commands/export/
--rw-rw-r--   0 michael   (1000) michael   (1000)     5451 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/commands/export/neuron.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4927 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/commands/export/neuronx.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.065550 optimum-neuron-0.0.5/optimum/commands/neuron/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1174 2023-05-24 11:58:50.000000 optimum-neuron-0.0.5/optimum/commands/neuron/base.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     8818 2023-06-23 15:37:53.000000 optimum-neuron-0.0.5/optimum/commands/neuron/cache.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.065550 optimum-neuron-0.0.5/optimum/commands/register/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1270 2023-04-28 16:14:49.000000 optimum-neuron-0.0.5/optimum/commands/register/register_export.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      755 2023-04-28 16:14:49.000000 optimum-neuron-0.0.5/optimum/commands/register/register_neuron.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.065550 optimum-neuron-0.0.5/optimum/exporters/
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.065550 optimum-neuron-0.0.5/optimum/exporters/neuron/
--rw-rw-r--   0 michael   (1000) michael   (1000)      705 2023-04-14 14:05:35.000000 optimum-neuron-0.0.5/optimum/exporters/neuron/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5317 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/exporters/neuron/__main__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    11086 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/exporters/neuron/base.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1132 2023-04-14 14:05:35.000000 optimum-neuron-0.0.5/optimum/exporters/neuron/config.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    12824 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/exporters/neuron/convert.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4092 2023-05-30 08:48:22.000000 optimum-neuron-0.0.5/optimum/exporters/neuron/model_configs.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.065550 optimum-neuron-0.0.5/optimum/neuron/
--rw-rw-r--   0 michael   (1000) michael   (1000)     2431 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/optimum/neuron/__init__.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/optimum/neuron/accelerate/
--rw-rw-r--   0 michael   (1000) michael   (1000)      732 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/optimum/neuron/accelerate/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    12887 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/accelerate/accelerator.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2330 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/accelerate/optimizer.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2212 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/optimum/neuron/accelerate/scheduler.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    15103 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/accelerate/state.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/optimum/neuron/accelerate/utils/
--rw-rw-r--   0 michael   (1000) michael   (1000)      764 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/accelerate/utils/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6605 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/accelerate/utils/dataclasses.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1076 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/optimum/neuron/accelerate/utils/misc.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/optimum/neuron/distributed/
--rw-rw-r--   0 michael   (1000) michael   (1000)      714 2023-06-15 15:45:47.000000 optimum-neuron-0.0.5/optimum/neuron/distributed/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     7136 2023-06-15 15:45:47.000000 optimum-neuron-0.0.5/optimum/neuron/distributed/base.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3797 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/distributed/encoder_models.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2172 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/distributed/parallelizers_manager.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2324 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/distributed/utils.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/optimum/neuron/generation/
--rw-rw-r--   0 michael   (1000) michael   (1000)      668 2023-05-12 19:29:59.000000 optimum-neuron-0.0.5/optimum/neuron/generation/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    70566 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/neuron/generation/utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2340 2023-05-24 11:58:50.000000 optimum-neuron-0.0.5/optimum/neuron/hf_argparser.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    18847 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/neuron/modeling.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    18203 2023-06-23 15:37:53.000000 optimum-neuron-0.0.5/optimum/neuron/modeling_base.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    12800 2023-06-08 09:55:27.000000 optimum-neuron-0.0.5/optimum/neuron/trainer_callback.py
--rwxrwxr-x   0 michael   (1000) michael   (1000)    15201 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/trainers.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     8564 2023-06-23 15:37:53.000000 optimum-neuron-0.0.5/optimum/neuron/training_args.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/optimum/neuron/utils/
--rw-rw-r--   0 michael   (1000) michael   (1000)     1244 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/optimum/neuron/utils/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     5967 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/neuron/utils/argument_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    29996 2023-06-23 15:37:53.000000 optimum-neuron-0.0.5/optimum/neuron/utils/cache_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    16580 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/neuron/utils/compilation_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      701 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/optimum/neuron/utils/constant.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1879 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/optimum/neuron/utils/import_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     2187 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/optimum/neuron/utils/misc.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     6684 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/optimum/neuron/utils/patching.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1644 2023-04-14 14:05:35.000000 optimum-neuron-0.0.5/optimum/neuron/utils/testing_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    10129 2023-06-23 15:37:47.000000 optimum-neuron-0.0.5/optimum/neuron/utils/training_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      858 2023-05-24 11:58:50.000000 optimum-neuron-0.0.5/optimum/neuron/utils/version_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      639 2023-06-23 15:38:20.000000 optimum-neuron-0.0.5/optimum/neuron/version.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/optimum_neuron.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)    10761 2023-06-23 16:06:47.000000 optimum-neuron-0.0.5/optimum_neuron.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)     2212 2023-06-23 16:06:47.000000 optimum-neuron-0.0.5/optimum_neuron.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       39 2023-06-23 16:06:47.000000 optimum-neuron-0.0.5/optimum_neuron.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       66 2023-06-23 16:06:47.000000 optimum-neuron-0.0.5/optimum_neuron.egg-info/entry_points.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-02-15 10:08:35.000000 optimum-neuron-0.0.5/optimum_neuron.egg-info/not-zip-safe
--rw-rw-r--   0 michael   (1000) michael   (1000)      406 2023-06-23 16:06:47.000000 optimum-neuron-0.0.5/optimum_neuron.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        8 2023-06-23 16:06:47.000000 optimum-neuron-0.0.5/optimum_neuron.egg-info/top_level.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)     1161 2023-04-14 14:05:35.000000 optimum-neuron-0.0.5/pyproject.toml
--rw-rw-r--   0 michael   (1000) michael   (1000)      430 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/setup.cfg
--rw-rw-r--   0 michael   (1000) michael   (1000)     2882 2023-06-23 15:59:16.000000 optimum-neuron-0.0.5/setup.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-23 16:06:47.069550 optimum-neuron-0.0.5/tests/
--rw-rw-r--   0 michael   (1000) michael   (1000)    34743 2023-06-13 15:28:53.000000 optimum-neuron-0.0.5/tests/test_cache_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3415 2023-05-24 11:58:50.000000 optimum-neuron-0.0.5/tests/test_compilation_utils.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    27302 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/tests/test_examples.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     4696 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/tests/test_generate.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    45311 2023-06-15 09:54:42.000000 optimum-neuron-0.0.5/tests/test_modeling.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     9283 2023-05-30 08:48:22.000000 optimum-neuron-0.0.5/tests/test_trainer_callback.py
--rw-rw-r--   0 michael   (1000) michael   (1000)    17857 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/tests/test_trainers.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     8584 2023-06-20 12:11:35.000000 optimum-neuron-0.0.5/tests/test_utils.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.907713 optimum-neuron-0.0.6/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    11357 2023-02-01 11:11:22.000000 optimum-neuron-0.0.6/LICENSE
+-rw-rw-r--   0 michael   (1000) michael   (1000)      651 2023-02-10 14:28:23.000000 optimum-neuron-0.0.6/MANIFEST.in
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10761 2023-06-26 16:36:24.907713 optimum-neuron-0.0.6/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9532 2023-06-15 15:45:47.000000 optimum-neuron-0.0.6/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.899713 optimum-neuron-0.0.6/optimum/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.899713 optimum-neuron-0.0.6/optimum/commands/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/commands/export/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5451 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/commands/export/neuron.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4927 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/commands/export/neuronx.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/commands/neuron/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1174 2023-05-24 11:58:50.000000 optimum-neuron-0.0.6/optimum/commands/neuron/base.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8818 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/commands/neuron/cache.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/commands/register/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1270 2023-04-28 16:14:49.000000 optimum-neuron-0.0.6/optimum/commands/register/register_export.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      755 2023-04-28 16:14:49.000000 optimum-neuron-0.0.6/optimum/commands/register/register_neuron.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.899713 optimum-neuron-0.0.6/optimum/exporters/
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/exporters/neuron/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      705 2023-04-14 14:05:35.000000 optimum-neuron-0.0.6/optimum/exporters/neuron/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5317 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/exporters/neuron/__main__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    11086 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/exporters/neuron/base.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1132 2023-04-14 14:05:35.000000 optimum-neuron-0.0.6/optimum/exporters/neuron/config.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    12824 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/exporters/neuron/convert.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4092 2023-05-30 08:48:22.000000 optimum-neuron-0.0.6/optimum/exporters/neuron/model_configs.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/neuron/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2431 2023-06-20 12:11:35.000000 optimum-neuron-0.0.6/optimum/neuron/__init__.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/neuron/accelerate/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      732 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/accelerate/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    12887 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/accelerate/accelerator.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2330 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/accelerate/optimizer.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2212 2023-06-20 12:11:35.000000 optimum-neuron-0.0.6/optimum/neuron/accelerate/scheduler.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    15103 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/accelerate/state.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/neuron/accelerate/utils/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      764 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/accelerate/utils/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6605 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/accelerate/utils/dataclasses.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1076 2023-06-20 12:11:35.000000 optimum-neuron-0.0.6/optimum/neuron/accelerate/utils/misc.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/neuron/distributed/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      714 2023-06-15 15:45:47.000000 optimum-neuron-0.0.6/optimum/neuron/distributed/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     7136 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/distributed/base.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3797 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/distributed/encoder_models.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2172 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/distributed/parallelizers_manager.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2324 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/distributed/utils.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/neuron/generation/
+-rw-rw-r--   0 michael   (1000) michael   (1000)      668 2023-05-12 19:29:59.000000 optimum-neuron-0.0.6/optimum/neuron/generation/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    70566 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/neuron/generation/utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2340 2023-05-24 11:58:50.000000 optimum-neuron-0.0.6/optimum/neuron/hf_argparser.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    18847 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/neuron/modeling.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    18203 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/modeling_base.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    12800 2023-06-08 09:55:27.000000 optimum-neuron-0.0.6/optimum/neuron/trainer_callback.py
+-rwxrwxr-x   0 michael   (1000) michael   (1000)    15201 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/trainers.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8663 2023-06-26 16:31:54.000000 optimum-neuron-0.0.6/optimum/neuron/training_args.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.903713 optimum-neuron-0.0.6/optimum/neuron/utils/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1244 2023-06-20 12:11:35.000000 optimum-neuron-0.0.6/optimum/neuron/utils/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5967 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/neuron/utils/argument_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    29996 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/utils/cache_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    16580 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/neuron/utils/compilation_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      701 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/optimum/neuron/utils/constant.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1879 2023-06-20 12:11:35.000000 optimum-neuron-0.0.6/optimum/neuron/utils/import_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2187 2023-06-20 12:11:35.000000 optimum-neuron-0.0.6/optimum/neuron/utils/misc.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     6684 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/utils/patching.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1644 2023-04-14 14:05:35.000000 optimum-neuron-0.0.6/optimum/neuron/utils/testing_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10129 2023-06-26 16:31:49.000000 optimum-neuron-0.0.6/optimum/neuron/utils/training_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      858 2023-05-24 11:58:50.000000 optimum-neuron-0.0.6/optimum/neuron/utils/version_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)      639 2023-06-26 16:32:38.000000 optimum-neuron-0.0.6/optimum/neuron/version.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.907713 optimum-neuron-0.0.6/optimum_neuron.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    10761 2023-06-26 16:36:24.000000 optimum-neuron-0.0.6/optimum_neuron.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2212 2023-06-26 16:36:24.000000 optimum-neuron-0.0.6/optimum_neuron.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       39 2023-06-26 16:36:24.000000 optimum-neuron-0.0.6/optimum_neuron.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       66 2023-06-26 16:36:24.000000 optimum-neuron-0.0.6/optimum_neuron.egg-info/entry_points.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-02-15 10:08:35.000000 optimum-neuron-0.0.6/optimum_neuron.egg-info/not-zip-safe
+-rw-rw-r--   0 michael   (1000) michael   (1000)      406 2023-06-26 16:36:24.000000 optimum-neuron-0.0.6/optimum_neuron.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        8 2023-06-26 16:36:24.000000 optimum-neuron-0.0.6/optimum_neuron.egg-info/top_level.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1161 2023-04-14 14:05:35.000000 optimum-neuron-0.0.6/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)      430 2023-06-26 16:36:24.907713 optimum-neuron-0.0.6/setup.cfg
+-rw-rw-r--   0 michael   (1000) michael   (1000)     2882 2023-06-26 16:36:15.000000 optimum-neuron-0.0.6/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2023-06-26 16:36:24.907713 optimum-neuron-0.0.6/tests/
+-rw-rw-r--   0 michael   (1000) michael   (1000)    34743 2023-06-13 15:28:53.000000 optimum-neuron-0.0.6/tests/test_cache_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     3415 2023-05-24 11:58:50.000000 optimum-neuron-0.0.6/tests/test_compilation_utils.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    27302 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/tests/test_examples.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     4696 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/tests/test_generate.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    45311 2023-06-15 09:54:42.000000 optimum-neuron-0.0.6/tests/test_modeling.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     9283 2023-05-30 08:48:22.000000 optimum-neuron-0.0.6/tests/test_trainer_callback.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)    17857 2023-06-20 12:11:35.000000 optimum-neuron-0.0.6/tests/test_trainers.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     8584 2023-06-20 12:11:35.000000 optimum-neuron-0.0.6/tests/test_utils.py
```

### Comparing `optimum-neuron-0.0.5/LICENSE` & `optimum-neuron-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/MANIFEST.in` & `optimum-neuron-0.0.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/PKG-INFO` & `optimum-neuron-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-neuron
-Version: 0.0.5
+Version: 0.0.6
 Summary: Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS Tranium and Inferentia accelerators. It provides a set of tools enabling easy model loading, training and inference on single and multiple neuron core settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/aws
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,inference,tranium,inferentia,aws
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `optimum-neuron-0.0.5/README.md` & `optimum-neuron-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/commands/export/neuron.py` & `optimum-neuron-0.0.6/optimum/commands/export/neuron.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/commands/export/neuronx.py` & `optimum-neuron-0.0.6/optimum/commands/export/neuronx.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/commands/neuron/base.py` & `optimum-neuron-0.0.6/optimum/commands/neuron/base.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/commands/neuron/cache.py` & `optimum-neuron-0.0.6/optimum/commands/neuron/cache.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/commands/register/register_export.py` & `optimum-neuron-0.0.6/optimum/commands/register/register_export.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/commands/register/register_neuron.py` & `optimum-neuron-0.0.6/optimum/commands/register/register_neuron.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/exporters/neuron/__init__.py` & `optimum-neuron-0.0.6/optimum/exporters/neuron/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/exporters/neuron/__main__.py` & `optimum-neuron-0.0.6/optimum/exporters/neuron/__main__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/exporters/neuron/base.py` & `optimum-neuron-0.0.6/optimum/exporters/neuron/base.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/exporters/neuron/config.py` & `optimum-neuron-0.0.6/optimum/exporters/neuron/config.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/exporters/neuron/convert.py` & `optimum-neuron-0.0.6/optimum/exporters/neuron/convert.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/exporters/neuron/model_configs.py` & `optimum-neuron-0.0.6/optimum/exporters/neuron/model_configs.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/__init__.py` & `optimum-neuron-0.0.6/optimum/neuron/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/accelerate/__init__.py` & `optimum-neuron-0.0.6/optimum/neuron/accelerate/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/accelerate/accelerator.py` & `optimum-neuron-0.0.6/optimum/neuron/accelerate/accelerator.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/accelerate/optimizer.py` & `optimum-neuron-0.0.6/optimum/neuron/accelerate/optimizer.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/accelerate/scheduler.py` & `optimum-neuron-0.0.6/optimum/neuron/accelerate/scheduler.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/accelerate/state.py` & `optimum-neuron-0.0.6/optimum/neuron/accelerate/state.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/accelerate/utils/__init__.py` & `optimum-neuron-0.0.6/optimum/neuron/accelerate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/accelerate/utils/dataclasses.py` & `optimum-neuron-0.0.6/optimum/neuron/accelerate/utils/dataclasses.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/accelerate/utils/misc.py` & `optimum-neuron-0.0.6/optimum/neuron/accelerate/utils/misc.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/distributed/__init__.py` & `optimum-neuron-0.0.6/optimum/neuron/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/distributed/base.py` & `optimum-neuron-0.0.6/optimum/neuron/distributed/base.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/distributed/encoder_models.py` & `optimum-neuron-0.0.6/optimum/neuron/distributed/encoder_models.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/distributed/parallelizers_manager.py` & `optimum-neuron-0.0.6/optimum/neuron/distributed/parallelizers_manager.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/distributed/utils.py` & `optimum-neuron-0.0.6/optimum/neuron/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/generation/__init__.py` & `optimum-neuron-0.0.6/optimum/neuron/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/generation/utils.py` & `optimum-neuron-0.0.6/optimum/neuron/generation/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/hf_argparser.py` & `optimum-neuron-0.0.6/optimum/neuron/hf_argparser.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/modeling.py` & `optimum-neuron-0.0.6/optimum/neuron/modeling.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/modeling_base.py` & `optimum-neuron-0.0.6/optimum/neuron/modeling_base.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/trainer_callback.py` & `optimum-neuron-0.0.6/optimum/neuron/trainer_callback.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/trainers.py` & `optimum-neuron-0.0.6/optimum/neuron/trainers.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/training_args.py` & `optimum-neuron-0.0.6/optimum/neuron/training_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,17 @@
                     f"{TRANSFORMERS_MIN_VERSION_FOR_XLA_FSDP} but {transformers.__version__} is installed."
                 )
         super().__post_init__()
 
     # Needed only to specialize the warning message for FSDP.
     @cached_property
     def _setup_devices(self) -> "torch.device":
+        if not check_if_transformers_greater("4.30.0"):
+            return super()._setup_devices
+
         requires_backends(self, ["torch"])
         logger.info("PyTorch: setting up devices")
         NeuronAcceleratorState._reset_state()
         NeuronPartialState._reset_state()
         if not is_sagemaker_mp_enabled() and not is_accelerate_available():
             raise ImportError(
                 "Using the `Trainer` with `PyTorch` requires `accelerate>=0.20.1`: Please run `pip install "
```

### Comparing `optimum-neuron-0.0.5/optimum/neuron/utils/__init__.py` & `optimum-neuron-0.0.6/optimum/neuron/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/utils/argument_utils.py` & `optimum-neuron-0.0.6/optimum/neuron/utils/argument_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/utils/cache_utils.py` & `optimum-neuron-0.0.6/optimum/neuron/utils/cache_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/utils/compilation_utils.py` & `optimum-neuron-0.0.6/optimum/neuron/utils/compilation_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/utils/constant.py` & `optimum-neuron-0.0.6/optimum/neuron/utils/constant.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/utils/import_utils.py` & `optimum-neuron-0.0.6/optimum/neuron/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/utils/misc.py` & `optimum-neuron-0.0.6/optimum/neuron/utils/misc.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/utils/patching.py` & `optimum-neuron-0.0.6/optimum/neuron/utils/patching.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/utils/testing_utils.py` & `optimum-neuron-0.0.6/optimum/neuron/utils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/utils/training_utils.py` & `optimum-neuron-0.0.6/optimum/neuron/utils/training_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/utils/version_utils.py` & `optimum-neuron-0.0.6/optimum/neuron/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/optimum/neuron/version.py` & `optimum-neuron-0.0.6/optimum/neuron/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
```

### Comparing `optimum-neuron-0.0.5/optimum_neuron.egg-info/PKG-INFO` & `optimum-neuron-0.0.6/optimum_neuron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-neuron
-Version: 0.0.5
+Version: 0.0.6
 Summary: Optimum Neuron is the interface between the Hugging Face Transformers and Diffusers libraries and AWS Tranium and Inferentia accelerators. It provides a set of tools enabling easy model loading, training and inference on single and multiple neuron core settings for different downstream tasks.
 Home-page: https://huggingface.co/hardware/aws
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,diffusers,mixed-precision training,fine-tuning,inference,tranium,inferentia,aws
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `optimum-neuron-0.0.5/optimum_neuron.egg-info/SOURCES.txt` & `optimum-neuron-0.0.6/optimum_neuron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/pyproject.toml` & `optimum-neuron-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/setup.py` & `optimum-neuron-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/tests/test_cache_utils.py` & `optimum-neuron-0.0.6/tests/test_cache_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/tests/test_compilation_utils.py` & `optimum-neuron-0.0.6/tests/test_compilation_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/tests/test_examples.py` & `optimum-neuron-0.0.6/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/tests/test_generate.py` & `optimum-neuron-0.0.6/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/tests/test_modeling.py` & `optimum-neuron-0.0.6/tests/test_modeling.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/tests/test_trainer_callback.py` & `optimum-neuron-0.0.6/tests/test_trainer_callback.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/tests/test_trainers.py` & `optimum-neuron-0.0.6/tests/test_trainers.py`

 * *Files identical despite different names*

### Comparing `optimum-neuron-0.0.5/tests/test_utils.py` & `optimum-neuron-0.0.6/tests/test_utils.py`

 * *Files identical despite different names*

