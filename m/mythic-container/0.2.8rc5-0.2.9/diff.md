# Comparing `tmp/mythic_container-0.2.8rc5.tar.gz` & `tmp/mythic_container-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mythic_container-0.2.8rc5.tar", last modified: Thu May 18 13:49:10 2023, max compression
+gzip compressed data, was "mythic_container-0.2.9.tar", last modified: Tue May 23 20:31:29 2023, max compression
```

## Comparing `mythic_container-0.2.8rc5.tar` & `mythic_container-0.2.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-18 13:49:10.592763 mythic_container-0.2.8rc5/
--rw-r--r--   0 itsafeature   (501) staff       (20)     1481 2023-03-07 22:54:23.000000 mythic_container-0.2.8rc5/LICENSE.md
--rw-r--r--   0 itsafeature   (501) staff       (20)     1441 2023-05-18 13:49:10.592198 mythic_container-0.2.8rc5/PKG-INFO
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      993 2023-04-25 19:15:08.000000 mythic_container-0.2.8rc5/README.md
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-18 13:49:10.527344 mythic_container-0.2.8rc5/mythic_container/
--rw-r--r--   0 itsafeature   (501) staff       (20)    29750 2023-05-17 15:58:25.000000 mythic_container-0.2.8rc5/mythic_container/C2ProfileBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    26032 2023-04-20 01:54:22.000000 mythic_container-0.2.8rc5/mythic_container/LoggingBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    79103 2023-05-18 13:47:52.000000 mythic_container-0.2.8rc5/mythic_container/MythicCommandBase.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-18 13:49:10.586877 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2482 2023-04-01 06:52:48.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1368 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1214 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1721 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1562 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2181 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1316 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3360 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1710 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1343 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7581 2023-05-09 13:37:04.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2273 2023-04-04 02:07:20.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3309 2023-04-26 14:57:11.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4295 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1474 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3478 2023-04-01 06:52:13.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2267 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2495 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2767 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1330 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1785 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4453 2023-04-13 18:13:16.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2216 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3713 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1771 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1852 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2621 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1898 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2572 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1332 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4632 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     6013 2023-04-01 05:24:39.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1748 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2017 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3097 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4779 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2101 2023-05-08 14:43:34.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1318 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1403 2023-03-25 00:41:22.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2081 2023-05-17 23:38:25.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1940 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2659 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1642 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7752 2023-02-22 19:46:40.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1372 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1375 2023-02-21 14:37:49.000000 mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    28320 2023-02-21 14:36:00.000000 mythic_container-0.2.8rc5/mythic_container/MythicRPC.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    22456 2023-05-05 22:49:39.000000 mythic_container-0.2.8rc5/mythic_container/PayloadBuilder.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    17326 2023-05-17 15:46:10.000000 mythic_container-0.2.8rc5/mythic_container/TranslationBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    13910 2023-05-08 15:16:26.000000 mythic_container-0.2.8rc5/mythic_container/WebhookBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2578 2023-05-18 13:48:56.000000 mythic_container-0.2.8rc5/mythic_container/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    37506 2023-05-10 16:58:58.000000 mythic_container-0.2.8rc5/mythic_container/agent_utils.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    27738 2023-04-24 22:49:45.000000 mythic_container-0.2.8rc5/mythic_container/c2_utils.py
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      262 2023-02-28 20:49:28.000000 mythic_container-0.2.8rc5/mythic_container/config.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-18 13:49:10.590160 mythic_container-0.2.8rc5/mythic_container/grpc/
--rw-r--r--   0 itsafeature   (501) staff       (20)        0 2023-02-20 17:25:18.000000 mythic_container-0.2.8rc5/mythic_container/grpc/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4479 2023-02-21 13:59:33.000000 mythic_container-0.2.8rc5/mythic_container/grpc/translationContainerGRPC_pb2.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7092 2023-02-21 17:37:56.000000 mythic_container-0.2.8rc5/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py
--rw-r--r--   0 itsafeature   (501) staff       (20)      937 2023-02-28 20:15:31.000000 mythic_container-0.2.8rc5/mythic_container/logging.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4025 2023-04-19 23:39:10.000000 mythic_container-0.2.8rc5/mythic_container/logging_utils.py
--rwxr-xr-x   0 itsafeature   (501) staff       (20)    29520 2023-04-27 21:29:31.000000 mythic_container-0.2.8rc5/mythic_container/mythic_service.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    15080 2023-04-27 21:25:32.000000 mythic_container-0.2.8rc5/mythic_container/rabbitmq.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1670 2023-02-21 14:36:00.000000 mythic_container-0.2.8rc5/mythic_container/utils_mythic_file_transfer.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2821 2023-04-20 15:20:17.000000 mythic_container-0.2.8rc5/mythic_container/webhook_utils.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-18 13:49:10.530429 mythic_container-0.2.8rc5/mythic_container.egg-info/
--rw-r--r--   0 itsafeature   (501) staff       (20)     1441 2023-05-18 13:49:10.000000 mythic_container-0.2.8rc5/mythic_container.egg-info/PKG-INFO
--rw-r--r--   0 itsafeature   (501) staff       (20)     4375 2023-05-18 13:49:10.000000 mythic_container-0.2.8rc5/mythic_container.egg-info/SOURCES.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-05-18 13:49:10.000000 mythic_container-0.2.8rc5/mythic_container.egg-info/dependency_links.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       95 2023-05-18 13:49:10.000000 mythic_container-0.2.8rc5/mythic_container.egg-info/requires.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       17 2023-05-18 13:49:10.000000 mythic_container-0.2.8rc5/mythic_container.egg-info/top_level.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-05-18 13:49:10.592967 mythic_container-0.2.8rc5/setup.cfg
--rwxr-xr-x   0 itsafeature   (501) staff       (20)     1093 2023-05-18 13:48:50.000000 mythic_container-0.2.8rc5/setup.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-23 20:31:29.370063 mythic_container-0.2.9/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1481 2023-03-07 22:54:23.000000 mythic_container-0.2.9/LICENSE.md
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1438 2023-05-23 20:31:29.369815 mythic_container-0.2.9/PKG-INFO
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      993 2023-04-25 19:15:08.000000 mythic_container-0.2.9/README.md
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-23 20:31:29.301180 mythic_container-0.2.9/mythic_container/
+-rw-r--r--   0 itsafeature   (501) staff       (20)    34878 2023-05-23 16:12:07.000000 mythic_container-0.2.9/mythic_container/C2ProfileBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    26032 2023-04-20 01:54:22.000000 mythic_container-0.2.9/mythic_container/LoggingBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    79359 2023-05-23 20:23:23.000000 mythic_container-0.2.9/mythic_container/MythicCommandBase.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-23 20:31:29.366312 mythic_container-0.2.9/mythic_container/MythicGoRPC/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2482 2023-04-01 06:52:48.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1368 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1214 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1721 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1562 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2181 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1316 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3360 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1710 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1343 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7581 2023-05-09 13:37:04.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2273 2023-04-04 02:07:20.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3309 2023-04-26 14:57:11.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4295 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1474 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3478 2023-04-01 06:52:13.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2267 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2495 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2767 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1330 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1785 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4453 2023-04-13 18:13:16.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2370 2023-05-23 15:57:54.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3713 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1771 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1852 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2621 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1898 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2572 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1332 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4632 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     6013 2023-04-01 05:24:39.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1748 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2017 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3097 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4779 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2101 2023-05-08 14:43:34.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1318 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1403 2023-03-25 00:41:22.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2081 2023-05-17 23:38:25.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1940 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2659 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1642 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7752 2023-02-22 19:46:40.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1372 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1375 2023-02-21 14:37:49.000000 mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    28320 2023-02-21 14:36:00.000000 mythic_container-0.2.9/mythic_container/MythicRPC.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    22456 2023-05-05 22:49:39.000000 mythic_container-0.2.9/mythic_container/PayloadBuilder.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    17326 2023-05-17 15:46:10.000000 mythic_container-0.2.9/mythic_container/TranslationBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    13910 2023-05-08 15:16:26.000000 mythic_container-0.2.9/mythic_container/WebhookBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2679 2023-05-23 20:13:12.000000 mythic_container-0.2.9/mythic_container/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    37592 2023-05-23 20:30:41.000000 mythic_container-0.2.9/mythic_container/agent_utils.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    33185 2023-05-23 16:15:19.000000 mythic_container-0.2.9/mythic_container/c2_utils.py
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      262 2023-02-28 20:49:28.000000 mythic_container-0.2.9/mythic_container/config.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-23 20:31:29.368826 mythic_container-0.2.9/mythic_container/grpc/
+-rw-r--r--   0 itsafeature   (501) staff       (20)        0 2023-02-20 17:25:18.000000 mythic_container-0.2.9/mythic_container/grpc/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4479 2023-02-21 13:59:33.000000 mythic_container-0.2.9/mythic_container/grpc/translationContainerGRPC_pb2.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7092 2023-02-21 17:37:56.000000 mythic_container-0.2.9/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)      937 2023-02-28 20:15:31.000000 mythic_container-0.2.9/mythic_container/logging.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4025 2023-04-19 23:39:10.000000 mythic_container-0.2.9/mythic_container/logging_utils.py
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)    30177 2023-05-23 16:17:44.000000 mythic_container-0.2.9/mythic_container/mythic_service.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    15080 2023-04-27 21:25:32.000000 mythic_container-0.2.9/mythic_container/rabbitmq.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1670 2023-02-21 14:36:00.000000 mythic_container-0.2.9/mythic_container/utils_mythic_file_transfer.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2821 2023-04-20 15:20:17.000000 mythic_container-0.2.9/mythic_container/webhook_utils.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-05-23 20:31:29.303123 mythic_container-0.2.9/mythic_container.egg-info/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1438 2023-05-23 20:31:29.000000 mythic_container-0.2.9/mythic_container.egg-info/PKG-INFO
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4375 2023-05-23 20:31:29.000000 mythic_container-0.2.9/mythic_container.egg-info/SOURCES.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-05-23 20:31:29.000000 mythic_container-0.2.9/mythic_container.egg-info/dependency_links.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       95 2023-05-23 20:31:29.000000 mythic_container-0.2.9/mythic_container.egg-info/requires.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       17 2023-05-23 20:31:29.000000 mythic_container-0.2.9/mythic_container.egg-info/top_level.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-05-23 20:31:29.370165 mythic_container-0.2.9/setup.cfg
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)     1088 2023-05-23 20:13:05.000000 mythic_container-0.2.9/setup.py
```

### Comparing `mythic_container-0.2.8rc5/LICENSE.md` & `mythic_container-0.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/PKG-INFO` & `mythic_container-0.2.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic_container
-Version: 0.2.8rc5
+Version: 0.2.9
 Summary: Functionality for Mythic Services
 Home-page: https://docs.mythic-c2.net/customizing/payload-type-development
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mythic_container-0.2.8rc5/README.md` & `mythic_container-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/C2ProfileBase.py` & `mythic_container-0.2.9/mythic_container/C2ProfileBase.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from enum import Enum
 from abc import abstractmethod
 import json
 from collections.abc import Awaitable, Callable
 from .logging import logger
 import base64
 import sys
