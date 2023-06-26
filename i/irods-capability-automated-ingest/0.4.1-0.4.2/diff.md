# Comparing `tmp/irods-capability-automated-ingest-0.4.1.tar.gz` & `tmp/irods-capability-automated-ingest-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irods-capability-automated-ingest-0.4.1.tar", last modified: Sun Mar 26 16:22:03 2023, max compression
+gzip compressed data, was "irods-capability-automated-ingest-0.4.2.tar", last modified: Mon Jun 26 16:50:00 2023, max compression
```

## Comparing `irods-capability-automated-ingest-0.4.1.tar` & `irods-capability-automated-ingest-0.4.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-03-26 16:22:03.593054 irods-capability-automated-ingest-0.4.1/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      143 2018-05-31 00:38:01.000000 irods-capability-automated-ingest-0.4.1/AUTHORS
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     5127 2023-03-26 16:18:16.000000 irods-capability-automated-ingest-0.4.1/CHANGELOG.md
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1541 2018-05-31 00:38:02.000000 irods-capability-automated-ingest-0.4.1/LICENSE.txt
--rw-rw-r--   0 tgr       (1000) tgr       (1000)       50 2018-05-31 00:38:02.000000 irods-capability-automated-ingest-0.4.1/MANIFEST.in
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    23659 2023-03-26 16:22:03.593054 irods-capability-automated-ingest-0.4.1/PKG-INFO
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    17844 2023-03-24 13:01:22.000000 irods-capability-automated-ingest-0.4.1/README.md
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-03-26 16:22:03.585054 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)        0 2018-05-31 00:38:02.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/__init__.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     4633 2023-03-24 13:01:22.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/char_map_util.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1235 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/core.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3428 2022-02-25 02:13:17.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/custom_event_handler.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1101 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/evhdlr.py
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-03-26 16:22:03.593054 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)        0 2018-05-31 00:38:02.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/__init__.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      247 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/append.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      435 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/append_json.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      340 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/append_non_leaf_non_root_with_resc_name.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      344 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/append_root_with_resc_name.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      341 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/append_with_resc_name.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      967 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/metadata.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      242 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/no_op.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      708 2022-02-23 19:07:56.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/no_retry.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      378 2022-02-23 19:07:56.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/post_job.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      371 2022-02-23 19:07:56.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/pre_job.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      241 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/put.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      334 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/put_non_leaf_non_root_with_resc_name.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      338 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/put_root_with_resc_name.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      508 2023-03-24 13:01:22.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/put_using_char_map.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      335 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/put_with_resc_name.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      249 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/register.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      343 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/register_non_leaf_non_root_with_resc_name.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      347 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/register_root_with_resc_name.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      517 2023-03-24 13:01:22.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/register_using_char_map.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1760 2019-04-10 14:17:13.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/register_with_peps.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      344 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/register_with_resc_name.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      361 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/replica_root_with_resc_name.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      357 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/replica_with_non_leaf_non_root_resc_name.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      358 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/replica_with_resc_name.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      873 2022-02-23 19:07:56.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/retry.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1146 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/statistics.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      245 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/sync.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      338 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/sync_non_leaf_non_root_with_resc_name.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      326 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/sync_retry.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      342 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/sync_root_with_resc_name.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      339 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/sync_with_resc_name.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      445 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/timeout.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     2784 2018-09-19 17:28:05.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/flask_app.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    11974 2023-03-26 16:18:16.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/irods_sync.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1117 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/irods_worker.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     2111 2018-09-08 02:27:08.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/phl.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     5327 2022-02-25 02:13:17.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/redis_key.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     7787 2022-02-25 02:13:17.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/scanner.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     7499 2022-10-07 14:28:54.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/sync_actions.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    18898 2023-03-24 13:01:22.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/sync_irods.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     2781 2022-02-25 02:13:17.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/sync_job.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     2065 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/sync_logging.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    13843 2023-03-24 13:01:22.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/sync_task.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1076 2022-02-23 19:07:56.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/sync_utils.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1016 2022-02-23 19:07:56.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/task_queue.py
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-03-26 16:22:03.593054 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/test/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)        0 2018-05-31 00:38:02.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/test/__init__.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    70956 2023-03-26 16:18:16.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/test/test_irods_sync.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     1009 2022-02-23 19:07:56.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/utils.py
--rw-rw-r--   0 tgr       (1000) tgr       (1000)       22 2023-03-26 16:18:16.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/version.py
-drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-03-26 16:22:03.585054 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest.egg-info/
--rw-rw-r--   0 tgr       (1000) tgr       (1000)    23659 2023-03-26 16:22:03.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest.egg-info/PKG-INFO
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     3612 2023-03-26 16:22:03.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest.egg-info/SOURCES.txt
--rw-rw-r--   0 tgr       (1000) tgr       (1000)        1 2023-03-26 16:22:03.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest.egg-info/dependency_links.txt
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      105 2023-03-26 16:22:03.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest.egg-info/entry_points.txt
--rw-rw-r--   0 tgr       (1000) tgr       (1000)      194 2023-03-26 16:22:03.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest.egg-info/requires.txt
--rw-rw-r--   0 tgr       (1000) tgr       (1000)       34 2023-03-26 16:22:03.000000 irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest.egg-info/top_level.txt
--rw-rw-r--   0 tgr       (1000) tgr       (1000)       79 2023-03-26 16:22:03.593054 irods-capability-automated-ingest-0.4.1/setup.cfg
--rw-rw-r--   0 tgr       (1000) tgr       (1000)     2238 2022-02-25 02:13:17.000000 irods-capability-automated-ingest-0.4.1/setup.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-06-26 16:50:00.387288 irods-capability-automated-ingest-0.4.2/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      143 2018-05-31 00:38:01.000000 irods-capability-automated-ingest-0.4.2/AUTHORS
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     5624 2023-06-26 16:46:01.000000 irods-capability-automated-ingest-0.4.2/CHANGELOG.md
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1541 2018-05-31 00:38:02.000000 irods-capability-automated-ingest-0.4.2/LICENSE.txt
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)       50 2018-05-31 00:38:02.000000 irods-capability-automated-ingest-0.4.2/MANIFEST.in
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    23710 2023-06-26 16:50:00.387288 irods-capability-automated-ingest-0.4.2/PKG-INFO
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    17844 2023-03-24 13:01:22.000000 irods-capability-automated-ingest-0.4.2/README.md
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-06-26 16:50:00.379289 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)        0 2018-05-31 00:38:02.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/__init__.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     4633 2023-03-24 13:01:22.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/char_map_util.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1235 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/core.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3428 2022-02-25 02:13:17.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/custom_event_handler.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1101 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/evhdlr.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-06-26 16:50:00.387288 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)        0 2018-05-31 00:38:02.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/__init__.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      247 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/append.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      435 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/append_json.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      340 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/append_non_leaf_non_root_with_resc_name.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      344 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/append_root_with_resc_name.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      341 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/append_with_resc_name.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      967 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/metadata.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      242 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/no_op.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      708 2022-02-23 19:07:56.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/no_retry.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      470 2023-06-26 16:36:42.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/post_job.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      371 2022-02-23 19:07:56.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/pre_job.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      241 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/put.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      334 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/put_non_leaf_non_root_with_resc_name.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      338 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/put_root_with_resc_name.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      508 2023-03-24 13:01:22.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/put_using_char_map.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      335 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/put_with_resc_name.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      249 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/register.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      343 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/register_non_leaf_non_root_with_resc_name.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      347 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/register_root_with_resc_name.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      517 2023-03-24 13:01:22.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/register_using_char_map.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1760 2019-04-10 14:17:13.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/register_with_peps.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      344 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/register_with_resc_name.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      361 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/replica_root_with_resc_name.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      357 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/replica_with_non_leaf_non_root_resc_name.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      358 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/replica_with_resc_name.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      873 2022-02-23 19:07:56.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/retry.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1146 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/statistics.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      245 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/sync.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      338 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/sync_non_leaf_non_root_with_resc_name.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      326 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/sync_retry.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      342 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/sync_root_with_resc_name.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      339 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/sync_with_resc_name.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      445 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/timeout.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     2784 2018-09-19 17:28:05.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/flask_app.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    11974 2023-03-26 16:18:16.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/irods_sync.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1117 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/irods_worker.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     2111 2018-09-08 02:27:08.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/phl.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     5327 2022-02-25 02:13:17.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/redis_key.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     7789 2023-06-26 16:36:42.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/scanner.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     7499 2022-10-07 14:28:54.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/sync_actions.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    18898 2023-03-24 13:01:22.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/sync_irods.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     2781 2022-02-25 02:13:17.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/sync_job.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     2065 2018-09-04 02:38:35.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/sync_logging.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    13848 2023-06-26 16:36:42.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/sync_task.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1076 2022-02-23 19:07:56.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/sync_utils.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1016 2022-02-23 19:07:56.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/task_queue.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-06-26 16:50:00.387288 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/test/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)        0 2018-05-31 00:38:02.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/test/__init__.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    73847 2023-06-26 16:36:42.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/test/test_irods_sync.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     1009 2022-02-23 19:07:56.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/utils.py
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)       22 2023-06-26 16:46:01.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/version.py
+drwxrwxr-x   0 tgr       (1000) tgr       (1000)        0 2023-06-26 16:50:00.383288 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest.egg-info/
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)    23710 2023-06-26 16:50:00.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest.egg-info/PKG-INFO
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     3612 2023-06-26 16:50:00.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest.egg-info/SOURCES.txt
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)        1 2023-06-26 16:50:00.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest.egg-info/dependency_links.txt
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      105 2023-06-26 16:50:00.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest.egg-info/entry_points.txt
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)      194 2023-06-26 16:50:00.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest.egg-info/requires.txt
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)       34 2023-06-26 16:50:00.000000 irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest.egg-info/top_level.txt
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)       79 2023-06-26 16:50:00.387288 irods-capability-automated-ingest-0.4.2/setup.cfg
+-rw-rw-r--   0 tgr       (1000) tgr       (1000)     2288 2023-06-26 16:36:42.000000 irods-capability-automated-ingest-0.4.2/setup.py
```

### Comparing `irods-capability-automated-ingest-0.4.1/CHANGELOG.md` & `irods-capability-automated-ingest-0.4.2/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # Changelog
 
