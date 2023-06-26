# Comparing `tmp/assemblyline-core-4.4.1.dev98.tar.gz` & `tmp/assemblyline-core-4.4.1.dev99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyline-core-4.4.1.dev98.tar", last modified: Mon May 29 16:04:22 2023, max compression
+gzip compressed data, was "assemblyline-core-4.4.1.dev99.tar", last modified: Mon May 29 22:47:49 2023, max compression
```

## Comparing `assemblyline-core-4.4.1.dev98.tar` & `assemblyline-core-4.4.1.dev99.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:22.119286 assemblyline-core-4.4.1.dev98/
--rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/LICENCE.md
--rw-r--r--   0 vsts      (1001) docker     (122)     1681 2023-05-29 16:04:22.119286 assemblyline-core-4.4.1.dev98/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      860 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:22.087286 assemblyline-core-4.4.1.dev98/assemblyline_core/
--rw-r--r--   0 vsts      (1001) docker     (122)       12 2023-05-29 16:04:20.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/VERSION
--rw-r--r--   0 vsts      (1001) docker     (122)       49 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:22.087286 assemblyline-core-4.4.1.dev98/assemblyline_core/alerter/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/alerter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15689 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/alerter/processing.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4871 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/alerter/run_alerter.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:22.091286 assemblyline-core-4.4.1.dev98/assemblyline_core/archiver/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/archiver/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8210 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/archiver/run_archiver.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:22.091286 assemblyline-core-4.4.1.dev98/assemblyline_core/dispatching/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/dispatching/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      122 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/dispatching/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16929 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/dispatching/client.py
--rw-r--r--   0 vsts      (1001) docker     (122)    83163 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/dispatching/dispatcher.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7289 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/dispatching/schedules.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2050 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/dispatching/timeout.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:22.091286 assemblyline-core-4.4.1.dev98/assemblyline_core/expiry/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/expiry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13558 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/expiry/run_expiry.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:22.095286 assemblyline-core-4.4.1.dev98/assemblyline_core/ingester/
--rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/ingester/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/ingester/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/ingester/constants.py
--rw-r--r--   0 vsts      (1001) docker     (122)    35958 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/ingester/ingester.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:22.095286 assemblyline-core-4.4.1.dev98/assemblyline_core/metrics/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/metrics/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    30681 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/metrics/es_metrics.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13019 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/metrics/heartbeat_formatter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7559 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/metrics/helper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17144 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/metrics/metrics_server.py
--rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/metrics/run_heartbeat_manager.py
--rw-r--r--   0 vsts      (1001) docker     (122)      250 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/metrics/run_metrics_aggregator.py
--rw-r--r--   0 vsts      (1001) docker     (122)      274 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/metrics/run_statistics_aggregator.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:22.095286 assemblyline-core-4.4.1.dev98/assemblyline_core/plumber/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/plumber/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6434 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/plumber/run_plumber.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:22.111286 assemblyline-core-4.4.1.dev98/assemblyline_core/replay/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/replay/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12345 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/replay/client.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:22.111286 assemblyline-core-4.4.1.dev98/assemblyline_core/replay/creator/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/replay/creator/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2168 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/replay/creator/run.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4743 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/replay/creator/run_worker.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:22.111286 assemblyline-core-4.4.1.dev98/assemblyline_core/replay/loader/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/replay/loader/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3533 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/replay/loader/run.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2999 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/replay/loader/run_worker.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2577 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/replay/replay.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2498 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/safelist_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:22.111286 assemblyline-core-4.4.1.dev98/assemblyline_core/scaler/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/scaler/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1858 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/scaler/collection.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:22.115286 assemblyline-core-4.4.1.dev98/assemblyline_core/scaler/controllers/
--rw-r--r--   0 vsts      (1001) docker     (122)       90 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/scaler/controllers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    24018 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/scaler/controllers/docker_ctl.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2174 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/scaler/controllers/interface.py
--rw-r--r--   0 vsts      (1001) docker     (122)    54253 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/scaler/controllers/kubernetes_ctl.py
--rw-r--r--   0 vsts      (1001) docker     (122)      160 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/scaler/run_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (122)    48567 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/scaler/scaler_server.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12219 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/server_base.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10353 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/submission_client.py
--rw-r--r--   0 vsts      (1001) docker     (122)    22003 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/tasking_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:22.115286 assemblyline-core-4.4.1.dev98/assemblyline_core/updater/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/updater/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9293 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/updater/helper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    32180 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/updater/run_updater.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:22.115286 assemblyline-core-4.4.1.dev98/assemblyline_core/vacuum/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/vacuum/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5628 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/vacuum/crawler.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2675 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/vacuum/department_map.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3478 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/vacuum/safelist.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3136 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/vacuum/stream_map.py
--rw-r--r--   0 vsts      (1001) docker     (122)    29284 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/vacuum/worker.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:22.115286 assemblyline-core-4.4.1.dev98/assemblyline_core/workflow/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9532 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/assemblyline_core/workflow/run_workflow.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:22.087286 assemblyline-core-4.4.1.dev98/assemblyline_core.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1681 2023-05-29 16:04:22.000000 assemblyline-core-4.4.1.dev98/assemblyline_core.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     2975 2023-05-29 16:04:22.000000 assemblyline-core-4.4.1.dev98/assemblyline_core.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-29 16:04:22.000000 assemblyline-core-4.4.1.dev98/assemblyline_core.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       66 2023-05-29 16:04:22.000000 assemblyline-core-4.4.1.dev98/assemblyline_core.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       18 2023-05-29 16:04:22.000000 assemblyline-core-4.4.1.dev98/assemblyline_core.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-05-29 16:04:22.119286 assemblyline-core-4.4.1.dev98/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     1870 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 16:04:22.119286 assemblyline-core-4.4.1.dev98/test/
--rw-r--r--   0 vsts      (1001) docker     (122)     5768 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/test/test_alerter.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15228 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/test/test_dispatcher.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2043 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/test/test_expiry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2506 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/test/test_plumber.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6995 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/test/test_replay.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2006 2023-05-29 16:04:01.000000 assemblyline-core-4.4.1.dev98/test/test_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5313 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/test/test_scheduler.py
--rw-r--r--   0 vsts      (1001) docker     (122)    38685 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/test/test_simulation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4419 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/test/test_vacuum.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6792 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/test/test_worker_ingest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4780 2023-05-29 16:04:02.000000 assemblyline-core-4.4.1.dev98/test/test_worker_submit.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:49.553627 assemblyline-core-4.4.1.dev99/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/LICENCE.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     1681 2023-05-29 22:47:49.553627 assemblyline-core-4.4.1.dev99/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      860 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:49.501627 assemblyline-core-4.4.1.dev99/assemblyline_core/
+-rw-r--r--   0 vsts      (1001) docker     (122)       12 2023-05-29 22:47:47.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/VERSION
+-rw-r--r--   0 vsts      (1001) docker     (122)       49 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:49.509627 assemblyline-core-4.4.1.dev99/assemblyline_core/alerter/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/alerter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15689 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/alerter/processing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4871 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/alerter/run_alerter.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:49.509627 assemblyline-core-4.4.1.dev99/assemblyline_core/archiver/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/archiver/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8210 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/archiver/run_archiver.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:49.513627 assemblyline-core-4.4.1.dev99/assemblyline_core/dispatching/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/dispatching/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      122 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/dispatching/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16929 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/dispatching/client.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    83178 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/dispatching/dispatcher.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7289 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/dispatching/schedules.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2050 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/dispatching/timeout.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:49.513627 assemblyline-core-4.4.1.dev99/assemblyline_core/expiry/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/expiry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13558 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/expiry/run_expiry.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:49.513627 assemblyline-core-4.4.1.dev99/assemblyline_core/ingester/
+-rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/ingester/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/ingester/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/ingester/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    35958 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/ingester/ingester.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:49.521627 assemblyline-core-4.4.1.dev99/assemblyline_core/metrics/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/metrics/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    30681 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/metrics/es_metrics.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13019 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/metrics/heartbeat_formatter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7559 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/metrics/helper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17144 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/metrics/metrics_server.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/metrics/run_heartbeat_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      250 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/metrics/run_metrics_aggregator.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      274 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/metrics/run_statistics_aggregator.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:49.521627 assemblyline-core-4.4.1.dev99/assemblyline_core/plumber/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/plumber/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6434 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/plumber/run_plumber.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:49.521627 assemblyline-core-4.4.1.dev99/assemblyline_core/replay/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/replay/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12345 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/replay/client.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:49.533627 assemblyline-core-4.4.1.dev99/assemblyline_core/replay/creator/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/replay/creator/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2168 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/replay/creator/run.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4743 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/replay/creator/run_worker.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:49.533627 assemblyline-core-4.4.1.dev99/assemblyline_core/replay/loader/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/replay/loader/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3533 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/replay/loader/run.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2999 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/replay/loader/run_worker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2577 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/replay/replay.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2498 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/safelist_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:49.533627 assemblyline-core-4.4.1.dev99/assemblyline_core/scaler/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/scaler/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1858 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/scaler/collection.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:49.533627 assemblyline-core-4.4.1.dev99/assemblyline_core/scaler/controllers/
+-rw-r--r--   0 vsts      (1001) docker     (122)       90 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/scaler/controllers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    24018 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/scaler/controllers/docker_ctl.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2174 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/scaler/controllers/interface.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    54253 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/scaler/controllers/kubernetes_ctl.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      160 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/scaler/run_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    48567 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/scaler/scaler_server.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12219 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/server_base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10353 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/submission_client.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    22003 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/tasking_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:49.533627 assemblyline-core-4.4.1.dev99/assemblyline_core/updater/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/updater/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9293 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/updater/helper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    32180 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/updater/run_updater.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:49.537627 assemblyline-core-4.4.1.dev99/assemblyline_core/vacuum/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/vacuum/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5628 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/vacuum/crawler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2675 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/vacuum/department_map.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3478 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/vacuum/safelist.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3136 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/vacuum/stream_map.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    29284 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/vacuum/worker.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:49.553627 assemblyline-core-4.4.1.dev99/assemblyline_core/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9532 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/assemblyline_core/workflow/run_workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:49.501627 assemblyline-core-4.4.1.dev99/assemblyline_core.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1681 2023-05-29 22:47:49.000000 assemblyline-core-4.4.1.dev99/assemblyline_core.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     2975 2023-05-29 22:47:49.000000 assemblyline-core-4.4.1.dev99/assemblyline_core.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-29 22:47:49.000000 assemblyline-core-4.4.1.dev99/assemblyline_core.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       66 2023-05-29 22:47:49.000000 assemblyline-core-4.4.1.dev99/assemblyline_core.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       18 2023-05-29 22:47:49.000000 assemblyline-core-4.4.1.dev99/assemblyline_core.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-05-29 22:47:49.553627 assemblyline-core-4.4.1.dev99/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     1870 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-29 22:47:49.553627 assemblyline-core-4.4.1.dev99/test/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5768 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/test/test_alerter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15228 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/test/test_dispatcher.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2043 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/test/test_expiry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2506 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/test/test_plumber.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6995 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/test/test_replay.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2006 2023-05-29 22:47:36.000000 assemblyline-core-4.4.1.dev99/test/test_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5313 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/test/test_scheduler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    38685 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/test/test_simulation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4419 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/test/test_vacuum.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6792 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/test/test_worker_ingest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4780 2023-05-29 22:47:37.000000 assemblyline-core-4.4.1.dev99/test/test_worker_submit.py
```

### Comparing `assemblyline-core-4.4.1.dev98/LICENCE.md` & `assemblyline-core-4.4.1.dev99/LICENCE.md`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/PKG-INFO` & `assemblyline-core-4.4.1.dev99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline-core
-Version: 4.4.1.dev98
+Version: 4.4.1.dev99
 Summary: Assemblyline 4 - Core components
 Home-page: https://github.com/CybercentreCanada/assemblyline-core/
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Platform: UNKNOWN
```