+from typing import List
 
 
 class C2OPSECMessage:
     """Payload's C2 Profile configuration for OPSEC checking
 
     Attributes:
         Name (str): Name of the C2 Profile
@@ -132,14 +133,162 @@
             "message": self.Message
         }
 
     def __str__(self):
         return json.dumps(self.to_json(), sort_keys=True, indent=2)
 
 
+class C2GetIOCMessage:
+    """Payload's C2 Profile configuration for getting IOCs
+
+    Attributes:
+        Name (str): Name of the C2 Profile
+        Parameters (dict): Dictionary of C2 Parameter name:value
+
+    Functions:
+        to_json(self): return dictionary form of class
+    """
+
+    def __init__(self,
+                 c2_profile_name: str,
+                 parameters: dict,
+                 **kwargs):
+        self.Name = c2_profile_name
+        self.Parameters = parameters
+        for k, v in kwargs.items():
+            logger.error(f"unknown kwarg {k} {v}")
+
+    def to_json(self):
+        return {
+            "c2_profile_name": self.Name,
+            "parameters": self.Parameters
+        }
+
+    def __str__(self):
+        return json.dumps(self.to_json(), sort_keys=True, indent=2)
+
+
+class C2GetIOCMessageResponseIOC:
+    """An IOC to report back as part of a C2 Profile's get_ioc function
+
+    Attributes:
+        Type (str): The type of IOC (ex: Hash, URL)
+        IOC (str): The actual IOC value
+    """
+    def __init__(self,
+                 Type: str,
+                 IOC: str):
+        self.Type = Type
+        self.IOC = IOC
+
+    def to_json(self):
+        return {
+            "type": self.Type,
+            "ioc": self.IOC
+        }
+
+
+class C2GetIOCMessageResponse:
+    """Status of running C2 Profile's get_ioc function
+
+    Attributes:
+        Success (bool): Did the get ioc request succeed or fail
+        Error (str): Error message if the get ioc request failed
+        IOCs (List[C2GetIOCMessageResponseIOC]): List of the IOC values
+
+    Functions:
+        to_json(self): return dictionary form of class
+    """
+
+    def __init__(self,
+                 Success: bool,
+                 Error: str = "",
+                 IOCs: List[C2GetIOCMessageResponseIOC] = [],
+                 **kwargs):
+        self.Success = Success
+        self.Error = Error
+        self.IOCs = IOCs
+        for k, v in kwargs.items():
+            logger.error(f"unknown kwarg {k} {v}")
+
+    def to_json(self):
+        return {
+            "success": self.Success,
+            "error": self.Error,
+            "iocs": self.IOCs
+        }
+
+    def __str__(self):
+        return json.dumps(self.to_json(), sort_keys=True, indent=2)
+
+
+class C2SampleMessageMessage:
+    """Sample C2 message based on the Payload's configuration
+
+    Attributes:
+        Name (str): Name of the C2 Profile
+        Parameters (dict): Dictionary of C2 Parameter name:value
+
+    Functions:
+        to_json(self): return dictionary form of class
+    """
+
+    def __init__(self,
+                 c2_profile_name: str,
+                 parameters: dict,
+                 **kwargs):
+        self.Name = c2_profile_name
+        self.Parameters = parameters
+        for k, v in kwargs.items():
+            logger.error(f"unknown kwarg {k} {v}")
+
+    def to_json(self):
+        return {
+            "c2_profile_name": self.Name,
+            "parameters": self.Parameters
+        }
+
+    def __str__(self):
+        return json.dumps(self.to_json(), sort_keys=True, indent=2)
+
+
+class C2SampleMessageMessageResponse:
+    """Sample C2 Message based on the payload's configuration
+
+    Attributes:
+        Success (bool): Did the sample message generation succeed or fail
+        Error (str): Error message if the sample message generation failed
+        Message (str): Sample message to represent that C2 traffic would look like for this payload
+
+    Functions:
+        to_json(self): return dictionary form of class
+    """
+
+    def __init__(self,
+                 Success: bool,
+                 Error: str = "",
+                 Message: str = "",
+                 **kwargs):
+        self.Success = Success
+        self.Error = Error
+        self.Message = Message
+        for k, v in kwargs.items():
+            logger.error(f"unknown kwarg {k} {v}")
+
+    def to_json(self):
+        return {
+            "success": self.Success,
+            "error": self.Error,
+            "message": self.Message
+        }
+
+    def __str__(self):
+        return json.dumps(self.to_json(), sort_keys=True, indent=2)
+
+
 class C2GetDebugOutputMessage:
     """Try to get debug output from subprocess running internal server code
 
     Attributes:
         Name (str): Name of the C2 Profile
 
     Functions:
