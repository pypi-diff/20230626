# Comparing `tmp/openmetadata_managed_apis-1.0.5.0.tar.gz` & `tmp/openmetadata_managed_apis-1.1.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmetadata_managed_apis-1.0.5.0.tar", last modified: Mon Jun 19 13:23:31 2023, max compression
+gzip compressed data, was "openmetadata_managed_apis-1.1.0.0.dev0.tar", last modified: Mon Jun 26 12:17:36 2023, max compression
```

## Comparing `openmetadata_managed_apis-1.0.5.0.tar` & `openmetadata_managed_apis-1.1.0.0.dev0.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:23:31.940691 openmetadata_managed_apis-1.0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-06-19 13:23:31.940691 openmetadata_managed_apis-1.0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:23:31.928691 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:23:31.932691 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/apis_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:23:31.932691 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/disable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/enable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/health.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/kill.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/last_dag_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/run_automation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:23:31.936691 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/operations/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/operations/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/operations/kill_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/operations/last_dag_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/operations/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/operations/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/operations/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:23:31.936691 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/resources/dag_runner.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:23:31.936691 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/utils/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:23:31.936691 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/views/rest_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:23:31.928691 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/views/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:23:31.936691 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/views/templates/rest_api/
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/views/templates/rest_api/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:23:31.936691 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:23:31.940691 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/credentials_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/data_insight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/dbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/es_reindex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/lineage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/workflow_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/workflow_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:23:31.928691 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-06-19 13:23:28.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-19 13:23:28.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:23:28.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-19 13:23:28.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:23:13.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-19 13:23:28.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-19 13:23:28.000000 openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 13:23:31.940691 openmetadata_managed_apis-1.0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-19 13:21:38.000000 openmetadata_managed_apis-1.0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.778164 openmetadata_managed_apis-1.1.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-06-26 12:17:36.778164 openmetadata_managed_apis-1.1.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.770165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.774165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/apis_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.774165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/disable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/enable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/health_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/kill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/last_dag_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/run_automation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.774165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/kill_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/last_dag_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.774165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/resources/dag_runner.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.774165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/utils/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.774165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/views/rest_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.770165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/views/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.774165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/views/templates/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/views/templates/rest_api/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.778164 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.778164 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13613 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/data_insight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/es_reindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/workflow_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/workflow_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:36.770165 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-06-26 12:17:32.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-26 12:17:32.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:17:32.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-26 12:17:32.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:17:18.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-26 12:17:32.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-26 12:17:32.000000 openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 12:17:36.778164 openmetadata_managed_apis-1.1.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-26 12:15:58.000000 openmetadata_managed_apis-1.1.0.0.dev0/setup.py
```

### Comparing `openmetadata_managed_apis-1.0.5.0/PKG-INFO` & `openmetadata_managed_apis-1.1.0.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmetadata_managed_apis
-Version: 1.0.5.0
+Version: 1.1.0.0.dev0
 Summary: Airflow REST APIs to create and manage DAGS
 Home-page: https://open-metadata.org/
 Author: OpenMetadata Committers
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.open-metadata.org/
 Project-URL: Source, https://github.com/open-metadata/OpenMetadata
 Requires-Python: >=3.7
```

### Comparing `openmetadata_managed_apis-1.0.5.0/README.md` & `openmetadata_managed_apis-1.1.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/__init__.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/__init__.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/apis_metadata.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/apis_metadata.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/app.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/app.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/config.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/config.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/error_handlers.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/error_handlers.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/response.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/response.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/delete.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/delete.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/deploy.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/deploy.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         try:
             if json_request is None:
                 return ApiResponse.error(
                     status=ApiResponse.STATUS_BAD_REQUEST,
                     error=f"Did not receive any JSON request to deploy",
                 )
 
-            ingestion_pipeline = IngestionPipeline(**json_request)
+            ingestion_pipeline = IngestionPipeline.parse_obj(json_request)
 
             deployer = DagDeployer(ingestion_pipeline)
             response = deployer.deploy()
 
             return response
 
         except ValidationError as err:
