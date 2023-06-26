# Comparing `tmp/acryl-datahub-actions-0.0.8.tar.gz` & `tmp/acryl-datahub-actions-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acryl-datahub-actions-0.0.8.tar", last modified: Fri Sep 23 01:12:13 2022, max compression
+gzip compressed data, was "acryl-datahub-actions-0.0.9.tar", last modified: Sun Dec  4 21:34:49 2022, max compression
```

## Comparing `acryl-datahub-actions-0.0.8.tar` & `acryl-datahub-actions-0.0.9.tar`

### file list

```diff
@@ -1,77 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.590940 acryl-datahub-actions-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     8888 2022-09-23 01:12:13.590940 acryl-datahub-actions-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7417 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-09-23 01:12:13.590940 acryl-datahub-actions-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     8434 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.578940 acryl-datahub-actions-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.582940 acryl-datahub-actions-0.0.8/src/acryl_datahub_actions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8888 2022-09-23 01:12:13.000000 acryl-datahub-actions-0.0.8/src/acryl_datahub_actions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2442 2022-09-23 01:12:13.000000 acryl-datahub-actions-0.0.8/src/acryl_datahub_actions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-23 01:12:13.000000 acryl-datahub-actions-0.0.8/src/acryl_datahub_actions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-09-23 01:12:13.000000 acryl-datahub-actions-0.0.8/src/acryl_datahub_actions.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-23 01:10:00.000000 acryl-datahub-actions-0.0.8/src/acryl_datahub_actions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     3333 2022-09-23 01:12:13.000000 acryl-datahub-actions-0.0.8/src/acryl_datahub_actions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-23 01:12:13.000000 acryl-datahub-actions-0.0.8/src/acryl_datahub_actions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.582940 acryl-datahub-actions-0.0.8/src/datahub_actions/
--rw-r--r--   0 runner    (1001) docker     (121)      914 2022-09-23 01:12:05.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.582940 acryl-datahub-actions-0.0.8/src/datahub_actions/action/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/action/action.py
--rw-r--r--   0 runner    (1001) docker     (121)      948 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/action/action_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1346 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/action/action_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.582940 acryl-datahub-actions-0.0.8/src/datahub_actions/api/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11119 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/api/action_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.582940 acryl-datahub-actions-0.0.8/src/datahub_actions/cli/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3697 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/cli/actions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4902 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/entrypoints.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.586940 acryl-datahub-actions-0.0.8/src/datahub_actions/event/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/event/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     2255 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/event/event_envelope.py
--rw-r--r--   0 runner    (1001) docker     (121)     3723 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/event/event_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.586940 acryl-datahub-actions-0.0.8/src/datahub_actions/pipeline/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11716 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)     2156 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/pipeline/pipeline_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/pipeline/pipeline_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     4028 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/pipeline/pipeline_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     5058 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/pipeline/pipeline_stats.py
--rw-r--r--   0 runner    (1001) docker     (121)     5545 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/pipeline/pipeline_util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.586940 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.586940 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/action/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/action/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.586940 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/action/execution/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/action/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8343 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/action/execution/executor_action.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.586940 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/action/hello_world/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/action/hello_world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/action/hello_world/hello_world.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.586940 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/source/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.586940 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/source/kafka/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/source/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8128 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/source/kafka/kafka_event_source.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.586940 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/transform/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.586940 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/transform/filter/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/transform/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3133 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/transform/filter/filter_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.590940 acryl-datahub-actions-0.0.8/src/datahub_actions/source/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/source/event_source.py
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/source/event_source_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.590940 acryl-datahub-actions-0.0.8/src/datahub_actions/transform/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/transform/transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/transform/transformer_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1689 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/transform/transformer_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 01:12:13.590940 acryl-datahub-actions-0.0.8/src/datahub_actions/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/utils/collection_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1957 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/utils/datahub_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     5444 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/utils/delta_extractor_mcl.py
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2022-09-23 01:08:48.000000 acryl-datahub-actions-0.0.8/src/datahub_actions/utils/event_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.666811 acryl-datahub-actions-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     8933 2022-12-04 21:34:49.666811 acryl-datahub-actions-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2022-12-04 21:34:49.670811 acryl-datahub-actions-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.658811 acryl-datahub-actions-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.662811 acryl-datahub-actions-0.0.9/src/acryl_datahub_actions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8933 2022-12-04 21:34:49.000000 acryl-datahub-actions-0.0.9/src/acryl_datahub_actions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2022-12-04 21:34:49.000000 acryl-datahub-actions-0.0.9/src/acryl_datahub_actions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-04 21:34:49.000000 acryl-datahub-actions-0.0.9/src/acryl_datahub_actions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2022-12-04 21:34:49.000000 acryl-datahub-actions-0.0.9/src/acryl_datahub_actions.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-04 21:32:20.000000 acryl-datahub-actions-0.0.9/src/acryl_datahub_actions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2022-12-04 21:34:49.000000 acryl-datahub-actions-0.0.9/src/acryl_datahub_actions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-04 21:34:49.000000 acryl-datahub-actions-0.0.9/src/acryl_datahub_actions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.662811 acryl-datahub-actions-0.0.9/src/datahub_actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2022-12-04 21:34:42.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.662811 acryl-datahub-actions-0.0.9/src/datahub_actions/action/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/action/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/action/action_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/action/action_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.662811 acryl-datahub-actions-0.0.9/src/datahub_actions/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10878 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/api/action_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.662811 acryl-datahub-actions-0.0.9/src/datahub_actions/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/cli/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/entrypoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.662811 acryl-datahub-actions-0.0.9/src/datahub_actions/event/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/event/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/event/event_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/event/event_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.666811 acryl-datahub-actions-0.0.9/src/datahub_actions/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/pipeline/pipeline_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/pipeline/pipeline_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/pipeline/pipeline_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/pipeline/pipeline_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/pipeline/pipeline_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.666811 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.666811 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.666811 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8466 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/execution/executor_action.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.666811 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/hello_world/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/hello_world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/hello_world/hello_world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.666811 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/slack/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.666811 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/teams/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/teams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/teams/teams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.666811 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.666811 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/source/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/source/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/source/kafka/kafka_event_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.666811 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.666811 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/transform/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/transform/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/transform/filter/filter_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.666811 acryl-datahub-actions-0.0.9/src/datahub_actions/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/source/event_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/source/event_source_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.666811 acryl-datahub-actions-0.0.9/src/datahub_actions/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/transform/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/transform/transformer_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/transform/transformer_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-04 21:34:49.666811 acryl-datahub-actions-0.0.9/src/datahub_actions/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/utils/collection_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/utils/datahub_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/utils/delta_extractor_mcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/utils/event_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/utils/name_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2022-12-04 21:31:39.000000 acryl-datahub-actions-0.0.9/src/datahub_actions/utils/social_util.py
```

### Comparing `acryl-datahub-actions-0.0.8/PKG-INFO` & `acryl-datahub-actions-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 Metadata-Version: 2.1
 Name: acryl-datahub-actions