@@ -866,14 +1015,18 @@
     Functions:
         opsec
 
         config_check
 
         redirect_rules
 
+        get_ioc
+
+        sample_message
+
     """
 
     async def opsec(self, inputMsg: C2OPSECMessage) -> C2OPSECMessageResponse:
         """Check payload's C2 configuration for OPSEC issues
 
         :param inputMsg: Payload's C2 Profile configuration
         :return: C2OPSECMessageResponse detailing the results of the OPSEC check
@@ -901,14 +1054,35 @@
         :return: C2GetRedirectorRulesMessageResponse detailing some Apache ModRewrite rules for the payload
         """
         response = C2GetRedirectorRulesMessageResponse(Success=True)
         response.Message = "Not Implemented"
         response.Message += f"\nInput: {json.dumps(inputMsg.to_json(), indent=4)}"
         return response
 
+    async def get_ioc(self, inputMsg: C2GetIOCMessage) -> C2GetIOCMessageResponse:
+        """Generate IOCs for the network traffic associated with the specified c2 configuration
+
+        :param inputMsg: Payload's C2 Profile configuration
+        :return: C2GetIOCMessageResponse detailing some IOCs
+        """
+        response = C2GetIOCMessageResponse(Success=True)
+        response.IOCs = []
+        return response
+
+    async def sample_message(self, inputMsg: C2SampleMessageMessage) -> C2SampleMessageMessageResponse:
+        """Generate a sample message for this c2 profile based on the configuration specified
+
+        :param inputMsg: Payload's C2 Profile configuration
+        :return: C2SampleMessageMessageResponse detailing a sample message
+        """
+        response = C2SampleMessageMessageResponse(Success=True)
+        response.Message = "Not Implemented"
+        response.Message += f"\nInput: {json.dumps(inputMsg.to_json(), indent=4)}"
+        return response
+
     custom_rpc_functions: dict[
         str, Callable[[C2OtherServiceRPCMessage], Awaitable[C2OtherServiceRPCMessageResponse]]] = {}
     server_folder_path: pathlib.Path
     server_binary_path: pathlib.Path
 
     @property
     @abstractmethod
```

### Comparing `mythic_container-0.2.8rc5/mythic_container/LoggingBase.py` & `mythic_container-0.2.9/mythic_container/LoggingBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicCommandBase.py` & `mythic_container-0.2.9/mythic_container/MythicCommandBase.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,20 +566,22 @@
     """
     manual_args: str = None
 
     def __init__(self,
                  command_line: str = "",
                  tasking_location: str = "command_line",
                  raw_command_line: str = "",
-                 task_dictionary: dict = {}):
+                 task_dictionary: dict = {},
+                 initial_parameter_group: str = ""):
         self.command_line = str(command_line)
         self.tasking_location = tasking_location
         self.raw_command_line = raw_command_line
         self.task_dictionary = task_dictionary
         self.parameter_group_name = None