### Comparing `assemblyline-core-4.4.1.dev98/README.md` & `assemblyline-core-4.4.1.dev99/README.md`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/alerter/processing.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/alerter/processing.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/alerter/run_alerter.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/alerter/run_alerter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/archiver/run_archiver.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/archiver/run_archiver.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/dispatching/client.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/dispatching/client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/dispatching/dispatcher.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/dispatching/dispatcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import dataclasses
 
 import elasticapm
 
 from assemblyline.common import isotime
 from assemblyline.common.constants import make_watcher_list_name, SUBMISSION_QUEUE, \
     DISPATCH_RUNNING_TASK_HASH, SCALER_TIMEOUT_QUEUE, DISPATCH_TASK_HASH
-from assemblyline.common.forge import get_service_queue, get_apm_client, get_datastore, get_classification
+from assemblyline.common.forge import get_service_queue, get_apm_client, get_classification
 from assemblyline.common.isotime import now_as_iso
 from assemblyline.common.metrics import MetricsFactory
 from assemblyline.common.postprocess import ActionWorker
 from assemblyline.odm.messages.changes import ServiceChange, Operation
 from assemblyline.odm.messages.dispatcher_heartbeat import Metrics
 from assemblyline.odm.messages.service_heartbeat import Metrics as ServiceMetrics
 from assemblyline.odm.messages.dispatching import WatchQueueMessage, CreateWatch, DispatcherCommandMessage, \
