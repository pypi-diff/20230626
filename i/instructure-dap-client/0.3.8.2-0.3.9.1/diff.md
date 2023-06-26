# Comparing `tmp/instructure-dap-client-0.3.8.2.tar.gz` & `tmp/instructure-dap-client-0.3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructure-dap-client-0.3.8.2.tar", last modified: Mon Jun  5 14:39:23 2023, max compression
+gzip compressed data, was "instructure-dap-client-0.3.9.1.tar", last modified: Mon Jun 26 11:35:04 2023, max compression
```

## Comparing `instructure-dap-client-0.3.8.2.tar` & `instructure-dap-client-0.3.9.1.tar`

### file list

```diff
@@ -1,66 +1,81 @@
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-05 14:39:23.738480 instructure-dap-client-0.3.8.2/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1079 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.8.2/LICENSE
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    19537 2023-06-05 14:39:23.738777 instructure-dap-client-0.3.8.2/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18685 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/README.md
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-05 14:39:23.710516 instructure-dap-client-0.3.8.2/dap/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      526 2023-06-05 14:38:28.000000 instructure-dap-client-0.3.8.2/dap/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4682 2023-06-02 09:11:37.000000 instructure-dap-client-0.3.8.2/dap/__main__.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-05 14:39:23.713461 instructure-dap-client-0.3.8.2/dap/actions/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8.2/dap/actions/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1064 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/actions/drop_db.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      572 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/actions/init_db.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      573 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/actions/sync_db.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    21555 2023-06-01 21:13:57.000000 instructure-dap-client-0.3.8.2/dap/api.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2997 2023-06-02 09:11:37.000000 instructure-dap-client-0.3.8.2/dap/arguments.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-05 14:39:23.722763 instructure-dap-client-0.3.8.2/dap/commands/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.8.2/dap/commands/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      491 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/commands/abstract_db_command.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2011 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8.2/dap/commands/base.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6751 2023-03-31 08:29:45.000000 instructure-dap-client-0.3.8.2/dap/commands/commands.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2842 2023-06-02 09:11:37.000000 instructure-dap-client-0.3.8.2/dap/commands/commonargs.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      502 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8.2/dap/commands/dbargs.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1119 2023-06-02 09:11:37.000000 instructure-dap-client-0.3.8.2/dap/commands/dropdb_command.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1370 2023-06-02 09:11:37.000000 instructure-dap-client-0.3.8.2/dap/commands/initdb_command.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1322 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8.2/dap/commands/queryargs.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1704 2023-06-02 09:11:37.000000 instructure-dap-client-0.3.8.2/dap/commands/syncdb_command.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      889 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.8.2/dap/commands/timestampargs.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5928 2023-04-07 11:43:57.000000 instructure-dap-client-0.3.8.2/dap/concurrency.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     8018 2023-06-05 14:37:38.000000 instructure-dap-client-0.3.8.2/dap/conversion_common.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      635 2023-06-01 13:11:03.000000 instructure-dap-client-0.3.8.2/dap/conversion_nonperf.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      701 2023-04-26 20:18:45.000000 instructure-dap-client-0.3.8.2/dap/conversion_perf.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3688 2023-06-01 21:13:57.000000 instructure-dap-client-0.3.8.2/dap/dap_error.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18466 2023-05-09 18:21:54.000000 instructure-dap-client-0.3.8.2/dap/dap_types.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-05 14:39:23.728778 instructure-dap-client-0.3.8.2/dap/database/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/database/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2318 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/database/base_processor.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2442 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/database/connection.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1121 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/database/database_errors.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3835 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/database/database_operations.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2751 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/database/init_processor.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3671 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/database/sync_processor.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5861 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/downloader.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      684 2023-05-09 18:21:54.000000 instructure-dap-client-0.3.8.2/dap/log.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-05 14:39:23.731267 instructure-dap-client-0.3.8.2/dap/model/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.8.2/dap/model/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      987 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/model/ddl.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    16280 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/model/meta_table.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7091 2023-05-09 18:21:54.000000 instructure-dap-client-0.3.8.2/dap/model/metadata.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      932 2023-04-27 21:19:13.000000 instructure-dap-client-0.3.8.2/dap/networking.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1353 2023-04-05 14:04:38.000000 instructure-dap-client-0.3.8.2/dap/payload.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-04-25 19:15:30.000000 instructure-dap-client-0.3.8.2/dap/py.typed
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-05 14:39:23.732664 instructure-dap-client-0.3.8.2/dap/replicator/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 14:59:52.000000 instructure-dap-client-0.3.8.2/dap/replicator/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2571 2023-05-31 11:35:50.000000 instructure-dap-client-0.3.8.2/dap/replicator/sql.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1355 2023-04-27 21:19:13.000000 instructure-dap-client-0.3.8.2/dap/timer.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2264 2023-06-05 14:37:38.000000 instructure-dap-client-0.3.8.2/dap/timestamp.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-05 14:39:23.737695 instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    19537 2023-06-05 14:39:23.000000 instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1408 2023-06-05 14:39:23.000000 instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/SOURCES.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-06-05 14:39:23.000000 instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/dependency_links.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       51 2023-06-05 14:39:23.000000 instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/entry_points.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      153 2023-06-05 14:39:23.000000 instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/requires.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        4 2023-06-05 14:39:23.000000 instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/top_level.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-06-05 14:39:23.000000 instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/zip-safe
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2023-04-25 19:13:58.000000 instructure-dap-client-0.3.8.2/pyproject.toml
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1254 2023-06-05 14:39:23.739981 instructure-dap-client-0.3.8.2/setup.cfg
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       69 2022-07-21 14:42:23.000000 instructure-dap-client-0.3.8.2/setup.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-26 11:35:04.896825 instructure-dap-client-0.3.9.1/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1079 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.9.1/LICENSE
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    19807 2023-06-26 11:35:04.897227 instructure-dap-client-0.3.9.1/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18974 2023-06-21 15:09:03.000000 instructure-dap-client-0.3.9.1/README.md
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-26 11:35:04.843701 instructure-dap-client-0.3.9.1/dap/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      495 2023-06-26 11:33:13.000000 instructure-dap-client-0.3.9.1/dap/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4722 2023-06-14 16:27:38.000000 instructure-dap-client-0.3.9.1/dap/__main__.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-26 11:35:04.848987 instructure-dap-client-0.3.9.1/dap/actions/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 13:59:23.000000 instructure-dap-client-0.3.9.1/dap/actions/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      320 2023-06-20 17:25:31.000000 instructure-dap-client-0.3.9.1/dap/actions/drop_db.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      573 2023-06-16 08:05:53.000000 instructure-dap-client-0.3.9.1/dap/actions/init_db.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      574 2023-06-16 08:05:56.000000 instructure-dap-client-0.3.9.1/dap/actions/sync_db.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    21629 2023-06-21 15:09:03.000000 instructure-dap-client-0.3.9.1/dap/api.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2997 2023-06-16 08:08:08.000000 instructure-dap-client-0.3.9.1/dap/arguments.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-26 11:35:04.861101 instructure-dap-client-0.3.9.1/dap/commands/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-02-24 11:13:34.000000 instructure-dap-client-0.3.9.1/dap/commands/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      492 2023-06-16 08:06:04.000000 instructure-dap-client-0.3.9.1/dap/commands/abstract_db_command.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2011 2023-06-16 08:06:07.000000 instructure-dap-client-0.3.9.1/dap/commands/base.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6751 2023-06-16 08:06:11.000000 instructure-dap-client-0.3.9.1/dap/commands/commands.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2842 2023-06-16 08:06:17.000000 instructure-dap-client-0.3.9.1/dap/commands/commonargs.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      502 2023-06-16 08:06:21.000000 instructure-dap-client-0.3.9.1/dap/commands/dbargs.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1119 2023-06-16 08:06:25.000000 instructure-dap-client-0.3.9.1/dap/commands/dropdb_command.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1370 2023-06-16 08:06:28.000000 instructure-dap-client-0.3.9.1/dap/commands/initdb_command.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1322 2023-06-16 08:06:40.000000 instructure-dap-client-0.3.9.1/dap/commands/queryargs.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1704 2023-06-16 08:06:43.000000 instructure-dap-client-0.3.9.1/dap/commands/syncdb_command.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      889 2023-06-16 08:06:47.000000 instructure-dap-client-0.3.9.1/dap/commands/timestampargs.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5928 2023-06-16 08:08:11.000000 instructure-dap-client-0.3.9.1/dap/concurrency.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     8609 2023-06-21 15:09:03.000000 instructure-dap-client-0.3.9.1/dap/conversion_common.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      645 2023-06-14 16:27:38.000000 instructure-dap-client-0.3.9.1/dap/conversion_nonperf.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      719 2023-06-16 08:08:32.000000 instructure-dap-client-0.3.9.1/dap/conversion_perf.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1553 2023-06-16 08:08:34.000000 instructure-dap-client-0.3.9.1/dap/counted.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3674 2023-06-16 08:08:37.000000 instructure-dap-client-0.3.9.1/dap/dap_error.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18530 2023-06-16 08:08:45.000000 instructure-dap-client-0.3.9.1/dap/dap_types.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     6041 2023-06-20 17:25:31.000000 instructure-dap-client-0.3.9.1/dap/downloader.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-26 11:35:04.870431 instructure-dap-client-0.3.9.1/dap/integration/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-06-14 16:27:38.000000 instructure-dap-client-0.3.9.1/dap/integration/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2186 2023-06-21 15:09:03.000000 instructure-dap-client-0.3.9.1/dap/integration/base_connection.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5889 2023-06-20 17:25:31.000000 instructure-dap-client-0.3.9.1/dap/integration/base_meta_table.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1879 2023-06-20 17:25:31.000000 instructure-dap-client-0.3.9.1/dap/integration/connection.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1834 2023-06-21 15:09:03.000000 instructure-dap-client-0.3.9.1/dap/integration/database.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1115 2023-06-21 15:09:03.000000 instructure-dap-client-0.3.9.1/dap/integration/database_errors.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3320 2023-06-20 17:25:31.000000 instructure-dap-client-0.3.9.1/dap/integration/meta_table.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3160 2023-06-21 15:09:03.000000 instructure-dap-client-0.3.9.1/dap/integration/plugin.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1717 2023-06-21 15:09:03.000000 instructure-dap-client-0.3.9.1/dap/integration/processor.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      445 2023-06-21 15:09:03.000000 instructure-dap-client-0.3.9.1/dap/integration/validator.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      684 2023-06-16 08:08:48.000000 instructure-dap-client-0.3.9.1/dap/log.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2120 2023-06-21 15:09:03.000000 instructure-dap-client-0.3.9.1/dap/networking.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1358 2023-06-16 08:08:55.000000 instructure-dap-client-0.3.9.1/dap/payload.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-26 11:35:04.871310 instructure-dap-client-0.3.9.1/dap/plugins/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      196 2023-06-20 17:25:31.000000 instructure-dap-client-0.3.9.1/dap/plugins/__init__.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-26 11:35:04.882092 instructure-dap-client-0.3.9.1/dap/plugins/postgres/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-06-14 16:27:38.000000 instructure-dap-client-0.3.9.1/dap/plugins/postgres/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      774 2023-06-20 17:25:31.000000 instructure-dap-client-0.3.9.1/dap/plugins/postgres/ddl.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2746 2023-06-21 15:09:03.000000 instructure-dap-client-0.3.9.1/dap/plugins/postgres/init_processor.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    19521 2023-06-21 15:09:03.000000 instructure-dap-client-0.3.9.1/dap/plugins/postgres/meta_table.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     9826 2023-06-21 15:09:03.000000 instructure-dap-client-0.3.9.1/dap/plugins/postgres/metadata.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2768 2023-06-21 15:09:03.000000 instructure-dap-client-0.3.9.1/dap/plugins/postgres/plugin.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      837 2023-06-20 17:25:31.000000 instructure-dap-client-0.3.9.1/dap/plugins/postgres/queries.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4346 2023-06-21 15:09:03.000000 instructure-dap-client-0.3.9.1/dap/plugins/postgres/sync_processor.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1884 2023-06-21 15:09:03.000000 instructure-dap-client-0.3.9.1/dap/plugins/postgres/validator.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-26 11:35:04.885462 instructure-dap-client-0.3.9.1/dap/plugins/sqlalchemy/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-06-26 11:32:47.000000 instructure-dap-client-0.3.9.1/dap/plugins/sqlalchemy/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1524 2023-06-20 17:25:31.000000 instructure-dap-client-0.3.9.1/dap/plugins/sqlalchemy/connection.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1542 2023-06-20 17:25:31.000000 instructure-dap-client-0.3.9.1/dap/plugins/sqlalchemy/queries.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-04-25 19:15:30.000000 instructure-dap-client-0.3.9.1/dap/py.typed
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-26 11:35:04.888014 instructure-dap-client-0.3.9.1/dap/replicator/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-03-30 14:59:52.000000 instructure-dap-client-0.3.9.1/dap/replicator/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4563 2023-06-21 15:09:03.000000 instructure-dap-client-0.3.9.1/dap/replicator/sql.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1355 2023-06-16 08:09:00.000000 instructure-dap-client-0.3.9.1/dap/timer.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2310 2023-06-20 17:25:31.000000 instructure-dap-client-0.3.9.1/dap/timestamp.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-06-26 11:35:04.896061 instructure-dap-client-0.3.9.1/instructure_dap_client.egg-info/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    19807 2023-06-26 11:35:04.000000 instructure-dap-client-0.3.9.1/instructure_dap_client.egg-info/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1864 2023-06-26 11:35:04.000000 instructure-dap-client-0.3.9.1/instructure_dap_client.egg-info/SOURCES.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-06-26 11:35:04.000000 instructure-dap-client-0.3.9.1/instructure_dap_client.egg-info/dependency_links.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       51 2023-06-26 11:35:04.000000 instructure-dap-client-0.3.9.1/instructure_dap_client.egg-info/entry_points.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      152 2023-06-26 11:35:04.000000 instructure-dap-client-0.3.9.1/instructure_dap_client.egg-info/requires.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        4 2023-06-26 11:35:04.000000 instructure-dap-client-0.3.9.1/instructure_dap_client.egg-info/top_level.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-06-26 11:35:04.000000 instructure-dap-client-0.3.9.1/instructure_dap_client.egg-info/zip-safe
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       94 2023-04-25 19:13:58.000000 instructure-dap-client-0.3.9.1/pyproject.toml
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1221 2023-06-26 11:35:04.899042 instructure-dap-client-0.3.9.1/setup.cfg
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       69 2023-06-16 08:09:09.000000 instructure-dap-client-0.3.9.1/setup.py
```

### Comparing `instructure-dap-client-0.3.8.2/LICENSE` & `instructure-dap-client-0.3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8.2/PKG-INFO` & `instructure-dap-client-0.3.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: instructure-dap-client
-Version: 0.3.8.2
+Version: 0.3.9.1
 Summary: Data Access Platform client library