+        self.initial_parameter_group = initial_parameter_group
 
     @property
     def args(self) -> list[CommandParameter]:
         return self._args
 
     @args.setter
     def args(self, args):
@@ -709,14 +711,16 @@
                                 has_all_values = False
                 if has_all_values:
                     finalMatchingGroupNames.append(groupNameOption)
             if len(finalMatchingGroupNames) == 0:
                 raise ValueError(
                     f"Supplied Arguments, {suppliedArgNames}, match more than one parameter group, {groupNameOptions}, and all require at least one more value from the user")
             elif len(finalMatchingGroupNames) > 1:
+                if self.initial_parameter_group in finalMatchingGroupNames:
+                    return self.initial_parameter_group
                 raise ValueError(
                     f"Supplied Arguments, {suppliedArgNames}, match more than one parameter group, {finalMatchingGroupNames}")
             else:
                 return finalMatchingGroupNames[0]
         else:
             return groupNameOptions[0]
 
@@ -834,31 +838,28 @@
     def to_json(self, base_path: Path):
         try:
             code_file = (
                     base_path
                     / "{}.js".format(self.script_name)
             )
             if code_file.exists():
-                code = code_file.read_bytes()
-                code = base64.b64encode(code).decode()
+                code = code_file.read_bytes().decode()
+                #code = base64.b64encode(code).decode()
                 return {"script": code, "name": self.script_name, "author": self.author}
             elif Path(self.script_name).exists():