@@ -103,18 +103,18 @@
         self.score: int = score
         self.children: list[str, str] = children
 
 
 class SubmissionTask:
     """Dispatcher internal model for submissions"""
 
-    def __init__(self, submission, completed_queue, scheduler, results=None,
+    def __init__(self, submission, completed_queue, scheduler, datastore, results=None,
                  file_infos=None, file_tree=None, errors: Optional[Iterable[str]] = None):
         self.submission: Submission = Submission(submission)
-        self.submitter: User = get_datastore().user.get(self.submission.params.submitter)
+        self.submitter: User = datastore.user.get(self.submission.params.submitter)
 
         self.completed_queue = None
         if completed_queue:
             self.completed_queue = str(completed_queue)
 
         self.file_info: dict[str, Optional[FileInfo]] = {}
         self.file_names: dict[str, str] = {}
@@ -351,15 +351,14 @@
         self.redis_bad_sids = Set(BAD_SID_HASH, host=self.redis_persist)
         self.bad_sids: set[str] = set(self.redis_bad_sids.members())
 
         # Event Watchers
         self.service_change_watcher = EventWatcher(self.redis, deserializer=ServiceChange.deserialize)
         self.service_change_watcher.register('changes.services.*', self._handle_service_change_event)
 
-
     def stop(self):
         super().stop()
         self.service_change_watcher.stop()
         self.postprocess_worker.stop()
 
     def interrupt_handler(self, signum, stack_frame):
         self.log.info("Instance caught signal. Beginning to drain work.")
@@ -491,15 +490,15 @@
 
                 if not message:
                     continue
 
                 # Start of process dispatcher transaction
                 with apm_span(self.apm_client, 'submission_message'):
                     # This is probably a complete task
-                    task = SubmissionTask(scheduler=self.scheduler, **message)
+                    task = SubmissionTask(scheduler=self.scheduler, datastore=self.datastore, **message)
 
                     # Check the sid table
                     if task.sid in self.bad_sids:
                         task.submission.to_be_deleted = True
 
                     if self.apm_client:
                         elasticapm.label(sid=task.submission.sid)
```

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/dispatching/schedules.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/dispatching/schedules.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/dispatching/timeout.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/dispatching/timeout.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/expiry/run_expiry.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/expiry/run_expiry.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/ingester/ingester.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/ingester/ingester.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/metrics/es_metrics.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/metrics/es_metrics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/metrics/heartbeat_formatter.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/metrics/heartbeat_formatter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/metrics/helper.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/metrics/helper.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/metrics/metrics_server.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/metrics/metrics_server.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/plumber/run_plumber.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/plumber/run_plumber.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/replay/client.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/replay/client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/replay/creator/run.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/replay/creator/run.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/replay/creator/run_worker.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/replay/creator/run_worker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/replay/loader/run.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/replay/loader/run.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/replay/loader/run_worker.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/replay/loader/run_worker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/replay/replay.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/replay/replay.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/safelist_client.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/safelist_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/scaler/collection.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/scaler/collection.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/scaler/controllers/docker_ctl.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/scaler/controllers/docker_ctl.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/scaler/controllers/interface.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/scaler/controllers/interface.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/scaler/controllers/kubernetes_ctl.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/scaler/controllers/kubernetes_ctl.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/scaler/scaler_server.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/scaler/scaler_server.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/server_base.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/server_base.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/submission_client.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/submission_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/tasking_client.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/tasking_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/updater/helper.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/updater/helper.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/updater/run_updater.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/updater/run_updater.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/vacuum/crawler.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/vacuum/crawler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/vacuum/department_map.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/vacuum/department_map.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/vacuum/safelist.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/vacuum/safelist.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/vacuum/stream_map.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/vacuum/stream_map.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/vacuum/worker.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/vacuum/worker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core/workflow/run_workflow.py` & `assemblyline-core-4.4.1.dev99/assemblyline_core/workflow/run_workflow.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core.egg-info/PKG-INFO` & `assemblyline-core-4.4.1.dev99/assemblyline_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline-core
-Version: 4.4.1.dev98
+Version: 4.4.1.dev99
 Summary: Assemblyline 4 - Core components
 Home-page: https://github.com/CybercentreCanada/assemblyline-core/
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Platform: UNKNOWN
```

### Comparing `assemblyline-core-4.4.1.dev98/assemblyline_core.egg-info/SOURCES.txt` & `assemblyline-core-4.4.1.dev99/assemblyline_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/setup.py` & `assemblyline-core-4.4.1.dev99/setup.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/test/test_alerter.py` & `assemblyline-core-4.4.1.dev99/test/test_alerter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/test/test_dispatcher.py` & `assemblyline-core-4.4.1.dev99/test/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/test/test_expiry.py` & `assemblyline-core-4.4.1.dev99/test/test_expiry.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/test/test_plumber.py` & `assemblyline-core-4.4.1.dev99/test/test_plumber.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/test/test_replay.py` & `assemblyline-core-4.4.1.dev99/test/test_replay.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/test/test_scaler.py` & `assemblyline-core-4.4.1.dev99/test/test_scaler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/test/test_scheduler.py` & `assemblyline-core-4.4.1.dev99/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/test/test_simulation.py` & `assemblyline-core-4.4.1.dev99/test/test_simulation.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/test/test_vacuum.py` & `assemblyline-core-4.4.1.dev99/test/test_vacuum.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/test/test_worker_ingest.py` & `assemblyline-core-4.4.1.dev99/test/test_worker_ingest.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev98/test/test_worker_submit.py` & `assemblyline-core-4.4.1.dev99/test/test_worker_submit.py`

 * *Files identical despite different names*