-Author: Levente Hunyadi
-Author-email: levente.hunyadi@instructure.com
 Maintainer: Edina Tipter
 Maintainer-email: edina.tipter@instructure.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -307,15 +306,15 @@
 1. initialize a database, and
 2. synchronize a database with the data in DAP.
 
 In order to replicate data in DAP locally, we must first initialize a database:
 
 ```python
 from dap.api import DAPClient
-from dap.database.connection import DatabaseConnection
+from dap.integration.database import DatabaseConnection
 from dap.replicator.sql import SQLReplicator
 
 connection_string: str = "postgresql://scott:password@localhost/testdb"
 async with DatabaseConnection(connection_string).open() as db_connection:
     async with DAPClient() as session:
         await SQLReplicator(session, db_connection).initialize(namespace, table_name)
 ```
@@ -341,7 +340,16 @@
 * A new enumeration value is added to an existing enumeration type.
 * A new enumeration type is introduced.
 * A field (column) is removed from a table.
 
 Behind the scenes, the client library uses SQL commands such as `ALTER TABLE ... ADD COLUMN ...` or `ALTER TYPE ... ADD VALUE ...` to replicate schema changes in DAP in our local database. If the JSON schema change couldn't be mapped to a series of these SQL statements, the client library wouldn't be able to synchronize with DAP using incremental queries, and would have to issue an expensive snapshot query.
 
 Once the local database table structure has been reconciled with the new schema in DAP, and the meta-table has been updated, data synchronization proceeds normally with insert, update and delete SQL statements.