-                code = Path(self.script_name).read_bytes()
-                code = base64.b64encode(code).decode()
+                code = Path(self.script_name).read_bytes().decode()
+                #code = base64.b64encode(code).decode()
                 return {"script": code, "name": self.script_name, "author": self.author}
             else:
                 raise Exception(
                     "Code for Browser Script, " + self.script_name + ", does not exist on disk at path: " + str(
                         code_file))
         except Exception as e:
             raise e
 
-    def __str__(self):
-        return json.dumps(self.to_json(), sort_keys=True, indent=2)
-
 
 class MythicTask:
     """Instance of Mythic Tasking used with `create_tasking`. Use `create_go_tasking` instead.
 
     Deprecated
     """
 
@@ -1498,15 +1499,16 @@
         self.PayloadType = payload_type
         self.BuildParameters = [MythicRPCPayloadConfigurationBuildParameter(**x) for x in build_parameters]
         self.C2Profiles = [MythicRPCPayloadConfigurationC2Profile(**x) for x in c2info]
         if args is not None:
             self.args = args(command_line=task["params"],
                              tasking_location=task["tasking_location"],
                              raw_command_line=task["original_params"],
-                             task_dictionary=task, )
+                             task_dictionary=task,
+                             initial_parameter_group=task["parameter_group_name"])
         else:
             self.args = args
         for k, v in kwargs.items():
             logger.info(f"unknown kwarg {k} with value {v}")
 
     def to_json(self):
         return {
```

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/__init__.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/__init__.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,31 +9,34 @@
     def __init__(self,
                  AgentFileID: str,
                  Comment: str = None,
                  Filename: str = None,
                  AppendContents: bytes = None,
                  ReplaceContents: bytes = None,
                  Delete: bool = None,
+                 DeleteAfterFetch: bool = None,
                  **kwargs):
         self.AgentFileID = AgentFileID
         self.Filename = Filename
         self.Comment = Comment
         self.AppendContents = AppendContents
         self.ReplaceContents = ReplaceContents
         self.Delete = Delete
+        self.DeleteAfterFetch = DeleteAfterFetch
         for k, v in kwargs.items():
             logger.info(f"Unknown kwarg {k} - {v}")
 
     def to_json(self):
         return {
             "file_id": self.AgentFileID,
             "filename": self.Filename,
             "comment": self.Comment,
             "append_contents": self.AppendContents,
-            "delete": self.Delete
+            "delete": self.Delete,
+            "delete_after_fetch": self.DeleteAfterFetch
         }
 
 
 class MythicRPCFileUpdateMessageResponse:
     def __init__(self,
                  success: bool = False,
                  error: str = "",
```

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py` & `mythic_container-0.2.9/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/MythicRPC.py` & `mythic_container-0.2.9/mythic_container/MythicRPC.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/PayloadBuilder.py` & `mythic_container-0.2.9/mythic_container/PayloadBuilder.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/TranslationBase.py` & `mythic_container-0.2.9/mythic_container/TranslationBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/WebhookBase.py` & `mythic_container-0.2.9/mythic_container/WebhookBase.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/__init__.py` & `mythic_container-0.2.9/mythic_container/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .rabbitmq import rabbitmqConnectionClass
 from .mythic_service import start_and_run_forever, test_command
 
-containerVersion = "v1.0.6"
+containerVersion = "v1.0.7"
 
-PyPi_version = "0.2.8-rc05"
+PyPi_version = "0.2.9"
 
 RabbitmqConnection = rabbitmqConnectionClass()
 
 MYTHIC_RPC_OTHER_SERVICES_RPC = "mythic_rpc_other_service_rpc"
 PAYLOAD_BUILD_C2_ROUTING_KEY = "payload_c2_build"
 # payload routes
 PT_SYNC_ROUTING_KEY = "pt_sync"
@@ -27,14 +27,16 @@
 PT_TASK_PROCESS_RESPONSE = "pt_task_process_response"
 PT_TASK_PROCESS_RESPONSE_RESPONSE = "pt_task_process_response_response"
 # c2 routes
 C2_SYNC_ROUTING_KEY = "c2_sync"
 C2_RPC_RESYNC_ROUTING_KEY = "c2_rpc_resync"
 C2_RPC_OPSEC_CHECKS_ROUTING_KEY = "c2_rpc_opsec_check"
 C2_RPC_CONFIG_CHECK_ROUTING_KEY = "c2_rpc_config_check"
+C2_RPC_GET_IOC_ROUTING_KEY = "c2_rpc_get_ioc"
+C2_RPC_SAMPLE_MESSAGE_ROUTING_KEY = "c2_rpc_sample_message"
 C2_RPC_REDIRECTOR_RULES_ROUTING_KEY = "c2_rpc_redirector_rules"
 C2_RPC_START_SERVER_ROUTING_KEY = "c2_rpc_start_server"
 C2_RPC_STOP_SERVER_ROUTING_KEY = "c2_rpc_stop_server"
 C2_RPC_GET_SERVER_DEBUG_OUTPUT = "c2_rpc_get_server_debug_output"
 C2_RPC_GET_AVAILABLE_UI_FUNCTIONS = "c2_rpc_get_ui_functions"
 C2_RPC_GET_FILE = "c2_rpc_get_file"
 C2_RPC_REMOVE_FILE = "c2_rpc_remove_file"
```

### Comparing `mythic_container-0.2.8rc5/mythic_container/agent_utils.py` & `mythic_container-0.2.9/mythic_container/agent_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
     try:
         task = MythicCommandBase.MythicTask(
             message_json["task"],
             args=command_class.argument_class(
                 command_line=message_json["task"]["params"],
                 tasking_location=message_json["task"]["tasking_location"],
                 raw_command_line=message_json["task"]["original_params"],
+                initial_parameter_group=message_json["task"]["parameter_group_name"],
                 task_dictionary=message_json["task"],
             ),
             callback_info=message_json["callback"]
         )
         # if tasking came from the command_line or an unknown source, call parse_arguments to deal with unknown text
         if task.args.tasking_location == "command_line":
             await task.args.parse_arguments()
```

### Comparing `mythic_container-0.2.8rc5/mythic_container/c2_utils.py` & `mythic_container-0.2.9/mythic_container/c2_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -131,14 +131,110 @@
         response = mythic_container.C2ProfileBase.C2ConfigCheckMessageResponse(
             Success=False,
             Error=f"Hit exception trying to call config check function function: {traceback.format_exc()}\n{e}"
         )
         return ujson.dumps(response.to_json()).encode()
 
 
+async def getIOC(msg: bytes) -> bytes:
+    try:
+        msgDict = ujson.loads(msg)
+        for name, c2 in mythic_container.C2ProfileBase.c2Profiles.items():
+            if c2.name == msgDict["c2_profile_name"]:
+                if callable(c2.get_ioc):
+                    try:
+                        result = await c2.config_check(mythic_container.C2ProfileBase.C2GetIOCMessage(**msgDict))
+                    except Exception as callEx:
+                        logger.exception(
+                            f"Failed to call get_ioc for {c2.name}")
+                        response = mythic_container.C2ProfileBase.C2GetIOCMessageResponse(
+                            Success=False,
+                            Error=f"Failed to call config check function: {traceback.format_exc()}\n{callEx}"
+                        )
+                        return ujson.dumps(response.to_json()).encode()
+                    if result is None:
+                        response = mythic_container.C2ProfileBase.C2GetIOCMessageResponse(
+                            Success=False,
+                            Error=f"Failed to call config check function: No result returned"
+                        )
+                        return ujson.dumps(response.to_json()).encode()
+                    elif isinstance(result, dict):
+                        response = mythic_container.C2ProfileBase.C2GetIOCMessageResponse(**result)
+                        return ujson.dumps(response).encode()
+                    elif isinstance(result, mythic_container.C2ProfileBase.C2GetIOCMessageResponse):
+                        return ujson.dumps(result.to_json()).encode()
+                    else:
+                        response = mythic_container.C2ProfileBase.C2GetIOCMessageResponse(
+                            Success=False,
+                            Error=f"unknown result type from function: {result}"
+                        )
+                        return ujson.dumps(response.to_json()).encode()
+                else:
+                    logger.error(f"get_ioc function for {c2.name} isn't callable")
+                    response = mythic_container.C2ProfileBase.C2GetIOCMessageResponse(
+                        Success=False,
+                        Error=f"get ioc function for {c2.name} isn't callable"
+                    )
+                    return ujson.dumps(response.to_json()).encode()
+    except Exception as e:
+        response = mythic_container.C2ProfileBase.C2GetIOCMessageResponse(
+            Success=False,
+            Error=f"Hit exception trying to call get_ioc function: {traceback.format_exc()}\n{e}"
+        )
+        return ujson.dumps(response.to_json()).encode()
+
+
+async def sampleMessage(msg: bytes) -> bytes:
+    try:
+        msgDict = ujson.loads(msg)
+        for name, c2 in mythic_container.C2ProfileBase.c2Profiles.items():
+            if c2.name == msgDict["c2_profile_name"]:
+                if callable(c2.sample_message):
+                    try:
+                        result = await c2.config_check(mythic_container.C2ProfileBase.C2SampleMessageMessage(**msgDict))
+                    except Exception as callEx:
+                        logger.exception(
+                            f"Failed to call get_ioc for {c2.name}")
+                        response = mythic_container.C2ProfileBase.C2SampleMessageMessageResponse(
+                            Success=False,
+                            Error=f"Failed to call sample_message function: {traceback.format_exc()}\n{callEx}"
+                        )
+                        return ujson.dumps(response.to_json()).encode()
+                    if result is None:
+                        response = mythic_container.C2ProfileBase.C2SampleMessageMessageResponse(
+                            Success=False,
+                            Error=f"Failed to call sample message function: No result returned"
+                        )
+                        return ujson.dumps(response.to_json()).encode()
+                    elif isinstance(result, dict):
+                        response = mythic_container.C2ProfileBase.C2SampleMessageMessageResponse(**result)
+                        return ujson.dumps(response).encode()
+                    elif isinstance(result, mythic_container.C2ProfileBase.C2SampleMessageMessageResponse):
+                        return ujson.dumps(result.to_json()).encode()
+                    else:
+                        response = mythic_container.C2ProfileBase.C2SampleMessageMessageResponse(
+                            Success=False,
+                            Error=f"unknown result type from function: {result}"
+                        )
+                        return ujson.dumps(response.to_json()).encode()
+                else:
+                    logger.error(f"sample_message function for {c2.name} isn't callable")
+                    response = mythic_container.C2ProfileBase.C2SampleMessageMessageResponse(
+                        Success=False,
+                        Error=f"sample message function for {c2.name} isn't callable"
+                    )
+                    return ujson.dumps(response.to_json()).encode()
+    except Exception as e:
+        response = mythic_container.C2ProfileBase.C2SampleMessageMessageResponse(
+            Success=False,
+            Error=f"Hit exception trying to call sample_message function: {traceback.format_exc()}\n{e}"
+        )
+        return ujson.dumps(response.to_json()).encode()
+
+
 async def getDebugOutput(msg: bytes) -> bytes:
     try:
         msgDict = ujson.loads(msg)
         for name, c2 in mythic_container.C2ProfileBase.c2Profiles.items():
             if c2.name == msgDict["c2_profile_name"]:
                 if mythic_container.C2ProfileBase.runningServers[c2.name]["process"] is not None:
                     if mythic_container.C2ProfileBase.runningServers[c2.name]["process"].returncode is None:
```

### Comparing `mythic_container-0.2.8rc5/mythic_container/grpc/translationContainerGRPC_pb2.py` & `mythic_container-0.2.9/mythic_container/grpc/translationContainerGRPC_pb2.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py` & `mythic_container-0.2.9/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/logging.py` & `mythic_container-0.2.9/mythic_container/logging.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/logging_utils.py` & `mythic_container-0.2.9/mythic_container/logging_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/mythic_service.py` & `mythic_container-0.2.9/mythic_container/mythic_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,24 @@
         handler=c2_utils.customRPCFunction
     )))
     payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromRPCQueue(
         queue=getRoutingKey(c2.name, mythic_container.C2_RPC_RESYNC_ROUTING_KEY),
         routing_key=getRoutingKey(c2.name, mythic_container.C2_RPC_RESYNC_ROUTING_KEY),
         handler=c2_utils.reSyncC2Profile
     )))