-Version: 0.0.8
+Version: 0.0.9
 Summary: An action framework to work with DataHub real time changes.
 Home-page: https://datahubproject.io/
 License: Apache License 2.0
 Project-URL: Documentation, https://datahubproject.io/docs/actions
 Project-URL: Source, https://github.com/acryldata/datahub-actions
 Project-URL: Changelog, https://github.com/acryldata/datahub-actions/releases
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Topic :: Software Development
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: base
 Provides-Extra: kafka
 Provides-Extra: executor
+Provides-Extra: slack
+Provides-Extra: teams
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: integration-tests
 
 # ⚡ DataHub Actions Framework
 
 Welcome to DataHub Actions! The Actions framework makes responding to realtime changes in your Metadata Graph easy, enabling you to seamlessly integrate [DataHub](https://github.com/datahub-project/datahub) into a broader events-based architecture.
```

### Comparing `acryl-datahub-actions-0.0.8/README.md` & `acryl-datahub-actions-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/setup.cfg` & `acryl-datahub-actions-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/acryl_datahub_actions.egg-info/PKG-INFO` & `acryl-datahub-actions-0.0.9/src/acryl_datahub_actions.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 Metadata-Version: 2.1
 Name: acryl-datahub-actions
-Version: 0.0.8
+Version: 0.0.9
 Summary: An action framework to work with DataHub real time changes.
 Home-page: https://datahubproject.io/
 License: Apache License 2.0
 Project-URL: Documentation, https://datahubproject.io/docs/actions
 Project-URL: Source, https://github.com/acryldata/datahub-actions
 Project-URL: Changelog, https://github.com/acryldata/datahub-actions/releases
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Topic :: Software Development
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: base
 Provides-Extra: kafka
 Provides-Extra: executor
+Provides-Extra: slack
+Provides-Extra: teams
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: integration-tests
 
 # ⚡ DataHub Actions Framework
 
 Welcome to DataHub Actions! The Actions framework makes responding to realtime changes in your Metadata Graph easy, enabling you to seamlessly integrate [DataHub](https://github.com/datahub-project/datahub) into a broader events-based architecture.
```

### Comparing `acryl-datahub-actions-0.0.8/src/acryl_datahub_actions.egg-info/SOURCES.txt` & `acryl-datahub-actions-0.0.9/src/acryl_datahub_actions.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,18 @@
 src/datahub_actions/pipeline/pipeline_util.py
 src/datahub_actions/plugin/__init__.py
 src/datahub_actions/plugin/action/__init__.py
 src/datahub_actions/plugin/action/execution/__init__.py
 src/datahub_actions/plugin/action/execution/executor_action.py
 src/datahub_actions/plugin/action/hello_world/__init__.py
 src/datahub_actions/plugin/action/hello_world/hello_world.py
+src/datahub_actions/plugin/action/slack/__init__.py
+src/datahub_actions/plugin/action/slack/slack.py
+src/datahub_actions/plugin/action/teams/__init__.py
+src/datahub_actions/plugin/action/teams/teams.py
 src/datahub_actions/plugin/source/__init__.py
 src/datahub_actions/plugin/source/kafka/__init__.py
 src/datahub_actions/plugin/source/kafka/kafka_event_source.py
 src/datahub_actions/plugin/transform/__init__.py
 src/datahub_actions/plugin/transform/filter/__init__.py
 src/datahub_actions/plugin/transform/filter/filter_transformer.py
 src/datahub_actions/source/__init__.py
@@ -49,8 +53,10 @@
 src/datahub_actions/transform/transformer.py
 src/datahub_actions/transform/transformer_registry.py
 src/datahub_actions/transform/transformer_stats.py
 src/datahub_actions/utils/__init__.py
 src/datahub_actions/utils/collection_util.py
 src/datahub_actions/utils/datahub_util.py
 src/datahub_actions/utils/delta_extractor_mcl.py
-src/datahub_actions/utils/event_util.py
+src/datahub_actions/utils/event_util.py
+src/datahub_actions/utils/name_resolver.py
+src/datahub_actions/utils/social_util.py
```

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/__init__.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Published at https://pypi.org/project/acryl-datahub-actions/.
 __package_name__ = "acryl-datahub-actions"
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 
 def is_dev_mode() -> bool:
     return __version__ == "0.0.0.dev0"
 
 
 def nice_version_name() -> str:
```

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/action/__init__.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/action/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/action/action.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/action/action.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/action/action_registry.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/action/action_registry.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/action/action_stats.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/action/action_stats.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/api/__init__.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/api/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/api/action_graph.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/api/action_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,20 +215,17 @@
             entities = [x["entity"] for x in relnships]
             return target_urn in entities
         return False
 
     def add_tags_to_dataset(
         self, entity_urn: str, dataset_tags: List[str], field_tags: Dict = {}
     ) -> None:
-        aspect = "globalTags"
         global_tags = (
             self.graph.get_aspect(
                 entity_urn,
-                aspect,
-                aspect_type_name="com.linkedin.common.GlobalTags",
                 aspect_type=GlobalTagsClass,
             )
             or GlobalTagsClass.construct_with_defaults()
         )
 
         tag_map = {}
         for tag_assoc in global_tags.tags:
@@ -264,20 +261,16 @@
             #        aspect=global_tags,
             #    )
             # )
 
     def add_terms_to_dataset(
         self, entity_urn: str, dataset_terms: List[str], field_terms: Dict = {}
     ) -> None:
-        aspect = "glossaryTerms"
-
         glossary_terms = self.graph.get_aspect(
             entity_urn,
-            aspect,
-            aspect_type_name="com.linkedin.common.GlossaryTerms",
             aspect_type=GlossaryTermsClass,
         )
 
         if not glossary_terms:
             glossary_terms = GlossaryTermsClass(
                 terms=[],
                 auditStamp=AuditStampClass(
```

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/cli/__init__.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/cli/actions.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/cli/actions.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,40 +13,48 @@
 # limitations under the License.
 
 import logging
 import pathlib
 import signal
 import sys
 import time
+import unittest
 from typing import Any, List
 
 import click
 from click_default_group import DefaultGroup
-from datahub.configuration.config_loader import load_config_file
+from datahub.configuration.config_loader import load_config_file, resolve_element
 
 import datahub_actions as datahub_actions_package
 from datahub_actions.pipeline.pipeline import Pipeline
 from datahub_actions.pipeline.pipeline_manager import PipelineManager
 
 logger = logging.getLogger(__name__)
 
 
 # Instantiate a singleton instance of the Pipeline Manager.
 pipeline_manager = PipelineManager()
 
 
+def best_effort_resolve_element(x: str) -> str:
+    try:
+        return resolve_element(x)
+    except Exception:
+        return x
+
+
 def pipeline_config_to_pipeline(pipeline_config: dict) -> Pipeline:
     logger.debug(
-        f"Attempting to create Actions Pipeline using config {pipeline_config}"
+        f"Attempting to create Actions Pipeline using config {pipeline_config.get('name')}"
     )
     try:
         return Pipeline.create(pipeline_config)
     except Exception as e:
         raise Exception(
-            f"Failed to instantiate Actions Pipeline using config {pipeline_config}"
+            f"Failed to instantiate Actions Pipeline using config {pipeline_config.get('name')}: {e}"
         ) from e
 
 
 @click.group(cls=DefaultGroup, default="run")
 def actions() -> None:
     """Execute one or more Actions Pipelines"""
     pass
@@ -81,14 +89,27 @@
 
     logger.debug("Creating Actions Pipelines...")
 
     # If individual pipeline config was provided, create a pipeline from it.
     if config is not None:
         for pipeline_config in config:
             pipeline_config_file = pathlib.Path(pipeline_config)
+            with unittest.mock.patch(
+                "datahub.configuration.config_loader.resolve_element"
+            ) as mock_resolve_element:
+                mock_resolve_element.side_effect = best_effort_resolve_element
+                pipeline_config_dict = load_config_file(pipeline_config_file)
+                enabled = pipeline_config_dict.get("enabled", True)
+                if enabled == "false" or enabled is False:
+                    logger.warning(
+                        f"Skipping pipeline {pipeline_config_dict.get('name')} as it is not enabled"
+                    )
+                    continue
+
+            # now load the config with variable expansion
             pipeline_config_dict = load_config_file(pipeline_config_file)
             pipelines.append(
                 pipeline_config_to_pipeline(pipeline_config_dict)
             )  # Now, instantiate the pipeline.
 
     logger.debug("Starting Actions Pipelines")
```

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/entrypoints.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/entrypoints.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import logging
 import os
 import platform
 import sys
 
 import click
 import stackprinter
-from datahub.configuration import SensitiveError
 from prometheus_client import start_http_server
 
 import datahub_actions as datahub_package
 from datahub_actions.cli.actions import actions
 
 logger = logging.getLogger(__name__)
 
@@ -116,27 +115,21 @@
     except click.exceptions.Abort:
         # Click already automatically prints an abort message, so we can just exit.
         sys.exit(1)
     except click.ClickException as error:
         error.show()
         sys.exit(1)
     except Exception as exc:
-        kwargs = {}
-        sensitive_cause = SensitiveError.get_sensitive_cause(exc)
-        if sensitive_cause:
-            kwargs = {"show_vals": None}
-            exc = sensitive_cause
-
         logger.error(
             stackprinter.format(
                 exc,
                 line_wrap=MAX_CONTENT_WIDTH,
                 truncate_vals=10 * MAX_CONTENT_WIDTH,
                 suppressed_paths=[r"lib/python.*/site-packages/click/"],
-                **kwargs,
+                show_vals=False,
             )
         )
         logger.info(
             f"DataHub Actions version: {datahub_package.__version__} at {datahub_package.__file__}"
         )
         logger.info(
             f"Python version: {sys.version} at {sys.executable} on {platform.platform()}"
```

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/event/__init__.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/event/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/event/event.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/event/event.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/event/event_envelope.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/event/event_envelope.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/event/event_registry.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/event/event_registry.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/pipeline/__init__.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/pipeline/pipeline.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/pipeline/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,19 @@
         self._init_failed_events_dir()
 
     @classmethod
     def create(cls, config_dict: dict) -> "Pipeline":
         # Bind config
         config = PipelineConfig.parse_obj(config_dict)
 
+        if not config.enabled:
+            raise Exception(
+                "Pipeline is disabled, but create method was called unexpectedly."
+            )
+
         # Create Context
         ctx = create_action_context(config.name, config.datahub)
 
         # Create Event Source
         event_source = create_event_source(config.source, ctx)
 
         # Create Transforms
```

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/pipeline/pipeline_config.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/pipeline/pipeline_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,25 +52,23 @@
     failure_mode: Optional[FailureMode]
     failed_events_dir: Optional[str]  # The path where failed events should be logged.
 
     class Config:
         use_enum_values = True
 
 
-class PipelineConfig(BaseModel):
+class PipelineConfig(ConfigModel):
     """
     Configuration required to create a new Actions Pipeline.
 
     This exactly matches the structure of the YAML file used
     to configure a Pipeline.
     """
 
     name: str
+    enabled: bool = True
     source: SourceConfig
     filter: Optional[FilterConfig]
     transform: Optional[List[TransformConfig]]
     action: ActionConfig
     datahub: Optional[DatahubClientConfig]
     options: Optional[PipelineOptions]
-
-    class Config:
-        extra = "allow"
```

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/pipeline/pipeline_context.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/pipeline/pipeline_context.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/pipeline/pipeline_manager.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/pipeline/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/pipeline/pipeline_stats.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/pipeline/pipeline_stats.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/pipeline/pipeline_util.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/pipeline/pipeline_util.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/__init__.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/action/__init__.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/action/execution/__init__.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/action/execution/executor_action.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/execution/executor_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import importlib
 import json
 import logging
 import sys
-from typing import Any, Optional, cast
+from typing import Any, List, Optional, cast
 
 from acryl.executor.dispatcher.default_dispatcher import DefaultDispatcher
 from acryl.executor.execution.reporting_executor import (
     ReportingExecutor,
     ReportingExecutorConfig,
 )
 from acryl.executor.execution.task import TaskConfig
@@ -65,15 +65,15 @@
     for attr in object_name.split("."):
         item = getattr(item, attr)
     return item
 
 
 class ExecutorConfig(BaseModel):
     executor_id: Optional[str]
-    task_config: Optional[TaskConfig]
+    task_configs: Optional[List[TaskConfig]]
 
 
 # Listens to new Execution Requests & dispatches them to the appropriate handler.
 class ExecutorAction(Action):
     @classmethod
     def create(cls, config_dict: dict, ctx: PipelineContext) -> "Action":
         config = ExecutorConfig.parse_obj(config_dict or {})
@@ -170,39 +170,42 @@
                 self.dispatcher.dispatch_signal(signal_request)
             except Exception:
                 logger.error("ERROR", exc_info=sys.exc_info())
 
     def _build_executor_config(
         self, config: ExecutorConfig, ctx: PipelineContext
     ) -> ReportingExecutorConfig:
-
-        # Build default task config
-        ingest_task_config = config.task_config or TaskConfig(
-            name="RUN_INGEST",
-            type="acryl.executor.execution.sub_process_ingestion_task.SubProcessIngestionTask",
-            configs=dict({}),
-        )
-
-        test_connection_task_config = TaskConfig(
-            name="TEST_CONNECTION",
-            type="acryl.executor.execution.sub_process_test_connection_task.SubProcessTestConnectionTask",
-            configs={},
-        )
+        if config.task_configs:
+            task_configs = config.task_configs
+        else:
+            # Build default task config
+            task_configs = [
+                TaskConfig(
+                    name="RUN_INGEST",
+                    type="acryl.executor.execution.sub_process_ingestion_task.SubProcessIngestionTask",
+                    configs=dict({}),
+                ),
+                TaskConfig(
+                    name="TEST_CONNECTION",
+                    type="acryl.executor.execution.sub_process_test_connection_task.SubProcessTestConnectionTask",
+                    configs={},
+                ),
+            ]
 
         if not ctx.graph:
             raise Exception(
                 "Invalid configuration provided to action. DataHub Graph Client Required. Try including the 'datahub' block in your configuration."
             )
 
         graph = ctx.graph.graph
 
         # Build default executor config
         local_executor_config = ReportingExecutorConfig(
             id=config.executor_id or "default",
-            task_configs=[ingest_task_config, test_connection_task_config],
+            task_configs=task_configs,
             secret_stores=[
                 SecretStoreConfig(type="env", config=dict({})),
                 SecretStoreConfig(
                     type="datahub",
                     config=DataHubSecretStoreConfig(graph_client=graph),
                 ),
             ],
```

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/action/hello_world/__init__.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/hello_world/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/action/hello_world/hello_world.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/hello_world/hello_world.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/source/__init__.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/action/slack/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/source/kafka/__init__.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/source/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/source/kafka/kafka_event_source.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/source/kafka/kafka_event_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,26 @@
 
 ENTITY_CHANGE_EVENT_NAME = "entityChangeEvent"
 DEFAULT_TOPIC_ROUTES = {
     "mcl": "MetadataChangeLog_Versioned_v1",
     "pe": "PlatformEvent_v1",
 }
 
+OFFSET_METRIC = Gauge(
+    name="kafka_offset",
+    documentation="Kafka offsets per topic, partition",
+    labelnames=["topic", "partition", "pipeline_name"],
+)
+
+MESSAGE_COUNTER_METRIC = Counter(
+    name="kafka_messages",
+    documentation="Number of kafka messages",
+    labelnames=["pipeline_name", "error"],
+)
+
 
 # Converts a Kafka Message to a Kafka Metadata Dictionary.
 def build_kafka_meta(msg: Any) -> dict:
     return {
         "kafka": {
             "topic": msg.topic(),
             "offset": msg.offset(),
@@ -76,35 +88,27 @@
 
 
 class KafkaEventSourceConfig(ConfigModel):
     connection: KafkaConsumerConnectionConfig = KafkaConsumerConnectionConfig()
     topic_routes: Optional[Dict[str, str]]
 
 
-def kafka_messages_observer(labels: Dict[str, str] = {}) -> Callable:
-    print(["topic", "partition", *labels.keys()])
-    offset_metric = Gauge(
-        name="kafka_offset",
-        documentation="Kafka offsets per topic, partition",
-        labelnames=["topic", "partition", *labels.keys()],
-    )
-    counter = Counter(
-        name="kafka_messages_count",
-        documentation="Number of kafka messages",
-        labelnames=[*labels.keys(), "error"],
-    )
-
+def kafka_messages_observer(pipeline_name: str) -> Callable:
     def _observe(message):
         if message is not None:
             topic = message.topic()
             partition = message.partition()
             offset = message.offset()
             logger.debug(f"Kafka msg received: {topic}, {partition}, {offset}")
-            offset_metric.labels(topic=topic, partition=partition, **labels).set(offset)
-            counter.labels(error=message.error() is not None, **labels).inc()
+            OFFSET_METRIC.labels(
+                topic=topic, partition=partition, pipeline_name=pipeline_name
+            ).set(offset)
+            MESSAGE_COUNTER_METRIC.labels(
+                error=message.error() is not None, pipeline_name=pipeline_name
+            ).inc()
 
     return _observe
 
 
 # This is the default Kafka-based Event Source.
 @dataclass
 class KafkaEventSource(EventSource):
@@ -129,17 +133,15 @@
                     return_record_name=True,
                 ),
                 "session.timeout.ms": "10000",  # 10s timeout.
                 "max.poll.interval.ms": "10000",  # 10s poll max.
                 **self.source_config.connection.consumer_config,
             }
         )
-        self._observe_message: Callable = kafka_messages_observer(
-            {"pipeline_name": ctx.pipeline_name}
-        )
+        self._observe_message: Callable = kafka_messages_observer(ctx.pipeline_name)
 
     @classmethod
     def create(cls, config_dict: dict, ctx: PipelineContext) -> "EventSource":
         config = KafkaEventSourceConfig.parse_obj(config_dict)
         return cls(config, ctx)
 
     def events(self) -> Iterable[EventEnvelope]:
```

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/transform/__init__.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/source/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/transform/filter/__init__.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/plugin/transform/filter/filter_transformer.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/transform/filter/filter_transformer.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/source/__init__.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/plugin/transform/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/source/event_source.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/source/event_source.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/source/event_source_registry.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/source/event_source_registry.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/transform/__init__.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/source/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/transform/transformer.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/transform/transformer.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/transform/transformer_registry.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/transform/transformer_registry.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/transform/transformer_stats.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/transform/transformer_stats.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/utils/__init__.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/utils/collection_util.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/utils/collection_util.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/utils/datahub_util.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/utils/datahub_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 import re
 
+DATAHUB_SYSTEM_ACTOR_URN = "urn:li:corpuser:__datahub_system"
 ENTITY_TYPE_TO_URL_PATH_MAP = {
     "glossaryTerm": "glossary",
     "dataset": "dataset",
     "tag": "tag",
     "corpuser": "user",
 }
 logger = logging.getLogger(__name__)
```

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/utils/delta_extractor_mcl.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/utils/delta_extractor_mcl.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-actions-0.0.8/src/datahub_actions/utils/event_util.py` & `acryl-datahub-actions-0.0.9/src/datahub_actions/utils/event_util.py`

 * *Files identical despite different names*