+
+### Dropping data from a local database
+
+If the table is no longer needed, it can be dropped from the database using the following code:
+
+```python
+async with DatabaseConnection(connection_string).open() as db_connection:
+    await SQLDrop(db_connection).drop(namespace, table_name)
+```
```

### Comparing `instructure-dap-client-0.3.8.2/README.md` & `instructure-dap-client-0.3.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,15 @@
 1. initialize a database, and
 2. synchronize a database with the data in DAP.
 
 In order to replicate data in DAP locally, we must first initialize a database:
 
 ```python
 from dap.api import DAPClient
-from dap.database.connection import DatabaseConnection
+from dap.integration.database import DatabaseConnection
 from dap.replicator.sql import SQLReplicator
 
 connection_string: str = "postgresql://scott:password@localhost/testdb"
 async with DatabaseConnection(connection_string).open() as db_connection:
     async with DAPClient() as session:
         await SQLReplicator(session, db_connection).initialize(namespace, table_name)
 ```
@@ -317,7 +317,16 @@
 * A new enumeration value is added to an existing enumeration type.
 * A new enumeration type is introduced.
 * A field (column) is removed from a table.
 
 Behind the scenes, the client library uses SQL commands such as `ALTER TABLE ... ADD COLUMN ...` or `ALTER TYPE ... ADD VALUE ...` to replicate schema changes in DAP in our local database. If the JSON schema change couldn't be mapped to a series of these SQL statements, the client library wouldn't be able to synchronize with DAP using incremental queries, and would have to issue an expensive snapshot query.
 
 Once the local database table structure has been reconciled with the new schema in DAP, and the meta-table has been updated, data synchronization proceeds normally with insert, update and delete SQL statements.
+
+### Dropping data from a local database
+
+If the table is no longer needed, it can be dropped from the database using the following code:
+
+```python
+async with DatabaseConnection(connection_string).open() as db_connection:
+    await SQLDrop(db_connection).drop(namespace, table_name)
+```
```

### Comparing `instructure-dap-client-0.3.8.2/dap/__main__.py` & `instructure-dap-client-0.3.9.1/dap/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import asyncio
 import errno
 import logging
 import sys
 
+import dap.plugins
+
 from .arguments import Arguments
 from .commands.commands import (
     DapCommandRegistrar,
     IncrementalCommandRegistrar,
     ListCommandRegistrar,
     SchemaCommandRegistrar,
     SnapshotCommandRegistrar,
@@ -27,14 +29,16 @@
     TableArgumentRegistrar,
 )
 from .commands.syncdb_command import SyncDBCommandRegistrar
 from .commands.timestampargs import SinceArgumentRegistrar, UntilArgumentRegistrar
 from .dap_error import OperationError
 from .log import LevelFormatter
 