+    payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromRPCQueue(
+        queue=getRoutingKey(c2.name, mythic_container.C2_RPC_GET_IOC_ROUTING_KEY),
+        routing_key=getRoutingKey(c2.name, mythic_container.C2_RPC_GET_IOC_ROUTING_KEY),
+        handler=c2_utils.getIOC
+    )))
+    payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromRPCQueue(
+        queue=getRoutingKey(c2.name, mythic_container.C2_RPC_SAMPLE_MESSAGE_ROUTING_KEY),
+        routing_key=getRoutingKey(c2.name, mythic_container.C2_RPC_SAMPLE_MESSAGE_ROUTING_KEY),
+        handler=c2_utils.sampleMessage
+    )))
 
 
 async def syncC2ProfileData(c2: C2ProfileBase.C2Profile) -> None:
     syncMessage = {
         **c2.to_json(),
         "container_version": mythic_container.containerVersion
     }
```

### Comparing `mythic_container-0.2.8rc5/mythic_container/rabbitmq.py` & `mythic_container-0.2.9/mythic_container/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/utils_mythic_file_transfer.py` & `mythic_container-0.2.9/mythic_container/utils_mythic_file_transfer.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container/webhook_utils.py` & `mythic_container-0.2.9/mythic_container/webhook_utils.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/mythic_container.egg-info/PKG-INFO` & `mythic_container-0.2.9/mythic_container.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic-container
-Version: 0.2.8rc5
+Version: 0.2.9
 Summary: Functionality for Mythic Services
 Home-page: https://docs.mythic-c2.net/customizing/payload-type-development
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mythic_container-0.2.8rc5/mythic_container.egg-info/SOURCES.txt` & `mythic_container-0.2.9/mythic_container.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.8rc5/setup.py` & `mythic_container-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="mythic_container",
-    version="0.2.8-rc05",
+    version="0.2.9",
     description="Functionality for Mythic Services",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://docs.mythic-c2.net/customizing/payload-type-development",
     author="@its_a_feature_",
     author_email="",
     license="BSD3",
```