```

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/disable.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/disable.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/enable.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/enable.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/health.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/health.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,27 +7,25 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """
 Health endpoint. Globally accessible
 """
-import traceback
 from typing import Callable
 
 from flask import Blueprint
+from openmetadata_managed_apis.operations.health import health_response
 from openmetadata_managed_apis.utils.logger import routes_logger
 
 try:
     from importlib.metadata import version
 except ImportError:
     from importlib_metadata import version
 
-from openmetadata_managed_apis.api.response import ApiResponse
-
 logger = routes_logger()
 
 
 def get_fn(blueprint: Blueprint) -> Callable:
     """
     Return the function loaded to a route
     :param blueprint: Flask Blueprint to assign route to
@@ -41,21 +39,10 @@
     @blueprint.route("/health", methods=["GET"])
     @csrf.exempt
     def health():
         """
         /health endpoint to check Airflow REST status without auth
         """
 
-        try:
-            return ApiResponse.success(
-                {"status": "healthy", "version": version("openmetadata-ingestion")}
-            )
-        except Exception as exc:
-            msg = f"Error obtaining Airflow REST status due to [{exc}] "
-            logger.debug(traceback.format_exc())
-            logger.error(msg)
-            return ApiResponse.error(
-                status=ApiResponse.STATUS_BAD_REQUEST,
-                error=msg,
-            )
+        return health_response()
 
     return health
```

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/ip.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/ip.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 IP endpoint
 """
 import traceback
 from typing import Callable, Optional
 
 import requests
-from flask import Blueprint
+from flask import Blueprint, escape
 from openmetadata_managed_apis.api.response import ApiResponse
 from openmetadata_managed_apis.utils.logger import routes_logger
 from requests.exceptions import ConnectionError
 from urllib3.exceptions import NewConnectionError
 
 logger = routes_logger()
 
@@ -66,15 +66,15 @@
         this IP to access their source systems.
         """
 
         try:
             for ip_service in IP_SERVICES:
                 host_ip = _get_ip_safely(ip_service)
                 if host_ip:
-                    return ApiResponse.success({"ip": host_ip})
+                    return ApiResponse.success({"ip": escape(host_ip)})
 
             # If we cannot fetch the IP, still return a 200 but without informing the IP.
             return ApiResponse.success({"ip": "unknown"})
 
         except Exception as exc:
             msg = f"Internal error obtaining host IP due to [{exc}] "
             logger.debug(traceback.format_exc())
```

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/kill.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/kill.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/last_dag_logs.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/last_dag_logs.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/run_automation.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/run_automation.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,20 +10,17 @@
 #  limitations under the License.
 """
 Test the connection against a source system
 """
 import traceback
 from typing import Callable
 
-from flask import Blueprint, Response, request
+from flask import Blueprint, Response, escape, request
 from openmetadata_managed_apis.api.response import ApiResponse
 from openmetadata_managed_apis.utils.logger import routes_logger
-from openmetadata_managed_apis.workflows.ingestion.credentials_builder import (
-    build_secrets_manager_credentials,
-)
 from pydantic import ValidationError
 
 from metadata.automations.runner import execute
 from metadata.generated.schema.entity.automations.workflow import (
     Workflow as AutomationWorkflow,
 )
 from metadata.utils.secrets.secrets_manager_factory import SecretsManagerFactory
@@ -60,24 +57,22 @@
             automation_workflow: AutomationWorkflow = AutomationWorkflow.parse_obj(
                 json_request
             )
 
             # we need to instantiate the secret manager in case secrets are passed
             SecretsManagerFactory(
                 automation_workflow.openMetadataServerConnection.secretsManagerProvider,
-                build_secrets_manager_credentials(
-                    automation_workflow.openMetadataServerConnection.secretsManagerProvider
-                ),
+                automation_workflow.openMetadataServerConnection.secretsManagerLoader,
             )
 
             execute(automation_workflow)
 
             return ApiResponse.success(
                 {
-                    "message": f"Workflow [{automation_workflow.name}] has been triggered."
+                    "message": f"Workflow [{escape(automation_workflow.name)}] has been triggered."
                 }
             )
 
         except ValidationError as err:
             msg = f"Request Validation Error parsing payload: {err}"
             logger.debug(traceback.format_exc())
             logger.error(msg)
```

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/status.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/status.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/routes/trigger.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/routes/trigger.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/api/utils.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/api/utils.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/operations/delete.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/delete.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/operations/deploy.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/deploy.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,33 +11,30 @@
 
 import pkgutil
 import traceback
 from pathlib import Path
 from typing import Dict
 
 from airflow import DAG, settings