+dap.plugins.load()
+
 dapCommand = DapCommandRegistrar(
     arguments=[
         BaseUrlArgumentRegistrar(),
         OAuthCredentialsArgumentRegistrar(),
         LogLevelArgumentRegistrar(),
         HelpArgumentRegistrar(),
     ],
```

### Comparing `instructure-dap-client-0.3.8.2/dap/actions/init_db.py` & `instructure-dap-client-0.3.9.1/dap/actions/init_db.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ..api import DAPClient
 from ..dap_types import Credentials
-from ..database.connection import DatabaseConnection
+from ..integration.database import DatabaseConnection
 from ..replicator.sql import SQLReplicator
 
 
 async def init_db(
     base_url: str,
     credentials: Credentials,
     connection_string: str,
```

### Comparing `instructure-dap-client-0.3.8.2/dap/actions/sync_db.py` & `instructure-dap-client-0.3.9.1/dap/actions/sync_db.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ..api import DAPClient
 from ..dap_types import Credentials
-from ..database.connection import DatabaseConnection
+from ..integration.database import DatabaseConnection
 from ..replicator.sql import SQLReplicator
 
 
 async def sync_db(
     base_url: str,
     credentials: Credentials,
     connection_string: str,
```

### Comparing `instructure-dap-client-0.3.8.2/dap/api.py` & `instructure-dap-client-0.3.9.1/dap/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     Resource,
     ResourceResult,
     SnapshotQuery,
     TableList,
     TokenProperties,
     VersionedSchema,
 )
-from .networking import get_content_type
+from .networking import get_content_type, KeepAliveClientRequest
 
 logger = logging.getLogger("dap")
 
 T = TypeVar("T")
 
 
 class DAPClientError(RuntimeError):
@@ -97,14 +97,15 @@
 
         logger.debug(f"Client region: {self._credentials.client_region}")
 
     async def __aenter__(self) -> "DAPSession":
         session = aiohttp.ClientSession(
             headers={"User-Agent": f"DataAccessPlatform/{__version__}"},
             timeout=aiohttp.ClientTimeout(total=30 * 60, connect=30),
+            request_class=KeepAliveClientRequest,
         )
         self._session = DAPSession(session, self._base_url, self._credentials)
         return self._session
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
```

### Comparing `instructure-dap-client-0.3.8.2/dap/arguments.py` & `instructure-dap-client-0.3.9.1/dap/arguments.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8.2/dap/commands/base.py` & `instructure-dap-client-0.3.9.1/dap/commands/base.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8.2/dap/commands/commands.py` & `instructure-dap-client-0.3.9.1/dap/commands/commands.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8.2/dap/commands/commonargs.py` & `instructure-dap-client-0.3.9.1/dap/commands/commonargs.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8.2/dap/commands/dropdb_command.py` & `instructure-dap-client-0.3.9.1/dap/commands/dropdb_command.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8.2/dap/commands/initdb_command.py` & `instructure-dap-client-0.3.9.1/dap/commands/initdb_command.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8.2/dap/commands/queryargs.py` & `instructure-dap-client-0.3.9.1/dap/commands/queryargs.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8.2/dap/commands/syncdb_command.py` & `instructure-dap-client-0.3.9.1/dap/commands/syncdb_command.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8.2/dap/commands/timestampargs.py` & `instructure-dap-client-0.3.9.1/dap/commands/timestampargs.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8.2/dap/concurrency.py` & `instructure-dap-client-0.3.9.1/dap/concurrency.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8.2/dap/conversion_common.py` & `instructure-dap-client-0.3.9.1/dap/conversion_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 import logging
 import typing
+from ipaddress import ip_address
 from datetime import datetime
-from typing import Any, Callable, Dict, Optional, Type, TypeVar
+from uuid import UUID
+from typing import Any, Callable, Dict, Optional, Type, TypeVar, Union
 
 import orjson
 from sqlalchemy import ARRAY, JSON, TIMESTAMP, BigInteger, Boolean, Column, Double
 from sqlalchemy import Enum as SqlEnum
-from sqlalchemy import Float, Integer, SmallInteger, String
+from sqlalchemy import Float, Integer, SmallInteger, String, Uuid
+from sqlalchemy.dialects.postgresql import INET
 from sqlalchemy.sql.type_api import TypeEngine
 from strong_typing.core import JsonType
 
 from .timestamp import clamp_naive_datetime, valid_naive_datetime
 
 T = TypeVar("T")
 
 logger = logging.getLogger("dap")
 
 JsonRecord = Dict[str, Dict[str, JsonType]]
 DateTimeConverter = Callable[[str], datetime]
 JsonTypeCast = Callable[[JsonType], Any]
 RecordExtractor = Callable[[JsonRecord], Any]
+RecordExtractorDict = Dict[str, RecordExtractor]
+ValueConverter = Callable[[JsonType], Any]
+ValueConverterDict = Dict[str, ValueConverter]
 
 
 def _handle_exceptional_datetime(record_json: JsonRecord, column_name: str) -> datetime:
     key = record_json["key"]
     value = typing.cast(str, record_json["value"][column_name])
     clamped_value = clamp_naive_datetime(value)
     logger.warning(
@@ -186,29 +192,35 @@
     elif column_type is JSON:
         # original JSON type: `object` (nested)
         # deserialized Python type: `dict` (nested)
         # database type: `jsonb`
         # converted back to `str` to pass to database as `jsonb`
         type_cast = _json_dump
     elif column_type is TIMESTAMP:
-        # original JSON type: `str` (format: ISO-8601 string)
+        # original JSON type: `str` (format: ISO-8601 and RFC 3339 compliant string)
         # deserialized Python type: `str`
         # database type: `timestamp without time zone`
         # converted to naive `datetime` to pass to database
         type_cast = valid_naive_datetime  # type: ignore
     elif column_type is Boolean:
         # original JSON type: `boolean`
         # deserialized Python type: `bool`
         type_cast = None
+    elif column_type is INET:
+        # original JSON type: `string`
+        # deserialized Python type: `str`
+        # database type: inet
+        type_cast = ip_address # type: ignore[assignment]
+    elif column_type is Uuid:
+        # original JSON type: `string`
+        # deserialized Python type: `str`
+        # database type: uuid
+        type_cast = UUID # type: ignore[assignment]
     elif column_type is ARRAY:
         # original JSON type: `array` (nested)
         # deserialized Python type: `list` (nested)
         # convert elements recursively
         type_cast = None
     else:
         raise TypeError(f"cannot convert to {column_type}")
 
     return type_cast
-
-
-Converter = Callable[[JsonRecord], Any]
-ConverterDict = Dict[str, Converter]
```

### Comparing `instructure-dap-client-0.3.8.2/dap/conversion_nonperf.py` & `instructure-dap-client-0.3.9.1/dap/conversion_nonperf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Optional
 
 from sqlalchemy.sql.type_api import TypeEngine
 from strong_typing.core import JsonType
 
-from .conversion_common import Converter, JsonTypeCast, get_type_cast
+from .conversion_common import JsonTypeCast, ValueConverter, get_type_cast
 
 
-def create_value_converter(value_type: TypeEngine) -> Converter:
+def create_value_converter(value_type: TypeEngine) -> ValueConverter:
     type_cast: Optional[JsonTypeCast] = get_type_cast(type(value_type))
 
     if type_cast is None:
         return lambda value: value
     else:
         cast = type_cast  # hint to type checker
```

### Comparing `instructure-dap-client-0.3.8.2/dap/dap_error.py` & `instructure-dap-client-0.3.9.1/dap/dap_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import typing
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Literal, Optional
 
 from strong_typing.schema import json_schema_type
```

### Comparing `instructure-dap-client-0.3.8.2/dap/dap_types.py` & `instructure-dap-client-0.3.9.1/dap/dap_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from .dap_error import ProcessingError
 
 JobID = str
 ObjectID = str
 
 
-@json_schema_type(schema={"type": "string", "format": "uri", "pattern": "^https?://"})
+@json_schema_type(schema={"type": "string", "format": "uri", "pattern": "^https?://"})  # type: ignore
 @dataclass(frozen=True)
 class URL:
     "A Uniform Resource Locator (URL)."
 
     url: str
 
     @staticmethod
@@ -32,15 +32,15 @@
     def to_json(self) -> str:
         return self.url
 
     def __str__(self) -> str:
         return self.url
 
 
-@json_schema_type(
+@json_schema_type(  # type: ignore
     examples=[
         {
             "schema": {
                 "type": "object",
                 "properties": {
                     "id": {
                         "type": "integer",
@@ -215,15 +215,15 @@
     :param error: Provides more details on the error that occurred.
     """
 
     error: ProcessingError
 
 
 Job = Union[TableJob, CompleteSnapshotJob, CompleteIncrementalJob, FailedJob]
-register_schema(Job, name="Job")
+register_schema(Job, name="Job")  # type: ignore
 
 
 @dataclass(frozen=True)
 class TableList:
     "A list of tables that exist in the organization domain."
 
     tables: List[str]
@@ -420,15 +420,15 @@
             if not isinstance(self.until, datetime):
                 raise TypeError("timestamp `until` expects datetime type")
             if self.until.tzinfo is None:
                 raise ValueError("time zone designator required for timestamp `until`")
 
 
 Query = Union[SnapshotQuery, IncrementalQuery]
-register_schema(Query, name="Query")
+register_schema(Query, name="Query")  # type: ignore
 
 
 @dataclass(frozen=True)
 class ResourceResult:
     """
     Associates object identifiers with pre-signed URLs to output resources.
```

### Comparing `instructure-dap-client-0.3.8.2/dap/database/base_processor.py` & `instructure-dap-client-0.3.9.1/dap/integration/processor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import abc
 from dataclasses import dataclass
-from types import TracebackType
-from typing import Optional, Type
+from typing import AsyncIterator
 
 from ..conversion_common import JsonRecord
 from ..dap_types import JobID, ObjectID
 
 
 @dataclass(frozen=True)
 class ContextAwareObject:
@@ -16,69 +15,45 @@
     total_count: int
     job_id: JobID
 
     def __str__(self) -> str:
         return f"[object {self.index + 1}/{self.total_count} - job {self.job_id}]"
 
 
-class BaseBatch(abc.ABC):
-    "Base class for replicating data acquired from DAP API in a relational database."
-
-    @abc.abstractmethod
-    async def process(self, record: JsonRecord) -> None:
-        """
-        Processes a single record.
-
-        :param record: JSON object to process.
-        """
-        ...
-
-    @abc.abstractmethod
-    async def __aenter__(self) -> "BaseBatch":
-        ...
-
-    @abc.abstractmethod
-    async def __aexit__(
-        self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> None:
-        ...
-
-
-class BaseProcessor(abc.ABC):
+class AbstractProcessor(abc.ABC):
     @abc.abstractmethod
     async def prepare(self) -> None:
         """
         Prepares for processing of a stream of records.
 
         For initializing a database, this would issue SQL `CREATE TABLE` statements that records about to be received
         might be inserted into.
 
-        For synchronizing a database, this would check whether the table exists that is about to be synchronized.
         """
         ...
 
     @abc.abstractmethod
-    def batch(self, obj: ContextAwareObject) -> "BaseBatch":
+    async def process(
+        self, obj: ContextAwareObject, records: AsyncIterator[JsonRecord]
+    ) -> None:
         """
-        Starts processing a batch of records.
+        Starts processing a batch of records from the given object.
 
         :param obj: Object that the records belong to. This helps trace records back to their source.
+        :param records: The asynchronously iterable collection of records.
         """
         ...
 
     @abc.abstractmethod
     async def close(self) -> None:
         """
         Ends processing records. Invoked after all records have been processed.
         """
         ...
 
 
-class BaseInitProcessor(BaseProcessor):
+class AbstractInitProcessor(AbstractProcessor):
     "Base class for initializing a table in relational database with data acquired from DAP API."
 
 
-class BaseSyncProcessor(BaseProcessor):
+class AbstractSyncProcessor(AbstractProcessor):
     "Base class for synchronizing an existing table in a relational database with data from DAP API."
```

### Comparing `instructure-dap-client-0.3.8.2/dap/database/database_errors.py` & `instructure-dap-client-0.3.9.1/dap/integration/database_errors.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 class DatabaseError(Exception):
     """
     Generic exception class. Do not use it for raising any error, but use specific derived class.
     """
 
 
 class NonExistingTableError(DatabaseError):
-    def __init__(self, namespace: str, table_name: str) -> None:
-        super().__init__(f"table `{table_name}` does not exist in schema `{namespace}`")
+    def __init__(self, table_name: str, schema: str) -> None:
+        super().__init__(f"table `{table_name}` does not exist in schema `{schema}`")
 
 
 class TableAlreadyExistsError(DatabaseError):
     def __init__(self, table_name: str, schema: Optional[str]) -> None:
         super().__init__(f"table `{table_name}` already exists in schema `{schema}`")
```

### Comparing `instructure-dap-client-0.3.8.2/dap/downloader.py` & `instructure-dap-client-0.3.9.1/dap/downloader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import logging
-import typing
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Awaitable, Callable
+from typing import AsyncContextManager, Awaitable, Callable
 
 from .api import DAPSession, DownloadError
 from .concurrency import wait_n
 from .dap_types import (
     Format,
     GetTableDataResult,
     IncrementalQuery,
     Object,
     SnapshotQuery,
     VersionedSchema,
 )
-from .database.base_processor import (
-    BaseInitProcessor,
-    BaseSyncProcessor,
+from .integration.database_errors import SchemaVersionMismatchError
+from .integration.processor import (
+    AbstractInitProcessor,
+    AbstractSyncProcessor,
     ContextAwareObject,
-    JsonRecord,
 )
-from .database.database_errors import SchemaVersionMismatchError
 from .payload import get_json_lines_from_gzip_stream
 
 logger = logging.getLogger("dap")
 
 CONCURRENCY: int = 4
 
-SnapshotDownloader = Callable[[BaseInitProcessor], Awaitable[None]]
+DatabaseLock = Callable[[], AsyncContextManager]
+SnapshotDownloader = Callable[[DatabaseLock, AbstractInitProcessor], Awaitable[None]]
 
 
 @dataclass(frozen=True)
 class SnapshotClient:
     table_data: GetTableDataResult
     table_schema: VersionedSchema
     download: SnapshotDownloader
@@ -60,23 +59,25 @@
             raise SchemaVersionMismatchError(
                 table_schema.version, table_data.schema_version
             )
 
         object_count = len(table_data.objects)
         job_id = table_data.job_id
 
-        async def download(processor: BaseInitProcessor) -> None:
+        async def download(
+            db_lock: DatabaseLock, processor: AbstractInitProcessor
+        ) -> None:
             async def logged_download_and_save(obj: Object, object_index: int) -> None:
                 context_aware_object = ContextAwareObject(
                     id=obj.id,
                     index=object_index,
                     job_id=job_id,
                     total_count=object_count,
                 )
-                await self._download(context_aware_object, processor=processor)
+                await self._download(db_lock, context_aware_object, processor=processor)
 
             await wait_n(
                 [
                     logged_download_and_save(obj, obj_index)
                     for obj_index, obj in enumerate(table_data.objects)
                 ],
                 concurrency=CONCURRENCY,
@@ -86,31 +87,32 @@
 
         return SnapshotClient(
             table_schema=table_schema, table_data=table_data, download=download
         )
 
     async def _download(
         self,
+        db_lock: DatabaseLock,
         obj: ContextAwareObject,
-        processor: BaseInitProcessor,
+        processor: AbstractInitProcessor,
     ) -> None:
         resource_array = await self._session.get_resources([Object(id=obj.id)])
         if len(resource_array) != 1:
             raise DownloadError("unable to get resource URLs for objects")
 
         logger.info(f"Downloading {obj}")
 
         resource = resource_array[0]
         async with self._session.stream_resource(resource) as stream:
-            async with processor.batch(obj) as batch:
-                async for record in get_json_lines_from_gzip_stream(stream):
-                    await batch.process(typing.cast(JsonRecord, record))
+            records = get_json_lines_from_gzip_stream(stream)
+            async with db_lock():
+                await processor.process(obj, records)
 
 
-IncrementalDownloader = Callable[[BaseSyncProcessor], Awaitable[None]]
+IncrementalDownloader = Callable[[DatabaseLock, AbstractSyncProcessor], Awaitable[None]]
 
 
 @dataclass(frozen=True)
 class IncrementalClient:
     table_data: GetTableDataResult
     table_schema: VersionedSchema
     download: IncrementalDownloader
@@ -144,37 +146,42 @@
             raise SchemaVersionMismatchError(
                 table_schema.version, table_data.schema_version
             )
 
         job_id = table_data.job_id
         object_count = len(table_data.objects)
 
-        async def download(processor: BaseSyncProcessor) -> None:
+        async def download(
+            db_lock: DatabaseLock, processor: AbstractSyncProcessor
+        ) -> None:
             for object_index, obj in enumerate(table_data.objects):
                 context_aware_object = ContextAwareObject(
                     id=obj.id,
                     index=object_index,
                     job_id=job_id,
                     total_count=object_count,
                 )
-                await self._download_and_save(context_aware_object, processor)
+                await self._download_and_save(db_lock, context_aware_object, processor)
 
             await processor.close()
 
         return IncrementalClient(
             download=download, table_data=table_data, table_schema=table_schema
         )
 
     async def _download_and_save(
-        self, obj: ContextAwareObject, processor: BaseSyncProcessor
+        self,
+        db_lock: DatabaseLock,
+        obj: ContextAwareObject,
+        processor: AbstractSyncProcessor,
     ) -> None:
         "Reads JSON records from a stream and makes them upserted or deleted via the processor."
 
         resource_array = await self._session.get_resources([Object(id=obj.id)])
         if len(resource_array) != 1:
             raise DownloadError("unable to get resource URLs for objects")
 
         resource = resource_array[0]
         async with self._session.stream_resource(resource) as stream:
-            async with processor.batch(obj) as batch:
-                async for record in get_json_lines_from_gzip_stream(stream):
-                    await batch.process(typing.cast(JsonRecord, record))
+            records = get_json_lines_from_gzip_stream(stream)
+            async with db_lock():
+                await processor.process(obj, records)
```

### Comparing `instructure-dap-client-0.3.8.2/dap/log.py` & `instructure-dap-client-0.3.9.1/dap/log.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8.2/dap/model/ddl.py` & `instructure-dap-client-0.3.9.1/dap/plugins/postgres/ddl.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 from typing import Any, Optional
 
-from sqlalchemy import bindparam, column, table, text
-from sqlalchemy.ext.asyncio import AsyncConnection
+from sqlalchemy import bindparam, column, table
 
 logger = logging.getLogger("dap")
 
 
 def table_name(name: str, schema: Optional[str] = None) -> str:
     table_name_str = str(table(name=name, schema=schema))
     return table_name_str
@@ -23,12 +22,7 @@
 
 
 def value_literal(value: Any) -> str:
     value_str = (
         bindparam("value", value).compile(compile_kwargs={"literal_binds": True}).string
     )
     return value_str
-
-
-async def execute_ddl(conn: AsyncConnection, ddl_query: str) -> None:
-    logger.debug(f"DDL query: {ddl_query}")
-    await conn.execute(text(ddl_query))
```

### Comparing `instructure-dap-client-0.3.8.2/dap/model/metadata.py` & `instructure-dap-client-0.3.9.1/dap/plugins/postgres/metadata.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,105 @@
 import typing
 from typing import Any, Dict, List, Optional, Union
 
 import sqlalchemy
+import re
+from sqlalchemy.dialects.postgresql import INET
 from sqlalchemy.sql.type_api import TypeEngine
 from strong_typing.core import JsonType, Schema
 
-from ..api import DAPClientError
-from ..conversion_nonperf import create_value_converter
-from ..dap_types import VersionedSchema
+from ...api import DAPClientError
+from ...conversion_nonperf import create_value_converter
+from ...dap_types import VersionedSchema
 
 SqlAlchemyType = Union[
     sqlalchemy.BigInteger,
     sqlalchemy.Integer,
     sqlalchemy.SmallInteger,
     sqlalchemy.Float,
     sqlalchemy.Double,
     sqlalchemy.Enum,
     sqlalchemy.TIMESTAMP,
     sqlalchemy.String,
     sqlalchemy.JSON,
     sqlalchemy.Boolean,
     sqlalchemy.ARRAY,
+    sqlalchemy.Uuid,
+    INET,
 ]
 
 
+def get_nested(schema: Schema, keys: List[str]) -> Dict[str, JsonType]:
+    nested_value = typing.cast(Dict[str, JsonType], schema)
+    for key in keys:
+        nested_value = typing.cast(Dict[str, JsonType], nested_value[key])
+        
+    return nested_value
+
+
+def get_reference(schema: Schema, reference: str, table_name: str) -> Dict[str, JsonType]:
+    valid_ref = re.search(r"^#(/\w+)+", reference)
+    if not valid_ref:
+        raise ReferenceError(reference, table_name)
+    return get_nested(schema, reference.split('/')[1:])
+
+
+def resolve_ref(
+    schema: Schema, property_schema: Schema, table_name: str
+) -> Schema:
+    if "oneOf" in property_schema:
+        oneOfSchema = typing.cast(List[JsonType], property_schema["oneOf"])
+        for index, item in enumerate(oneOfSchema):
+            oneOfElement = typing.cast(Dict[str, JsonType], item)
+            if "$ref" in oneOfElement:
+                ref = typing.cast(str, oneOfElement["$ref"])
+                oneOfSchema[index] = get_reference(schema, ref, table_name)
+
+    if "$ref" in property_schema:
+        ref = typing.cast(str, property_schema["$ref"])
+        property_schema = get_reference(schema, ref, table_name)
+
+    return property_schema
+
+
 def match_type(
     schema: Schema, namespace: str, table_name: str, prop_name: str
 ) -> TypeEngine[Any]:
     detected_type: Optional[SqlAlchemyType] = None
 
     if "oneOf" in schema:
         oneOfSchema = typing.cast(List[JsonType], schema["oneOf"])
+        all_ip = True
         for item in oneOfSchema:
             oneOfElement = typing.cast(Dict[str, JsonType], item)
             if oneOfElement["type"] != "string":
                 raise OneOfTypeSchemaError(table_name)
-
+            if not "format" in oneOfElement:
+                all_ip = False
+            elif oneOfElement["format"] != "ipv4" and oneOfElement["format"] != "ipv6":
+                all_ip = False
+        if all_ip:
+            return INET()
         return sqlalchemy.String()
 
     if "type" not in schema:
         raise NoTypeSpecifiedError(table_name, prop_name)
 
     type_name = schema["type"]
 
     if type_name == "integer":
-        if schema["format"] == "int64":
+        if "enum" in schema:
+            enum_int_items = typing.cast(List[int], schema["enum"])
+            if min(enum_int_items) >= -2**15 and max(enum_int_items) <= 2**15-1:
+                detected_type = sqlalchemy.SmallInteger()
+            elif min(enum_int_items) >= -2**31 and max(enum_int_items) <= 2**31-1:
+                detected_type = sqlalchemy.Integer()
+            else:
+                detected_type = sqlalchemy.BigInteger()
+        elif schema["format"] == "int64":
             detected_type = sqlalchemy.BigInteger()
         elif schema["format"] == "int32":
             detected_type = sqlalchemy.Integer()
         elif schema["format"] == "int16":
             detected_type = sqlalchemy.SmallInteger()
 
     elif type_name == "number":
@@ -57,21 +108,28 @@
 
         elif schema["format"] == "float64":
             detected_type = sqlalchemy.Double()
 
     elif type_name == "string":
         if "enum" in schema:
             enum_name = f"{table_name}__{prop_name}"
+            enum_items = typing.cast(List[str], schema["enum"])
             detected_type = sqlalchemy.Enum(
-                *schema["enum"], name=enum_name, create_type=True, schema=namespace
+                *enum_items, name=enum_name, create_type=True, schema=namespace
             )
 
         elif "format" in schema and schema["format"] == "date-time":
             detected_type = sqlalchemy.TIMESTAMP(timezone=False)
 
+        elif "format" in schema and schema["format"] == "uuid":
+            detected_type = sqlalchemy.Uuid()
+
+        elif "format" in schema and (schema["format"] == "ipv4" or schema["format"] == "ipv6"):
+            detected_type = INET()
+
         elif "maxLength" in schema:
             max_length = typing.cast(int, schema["maxLength"])
             detected_type = sqlalchemy.String(length=max_length)
         else:
             detected_type = sqlalchemy.String()
 
     elif type_name == "object":
@@ -134,14 +192,21 @@
 class NoTypeSpecifiedError(DAPSchemaParsingError):
     def __init__(self, table_name: str, prop_name: str) -> None:
         super().__init__(
             f"Cannot recognize type without `type` field in {table_name}.{prop_name}"
         )
 
 
+class ReferenceError(DAPSchemaParsingError):
+    def __init__(self, reference: str, table_name: str) -> None:
+        super().__init__(
+            f"References must start by referencing the root (#), Found {reference} in {table_name}"
+        )
+
+
 class CompositeKeyError(DAPSchemaParsingError):
     "Raised when the table schema has a composite primary key that comprises of multiple fields/columns."
 
     def __init__(self, table_name: str) -> None:
         super().__init__(f"Composite keys are not supported. Found in {table_name}")
 
 
@@ -173,14 +238,15 @@
     value_schema = typing.cast(Dict[str, JsonType], schema["value"])
     value_schema_props = typing.cast(Dict[str, JsonType], value_schema["properties"])
     columns: List[sqlalchemy.Column] = []
 
     required_keys = typing.cast(List[str], key_schema.get("required", []))
     for id_prop_name in key_schema_props.keys():
         id_schema = typing.cast(Schema, key_schema_props[id_prop_name])
+        id_schema = resolve_ref(versioned_schema.schema, id_schema, table_name)
 
         column_type = match_type(id_schema, namespace, table_name, id_prop_name)
 
         columns.append(
             sqlalchemy.Column(
                 id_prop_name,
                 column_type,
@@ -189,14 +255,16 @@
                 comment=get_comment(id_schema),
             )
         )
 
     required_values = typing.cast(List[str], value_schema.get("required", []))
     for prop_name in value_schema_props.keys():
         prop_schema = typing.cast(Schema, value_schema_props[prop_name])
+        prop_schema = resolve_ref(versioned_schema.schema, prop_schema, table_name)
+
         column_type = match_type(prop_schema, namespace, table_name, prop_name)
 
         columns.append(
             sqlalchemy.Column(
                 prop_name,
                 column_type,
                 nullable=(prop_name not in required_values),
```

### Comparing `instructure-dap-client-0.3.8.2/dap/payload.py` & `instructure-dap-client-0.3.9.1/dap/payload.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import io
 import zlib
 from typing import AsyncIterator
 
 import aiohttp
 import orjson
-from strong_typing.core import JsonType
+
+from .conversion_common import JsonRecord
 
 
 async def get_json_lines_from_gzip_stream(
     stream: aiohttp.StreamReader,
-) -> AsyncIterator[JsonType]:
+) -> AsyncIterator[JsonRecord]:
     "Extracts JSON objects from a gzipped HTTP payload stream of content type JSONL."
 
     # use a special value for wbits (windowBits) to indicate gzip compression
     # see: https://docs.python.org/3/library/zlib.html#zlib.decompress
     decompressor = zlib.decompressobj(16 + zlib.MAX_WBITS)
 
     buf = io.BytesIO()
```

### Comparing `instructure-dap-client-0.3.8.2/dap/replicator/sql.py` & `instructure-dap-client-0.3.9.1/dap/plugins/postgres/plugin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,81 +1,73 @@
+from ...integration.validator import AbstractDatabaseValidator
 from typing import Optional
 
-from ..api import DAPSession
-from ..database.base_processor import BaseInitProcessor, BaseSyncProcessor
-from ..database.connection import DatabaseSession
-from ..database.init_processor import InitProcessor
-from ..database.sync_processor import SyncProcessor
-from ..downloader import IncrementalClientFactory, SnapshotClientFactory
-from ..model.meta_table import MetaTableManager
-
-
-class SQLReplicator:
-    """
-    Encapsulates logic that replicates changes acquired from DAP API in a SQL database.
-    """
-
-    def __init__(self, session: DAPSession, connection: DatabaseSession) -> None:
-        self._session = session
-        self._connection = connection
+from ...dap_types import VersionedSchema
+from ...integration.connection import AbstractDatabaseConnection
+from ...integration.database_errors import DatabaseConnectionError
+from ...integration.meta_table import AbstractMetaTableManager
+from ...integration.validator import AbstractDatabaseValidator
+from ...integration.processor import AbstractInitProcessor, AbstractSyncProcessor
+from .validator import DatabaseValidator
+from ...integration.plugin import DatabasePlugin
+from ...integration.processor import AbstractInitProcessor, AbstractSyncProcessor
+from ..sqlalchemy.connection import SqlAlchemyConnection
+from .init_processor import InitProcessor
+from .meta_table import MetaTableManager
+from .sync_processor import SyncProcessor
+
+
+class PostgresPlugin(DatabasePlugin):
+    
+    _connection: Optional[SqlAlchemyConnection]
+
+    def __init__(self) -> None:
+        self._connection = None
+
+    def connect(self, connection_string: str) -> None:
+        if self._connection is not None:
+            raise DatabaseConnectionError("already connected to the database")
 
-    async def initialize(
-        self,
-        namespace: str,
-        table_name: str,
-        processor: Optional[BaseInitProcessor] = None,
-    ) -> None:
-        """
-        Initializes database table. Processor
-        """
-        client = await SnapshotClientFactory(
-            self._session, namespace, table_name
-        ).get_client()
-
-        if processor is None:
-            processor = InitProcessor(
-                db_connection=self._connection,
-                namespace=namespace,
-                table_name=table_name,
-                table_schema=client.table_schema,
-            )
-
-        await processor.prepare()
-
-        await MetaTableManager(self._connection, namespace, table_name).initialize(
-            table_schema=client.table_schema, table_data=client.table_data
+        self._connection = SqlAlchemyConnection(
+            connection_string, {"postgresql": "asyncpg"}
         )
 
-        await client.download(processor)
-
-        async with self._connection.context() as conn:
-            await conn.commit()
+    def get_connection(self) -> AbstractDatabaseConnection:
+        if self._connection is None:
+            raise DatabaseConnectionError("not connected to the database")
+        return self._connection
+
+    def create_metatable_manager(
+        self, namespace: str, table: str
+    ) -> AbstractMetaTableManager:
+        if self._connection is None:
+            raise DatabaseConnectionError("not connected to the database")
+        return MetaTableManager(self._connection, namespace, table)
 
-    async def synchronize(
+    def create_init_processor(
         self,
         namespace: str,
-        table_name: str,
-        processor: Optional[BaseSyncProcessor] = None,
-    ) -> None:
-        meta_table_manager = MetaTableManager(self._connection, namespace, table_name)
-
-        since = await meta_table_manager.last_sync_datetime()
-
-        client = await IncrementalClientFactory(
-            self._session, namespace, table_name, since
-        ).get_client()
-
-        if processor is None:
-            processor = SyncProcessor(
-                db_connection=self._connection,
-                namespace=namespace,
-                table_name=table_name,
-                schema=client.table_schema,
-            )
-
-        await processor.prepare()
+        table: str,
+        schema: VersionedSchema,
+    ) -> AbstractInitProcessor:
+        if self._connection is None:
+            raise DatabaseConnectionError("not connected to the database")
+        return InitProcessor(self._connection, namespace, table, schema)
 
-        await meta_table_manager.synchronize(client.table_schema, client.table_data)
-        await client.download(processor)
-
-        async with self._connection.context() as conn:
-            await conn.commit()
+    def create_sync_processor(
+        self,
+        namespace: str,
+        table: str,
+        schema: VersionedSchema,
+    ) -> AbstractSyncProcessor:
+        if self._connection is None:
+            raise DatabaseConnectionError("not connected to the database")
+        return SyncProcessor(self._connection, namespace, table, schema)
+    
+    def create_database_validator(
+        self,
+        namespace: str,
+        table: str
+    ) -> AbstractDatabaseValidator:
+        if self._connection is None:
+            raise DatabaseConnectionError("not connected to the database")
+        return DatabaseValidator(self._connection, namespace, table)
```

### Comparing `instructure-dap-client-0.3.8.2/dap/timer.py` & `instructure-dap-client-0.3.9.1/dap/timer.py`

 * *Files identical despite different names*

### Comparing `instructure-dap-client-0.3.8.2/dap/timestamp.py` & `instructure-dap-client-0.3.9.1/dap/timestamp.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 )
 
 
 def valid_utc_datetime(s: str) -> datetime:
     """
     Converts a string into a UTC datetime instance.
 
-    :param s: An ISO 8601 timestamp string.
+    :param s: An ISO 8601 and RFC 3339 compliant timestamp string.
     :returns: A time zone aware datetime instance with time zone UTC.
     """
 
     # fromisoformat(...) supports military time zone designator "Zulu" to stand for UTC only in Python 3.11 and later
     if s.endswith("Z"):
         # remove time zone suffix "Z" (UTC), parse into naive datetime, and explicitly add time zone designator
         return datetime.fromisoformat(s[:-1]).replace(tzinfo=timezone.utc)
@@ -24,15 +24,15 @@
         return datetime.fromisoformat(s).astimezone(timezone.utc)
 
 
 def valid_naive_datetime(s: str) -> datetime:
     """
     Converts a string into a naive datetime instance.
 
-    :param s: An ISO 8601 timestamp string.
+    :param s: An ISO 8601 and RFC 3339 compliant timestamp string.
     :returns: A naive datetime instance that is implicitly assumed to be in time zone UTC.
     """
 
     # fromisoformat(...) supports military time zone designator "Zulu" to stand for UTC only in Python 3.11 and later
     if s.endswith("Z"):
         # remove time zone suffix "Z" (UTC) and parse into naive datetime
         return datetime.fromisoformat(s[:-1])
```

### Comparing `instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/PKG-INFO` & `instructure-dap-client-0.3.9.1/instructure_dap_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: instructure-dap-client
-Version: 0.3.8.2
+Version: 0.3.9.1
 Summary: Data Access Platform client library
-Author: Levente Hunyadi
-Author-email: levente.hunyadi@instructure.com
 Maintainer: Edina Tipter
 Maintainer-email: edina.tipter@instructure.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -307,15 +306,15 @@
 1. initialize a database, and
 2. synchronize a database with the data in DAP.
 
 In order to replicate data in DAP locally, we must first initialize a database:
 
 ```python
 from dap.api import DAPClient
-from dap.database.connection import DatabaseConnection
+from dap.integration.database import DatabaseConnection
 from dap.replicator.sql import SQLReplicator
 
 connection_string: str = "postgresql://scott:password@localhost/testdb"
 async with DatabaseConnection(connection_string).open() as db_connection:
     async with DAPClient() as session:
         await SQLReplicator(session, db_connection).initialize(namespace, table_name)
 ```
@@ -341,7 +340,16 @@
 * A new enumeration value is added to an existing enumeration type.
 * A new enumeration type is introduced.
 * A field (column) is removed from a table.
 
 Behind the scenes, the client library uses SQL commands such as `ALTER TABLE ... ADD COLUMN ...` or `ALTER TYPE ... ADD VALUE ...` to replicate schema changes in DAP in our local database. If the JSON schema change couldn't be mapped to a series of these SQL statements, the client library wouldn't be able to synchronize with DAP using incremental queries, and would have to issue an expensive snapshot query.
 
 Once the local database table structure has been reconciled with the new schema in DAP, and the meta-table has been updated, data synchronization proceeds normally with insert, update and delete SQL statements.
+
+### Dropping data from a local database
+
+If the table is no longer needed, it can be dropped from the database using the following code:
+
+```python
+async with DatabaseConnection(connection_string).open() as db_connection:
+    await SQLDrop(db_connection).drop(namespace, table_name)
+```
```

### Comparing `instructure-dap-client-0.3.8.2/instructure_dap_client.egg-info/SOURCES.txt` & `instructure-dap-client-0.3.9.1/instructure_dap_client.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 dap/__main__.py
 dap/api.py
 dap/arguments.py
 dap/concurrency.py
 dap/conversion_common.py
 dap/conversion_nonperf.py
 dap/conversion_perf.py
+dap/counted.py
 dap/dap_error.py
 dap/dap_types.py
 dap/downloader.py
 dap/log.py
 dap/networking.py
 dap/payload.py
 dap/py.typed
@@ -31,25 +32,37 @@
 dap/commands/commonargs.py
 dap/commands/dbargs.py
 dap/commands/dropdb_command.py
 dap/commands/initdb_command.py
 dap/commands/queryargs.py
 dap/commands/syncdb_command.py
 dap/commands/timestampargs.py
-dap/database/__init__.py
-dap/database/base_processor.py
-dap/database/connection.py
-dap/database/database_errors.py
-dap/database/database_operations.py
-dap/database/init_processor.py
-dap/database/sync_processor.py
-dap/model/__init__.py
-dap/model/ddl.py
-dap/model/meta_table.py
-dap/model/metadata.py
+dap/integration/__init__.py
+dap/integration/base_connection.py
+dap/integration/base_meta_table.py
+dap/integration/connection.py
+dap/integration/database.py
+dap/integration/database_errors.py
+dap/integration/meta_table.py
+dap/integration/plugin.py
+dap/integration/processor.py
+dap/integration/validator.py
+dap/plugins/__init__.py
+dap/plugins/postgres/__init__.py
+dap/plugins/postgres/ddl.py
+dap/plugins/postgres/init_processor.py
+dap/plugins/postgres/meta_table.py
+dap/plugins/postgres/metadata.py
+dap/plugins/postgres/plugin.py
+dap/plugins/postgres/queries.py
+dap/plugins/postgres/sync_processor.py
+dap/plugins/postgres/validator.py
+dap/plugins/sqlalchemy/__init__.py
+dap/plugins/sqlalchemy/connection.py
+dap/plugins/sqlalchemy/queries.py
 dap/replicator/__init__.py
 dap/replicator/sql.py
 instructure_dap_client.egg-info/PKG-INFO
 instructure_dap_client.egg-info/SOURCES.txt
 instructure_dap_client.egg-info/dependency_links.txt
 instructure_dap_client.egg-info/entry_points.txt
 instructure_dap_client.egg-info/requires.txt
```

### Comparing `instructure-dap-client-0.3.8.2/setup.cfg` & `instructure-dap-client-0.3.9.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [metadata]
 name = instructure-dap-client
 version = attr: dap.__version__
 description = Data Access Platform client library
-author = Levente Hunyadi
-author_email = levente.hunyadi@instructure.com
 maintainer = Edina Tipter
 maintainer_email = edina.tipter@instructure.com
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: Developers
+	Intended Audience :: End Users/Desktop
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
@@ -28,18 +27,18 @@
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	aiohttp >= 3.8.4
 	aiofiles >= 23.1.0
 	types-aiofiles >= 23.1.0
 	json_strong_typing >= 0.2.7
-	orjson >= 3.8.10
-	PyJWT >= 2.6.0
+	orjson >= 3.9.1
+	PyJWT >= 2.7.0
 	asyncpg >= 0.27.0
-	SQLAlchemy[asyncio] >= 2.0.10
+	SQLAlchemy[asyncio] >= 2.0.16
 
 [options.entry_points]
 console_scripts = 
 	dap = dap.__main__:console_entry
 
 [options.packages.find]
 exclude =
```