+## [v0.4.2] - 2023-06-26
+
+This release fixes the exclude and post_job behavior
+and updates two dependencies.
+
+- [#200] Add --exclude_file_type test
+- [#201] Amend test for post_job
+- [#195] apply CELERY_BROKER_URL env var globally to tests
+- [#198] update to Python 3.11 in docker test suite
+- [#201] Fix job done condition
+- [#200] Fix exclude_file_name/exclude_file_type
+- [#200] Add test for --exclude_file_name
+- Bump certifi from 2018.11.29 to 2022.12.7
+- Bump werkzeug from 0.15.3 to 2.2.3
+
 ## [v0.4.1] - 2023-03-26
 
 This release fixes an exit code bug and adds a
 character_map event handler method.
 
 - [#188] eliminate exit call in check_event_handler
 - [#40][#166] tests work for unicodeEncodeError and char_map put/register
```

### Comparing `irods-capability-automated-ingest-0.4.1/LICENSE.txt` & `irods-capability-automated-ingest-0.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/PKG-INFO` & `irods-capability-automated-ingest-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irods-capability-automated-ingest
-Version: 0.4.1
+Version: 0.4.2
 Summary: Implement filesystem scanners and landing zones
 Home-page: https://github.com/irods/irods_capability_automated_ingest
 Author: iRODS Consortium
 Author-email: support@irods.org
 License: BSD
 Project-URL: Bug Reports, https://github.com/irods/irods_capability_automated_ingest/issues
 Project-URL: Source, https://github.com/irods/irods_capability_automated_ingest
@@ -604,9 +604,10 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7,
 Description-Content-Type: text/markdown
```

### Comparing `irods-capability-automated-ingest-0.4.1/README.md` & `irods-capability-automated-ingest-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/char_map_util.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/char_map_util.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/core.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/core.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/custom_event_handler.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/custom_event_handler.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/evhdlr.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/evhdlr.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/metadata.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/metadata.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/no_retry.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/no_retry.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/register_using_char_map.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/register_using_char_map.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/register_with_peps.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/register_with_peps.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/retry.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/retry.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/examples/statistics.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/examples/statistics.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/flask_app.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/flask_app.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/irods_sync.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/irods_sync.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/irods_worker.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/irods_worker.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/phl.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/phl.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/redis_key.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/redis_key.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/scanner.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/scanner.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             if(dir_match == True):
                 break
 
         file_match = None
         for f in file_regex:
             file_match = None != f.match(full_path)
             if(file_match == True):
-                break
+                return True
 
         try:
             if mode is None:
                 mode = os.lstat(full_path).st_mode
         except FileNotFoundError:
             return False
 
@@ -97,15 +97,15 @@
         dir_regex = [re.compile(r) for r in meta['exclude_directory_name']]
 
         full_path = os.path.abspath(obj.path)
         mode = obj.stat(follow_symlinks=False).st_mode
 
         try:
             if self.exclude_file_type(dir_regex, file_regex, full_path, logger, mode):
-                return full_path, obj_stats
+                raise ContinueException
 
             if not obj.is_symlink() and not bool(mode & stat.S_IRGRP):
                 logger.error(
                     'physical path is not readable [{0}]'.format(full_path))
                 return full_path, obj_stats
 
             if obj.is_dir() and not obj.is_symlink() and not obj.is_file():
```

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/sync_actions.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/sync_actions.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/sync_irods.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/sync_irods.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/sync_job.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/sync_job.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/sync_logging.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/sync_logging.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/sync_task.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/sync_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         meta = args[0]
         config = meta["config"]
         job = sync_job.from_meta(meta)
         logger = sync_logging.get_sync_logger(config["log"])
         logger.info('decr_job_name', task=meta["task"], path=meta["path"], job_name=job.name(
         ), task_id=task_id, retval=retval)
 
-        done = job.tasks_handle().decr() and not job.periodic()
+        done = job.tasks_handle().decr() == 0 and not job.periodic()
         if done:
             job.cleanup()
 
         job.dequeue_handle().rpush(task_id)
 
         if done:
             event_handler = custom_event_handler(meta)
```

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/sync_utils.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/sync_utils.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/task_queue.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/task_queue.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/test/test_irods_sync.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/test/test_irods_sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from irods_capability_automated_ingest.sync_utils import size, app
 from irods_capability_automated_ingest.sync_utils import get_redis as sync_utils_get_redis
 from irods_capability_automated_ingest.sync_job import sync_job
 from irods.data_object import irods_dirname, irods_basename
 import irods_capability_automated_ingest.examples
 import irods.keywords as kw
 
+os.environ["CELERY_BROKER_URL"] = "redis://redis:6379/0"
+
 LOG_FILE = "/tmp/a"
 
 ZONENAME = "tempZone"
 RODSADMIN = "rods"
 
 IRODS_SYNC_PY = "irods_capability_automated_ingest.irods_sync"
 
@@ -280,16 +282,14 @@
 
 
 def event_handler_path(eh_name):
     return os.path.join(sys.modules["irods_capability_automated_ingest.examples"].__path__[0], eh_name + '.py')
 
 class automated_ingest_test_context(object):
     def setUp(self):
-        os.environ["CELERY_BROKER_URL"] = "redis://redis:6379/0"
-
         irmtrash()
         clear_redis()
         delete_collection_if_exists(PATH_TO_COLLECTION)
         create_files(NFILES)
         with iRODSSession(**get_kwargs()) as session:
             create_resources(session, HIERARCHY1)
 
@@ -554,15 +554,16 @@
 
     def do_post_job(self, eh_name, job_name = DEFAULT_JOB_NAME):
         eh = event_handler_path(eh_name)
 
         proc = subprocess.Popen(["python", "-m", IRODS_SYNC_PY, "start", PATH_TO_SOURCE_DIR, PATH_TO_COLLECTION, "--event_handler", eh, "--job_name", job_name, "--log_level", "INFO", '--files_per_task', '1'])
         proc.wait()
 
-        workers = start_workers(1)
+        # Start 4 workers to ensure that the post_job is executed only once per job, not once per worker.
+        workers = start_workers(4)
         wait_for(workers, job_name)
         with open(LOG_FILE,"r") as f:
             lines = f.readlines()
             self.assertEqual(lines, ["post_job"])
 
     def test_pre_job(self):
         job_name = 'test_pre_job.do_pre_job'
@@ -1397,14 +1398,86 @@
         except subprocess.CalledProcessError as e:
             self.assertTrue(expected_err_msg in str(e.stderr))
             return
         else:
             self.fail('target collection should fail to ingest')
 
 
+class test_exclude_options(automated_ingest_test_context, unittest.TestCase):
+    def setUp(self):
+        super(test_exclude_options, self).setUp()
+
+    def tearDown(self):
+        super(test_exclude_options, self).tearDown()
+
+    def assert_that_source_files_are_excluded_in_collection(self,
+                                                            source_dir=PATH_TO_SOURCE_DIR,
+                                                            destination_coll=PATH_TO_COLLECTION,
+                                                            excluded_files=[]):
+        with iRODSSession(**get_kwargs()) as session:
+            self.assertTrue(session.collections.exists(destination_coll))
+            for i in listdir(source_dir):
+                logical_path = destination_coll + "/" + i
+                if i in excluded_files:
+                    self.assertFalse(session.data_objects.exists(logical_path))
+                else:
+                    self.assertTrue(session.data_objects.exists(logical_path))
+
+
+    def test_exclude_file_name_single_file(self):
+        job_name = 'test_exclude_file_name'
+        exclude_file_name = '5'
+        exclude_file_path = os.path.join(PATH_TO_SOURCE_DIR, exclude_file_name)
+        sync_cmd = [
+            'python', '-m', IRODS_SYNC_PY, 'start',
+            PATH_TO_SOURCE_DIR,
+            PATH_TO_COLLECTION,
+            '--exclude_file_name', exclude_file_path,
+            '--job_name', job_name,
+            '--log_level', 'INFO',
+            '--files_per_task', '1']
+
+        proc = subprocess.Popen(sync_cmd)
+        proc.wait()
+        workers = start_workers(1)
+        wait_for(workers, job_name)
+
+        # Make sure no jobs fail
+        self.do_assert_failed_queue(count=None, job_name=job_name)
+
+        self.assert_that_source_files_are_excluded_in_collection(excluded_files=[exclude_file_name])
+
+
+    def test_exclude_file_type_single_file_link(self):
+        job_name = 'test_exclude_file_name'
+        exclude_file_name = 'link_to_5'
+        link_path = os.path.join(PATH_TO_SOURCE_DIR, 'link_to_5')
+        link_target = os.path.join(PATH_TO_SOURCE_DIR, '5')
+        sync_cmd = [
+            'python', '-m', IRODS_SYNC_PY, 'start',
+            PATH_TO_SOURCE_DIR,
+            PATH_TO_COLLECTION,
+            '--exclude_file_type', 'link',
+            '--job_name', job_name,
+            '--log_level', 'INFO',
+            '--files_per_task', '1']
+
+        os.symlink(link_target, link_path)
+
+        proc = subprocess.Popen(sync_cmd)
+        proc.wait()
+        workers = start_workers(1)
+        wait_for(workers, job_name)
+
+        # Make sure no jobs fail
+        self.do_assert_failed_queue(count=None, job_name=job_name)
+
+        self.assert_that_source_files_are_excluded_in_collection(excluded_files=[exclude_file_name])
+
+
 # TODO base64 transform should be the same for each of the current types of test
 
 def b64_calculation(this):
     utf8_escaped_abspath = this.bad_filepath
     this.b64_path_str = base64.b64encode(utf8_escaped_abspath)
```

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest/utils.py` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest/utils.py`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest.egg-info/PKG-INFO` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irods-capability-automated-ingest
-Version: 0.4.1
+Version: 0.4.2
 Summary: Implement filesystem scanners and landing zones
 Home-page: https://github.com/irods/irods_capability_automated_ingest
 Author: iRODS Consortium
 Author-email: support@irods.org
 License: BSD
 Project-URL: Bug Reports, https://github.com/irods/irods_capability_automated_ingest/issues
 Project-URL: Source, https://github.com/irods/irods_capability_automated_ingest
@@ -604,9 +604,10 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7,
 Description-Content-Type: text/markdown
```

### Comparing `irods-capability-automated-ingest-0.4.1/irods_capability_automated_ingest.egg-info/SOURCES.txt` & `irods-capability-automated-ingest-0.4.2/irods_capability_automated_ingest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irods-capability-automated-ingest-0.4.1/setup.py` & `irods-capability-automated-ingest-0.4.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,16 @@
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10'
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
     ],
     keywords='irods automated ingest landingzone filesystem',
     packages=find_packages(),
     install_requires=[
         'minio',
         'flask',
         'flask-restful',
```