-from airflow.jobs.scheduler_job import SchedulerJob
 from airflow.models import DagModel
+from flask import escape
 from jinja2 import Template
 from openmetadata_managed_apis.api.config import (
     AIRFLOW_DAGS_FOLDER,
     DAG_GENERATED_CONFIGS,
     PLUGIN_NAME,
 )
 from openmetadata_managed_apis.api.response import ApiResponse
 from openmetadata_managed_apis.api.utils import (
     clean_dag_id,
     get_dagbag,
     import_path,
     scan_dags_job_background,
 )
 from openmetadata_managed_apis.utils.logger import operations_logger
-from openmetadata_managed_apis.workflows.ingestion.credentials_builder import (
-    build_secrets_manager_credentials,
-)
 
 from metadata.generated.schema.entity.services.ingestionPipelines.ingestionPipeline import (
     IngestionPipeline,
 )
 from metadata.ingestion.models.encoders import show_secrets_encoder
 from metadata.utils.secrets.secrets_manager_factory import SecretsManagerFactory
 
@@ -59,17 +56,15 @@
     def __init__(self, ingestion_pipeline: IngestionPipeline):
         logger.info(
             f"Received the following Airflow Configuration: {ingestion_pipeline.airflowConfig}"
         )
         # we need to instantiate the secret manager in case secrets are passed
         SecretsManagerFactory(
             ingestion_pipeline.openMetadataServerConnection.secretsManagerProvider,
-            build_secrets_manager_credentials(
-                ingestion_pipeline.openMetadataServerConnection.secretsManagerProvider
-            ),
+            ingestion_pipeline.openMetadataServerConnection.secretsManagerLoader,
         )
         self.ingestion_pipeline = ingestion_pipeline
         self.dag_id = clean_dag_id(self.ingestion_pipeline.name.__root__)
 
     def store_airflow_pipeline_config(
         self, dag_config_file_path: Path
     ) -> Dict[str, str]:
@@ -90,15 +85,15 @@
         the rendered strings
         """
 
         dag_py_file = Path(AIRFLOW_DAGS_FOLDER) / f"{self.dag_id}.py"
 
         # Open the template and render
         raw_template = pkgutil.get_data(PLUGIN_NAME, "resources/dag_runner.j2").decode()
-        template = Template(raw_template)
+        template = Template(raw_template, autoescape=True)
 
         rendered_dag = template.render(dag_runner_config)
 
         # Create the DAGs path if it does not exist
         if not dag_py_file.parent.is_dir():
             dag_py_file.parent.mkdir(parents=True, exist_ok=True)
 
@@ -147,15 +142,15 @@
                 logger.debug(traceback.format_exc())
                 logger.error(msg)
                 return ApiResponse.server_error({f"message": msg})
 
         scan_dags_job_background()
 
         return ApiResponse.success(
-            {"message": f"Workflow [{self.dag_id}] has been created"}
+            {"message": f"Workflow [{escape(self.dag_id)}] has been created"}
         )
 
     def deploy(self):
         """
         Run all methods to deploy the DAG
         """
         dag_config_file_path = Path(DAG_GENERATED_CONFIGS) / f"{self.dag_id}.json"
```

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/operations/kill_all.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/kill_all.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/operations/last_dag_logs.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/last_dag_logs.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/operations/state.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/state.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/operations/status.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/status.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/operations/trigger.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/operations/trigger.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/plugin.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/plugin.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/utils/logger.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/utils/logger.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/utils/parser.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/utils/parser.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/views/rest_api.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/views/rest_api.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/views/templates/rest_api/index.html` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/views/templates/rest_api/index.html`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/config.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/config.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/common.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,31 +26,31 @@
 from metadata.generated.schema.entity.services.dashboardService import DashboardService
 from metadata.generated.schema.entity.services.databaseService import DatabaseService
 from metadata.generated.schema.entity.services.messagingService import MessagingService
 from metadata.generated.schema.entity.services.metadataService import MetadataService
 from metadata.generated.schema.entity.services.mlmodelService import MlModelService
 from metadata.generated.schema.entity.services.pipelineService import PipelineService
 from metadata.generated.schema.entity.services.storageService import StorageService
-from metadata.generated.schema.tests.testSuite import TestSuite
+from metadata.generated.schema.metadataIngestion.testSuitePipeline import (
+    TestSuitePipeline,
+)
 from metadata.ingestion.models.encoders import show_secrets_encoder
 from metadata.ingestion.ometa.ometa_api import OpenMetadata
+from metadata.utils.fqn import split
 
 try:
     from airflow.operators.python import PythonOperator
 except ModuleNotFoundError:
     from airflow.operators.python_operator import PythonOperator
 
 from openmetadata_managed_apis.utils.logger import set_operator_logger, workflow_logger
 from openmetadata_managed_apis.utils.parser import (
     parse_service_connection,
     parse_validation_err,
 )
-from openmetadata_managed_apis.workflows.ingestion.credentials_builder import (
-    build_secrets_manager_credentials,
-)
 
 from metadata.generated.schema.entity.services.ingestionPipelines.ingestionPipeline import (
     IngestionPipeline,
     PipelineState,
 )
 from metadata.generated.schema.metadataIngestion.workflow import (
     LogLevels,
@@ -100,48 +100,39 @@
     """
     Use the service EntityReference to build the Source.
     Building the source dynamically helps us to not store any
     sensitive info.
     :param ingestion_pipeline: With the service ref
     :return: WorkflowSource
     """
-    secrets_manager = (
-        ingestion_pipeline.openMetadataServerConnection.secretsManagerProvider
-    )
-    ingestion_pipeline.openMetadataServerConnection.secretsManagerCredentials = (
-        build_secrets_manager_credentials(secrets_manager)
-    )
 
     try:
         metadata = OpenMetadata(config=ingestion_pipeline.openMetadataServerConnection)
     except Exception as exc:
         raise ClientInitializationError(
             f"Failed to initialize the OpenMetadata client due to: {exc}."
             " Make sure that the Airflow host can reach the OpenMetadata"
             f" server running at {ingestion_pipeline.openMetadataServerConnection.hostPort}"
             " and that the client and server are in the same version."
         )
 
     service_type = ingestion_pipeline.service.type
 
-    if service_type == "testSuite":
-        service = metadata.get_by_name(
-            entity=TestSuite, fqn=ingestion_pipeline.service.name
-        )  # check we are able to access OM server
-        if not service:
-            raise GetServiceException(service_type, ingestion_pipeline.service.name)
-
-        return WorkflowSource(
-            type=service_type,
-            serviceName=ingestion_pipeline.service.name,
-            sourceConfig=ingestion_pipeline.sourceConfig,
-        )
-
     entity_class = None
     try:
+        if service_type == "testSuite":
+            # check we can access OM server
+            metadata.health_check()
+            return WorkflowSource(
+                type=service_type,
+                serviceName=ingestion_pipeline.service.name,
+                sourceConfig=ingestion_pipeline.sourceConfig,
+                serviceConnection=None,  # retrieved from the test suite workflow using the `sourceConfig.config.entityFullyQualifiedName`
+            )
+
         if service_type == "databaseService":
             entity_class = DatabaseService
             service: DatabaseService = metadata.get_by_name(
                 entity=entity_class, fqn=ingestion_pipeline.service.name
             )
         elif service_type == "pipelineService":
             entity_class = PipelineService
```

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/data_insight.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/data_insight.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/dbt.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/dbt.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     OpenMetadataConnection,
 )
 from metadata.generated.schema.entity.services.ingestionPipelines.ingestionPipeline import (
     IngestionPipeline,
 )
 from metadata.generated.schema.metadataIngestion.workflow import Sink
 from metadata.generated.schema.type.basic import ComponentConfig
-from metadata.utils.constants import ES_SOURCE_TO_ES_OBJ_ARGS
+from metadata.utils.constants import ES_SOURCE_IGNORE_KEYS, ES_SOURCE_TO_ES_OBJ_ARGS
 
 
 def build_elasticsearch_sink(
     openmetadata_service_connection: OpenMetadataConnection,
     ingestion_pipeline: IngestionPipeline,
 ) -> Sink:
     """
@@ -38,15 +38,15 @@
     elasticsearch_service_config_dict = (
         openmetadata_service_connection.elasticsSearch.config.dict()
     )
 
     elasticsearch_source_config_dict = {
         ES_SOURCE_TO_ES_OBJ_ARGS[key]: value
         for key, value in ingestion_pipeline.sourceConfig.config.dict().items()
-        if value and key != "type"
+        if value and key not in ES_SOURCE_IGNORE_KEYS
     }
 
     return Sink(
         type="elasticsearch",
         config=ComponentConfig(
             **elasticsearch_service_config_dict,
             **elasticsearch_source_config_dict,
```

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/es_reindex.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/es_reindex.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,17 +13,14 @@
 """
 from airflow import DAG
 from openmetadata_managed_apis.workflows.ingestion.common import (
     ClientInitializationError,
     build_dag,
     metadata_ingestion_workflow,
 )
-from openmetadata_managed_apis.workflows.ingestion.elasticsearch_sink import (
-    build_elasticsearch_sink,
-)
 
 from metadata.generated.schema.entity.services.connections.metadata.metadataESConnection import (
     MetadataESConnection,
 )
 from metadata.generated.schema.entity.services.ingestionPipelines.ingestionPipeline import (
     IngestionPipeline,
 )
@@ -35,19 +32,15 @@
     LogLevels,
     OpenMetadataWorkflowConfig,
     Sink,
 )
 from metadata.generated.schema.metadataIngestion.workflow import (
     Source as WorkflowSource,
 )
-from metadata.generated.schema.metadataIngestion.workflow import (
-    SourceConfig,
-    WorkflowConfig,
-)
-from metadata.generated.schema.type.basic import ComponentConfig
+from metadata.generated.schema.metadataIngestion.workflow import WorkflowConfig
 from metadata.ingestion.ometa.ometa_api import OpenMetadata
 
 
 def build_es_reindex_workflow_config(
     ingestion_pipeline: IngestionPipeline,
 ) -> OpenMetadataWorkflowConfig:
     """
@@ -63,24 +56,22 @@
         entity=MetadataService, fqn=ingestion_pipeline.service.fullyQualifiedName
     )
     if not openmetadata_service:
         raise ValueError(
             "Could not retrieve the OpenMetadata service! This should not happen."
         )
 
-    sink = build_elasticsearch_sink(
-        openmetadata_service.connection.config, ingestion_pipeline
-    )
+    sink = Sink(type="metadata-rest", config={})
 
     workflow_config = OpenMetadataWorkflowConfig(
         source=WorkflowSource(
             type="metadata_elasticsearch",
             serviceName=ingestion_pipeline.service.fullyQualifiedName,
             serviceConnection=MetadataConnection(config=MetadataESConnection()),
-            sourceConfig=SourceConfig(),
+            sourceConfig=ingestion_pipeline.sourceConfig,
         ),
         sink=sink,
         workflowConfig=WorkflowConfig(
             loggerLevel=ingestion_pipeline.loggerLevel or LogLevels.INFO,
             openMetadataServerConfig=ingestion_pipeline.openMetadataServerConnection,
         ),
         ingestionPipelineFQN=ingestion_pipeline.fullyQualifiedName.__root__,
```

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/lineage.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/lineage.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/metadata.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/metadata.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/profiler.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/profiler.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/registry.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/registry.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/test_suite.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/test_suite.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/ingestion/usage.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/ingestion/usage.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/workflow_builder.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/workflow_builder.py`

 * *Files identical despite different names*

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis/workflows/workflow_factory.py` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis/workflows/workflow_factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,17 +19,14 @@
 from typing import Any, Dict
 
 from airflow.models import DAG
 
 # these are params that cannot be a dag name
 from openmetadata_managed_apis.utils.logger import workflow_logger
 from openmetadata_managed_apis.workflows.config import load_config_file
-from openmetadata_managed_apis.workflows.ingestion.credentials_builder import (
-    build_secrets_manager_credentials,
-)
 from openmetadata_managed_apis.workflows.workflow_builder import WorkflowBuilder
 
 from metadata.generated.schema.entity.services.ingestionPipelines.ingestionPipeline import (
     IngestionPipeline,
 )
 from metadata.utils.secrets.secrets_manager_factory import SecretsManagerFactory
 
@@ -50,17 +47,15 @@
 
     def __init__(self, airflow_pipeline: IngestionPipeline) -> None:
         self.dag = None
         self.airflow_pipeline = airflow_pipeline
         # we need to instantiate the secret manager in case secrets are passed
         SecretsManagerFactory(
             airflow_pipeline.openMetadataServerConnection.secretsManagerProvider,
-            build_secrets_manager_credentials(
-                airflow_pipeline.openMetadataServerConnection.secretsManagerProvider
-            ),
+            airflow_pipeline.openMetadataServerConnection.secretsManagerLoader,
         )
 
     @classmethod
     def create(cls, config: str):
         config_file = pathlib.Path(config)
         workflow_config_dict = load_config_file(config_file)
         airflow_pipeline = IngestionPipeline(**workflow_config_dict)
```

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis.egg-info/PKG-INFO` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmetadata-managed-apis
-Version: 1.0.5.0
+Version: 1.1.0.0.dev0
 Summary: Airflow REST APIs to create and manage DAGS
 Home-page: https://open-metadata.org/
 Author: OpenMetadata Committers
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.open-metadata.org/
 Project-URL: Source, https://github.com/open-metadata/OpenMetadata
 Requires-Python: >=3.7
```

### Comparing `openmetadata_managed_apis-1.0.5.0/openmetadata_managed_apis.egg-info/SOURCES.txt` & `openmetadata_managed_apis-1.1.0.0.dev0/openmetadata_managed_apis.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -18,23 +18,25 @@
 openmetadata_managed_apis/api/utils.py
 openmetadata_managed_apis/api/routes/__init__.py
 openmetadata_managed_apis/api/routes/delete.py
 openmetadata_managed_apis/api/routes/deploy.py
 openmetadata_managed_apis/api/routes/disable.py
 openmetadata_managed_apis/api/routes/enable.py
 openmetadata_managed_apis/api/routes/health.py
+openmetadata_managed_apis/api/routes/health_auth.py
 openmetadata_managed_apis/api/routes/ip.py
 openmetadata_managed_apis/api/routes/kill.py
 openmetadata_managed_apis/api/routes/last_dag_logs.py
 openmetadata_managed_apis/api/routes/run_automation.py
 openmetadata_managed_apis/api/routes/status.py
 openmetadata_managed_apis/api/routes/trigger.py
 openmetadata_managed_apis/operations/__init__.py
 openmetadata_managed_apis/operations/delete.py
 openmetadata_managed_apis/operations/deploy.py
+openmetadata_managed_apis/operations/health.py
 openmetadata_managed_apis/operations/kill_all.py
 openmetadata_managed_apis/operations/last_dag_logs.py
 openmetadata_managed_apis/operations/state.py
 openmetadata_managed_apis/operations/status.py
 openmetadata_managed_apis/operations/trigger.py
 openmetadata_managed_apis/resources/__init__.py
 openmetadata_managed_apis/resources/dag_runner.j2
@@ -46,15 +48,14 @@
 openmetadata_managed_apis/views/templates/rest_api/index.html
 openmetadata_managed_apis/workflows/__init__.py
 openmetadata_managed_apis/workflows/config.py
 openmetadata_managed_apis/workflows/workflow_builder.py
 openmetadata_managed_apis/workflows/workflow_factory.py
 openmetadata_managed_apis/workflows/ingestion/__init__.py
 openmetadata_managed_apis/workflows/ingestion/common.py
-openmetadata_managed_apis/workflows/ingestion/credentials_builder.py
 openmetadata_managed_apis/workflows/ingestion/data_insight.py
 openmetadata_managed_apis/workflows/ingestion/dbt.py
 openmetadata_managed_apis/workflows/ingestion/elasticsearch_sink.py
 openmetadata_managed_apis/workflows/ingestion/es_reindex.py
 openmetadata_managed_apis/workflows/ingestion/lineage.py
 openmetadata_managed_apis/workflows/ingestion/metadata.py
 openmetadata_managed_apis/workflows/ingestion/profiler.py
```

### Comparing `openmetadata_managed_apis-1.0.5.0/setup.py` & `openmetadata_managed_apis-1.1.0.0.dev0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 }
 
 setup(
     name=PLUGIN_NAME,
     packages=find_packages(include=[f"{PLUGIN_NAME}.*", PLUGIN_NAME]),
     include_package_data=True,
     package_data={PLUGIN_NAME: get_package_data()},
-    version="1.0.5.0",
+    version="1.1.0.0.dev0",
     url="https://open-metadata.org/",
     author="OpenMetadata Committers",
     license="Apache License 2.0",
     description="Airflow REST APIs to create and manage DAGS",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     entry_points={
```

