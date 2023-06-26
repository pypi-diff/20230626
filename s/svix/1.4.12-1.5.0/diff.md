# Comparing `tmp/svix-1.4.12.tar.gz` & `tmp/svix-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svix-1.4.12.tar", last modified: Thu Jun  1 17:47:31 2023, max compression
+gzip compressed data, was "svix-1.5.0.tar", last modified: Mon Jun 26 13:26:11 2023, max compression
```

## Comparing `svix-1.4.12.tar` & `svix-1.5.0.tar`

### file list

```diff
@@ -1,262 +1,262 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.479306 svix-1.4.12/
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-01 17:47:31.479306 svix-1.4.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-01 17:46:54.000000 svix-1.4.12/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-01 17:46:54.000000 svix-1.4.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 17:47:31.479306 svix-1.4.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-01 17:46:54.000000 svix-1.4.12/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.455306 svix-1.4.12/svix/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-01 17:46:54.000000 svix-1.4.12/svix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40067 2023-06-01 17:46:54.000000 svix-1.4.12/svix/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-01 17:46:54.000000 svix-1.4.12/svix/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.455306 svix-1.4.12/svix/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.455306 svix-1.4.12/svix/internal/openapi_client/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.455306 svix-1.4.12/svix/internal/openapi_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.455306 svix-1.4.12/svix/internal/openapi_client/api/application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/api/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/application/get_app_usage_stats_api_v1_app_stats_usage_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/application/patch_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/application/v1_application_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/application/v1_application_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/application/v1_application_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/application/v1_application_get_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/application/v1_application_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/application/v1_application_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.455306 svix-1.4.12/svix/internal/openapi_client/api/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/api/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/authentication/v1_authentication_app_portal_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/authentication/v1_authentication_dashboard_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/authentication/v1_authentication_exchange_one_time_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/authentication/v1_authentication_expire_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/authentication/v1_authentication_logout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.455306 svix-1.4.12/svix/internal/openapi_client/api/background_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/api/background_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/background_tasks/get_background_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/background_tasks/list_background_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.459306 svix-1.4.12/svix/internal/openapi_client/api/broadcast/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/api/broadcast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/broadcast/create_broadcast_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.459306 svix-1.4.12/svix/internal/openapi_client/api/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/api/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/endpoint/patch_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_get_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_get_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-06-01 17:47:26.000000 svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_get_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_patch_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_recover.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_rotate_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_send_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_transformation_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_transformation_partial_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_transformation_simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_update_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.459306 svix-1.4.12/svix/internal/openapi_client/api/environment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/api/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/environment/v1_environment_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/environment/v1_environment_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.459306 svix-1.4.12/svix/internal/openapi_client/api/environment_settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/api/environment_settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/environment_settings/v1_environment_get_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.459306 svix-1.4.12/svix/internal/openapi_client/api/event_type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/api/event_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/event_type/patch_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/event_type/v1_event_type_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/event_type/v1_event_type_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/event_type/v1_event_type_generate_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/event_type/v1_event_type_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     7622 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/event_type/v1_event_type_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/event_type/v1_event_type_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.459306 svix-1.4.12/svix/internal/openapi_client/api/health/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/api/health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/health/v1_health_get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.463306 svix-1.4.12/svix/internal/openapi_client/api/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/api/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/integration/v1_integration_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/integration/v1_integration_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/integration/v1_integration_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/integration/v1_integration_get_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/integration/v1_integration_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-01 17:47:27.000000 svix-1.4.12/svix/internal/openapi_client/api/integration/v1_integration_rotate_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/api/integration/v1_integration_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.463306 svix-1.4.12/svix/internal/openapi_client/api/message/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/api/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/api/message/create_message_attempt_for_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/api/message/v1_message_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/api/message/v1_message_expunge_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/api/message/v1_message_get.py
--rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/api/message/v1_message_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.463306 svix-1.4.12/svix/internal/openapi_client/api/message_attempt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/api/message_attempt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_expunge_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_get_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_attempted_destinations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_attempted_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    13122 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_by_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12824 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_by_endpoint_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_by_msg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14242 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_by_msg_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_resend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.463306 svix-1.4.12/svix/internal/openapi_client/api/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/api/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/api/statistics/calculate_aggregate_app_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/api/statistics/v1_stats_app_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/api/statistics/v1_stats_endpoint_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.479306 svix-1.4.12/svix/internal/openapi_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/models/app_portal_access_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-01 17:47:28.000000 svix-1.4.12/svix/internal/openapi_client/models/app_portal_access_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/app_usage_stats_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/app_usage_stats_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/application_in.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/application_in_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/application_out.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/application_out_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/application_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/application_patch_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/application_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/application_token_expire_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/attempt_statistics_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/attempt_statistics_response.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/background_task_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/background_task_out.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-01 17:47:25.000000 svix-1.4.12/svix/internal/openapi_client/models/background_task_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-01 17:47:25.000000 svix-1.4.12/svix/internal/openapi_client/models/background_task_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/border_radius_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-01 17:47:25.000000 svix-1.4.12/svix/internal/openapi_client/models/border_radius_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/custom_color_palette.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/custom_theme_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/dashboard_access_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_created_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_created_event_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-01 17:47:25.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_created_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_deleted_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_deleted_event_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-01 17:47:25.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_deleted_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_disabled_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_disabled_event_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-01 17:47:25.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_disabled_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_headers_in.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_headers_in_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_headers_out.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_headers_out_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_headers_patch_in.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_headers_patch_in_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_in.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_in_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_message_out.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_message_out_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_out.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_out_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_patch_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_secret_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_secret_rotate_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_transformation_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_transformation_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_transformation_simulate_in.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_transformation_simulate_in_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_transformation_simulate_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_update.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_update_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_updated_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_updated_event_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-01 17:47:25.000000 svix-1.4.12/svix/internal/openapi_client/models/endpoint_updated_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/environment_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/environment_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/environment_settings_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/event_example_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/event_type_example_out.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/event_type_example_out_example.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/event_type_example_out_example_additional_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/event_type_in.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/event_type_in_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/event_type_in_schemas_additional_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/event_type_out.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/event_type_out_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/event_type_out_schemas_additional_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/event_type_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/event_type_patch_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/event_type_patch_schemas_additional_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-01 17:47:29.000000 svix-1.4.12/svix/internal/openapi_client/models/event_type_schema_in.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/event_type_schema_in_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/event_type_update.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/event_type_update_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/event_type_update_schemas_additional_property.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/export_environment_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/font_size_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/http_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/integration_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/integration_key_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/integration_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/integration_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/list_response_application_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/list_response_application_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/list_response_background_task_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/list_response_endpoint_message_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/list_response_endpoint_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/list_response_event_type_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/list_response_integration_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/list_response_message_attempt_endpoint_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/list_response_message_attempt_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/list_response_message_endpoint_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/list_response_message_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/message_attempt_endpoint_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/message_attempt_exhausted_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/message_attempt_exhausted_event_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-01 17:47:25.000000 svix-1.4.12/svix/internal/openapi_client/models/message_attempt_exhausted_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/message_attempt_failed_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/message_attempt_failing_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/message_attempt_failing_event_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-01 17:47:25.000000 svix-1.4.12/svix/internal/openapi_client/models/message_attempt_failing_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/message_attempt_headers_out.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/message_attempt_headers_out_sent_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/message_attempt_out.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-01 17:47:25.000000 svix-1.4.12/svix/internal/openapi_client/models/message_attempt_trigger_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/message_broadcast_in.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/message_broadcast_in_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/message_broadcast_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/message_endpoint_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/message_in.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/message_in_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/message_out.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/models/message_out_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-01 17:47:25.000000 svix-1.4.12/svix/internal/openapi_client/models/message_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/one_time_token_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/one_time_token_out.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-01 17:47:25.000000 svix-1.4.12/svix/internal/openapi_client/models/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/recover_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/recover_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/replay_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/replay_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/settings_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/settings_out.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-01 17:47:25.000000 svix-1.4.12/svix/internal/openapi_client/models/statistics_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-01 17:47:25.000000 svix-1.4.12/svix/internal/openapi_client/models/status_code_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-01 17:47:25.000000 svix-1.4.12/svix/internal/openapi_client/models/transformation_http_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 17:47:18.000000 svix-1.4.12/svix/internal/openapi_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-01 17:47:30.000000 svix-1.4.12/svix/internal/openapi_client/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:46:54.000000 svix-1.4.12/svix/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-01 17:46:54.000000 svix-1.4.12/svix/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.455306 svix-1.4.12/svix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-01 17:47:31.000000 svix-1.4.12/svix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14904 2023-06-01 17:47:31.000000 svix-1.4.12/svix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:47:31.000000 svix-1.4.12/svix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:47:01.000000 svix-1.4.12/svix.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-01 17:47:31.000000 svix-1.4.12/svix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 17:47:31.000000 svix-1.4.12/svix.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:47:31.479306 svix-1.4.12/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-01 17:46:54.000000 svix-1.4.12/tests/test_webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.449876 svix-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-26 13:26:11.449876 svix-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-26 13:25:14.000000 svix-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-26 13:25:14.000000 svix-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-26 13:26:11.449876 svix-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-26 13:25:14.000000 svix-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.413876 svix-1.5.0/svix/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-26 13:25:14.000000 svix-1.5.0/svix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-06-26 13:25:14.000000 svix-1.5.0/svix/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-26 13:25:14.000000 svix-1.5.0/svix/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.413876 svix-1.5.0/svix/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.417876 svix-1.5.0/svix/internal/openapi_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-26 13:26:03.000000 svix-1.5.0/svix/internal/openapi_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.417876 svix-1.5.0/svix/internal/openapi_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-26 13:25:53.000000 svix-1.5.0/svix/internal/openapi_client/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.417876 svix-1.5.0/svix/internal/openapi_client/api/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:53.000000 svix-1.5.0/svix/internal/openapi_client/api/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-06-26 13:26:03.000000 svix-1.5.0/svix/internal/openapi_client/api/application/get_app_usage_stats_api_v1_app_stats_usage_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-26 13:26:03.000000 svix-1.5.0/svix/internal/openapi_client/api/application/patch_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-06-26 13:26:03.000000 svix-1.5.0/svix/internal/openapi_client/api/application/v1_application_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-26 13:26:03.000000 svix-1.5.0/svix/internal/openapi_client/api/application/v1_application_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-06-26 13:26:03.000000 svix-1.5.0/svix/internal/openapi_client/api/application/v1_application_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-06-26 13:26:03.000000 svix-1.5.0/svix/internal/openapi_client/api/application/v1_application_get_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-06-26 13:26:03.000000 svix-1.5.0/svix/internal/openapi_client/api/application/v1_application_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-26 13:26:03.000000 svix-1.5.0/svix/internal/openapi_client/api/application/v1_application_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.417876 svix-1.5.0/svix/internal/openapi_client/api/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:53.000000 svix-1.5.0/svix/internal/openapi_client/api/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-06-26 13:26:03.000000 svix-1.5.0/svix/internal/openapi_client/api/authentication/v1_authentication_app_portal_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-26 13:26:03.000000 svix-1.5.0/svix/internal/openapi_client/api/authentication/v1_authentication_dashboard_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-26 13:26:03.000000 svix-1.5.0/svix/internal/openapi_client/api/authentication/v1_authentication_exchange_one_time_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-06-26 13:26:03.000000 svix-1.5.0/svix/internal/openapi_client/api/authentication/v1_authentication_expire_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-06-26 13:26:03.000000 svix-1.5.0/svix/internal/openapi_client/api/authentication/v1_authentication_logout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.417876 svix-1.5.0/svix/internal/openapi_client/api/background_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:53.000000 svix-1.5.0/svix/internal/openapi_client/api/background_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-06-26 13:26:04.000000 svix-1.5.0/svix/internal/openapi_client/api/background_tasks/get_background_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-06-26 13:26:04.000000 svix-1.5.0/svix/internal/openapi_client/api/background_tasks/list_background_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.417876 svix-1.5.0/svix/internal/openapi_client/api/broadcast/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:53.000000 svix-1.5.0/svix/internal/openapi_client/api/broadcast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-26 13:26:04.000000 svix-1.5.0/svix/internal/openapi_client/api/broadcast/create_broadcast_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.421876 svix-1.5.0/svix/internal/openapi_client/api/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:53.000000 svix-1.5.0/svix/internal/openapi_client/api/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-26 13:26:04.000000 svix-1.5.0/svix/internal/openapi_client/api/endpoint/patch_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-06-26 13:26:04.000000 svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-06-26 13:26:04.000000 svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-26 13:26:04.000000 svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-06-26 13:26:04.000000 svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_get_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-26 13:26:04.000000 svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-06-26 13:26:04.000000 svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_get_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-06-26 13:26:04.000000 svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-06-26 13:26:04.000000 svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_patch_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-06-26 13:26:04.000000 svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_recover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-06-26 13:26:04.000000 svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-06-26 13:26:04.000000 svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_rotate_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-06-26 13:26:04.000000 svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_send_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-26 13:26:04.000000 svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_transformation_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-06-26 13:26:05.000000 svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_transformation_partial_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-06-26 13:26:05.000000 svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_transformation_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-06-26 13:26:05.000000 svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-06-26 13:26:05.000000 svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_update_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.421876 svix-1.5.0/svix/internal/openapi_client/api/environment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:53.000000 svix-1.5.0/svix/internal/openapi_client/api/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-06-26 13:26:05.000000 svix-1.5.0/svix/internal/openapi_client/api/environment/v1_environment_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-26 13:26:05.000000 svix-1.5.0/svix/internal/openapi_client/api/environment/v1_environment_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.421876 svix-1.5.0/svix/internal/openapi_client/api/environment_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:53.000000 svix-1.5.0/svix/internal/openapi_client/api/environment_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-26 13:26:05.000000 svix-1.5.0/svix/internal/openapi_client/api/environment_settings/v1_environment_get_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.425876 svix-1.5.0/svix/internal/openapi_client/api/event_type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:53.000000 svix-1.5.0/svix/internal/openapi_client/api/event_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-06-26 13:26:05.000000 svix-1.5.0/svix/internal/openapi_client/api/event_type/patch_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-06-26 13:26:05.000000 svix-1.5.0/svix/internal/openapi_client/api/event_type/v1_event_type_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-06-26 13:26:05.000000 svix-1.5.0/svix/internal/openapi_client/api/event_type/v1_event_type_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-06-26 13:26:05.000000 svix-1.5.0/svix/internal/openapi_client/api/event_type/v1_event_type_generate_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-06-26 13:26:05.000000 svix-1.5.0/svix/internal/openapi_client/api/event_type/v1_event_type_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-06-26 13:26:05.000000 svix-1.5.0/svix/internal/openapi_client/api/event_type/v1_event_type_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-26 13:26:05.000000 svix-1.5.0/svix/internal/openapi_client/api/event_type/v1_event_type_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.425876 svix-1.5.0/svix/internal/openapi_client/api/health/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:53.000000 svix-1.5.0/svix/internal/openapi_client/api/health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-06-26 13:26:05.000000 svix-1.5.0/svix/internal/openapi_client/api/health/v1_health_get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.425876 svix-1.5.0/svix/internal/openapi_client/api/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:53.000000 svix-1.5.0/svix/internal/openapi_client/api/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-06-26 13:26:05.000000 svix-1.5.0/svix/internal/openapi_client/api/integration/v1_integration_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-26 13:26:06.000000 svix-1.5.0/svix/internal/openapi_client/api/integration/v1_integration_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-26 13:26:06.000000 svix-1.5.0/svix/internal/openapi_client/api/integration/v1_integration_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-06-26 13:26:06.000000 svix-1.5.0/svix/internal/openapi_client/api/integration/v1_integration_get_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-26 13:26:06.000000 svix-1.5.0/svix/internal/openapi_client/api/integration/v1_integration_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-06-26 13:26:06.000000 svix-1.5.0/svix/internal/openapi_client/api/integration/v1_integration_rotate_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-06-26 13:26:06.000000 svix-1.5.0/svix/internal/openapi_client/api/integration/v1_integration_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.425876 svix-1.5.0/svix/internal/openapi_client/api/message/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:53.000000 svix-1.5.0/svix/internal/openapi_client/api/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-06-26 13:26:06.000000 svix-1.5.0/svix/internal/openapi_client/api/message/create_message_attempt_for_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11909 2023-06-26 13:26:06.000000 svix-1.5.0/svix/internal/openapi_client/api/message/v1_message_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-06-26 13:26:06.000000 svix-1.5.0/svix/internal/openapi_client/api/message/v1_message_expunge_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-26 13:26:06.000000 svix-1.5.0/svix/internal/openapi_client/api/message/v1_message_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-06-26 13:26:06.000000 svix-1.5.0/svix/internal/openapi_client/api/message/v1_message_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.429876 svix-1.5.0/svix/internal/openapi_client/api/message_attempt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:53.000000 svix-1.5.0/svix/internal/openapi_client/api/message_attempt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7309 2023-06-26 13:26:06.000000 svix-1.5.0/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_expunge_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-06-26 13:26:06.000000 svix-1.5.0/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-06-26 13:26:06.000000 svix-1.5.0/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_get_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-06-26 13:26:07.000000 svix-1.5.0/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_attempted_destinations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-06-26 13:26:07.000000 svix-1.5.0/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_attempted_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14790 2023-06-26 13:26:07.000000 svix-1.5.0/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_by_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-06-26 13:26:07.000000 svix-1.5.0/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_by_endpoint_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-06-26 13:26:07.000000 svix-1.5.0/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_by_msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15918 2023-06-26 13:26:07.000000 svix-1.5.0/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_by_msg_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-06-26 13:26:07.000000 svix-1.5.0/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_resend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.429876 svix-1.5.0/svix/internal/openapi_client/api/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:53.000000 svix-1.5.0/svix/internal/openapi_client/api/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-06-26 13:26:07.000000 svix-1.5.0/svix/internal/openapi_client/api/statistics/calculate_aggregate_app_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-06-26 13:26:07.000000 svix-1.5.0/svix/internal/openapi_client/api/statistics/v1_stats_app_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-06-26 13:26:07.000000 svix-1.5.0/svix/internal/openapi_client/api/statistics/v1_stats_endpoint_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-26 13:26:07.000000 svix-1.5.0/svix/internal/openapi_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-26 13:26:07.000000 svix-1.5.0/svix/internal/openapi_client/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.449876 svix-1.5.0/svix/internal/openapi_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-06-26 13:25:53.000000 svix-1.5.0/svix/internal/openapi_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-26 13:26:07.000000 svix-1.5.0/svix/internal/openapi_client/models/app_portal_access_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-26 13:26:07.000000 svix-1.5.0/svix/internal/openapi_client/models/app_portal_access_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-26 13:26:07.000000 svix-1.5.0/svix/internal/openapi_client/models/app_usage_stats_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-26 13:26:07.000000 svix-1.5.0/svix/internal/openapi_client/models/app_usage_stats_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/application_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 13:26:01.000000 svix-1.5.0/svix/internal/openapi_client/models/application_in_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/application_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 13:26:01.000000 svix-1.5.0/svix/internal/openapi_client/models/application_out_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/application_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-26 13:26:01.000000 svix-1.5.0/svix/internal/openapi_client/models/application_patch_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/application_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/application_token_expire_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/attempt_statistics_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/attempt_statistics_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-26 13:25:59.000000 svix-1.5.0/svix/internal/openapi_client/models/background_task_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/background_task_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-26 13:26:02.000000 svix-1.5.0/svix/internal/openapi_client/models/background_task_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-26 13:26:02.000000 svix-1.5.0/svix/internal/openapi_client/models/background_task_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/border_radius_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-26 13:26:02.000000 svix-1.5.0/svix/internal/openapi_client/models/border_radius_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/custom_color_palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/custom_theme_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/dashboard_access_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_created_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_created_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-26 13:26:02.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_created_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_deleted_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_deleted_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-26 13:26:02.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_deleted_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_disabled_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_disabled_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-26 13:26:02.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_disabled_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_headers_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-26 13:25:59.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_headers_in_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_headers_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-26 13:25:59.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_headers_out_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_headers_patch_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-26 13:26:01.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_headers_patch_in_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-26 13:26:00.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_in_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_message_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-26 13:25:59.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_message_out_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 13:26:01.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_out_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 13:26:01.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_patch_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_secret_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_secret_rotate_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_transformation_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_transformation_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_transformation_simulate_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-26 13:26:01.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_transformation_simulate_in_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-26 13:26:08.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_transformation_simulate_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 13:25:59.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_update_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_updated_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_updated_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-26 13:26:02.000000 svix-1.5.0/svix/internal/openapi_client/models/endpoint_updated_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/environment_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/environment_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/environment_settings_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/event_example_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/event_type_example_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-26 13:26:01.000000 svix-1.5.0/svix/internal/openapi_client/models/event_type_example_out_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-26 13:26:01.000000 svix-1.5.0/svix/internal/openapi_client/models/event_type_example_out_example_additional_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/event_type_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-26 13:26:01.000000 svix-1.5.0/svix/internal/openapi_client/models/event_type_in_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-26 13:26:00.000000 svix-1.5.0/svix/internal/openapi_client/models/event_type_in_schemas_additional_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/event_type_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 13:26:00.000000 svix-1.5.0/svix/internal/openapi_client/models/event_type_out_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-26 13:26:01.000000 svix-1.5.0/svix/internal/openapi_client/models/event_type_out_schemas_additional_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/event_type_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-26 13:26:00.000000 svix-1.5.0/svix/internal/openapi_client/models/event_type_patch_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-26 13:26:00.000000 svix-1.5.0/svix/internal/openapi_client/models/event_type_patch_schemas_additional_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/event_type_schema_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-26 13:25:59.000000 svix-1.5.0/svix/internal/openapi_client/models/event_type_schema_in_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/event_type_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 13:26:00.000000 svix-1.5.0/svix/internal/openapi_client/models/event_type_update_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-26 13:26:01.000000 svix-1.5.0/svix/internal/openapi_client/models/event_type_update_schemas_additional_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-26 13:26:01.000000 svix-1.5.0/svix/internal/openapi_client/models/export_environment_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/font_size_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/integration_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/integration_key_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/integration_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/integration_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/list_response_application_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/list_response_application_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/list_response_background_task_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/list_response_endpoint_message_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/list_response_endpoint_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/list_response_event_type_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/list_response_integration_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/list_response_message_attempt_endpoint_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/list_response_message_attempt_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/list_response_message_endpoint_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/list_response_message_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-26 13:26:09.000000 svix-1.5.0/svix/internal/openapi_client/models/message_attempt_endpoint_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/message_attempt_exhausted_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/message_attempt_exhausted_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-26 13:26:02.000000 svix-1.5.0/svix/internal/openapi_client/models/message_attempt_exhausted_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/message_attempt_failed_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/message_attempt_failing_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/message_attempt_failing_event_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-26 13:26:02.000000 svix-1.5.0/svix/internal/openapi_client/models/message_attempt_failing_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/message_attempt_headers_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-26 13:26:00.000000 svix-1.5.0/svix/internal/openapi_client/models/message_attempt_headers_out_sent_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/message_attempt_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-26 13:26:02.000000 svix-1.5.0/svix/internal/openapi_client/models/message_attempt_trigger_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/message_broadcast_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-26 13:26:00.000000 svix-1.5.0/svix/internal/openapi_client/models/message_broadcast_in_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/message_broadcast_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/message_endpoint_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/message_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 13:25:59.000000 svix-1.5.0/svix/internal/openapi_client/models/message_in_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/message_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-26 13:25:59.000000 svix-1.5.0/svix/internal/openapi_client/models/message_out_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-26 13:26:02.000000 svix-1.5.0/svix/internal/openapi_client/models/message_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/one_time_token_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/one_time_token_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-26 13:26:02.000000 svix-1.5.0/svix/internal/openapi_client/models/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/recover_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/recover_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/replay_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/replay_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/settings_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/settings_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-26 13:26:02.000000 svix-1.5.0/svix/internal/openapi_client/models/statistics_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-26 13:26:02.000000 svix-1.5.0/svix/internal/openapi_client/models/status_code_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-26 13:26:02.000000 svix-1.5.0/svix/internal/openapi_client/models/transformation_http_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 13:25:53.000000 svix-1.5.0/svix/internal/openapi_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-26 13:26:10.000000 svix-1.5.0/svix/internal/openapi_client/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 13:25:14.000000 svix-1.5.0/svix/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-26 13:25:14.000000 svix-1.5.0/svix/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.413876 svix-1.5.0/svix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-26 13:26:11.000000 svix-1.5.0/svix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14904 2023-06-26 13:26:11.000000 svix-1.5.0/svix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:26:11.000000 svix-1.5.0/svix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 13:25:24.000000 svix-1.5.0/svix.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 13:26:11.000000 svix-1.5.0/svix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 13:26:11.000000 svix-1.5.0/svix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 13:26:11.449876 svix-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-26 13:25:14.000000 svix-1.5.0/tests/test_webhooks.py
```

### Comparing `svix-1.4.12/README.md` & `svix-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `svix-1.4.12/setup.py` & `svix-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `svix-1.4.12/svix/__init__.py` & `svix-1.5.0/svix/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,8 +33,8 @@
     "Svix",
     "SvixAsync",
     "SvixOptions",
     "Webhook",
     "WebhookVerificationError",
 ]
 
-__version__ = "1.4.12"
+__version__ = "1.5.0"
```

### Comparing `svix-1.4.12/svix/api.py` & `svix-1.5.0/svix/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -989,14 +989,16 @@
         host = options.server_url or regional_url or DEFAULT_SERVER_URL
         client = AuthenticatedClient(
             base_url=host,
             token=auth_token,
             headers={"user-agent": f"svix-libs/{__version__}/python"},
             verify_ssl=True,
             timeout=15,
+            follow_redirects=False,
+            raise_on_unexpected_status=True,
         )
         self._client = client
 
 
 class SvixAsync(ClientBase):
     @property
     def authentication(self) -> AuthenticationAsync:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/application/get_app_usage_stats_api_v1_app_stats_usage_get.py` & `svix-1.5.0/svix/internal/openapi_client/api/application/get_app_usage_stats_api_v1_app_stats_usage_get.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.list_response_application_stats import ListResponseApplicationStats
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
     since: datetime.datetime,
     until: datetime.datetime,
@@ -43,87 +47,98 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> ListResponseApplicationStats:
+def _parse_response(*, client: Client, response: httpx.Response) -> ListResponseApplicationStats:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ListResponseApplicationStats.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = ListResponseApplicationStats.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ListResponseApplicationStats]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
     since: datetime.datetime,
     until: datetime.datetime,
     limit: Union[Unset, None, int] = 50,
     iterator: Union[Unset, None, str] = UNSET,
-) -> ListResponseApplicationStats:
+) -> Response[ListResponseApplicationStats]:
     """Get App Usage Stats
 
      Get basic statistics for all applications.
 
     Args:
         since (datetime.datetime):
         until (datetime.datetime):
         limit (Union[Unset, None, int]):  Default: 50.
         iterator (Union[Unset, None, str]): The app's ID Example: app_1srOrx2ZWZBpBUvZwXKQmoEYga2.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseApplicationStats
+        Response[ListResponseApplicationStats]
     """
 
     kwargs = _get_kwargs(
         client=client,
         since=since,
         until=until,
         limit=limit,
         iterator=iterator,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
     since: datetime.datetime,
     until: datetime.datetime,
@@ -136,72 +151,77 @@
 
     Args:
         since (datetime.datetime):
         until (datetime.datetime):
         limit (Union[Unset, None, int]):  Default: 50.
         iterator (Union[Unset, None, str]): The app's ID Example: app_1srOrx2ZWZBpBUvZwXKQmoEYga2.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseApplicationStats
     """
 
     return sync_detailed(
         client=client,
         since=since,
         until=until,
         limit=limit,
         iterator=iterator,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
     since: datetime.datetime,
     until: datetime.datetime,
     limit: Union[Unset, None, int] = 50,
     iterator: Union[Unset, None, str] = UNSET,
-) -> ListResponseApplicationStats:
+) -> Response[ListResponseApplicationStats]:
     """Get App Usage Stats
 
      Get basic statistics for all applications.
 
     Args:
         since (datetime.datetime):
         until (datetime.datetime):
         limit (Union[Unset, None, int]):  Default: 50.
         iterator (Union[Unset, None, str]): The app's ID Example: app_1srOrx2ZWZBpBUvZwXKQmoEYga2.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseApplicationStats
+        Response[ListResponseApplicationStats]
     """
 
     kwargs = _get_kwargs(
         client=client,
         since=since,
         until=until,
         limit=limit,
         iterator=iterator,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
     since: datetime.datetime,
     until: datetime.datetime,
@@ -214,18 +234,24 @@
 
     Args:
         since (datetime.datetime):
         until (datetime.datetime):
         limit (Union[Unset, None, int]):  Default: 50.
         iterator (Union[Unset, None, str]): The app's ID Example: app_1srOrx2ZWZBpBUvZwXKQmoEYga2.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseApplicationStats
     """
 
-    return await asyncio_detailed(
-        client=client,
-        since=since,
-        until=until,
-        limit=limit,
-        iterator=iterator,
-    )
+    return (
+        await asyncio_detailed(
+            client=client,
+            since=since,
+            until=until,
+            limit=limit,
+            iterator=iterator,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/application/patch_application.py` & `svix-1.5.0/svix/internal/openapi_client/api/application/v1_application_delete.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,191 +1,199 @@
 import random
 from http import HTTPStatus
 from time import sleep
-from typing import Any, Dict
+from typing import Any, Dict, cast
 
 import httpx
 
-from ...client import AuthenticatedClient
-from ...models.application_out import ApplicationOut
-from ...models.application_patch import ApplicationPatch
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: ApplicationPatch,
 ) -> Dict[str, Any]:
     url = "{}/api/v1/app/{app_id}/".format(client.base_url, app_id=app_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    json_json_body = json_body.to_dict()
-
     return {
-        "method": "patch",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "json": json_json_body,
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> ApplicationOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> Any:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = ApplicationOut.from_dict(response.json())
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
-    return response_200
 
-
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[None]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: ApplicationPatch,
-) -> ApplicationOut:
-    """Patch Application
+) -> Response[None]:
+    """Delete Application
 
-     Partially update an application.
+     Delete an application.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        json_body (ApplicationPatch):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApplicationOut
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         client=client,
-        json_body=json_body,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: ApplicationPatch,
-) -> ApplicationOut:
-    """Patch Application
+) -> None:
+    """Delete Application
 
-     Partially update an application.
+     Delete an application.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        json_body (ApplicationPatch):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApplicationOut
+        None
     """
 
     return sync_detailed(
         app_id=app_id,
         client=client,
-        json_body=json_body,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: ApplicationPatch,
-) -> ApplicationOut:
-    """Patch Application
+) -> Response[None]:
+    """Delete Application
 
-     Partially update an application.
+     Delete an application.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        json_body (ApplicationPatch):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApplicationOut
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         client=client,
-        json_body=json_body,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: ApplicationPatch,
-) -> ApplicationOut:
-    """Patch Application
+) -> None:
+    """Delete Application
 
-     Partially update an application.
+     Delete an application.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        json_body (ApplicationPatch):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApplicationOut
+        None
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        client=client,
-        json_body=json_body,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            client=client,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/application/v1_application_create.py` & `svix-1.5.0/svix/internal/openapi_client/api/application/v1_application_create.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.application_in import ApplicationIn
 from ...models.application_out import ApplicationOut
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
     json_body: ApplicationIn,
     get_if_exists: Union[Unset, None, bool] = False,
@@ -37,86 +41,101 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> ApplicationOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> ApplicationOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ApplicationOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.CREATED:
+        response_201 = ApplicationOut.from_dict(response.json())
+
+        return response_201
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = ApplicationOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApplicationOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
     json_body: ApplicationIn,
     get_if_exists: Union[Unset, None, bool] = False,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> ApplicationOut:
+) -> Response[ApplicationOut]:
     """Create Application
 
      Create a new application.
 
     Args:
         get_if_exists (Union[Unset, None, bool]): Get an existing application, or create a new one
             if doesn't exist. It's two separate functions in the libs.
         idempotency_key (Union[Unset, str]):
         json_body (ApplicationIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ApplicationOut
+        Response[ApplicationOut]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
         get_if_exists=get_if_exists,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
     json_body: ApplicationIn,
     get_if_exists: Union[Unset, None, bool] = False,
@@ -128,69 +147,74 @@
 
     Args:
         get_if_exists (Union[Unset, None, bool]): Get an existing application, or create a new one
             if doesn't exist. It's two separate functions in the libs.
         idempotency_key (Union[Unset, str]):
         json_body (ApplicationIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ApplicationOut
     """
 
     return sync_detailed(
         client=client,
         json_body=json_body,
         get_if_exists=get_if_exists,
         idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
     json_body: ApplicationIn,
     get_if_exists: Union[Unset, None, bool] = False,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> ApplicationOut:
+) -> Response[ApplicationOut]:
     """Create Application
 
      Create a new application.
 
     Args:
         get_if_exists (Union[Unset, None, bool]): Get an existing application, or create a new one
             if doesn't exist. It's two separate functions in the libs.
         idempotency_key (Union[Unset, str]):
         json_body (ApplicationIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ApplicationOut
+        Response[ApplicationOut]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
         get_if_exists=get_if_exists,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
     json_body: ApplicationIn,
     get_if_exists: Union[Unset, None, bool] = False,
@@ -202,17 +226,23 @@
 
     Args:
         get_if_exists (Union[Unset, None, bool]): Get an existing application, or create a new one
             if doesn't exist. It's two separate functions in the libs.
         idempotency_key (Union[Unset, str]):
         json_body (ApplicationIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ApplicationOut
     """
 
-    return await asyncio_detailed(
-        client=client,
-        json_body=json_body,
-        get_if_exists=get_if_exists,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            client=client,
+            json_body=json_body,
+            get_if_exists=get_if_exists,
+            idempotency_key=idempotency_key,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/application/v1_application_delete.py` & `svix-1.5.0/svix/internal/openapi_client/api/health/v1_health_get.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,172 +1,178 @@
 import random
 from http import HTTPStatus
 from time import sleep
-from typing import Any, Dict
+from typing import Any, Dict, cast
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
-    app_id: str,
     *,
-    client: AuthenticatedClient,
+    client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/app/{app_id}/".format(client.base_url, app_id=app_id)
+    url = "{}/api/v1/health/".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "delete",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> None:
+def _parse_response(*, client: Client, response: httpx.Response) -> Any:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_204 = None
-    return response_204
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[None]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
-    app_id: str,
     *,
-    client: AuthenticatedClient,
-) -> None:
-    """Delete Application
-
-     Delete an application.
-
-    Args:
-        app_id (str): The app's ID or UID Example: unique-app-identifier.
+    client: Client,
+) -> Response[None]:
+    """Health
+
+     Verify the API server is up and running.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        None
+        Response[None]
     """
 
     kwargs = _get_kwargs(
-        app_id=app_id,
         client=client,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
-    app_id: str,
     *,
-    client: AuthenticatedClient,
+    client: Client,
 ) -> None:
-    """Delete Application
+    """Health
 
-     Delete an application.
+     Verify the API server is up and running.
 
-    Args:
-        app_id (str): The app's ID or UID Example: unique-app-identifier.
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         None
     """
 
     return sync_detailed(
-        app_id=app_id,
         client=client,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
-    app_id: str,
     *,
-    client: AuthenticatedClient,
-) -> None:
-    """Delete Application
-
-     Delete an application.
-
-    Args:
-        app_id (str): The app's ID or UID Example: unique-app-identifier.
+    client: Client,
+) -> Response[None]:
+    """Health
+
+     Verify the API server is up and running.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        None
+        Response[None]
     """
 
     kwargs = _get_kwargs(
-        app_id=app_id,
         client=client,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    app_id: str,
     *,
-    client: AuthenticatedClient,
+    client: Client,
 ) -> None:
-    """Delete Application
+    """Health
 
-     Delete an application.
+     Verify the API server is up and running.
 
-    Args:
-        app_id (str): The app's ID or UID Example: unique-app-identifier.
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         None
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        client=client,
-    )
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/application/v1_application_get.py` & `svix-1.5.0/svix/internal/openapi_client/api/background_tasks/get_background_task.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,174 +1,201 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict
 
 import httpx
 
-from ...client import AuthenticatedClient
-from ...models.application_out import ApplicationOut
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.background_task_out import BackgroundTaskOut
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
-    app_id: str,
+    task_id: str,
     *,
     client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/app/{app_id}/".format(client.base_url, app_id=app_id)
+    url = "{}/api/v1/background-task/{task_id}/".format(client.base_url, task_id=task_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> ApplicationOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> BackgroundTaskOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = BackgroundTaskOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = ApplicationOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[BackgroundTaskOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
-    app_id: str,
+    task_id: str,
     *,
     client: AuthenticatedClient,
-) -> ApplicationOut:
-    """Get Application
+) -> Response[BackgroundTaskOut]:
+    """Get Background Task
 
-     Get an application.
+     Get a background task by ID.
 
     Args:
-        app_id (str): The app's ID or UID Example: unique-app-identifier.
+        task_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApplicationOut
+        Response[BackgroundTaskOut]
     """
 
     kwargs = _get_kwargs(
-        app_id=app_id,
+        task_id=task_id,
         client=client,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
-    app_id: str,
+    task_id: str,
     *,
     client: AuthenticatedClient,
-) -> ApplicationOut:
-    """Get Application
+) -> BackgroundTaskOut:
+    """Get Background Task
 
-     Get an application.
+     Get a background task by ID.
 
     Args:
-        app_id (str): The app's ID or UID Example: unique-app-identifier.
+        task_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApplicationOut
+        BackgroundTaskOut
     """
 
     return sync_detailed(
-        app_id=app_id,
+        task_id=task_id,
         client=client,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
-    app_id: str,
+    task_id: str,
     *,
     client: AuthenticatedClient,
-) -> ApplicationOut:
-    """Get Application
+) -> Response[BackgroundTaskOut]:
+    """Get Background Task
 
-     Get an application.
+     Get a background task by ID.
 
     Args:
-        app_id (str): The app's ID or UID Example: unique-app-identifier.
+        task_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApplicationOut
+        Response[BackgroundTaskOut]
     """
 
     kwargs = _get_kwargs(
-        app_id=app_id,
+        task_id=task_id,
         client=client,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    app_id: str,
+    task_id: str,
     *,
     client: AuthenticatedClient,
-) -> ApplicationOut:
-    """Get Application
+) -> BackgroundTaskOut:
+    """Get Background Task
 
-     Get an application.
+     Get a background task by ID.
 
     Args:
-        app_id (str): The app's ID or UID Example: unique-app-identifier.
+        task_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApplicationOut
+        BackgroundTaskOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        client=client,
-    )
+    return (
+        await asyncio_detailed(
+            task_id=task_id,
+            client=client,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/application/v1_application_get_stats.py` & `svix-1.5.0/svix/internal/openapi_client/api/application/v1_application_get_stats.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.application_stats import ApplicationStats
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET
+from ...types import UNSET, Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     *,
     client: AuthenticatedClient,
     since: datetime.datetime,
@@ -38,84 +42,95 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> ApplicationStats:
+def _parse_response(*, client: Client, response: httpx.Response) -> ApplicationStats:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ApplicationStats.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = ApplicationStats.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApplicationStats]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     *,
     client: AuthenticatedClient,
     since: datetime.datetime,
     until: datetime.datetime,
-) -> ApplicationStats:
+) -> Response[ApplicationStats]:
     """Get App Stats
 
      Get basic statistics for the application
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         since (datetime.datetime):
         until (datetime.datetime):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ApplicationStats
+        Response[ApplicationStats]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         client=client,
         since=since,
         until=until,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     *,
     client: AuthenticatedClient,
     since: datetime.datetime,
@@ -126,68 +141,73 @@
      Get basic statistics for the application
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         since (datetime.datetime):
         until (datetime.datetime):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ApplicationStats
     """
 
     return sync_detailed(
         app_id=app_id,
         client=client,
         since=since,
         until=until,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     *,
     client: AuthenticatedClient,
     since: datetime.datetime,
     until: datetime.datetime,
-) -> ApplicationStats:
+) -> Response[ApplicationStats]:
     """Get App Stats
 
      Get basic statistics for the application
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         since (datetime.datetime):
         until (datetime.datetime):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ApplicationStats
+        Response[ApplicationStats]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         client=client,
         since=since,
         until=until,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     *,
     client: AuthenticatedClient,
     since: datetime.datetime,
@@ -198,17 +218,23 @@
      Get basic statistics for the application
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         since (datetime.datetime):
         until (datetime.datetime):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ApplicationStats
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        client=client,
-        since=since,
-        until=until,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            client=client,
+            since=since,
+            until=until,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/application/v1_application_list.py` & `svix-1.5.0/svix/internal/openapi_client/api/application/v1_application_list.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.list_response_application_out import ListResponseApplicationOut
 from ...models.ordering import Ordering
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
@@ -40,84 +44,95 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> ListResponseApplicationOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> ListResponseApplicationOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ListResponseApplicationOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = ListResponseApplicationOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ListResponseApplicationOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     order: Union[Unset, None, Ordering] = UNSET,
-) -> ListResponseApplicationOut:
+) -> Response[ListResponseApplicationOut]:
     """List Applications
 
      List of all the organization's applications.
 
     Args:
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The app's ID Example: app_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         order (Union[Unset, None, Ordering]): Defines the ordering in a listing of results.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseApplicationOut
+        Response[ListResponseApplicationOut]
     """
 
     kwargs = _get_kwargs(
         client=client,
         limit=limit,
         iterator=iterator,
         order=order,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
@@ -128,68 +143,73 @@
      List of all the organization's applications.
 
     Args:
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The app's ID Example: app_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         order (Union[Unset, None, Ordering]): Defines the ordering in a listing of results.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseApplicationOut
     """
 
     return sync_detailed(
         client=client,
         limit=limit,
         iterator=iterator,
         order=order,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     order: Union[Unset, None, Ordering] = UNSET,
-) -> ListResponseApplicationOut:
+) -> Response[ListResponseApplicationOut]:
     """List Applications
 
      List of all the organization's applications.
 
     Args:
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The app's ID Example: app_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         order (Union[Unset, None, Ordering]): Defines the ordering in a listing of results.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseApplicationOut
+        Response[ListResponseApplicationOut]
     """
 
     kwargs = _get_kwargs(
         client=client,
         limit=limit,
         iterator=iterator,
         order=order,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
@@ -200,17 +220,23 @@
      List of all the organization's applications.
 
     Args:
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The app's ID Example: app_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         order (Union[Unset, None, Ordering]): Defines the ordering in a listing of results.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseApplicationOut
     """
 
-    return await asyncio_detailed(
-        client=client,
-        limit=limit,
-        iterator=iterator,
-        order=order,
-    )
+    return (
+        await asyncio_detailed(
+            client=client,
+            limit=limit,
+            iterator=iterator,
+            order=order,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/authentication/v1_authentication_app_portal_access.py` & `svix-1.5.0/svix/internal/openapi_client/api/authentication/v1_authentication_app_portal_access.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.app_portal_access_in import AppPortalAccessIn
 from ...models.app_portal_access_out import AppPortalAccessOut
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     *,
     client: AuthenticatedClient,
     json_body: AppPortalAccessIn,
@@ -32,85 +36,96 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> AppPortalAccessOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> AppPortalAccessOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = AppPortalAccessOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = AppPortalAccessOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[AppPortalAccessOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     *,
     client: AuthenticatedClient,
     json_body: AppPortalAccessIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> AppPortalAccessOut:
+) -> Response[AppPortalAccessOut]:
     """Get Consumer App Portal Access
 
      Use this function to get magic links (and authentication codes) for connecting your users to the
     Consumer Application Portal.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (AppPortalAccessIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        AppPortalAccessOut
+        Response[AppPortalAccessOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     *,
     client: AuthenticatedClient,
     json_body: AppPortalAccessIn,
@@ -122,69 +137,74 @@
     Consumer Application Portal.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (AppPortalAccessIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         AppPortalAccessOut
     """
 
     return sync_detailed(
         app_id=app_id,
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     *,
     client: AuthenticatedClient,
     json_body: AppPortalAccessIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> AppPortalAccessOut:
+) -> Response[AppPortalAccessOut]:
     """Get Consumer App Portal Access
 
      Use this function to get magic links (and authentication codes) for connecting your users to the
     Consumer Application Portal.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (AppPortalAccessIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        AppPortalAccessOut
+        Response[AppPortalAccessOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     *,
     client: AuthenticatedClient,
     json_body: AppPortalAccessIn,
@@ -196,17 +216,23 @@
     Consumer Application Portal.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (AppPortalAccessIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         AppPortalAccessOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            client=client,
+            json_body=json_body,
+            idempotency_key=idempotency_key,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/authentication/v1_authentication_dashboard_access.py` & `svix-1.5.0/svix/internal/openapi_client/api/integration/v1_integration_create.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,203 +1,234 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
-from ...models.dashboard_access_out import DashboardAccessOut
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Unset
+from ...models.integration_in import IntegrationIn
+from ...models.integration_out import IntegrationOut
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     *,
     client: AuthenticatedClient,
+    json_body: IntegrationIn,
     idempotency_key: Union[Unset, str] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/auth/dashboard-access/{app_id}/".format(client.base_url, app_id=app_id)
+    url = "{}/api/v1/app/{app_id}/integration/".format(client.base_url, app_id=app_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     if not isinstance(idempotency_key, Unset):
         headers["idempotency-key"] = idempotency_key
 
+    json_json_body = json_body.to_dict()
+
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> DashboardAccessOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> IntegrationOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = IntegrationOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = DashboardAccessOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[IntegrationOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     *,
     client: AuthenticatedClient,
+    json_body: IntegrationIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> DashboardAccessOut:
-    """Dashboard Access
-
-     DEPRECATED: Please use `app-portal-access` instead.
+) -> Response[IntegrationOut]:
+    """Create Integration
 
-    Use this function to get magic links (and authentication codes) for connecting your users to the
-    Consumer Application Portal.
+     Create an integration.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         idempotency_key (Union[Unset, str]):
+        json_body (IntegrationIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        DashboardAccessOut
+        Response[IntegrationOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         client=client,
+        json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     *,
     client: AuthenticatedClient,
+    json_body: IntegrationIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> DashboardAccessOut:
-    """Dashboard Access
-
-     DEPRECATED: Please use `app-portal-access` instead.
+) -> IntegrationOut:
+    """Create Integration
 
-    Use this function to get magic links (and authentication codes) for connecting your users to the
-    Consumer Application Portal.
+     Create an integration.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         idempotency_key (Union[Unset, str]):
+        json_body (IntegrationIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        DashboardAccessOut
+        IntegrationOut
     """
 
     return sync_detailed(
         app_id=app_id,
         client=client,
+        json_body=json_body,
         idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     *,
     client: AuthenticatedClient,
+    json_body: IntegrationIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> DashboardAccessOut:
-    """Dashboard Access
+) -> Response[IntegrationOut]:
+    """Create Integration
 
-     DEPRECATED: Please use `app-portal-access` instead.
-
-    Use this function to get magic links (and authentication codes) for connecting your users to the
-    Consumer Application Portal.
+     Create an integration.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         idempotency_key (Union[Unset, str]):
+        json_body (IntegrationIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        DashboardAccessOut
+        Response[IntegrationOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         client=client,
+        json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     *,
     client: AuthenticatedClient,
+    json_body: IntegrationIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> DashboardAccessOut:
-    """Dashboard Access
-
-     DEPRECATED: Please use `app-portal-access` instead.
+) -> IntegrationOut:
+    """Create Integration
 
-    Use this function to get magic links (and authentication codes) for connecting your users to the
-    Consumer Application Portal.
+     Create an integration.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         idempotency_key (Union[Unset, str]):
+        json_body (IntegrationIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        DashboardAccessOut
+        IntegrationOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        client=client,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            client=client,
+            json_body=json_body,
+            idempotency_key=idempotency_key,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/authentication/v1_authentication_exchange_one_time_token.py` & `svix-1.5.0/svix/internal/openapi_client/api/authentication/v1_authentication_exchange_one_time_token.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.one_time_token_in import OneTimeTokenIn
 from ...models.one_time_token_out import OneTimeTokenOut
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
     json_body: OneTimeTokenIn,
     idempotency_key: Union[Unset, str] = UNSET,
@@ -31,81 +35,92 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> OneTimeTokenOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> OneTimeTokenOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = OneTimeTokenOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = OneTimeTokenOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[OneTimeTokenOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
     json_body: OneTimeTokenIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> OneTimeTokenOut:
+) -> Response[OneTimeTokenOut]:
     """Exchange One Time Token
 
      This is a one time token
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (OneTimeTokenIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        OneTimeTokenOut
+        Response[OneTimeTokenOut]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
     json_body: OneTimeTokenIn,
     idempotency_key: Union[Unset, str] = UNSET,
@@ -114,64 +129,69 @@
 
      This is a one time token
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (OneTimeTokenIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         OneTimeTokenOut
     """
 
     return sync_detailed(
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
     json_body: OneTimeTokenIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> OneTimeTokenOut:
+) -> Response[OneTimeTokenOut]:
     """Exchange One Time Token
 
      This is a one time token
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (OneTimeTokenIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        OneTimeTokenOut
+        Response[OneTimeTokenOut]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
     json_body: OneTimeTokenIn,
     idempotency_key: Union[Unset, str] = UNSET,
@@ -180,16 +200,22 @@
 
      This is a one time token
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (OneTimeTokenIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         OneTimeTokenOut
     """
 
-    return await asyncio_detailed(
-        client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            client=client,
+            json_body=json_body,
+            idempotency_key=idempotency_key,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/authentication/v1_authentication_expire_all.py` & `svix-1.5.0/svix/internal/openapi_client/api/application/v1_application_get.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,206 +1,201 @@
 import random
 from http import HTTPStatus
 from time import sleep
-from typing import Any, Dict, Union
+from typing import Any, Dict
 
 import httpx
 
-from ...client import AuthenticatedClient
-from ...models.application_token_expire_in import ApplicationTokenExpireIn
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.application_out import ApplicationOut
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Unset
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: ApplicationTokenExpireIn,
-    idempotency_key: Union[Unset, str] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/auth/app/{app_id}/expire-all/".format(client.base_url, app_id=app_id)
+    url = "{}/api/v1/app/{app_id}/".format(client.base_url, app_id=app_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    if not isinstance(idempotency_key, Unset):
-        headers["idempotency-key"] = idempotency_key
-
-    json_json_body = json_body.to_dict()
-
     return {
-        "method": "post",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "json": json_json_body,
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> None:
+def _parse_response(*, client: Client, response: httpx.Response) -> ApplicationOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ApplicationOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_204 = None
-    return response_204
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApplicationOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: ApplicationTokenExpireIn,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> None:
-    """Expire All
+) -> Response[ApplicationOut]:
+    """Get Application
 
-     Expire all of the tokens associated with a specific Application
+     Get an application.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        idempotency_key (Union[Unset, str]):
-        json_body (ApplicationTokenExpireIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        None
+        Response[ApplicationOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: ApplicationTokenExpireIn,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> None:
-    """Expire All
+) -> ApplicationOut:
+    """Get Application
 
-     Expire all of the tokens associated with a specific Application
+     Get an application.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        idempotency_key (Union[Unset, str]):
-        json_body (ApplicationTokenExpireIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        None
+        ApplicationOut
     """
 
     return sync_detailed(
         app_id=app_id,
         client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: ApplicationTokenExpireIn,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> None:
-    """Expire All
+) -> Response[ApplicationOut]:
+    """Get Application
 
-     Expire all of the tokens associated with a specific Application
+     Get an application.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        idempotency_key (Union[Unset, str]):
-        json_body (ApplicationTokenExpireIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        None
+        Response[ApplicationOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: ApplicationTokenExpireIn,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> None:
-    """Expire All
+) -> ApplicationOut:
+    """Get Application
 
-     Expire all of the tokens associated with a specific Application
+     Get an application.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        idempotency_key (Union[Unset, str]):
-        json_body (ApplicationTokenExpireIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        None
+        ApplicationOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            client=client,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/background_tasks/list_background_tasks.py` & `svix-1.5.0/svix/internal/openapi_client/api/background_tasks/list_background_tasks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.background_task_status import BackgroundTaskStatus
 from ...models.background_task_type import BackgroundTaskType
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.list_response_background_task_out import ListResponseBackgroundTaskOut
 from ...models.ordering import Ordering
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
     status: Union[Unset, None, BackgroundTaskStatus] = UNSET,
     task: Union[Unset, None, BackgroundTaskType] = UNSET,
@@ -56,90 +60,101 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> ListResponseBackgroundTaskOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> ListResponseBackgroundTaskOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ListResponseBackgroundTaskOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = ListResponseBackgroundTaskOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ListResponseBackgroundTaskOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
     status: Union[Unset, None, BackgroundTaskStatus] = UNSET,
     task: Union[Unset, None, BackgroundTaskType] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     order: Union[Unset, None, Ordering] = UNSET,
-) -> ListResponseBackgroundTaskOut:
+) -> Response[ListResponseBackgroundTaskOut]:
     """List Background Tasks
 
      List background tasks executed in the past 90 days.
 
     Args:
         status (Union[Unset, None, BackgroundTaskStatus]):
         task (Union[Unset, None, BackgroundTaskType]):
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]):
         order (Union[Unset, None, Ordering]): Defines the ordering in a listing of results.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseBackgroundTaskOut
+        Response[ListResponseBackgroundTaskOut]
     """
 
     kwargs = _get_kwargs(
         client=client,
         status=status,
         task=task,
         limit=limit,
         iterator=iterator,
         order=order,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
     status: Union[Unset, None, BackgroundTaskStatus] = UNSET,
     task: Union[Unset, None, BackgroundTaskType] = UNSET,
@@ -154,76 +169,81 @@
     Args:
         status (Union[Unset, None, BackgroundTaskStatus]):
         task (Union[Unset, None, BackgroundTaskType]):
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]):
         order (Union[Unset, None, Ordering]): Defines the ordering in a listing of results.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseBackgroundTaskOut
     """
 
     return sync_detailed(
         client=client,
         status=status,
         task=task,
         limit=limit,
         iterator=iterator,
         order=order,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
     status: Union[Unset, None, BackgroundTaskStatus] = UNSET,
     task: Union[Unset, None, BackgroundTaskType] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     order: Union[Unset, None, Ordering] = UNSET,
-) -> ListResponseBackgroundTaskOut:
+) -> Response[ListResponseBackgroundTaskOut]:
     """List Background Tasks
 
      List background tasks executed in the past 90 days.
 
     Args:
         status (Union[Unset, None, BackgroundTaskStatus]):
         task (Union[Unset, None, BackgroundTaskType]):
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]):
         order (Union[Unset, None, Ordering]): Defines the ordering in a listing of results.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseBackgroundTaskOut
+        Response[ListResponseBackgroundTaskOut]
     """
 
     kwargs = _get_kwargs(
         client=client,
         status=status,
         task=task,
         limit=limit,
         iterator=iterator,
         order=order,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
     status: Union[Unset, None, BackgroundTaskStatus] = UNSET,
     task: Union[Unset, None, BackgroundTaskType] = UNSET,
@@ -238,19 +258,25 @@
     Args:
         status (Union[Unset, None, BackgroundTaskStatus]):
         task (Union[Unset, None, BackgroundTaskType]):
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]):
         order (Union[Unset, None, Ordering]): Defines the ordering in a listing of results.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseBackgroundTaskOut
     """
 
-    return await asyncio_detailed(
-        client=client,
-        status=status,
-        task=task,
-        limit=limit,
-        iterator=iterator,
-        order=order,
-    )
+    return (
+        await asyncio_detailed(
+            client=client,
+            status=status,
+            task=task,
+            limit=limit,
+            iterator=iterator,
+            order=order,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/broadcast/create_broadcast_message.py` & `svix-1.5.0/svix/internal/openapi_client/api/broadcast/create_broadcast_message.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_broadcast_in import MessageBroadcastIn
 from ...models.message_broadcast_out import MessageBroadcastOut
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
     json_body: MessageBroadcastIn,
     idempotency_key: Union[Unset, str] = UNSET,
@@ -31,81 +35,92 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> MessageBroadcastOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> MessageBroadcastOut:
+    if response.status_code == HTTPStatus.ACCEPTED:
+        response_202 = MessageBroadcastOut.from_dict(response.json())
+
+        return response_202
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_202 = MessageBroadcastOut.from_dict(response.json())
-
-    return response_202
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[MessageBroadcastOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
     json_body: MessageBroadcastIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> MessageBroadcastOut:
+) -> Response[MessageBroadcastOut]:
     """Create Broadcast Message
 
      Creates a background task to send the same message to each application in your organization
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (MessageBroadcastIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        MessageBroadcastOut
+        Response[MessageBroadcastOut]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
     json_body: MessageBroadcastIn,
     idempotency_key: Union[Unset, str] = UNSET,
@@ -114,64 +129,69 @@
 
      Creates a background task to send the same message to each application in your organization
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (MessageBroadcastIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         MessageBroadcastOut
     """
 
     return sync_detailed(
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
     json_body: MessageBroadcastIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> MessageBroadcastOut:
+) -> Response[MessageBroadcastOut]:
     """Create Broadcast Message
 
      Creates a background task to send the same message to each application in your organization
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (MessageBroadcastIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        MessageBroadcastOut
+        Response[MessageBroadcastOut]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
     json_body: MessageBroadcastIn,
     idempotency_key: Union[Unset, str] = UNSET,
@@ -180,16 +200,22 @@
 
      Creates a background task to send the same message to each application in your organization
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (MessageBroadcastIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         MessageBroadcastOut
     """
 
-    return await asyncio_detailed(
-        client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            client=client,
+            json_body=json_body,
+            idempotency_key=idempotency_key,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/endpoint/patch_endpoint.py` & `svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_update.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,206 +1,237 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.endpoint_out import EndpointOut
-from ...models.endpoint_patch import EndpointPatch
+from ...models.endpoint_update import EndpointUpdate
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: EndpointPatch,
+    json_body: EndpointUpdate,
 ) -> Dict[str, Any]:
     url = "{}/api/v1/app/{app_id}/endpoint/{endpoint_id}/".format(
         client.base_url, app_id=app_id, endpoint_id=endpoint_id
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
-        "method": "patch",
+        "method": "put",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> EndpointOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> EndpointOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = EndpointOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.CREATED:
+        response_201 = EndpointOut.from_dict(response.json())
+
+        return response_201
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = EndpointOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[EndpointOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: EndpointPatch,
-) -> EndpointOut:
-    """Patch Endpoint
+    json_body: EndpointUpdate,
+) -> Response[EndpointOut]:
+    """Update Endpoint
 
-     Partially update an endpoint.
+     Update an endpoint.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
-        json_body (EndpointPatch):
+        json_body (EndpointUpdate):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        EndpointOut
+        Response[EndpointOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: EndpointPatch,
+    json_body: EndpointUpdate,
 ) -> EndpointOut:
-    """Patch Endpoint
+    """Update Endpoint
 
-     Partially update an endpoint.
+     Update an endpoint.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
-        json_body (EndpointPatch):
+        json_body (EndpointUpdate):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         EndpointOut
     """
 
     return sync_detailed(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: EndpointPatch,
-) -> EndpointOut:
-    """Patch Endpoint
+    json_body: EndpointUpdate,
+) -> Response[EndpointOut]:
+    """Update Endpoint
 
-     Partially update an endpoint.
+     Update an endpoint.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
-        json_body (EndpointPatch):
+        json_body (EndpointUpdate):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        EndpointOut
+        Response[EndpointOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: EndpointPatch,
+    json_body: EndpointUpdate,
 ) -> EndpointOut:
-    """Patch Endpoint
+    """Update Endpoint
 
-     Partially update an endpoint.
+     Update an endpoint.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
-        json_body (EndpointPatch):
+        json_body (EndpointUpdate):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         EndpointOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        endpoint_id=endpoint_id,
-        client=client,
-        json_body=json_body,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            endpoint_id=endpoint_id,
+            client=client,
+            json_body=json_body,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_create.py` & `svix-1.5.0/svix/internal/openapi_client/api/authentication/v1_authentication_logout.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,216 +1,210 @@
 import random
 from http import HTTPStatus
 from time import sleep
-from typing import Any, Dict, Union
+from typing import Any, Dict, Union, cast
 
 import httpx
 
-from ...client import AuthenticatedClient
-from ...models.endpoint_in import EndpointIn
-from ...models.endpoint_out import EndpointOut
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
-    app_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: EndpointIn,
     idempotency_key: Union[Unset, str] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/app/{app_id}/endpoint/".format(client.base_url, app_id=app_id)
+    url = "{}/api/v1/auth/logout/".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     if not isinstance(idempotency_key, Unset):
         headers["idempotency-key"] = idempotency_key
 
-    json_json_body = json_body.to_dict()
-
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "json": json_json_body,
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> EndpointOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> Any:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_201 = EndpointOut.from_dict(response.json())
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
-    return response_201
 
-
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[None]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
-    app_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: EndpointIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> EndpointOut:
-    """Create Endpoint
+) -> Response[None]:
+    """Logout
 
-     Create a new endpoint for the application.
+     Logout an app token.
 
-    When `secret` is `null` the secret is automatically generated (recommended)
+    Trying to log out other tokens will fail.
 
     Args:
-        app_id (str): The app's ID or UID Example: unique-app-identifier.
         idempotency_key (Union[Unset, str]):
-        json_body (EndpointIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        EndpointOut
+        Response[None]
     """
 
     kwargs = _get_kwargs(
-        app_id=app_id,
         client=client,
-        json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
-    app_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: EndpointIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> EndpointOut:
-    """Create Endpoint
+) -> None:
+    """Logout
 
-     Create a new endpoint for the application.
+     Logout an app token.
 
-    When `secret` is `null` the secret is automatically generated (recommended)
+    Trying to log out other tokens will fail.
 
     Args:
-        app_id (str): The app's ID or UID Example: unique-app-identifier.
         idempotency_key (Union[Unset, str]):
-        json_body (EndpointIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        EndpointOut
+        None
     """
 
     return sync_detailed(
-        app_id=app_id,
         client=client,
-        json_body=json_body,
         idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
-    app_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: EndpointIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> EndpointOut:
-    """Create Endpoint
+) -> Response[None]:
+    """Logout
 
-     Create a new endpoint for the application.
+     Logout an app token.
 
-    When `secret` is `null` the secret is automatically generated (recommended)
+    Trying to log out other tokens will fail.
 
     Args:
-        app_id (str): The app's ID or UID Example: unique-app-identifier.
         idempotency_key (Union[Unset, str]):
-        json_body (EndpointIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        EndpointOut
+        Response[None]
     """
 
     kwargs = _get_kwargs(
-        app_id=app_id,
         client=client,
-        json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    app_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: EndpointIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> EndpointOut:
-    """Create Endpoint
+) -> None:
+    """Logout
 
-     Create a new endpoint for the application.
+     Logout an app token.
 
-    When `secret` is `null` the secret is automatically generated (recommended)
+    Trying to log out other tokens will fail.
 
     Args:
-        app_id (str): The app's ID or UID Example: unique-app-identifier.
         idempotency_key (Union[Unset, str]):
-        json_body (EndpointIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        EndpointOut
+        None
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            client=client,
+            idempotency_key=idempotency_key,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_get_headers.py` & `svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_update_headers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,189 +1,231 @@
 import random
 from http import HTTPStatus
 from time import sleep
-from typing import Any, Dict
+from typing import Any, Dict, cast
 
 import httpx
 
-from ...client import AuthenticatedClient
-from ...models.endpoint_headers_out import EndpointHeadersOut
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.endpoint_headers_in import EndpointHeadersIn
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
+    json_body: EndpointHeadersIn,
 ) -> Dict[str, Any]:
     url = "{}/api/v1/app/{app_id}/endpoint/{endpoint_id}/headers/".format(
         client.base_url, app_id=app_id, endpoint_id=endpoint_id
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
+    json_json_body = json_body.to_dict()
+
     return {
-        "method": "get",
+        "method": "put",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> EndpointHeadersOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> Any:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = EndpointHeadersOut.from_dict(response.json())
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
-    return response_200
 
-
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[None]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-) -> EndpointHeadersOut:
-    """Get Endpoint Headers
+    json_body: EndpointHeadersIn,
+) -> Response[None]:
+    """Update Endpoint Headers
 
-     Get the additional headers to be sent with the webhook
+     Set the additional headers to be sent with the webhook
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
+        json_body (EndpointHeadersIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        EndpointHeadersOut
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
+        json_body=json_body,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-) -> EndpointHeadersOut:
-    """Get Endpoint Headers
+    json_body: EndpointHeadersIn,
+) -> None:
+    """Update Endpoint Headers
 
-     Get the additional headers to be sent with the webhook
+     Set the additional headers to be sent with the webhook
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
+        json_body (EndpointHeadersIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        EndpointHeadersOut
+        None
     """
 
     return sync_detailed(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
-    )
+        json_body=json_body,
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-) -> EndpointHeadersOut:
-    """Get Endpoint Headers
+    json_body: EndpointHeadersIn,
+) -> Response[None]:
+    """Update Endpoint Headers
 
-     Get the additional headers to be sent with the webhook
+     Set the additional headers to be sent with the webhook
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
+        json_body (EndpointHeadersIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        EndpointHeadersOut
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
+        json_body=json_body,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-) -> EndpointHeadersOut:
-    """Get Endpoint Headers
+    json_body: EndpointHeadersIn,
+) -> None:
+    """Update Endpoint Headers
 
-     Get the additional headers to be sent with the webhook
+     Set the additional headers to be sent with the webhook
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
+        json_body (EndpointHeadersIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        EndpointHeadersOut
+        None
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        endpoint_id=endpoint_id,
-        client=client,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            endpoint_id=endpoint_id,
+            client=client,
+            json_body=json_body,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_get_secret.py` & `svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_get.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,205 +1,216 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict
 
 import httpx
 
-from ...client import AuthenticatedClient
-from ...models.endpoint_secret_out import EndpointSecretOut
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.endpoint_out import EndpointOut
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/app/{app_id}/endpoint/{endpoint_id}/secret/".format(
+    url = "{}/api/v1/app/{app_id}/endpoint/{endpoint_id}/".format(
         client.base_url, app_id=app_id, endpoint_id=endpoint_id
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> EndpointSecretOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> EndpointOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = EndpointOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = EndpointSecretOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[EndpointOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-) -> EndpointSecretOut:
-    """Get Endpoint Secret
+) -> Response[EndpointOut]:
+    """Get Endpoint
 
-     Get the endpoint's signing secret.
-
-    This is used to verify the authenticity of the webhook.
-    For more information please refer to [the consuming webhooks docs](https://docs.svix.com/consuming-
-    webhooks/).
+     Get an endpoint.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        EndpointSecretOut
+        Response[EndpointOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-) -> EndpointSecretOut:
-    """Get Endpoint Secret
+) -> EndpointOut:
+    """Get Endpoint
 
-     Get the endpoint's signing secret.
-
-    This is used to verify the authenticity of the webhook.
-    For more information please refer to [the consuming webhooks docs](https://docs.svix.com/consuming-
-    webhooks/).
+     Get an endpoint.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        EndpointSecretOut
+        EndpointOut
     """
 
     return sync_detailed(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-) -> EndpointSecretOut:
-    """Get Endpoint Secret
-
-     Get the endpoint's signing secret.
+) -> Response[EndpointOut]:
+    """Get Endpoint
 
-    This is used to verify the authenticity of the webhook.
-    For more information please refer to [the consuming webhooks docs](https://docs.svix.com/consuming-
-    webhooks/).
+     Get an endpoint.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        EndpointSecretOut
+        Response[EndpointOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-) -> EndpointSecretOut:
-    """Get Endpoint Secret
-
-     Get the endpoint's signing secret.
+) -> EndpointOut:
+    """Get Endpoint
 
-    This is used to verify the authenticity of the webhook.
-    For more information please refer to [the consuming webhooks docs](https://docs.svix.com/consuming-
-    webhooks/).
+     Get an endpoint.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        EndpointSecretOut
+        EndpointOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        endpoint_id=endpoint_id,
-        client=client,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            endpoint_id=endpoint_id,
+            client=client,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_get_stats.py` & `svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_get_stats.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.endpoint_stats import EndpointStats
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -45,87 +49,98 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> EndpointStats:
+def _parse_response(*, client: Client, response: httpx.Response) -> EndpointStats:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = EndpointStats.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = EndpointStats.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[EndpointStats]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
     since: Union[Unset, None, datetime.datetime] = UNSET,
     until: Union[Unset, None, datetime.datetime] = UNSET,
-) -> EndpointStats:
+) -> Response[EndpointStats]:
     """Endpoint Stats
 
      Get basic statistics for the endpoint.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         since (Union[Unset, None, datetime.datetime]):
         until (Union[Unset, None, datetime.datetime]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        EndpointStats
+        Response[EndpointStats]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         since=since,
         until=until,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -138,72 +153,77 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         since (Union[Unset, None, datetime.datetime]):
         until (Union[Unset, None, datetime.datetime]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         EndpointStats
     """
 
     return sync_detailed(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         since=since,
         until=until,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
     since: Union[Unset, None, datetime.datetime] = UNSET,
     until: Union[Unset, None, datetime.datetime] = UNSET,
-) -> EndpointStats:
+) -> Response[EndpointStats]:
     """Endpoint Stats
 
      Get basic statistics for the endpoint.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         since (Union[Unset, None, datetime.datetime]):
         until (Union[Unset, None, datetime.datetime]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        EndpointStats
+        Response[EndpointStats]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         since=since,
         until=until,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -216,18 +236,24 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         since (Union[Unset, None, datetime.datetime]):
         until (Union[Unset, None, datetime.datetime]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         EndpointStats
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        endpoint_id=endpoint_id,
-        client=client,
-        since=since,
-        until=until,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            endpoint_id=endpoint_id,
+            client=client,
+            since=since,
+            until=until,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_list.py` & `svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_list.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.list_response_endpoint_out import ListResponseEndpointOut
 from ...models.ordering import Ordering
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
@@ -41,87 +45,98 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> ListResponseEndpointOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> ListResponseEndpointOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ListResponseEndpointOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = ListResponseEndpointOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ListResponseEndpointOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     order: Union[Unset, None, Ordering] = UNSET,
-) -> ListResponseEndpointOut:
+) -> Response[ListResponseEndpointOut]:
     """List Endpoints
 
      List the application's endpoints.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The ep's ID Example: ep_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         order (Union[Unset, None, Ordering]): Defines the ordering in a listing of results.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseEndpointOut
+        Response[ListResponseEndpointOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         client=client,
         limit=limit,
         iterator=iterator,
         order=order,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
@@ -134,72 +149,77 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The ep's ID Example: ep_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         order (Union[Unset, None, Ordering]): Defines the ordering in a listing of results.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseEndpointOut
     """
 
     return sync_detailed(
         app_id=app_id,
         client=client,
         limit=limit,
         iterator=iterator,
         order=order,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     order: Union[Unset, None, Ordering] = UNSET,
-) -> ListResponseEndpointOut:
+) -> Response[ListResponseEndpointOut]:
     """List Endpoints
 
      List the application's endpoints.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The ep's ID Example: ep_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         order (Union[Unset, None, Ordering]): Defines the ordering in a listing of results.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseEndpointOut
+        Response[ListResponseEndpointOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         client=client,
         limit=limit,
         iterator=iterator,
         order=order,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
@@ -212,18 +232,24 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The ep's ID Example: ep_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         order (Union[Unset, None, Ordering]): Defines the ordering in a listing of results.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseEndpointOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        client=client,
-        limit=limit,
-        iterator=iterator,
-        order=order,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            client=client,
+            limit=limit,
+            iterator=iterator,
+            order=order,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_recover.py` & `svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_get_secret.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,223 +1,232 @@
 import random
 from http import HTTPStatus
 from time import sleep
-from typing import Any, Dict, Union
+from typing import Any, Dict
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.endpoint_secret_out import EndpointSecretOut
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...models.recover_in import RecoverIn
-from ...models.recover_out import RecoverOut
-from ...types import UNSET, Unset
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: RecoverIn,
-    idempotency_key: Union[Unset, str] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/app/{app_id}/endpoint/{endpoint_id}/recover/".format(
+    url = "{}/api/v1/app/{app_id}/endpoint/{endpoint_id}/secret/".format(
         client.base_url, app_id=app_id, endpoint_id=endpoint_id
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    if not isinstance(idempotency_key, Unset):
-        headers["idempotency-key"] = idempotency_key
-
-    json_json_body = json_body.to_dict()
-
     return {
-        "method": "post",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "json": json_json_body,
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> RecoverOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> EndpointSecretOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = EndpointSecretOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_202 = RecoverOut.from_dict(response.json())
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
-    return response_202
 
-
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[EndpointSecretOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: RecoverIn,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> RecoverOut:
-    """Recover Failed Webhooks
+) -> Response[EndpointSecretOut]:
+    """Get Endpoint Secret
 
-     Resend all failed messages since a given time.
+     Get the endpoint's signing secret.
+
+    This is used to verify the authenticity of the webhook.
+    For more information please refer to [the consuming webhooks docs](https://docs.svix.com/consuming-
+    webhooks/).
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
-        idempotency_key (Union[Unset, str]):
-        json_body (RecoverIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        RecoverOut
+        Response[EndpointSecretOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: RecoverIn,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> RecoverOut:
-    """Recover Failed Webhooks
+) -> EndpointSecretOut:
+    """Get Endpoint Secret
+
+     Get the endpoint's signing secret.
 
-     Resend all failed messages since a given time.
+    This is used to verify the authenticity of the webhook.
+    For more information please refer to [the consuming webhooks docs](https://docs.svix.com/consuming-
+    webhooks/).
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
-        idempotency_key (Union[Unset, str]):
-        json_body (RecoverIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        RecoverOut
+        EndpointSecretOut
     """
 
     return sync_detailed(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: RecoverIn,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> RecoverOut:
-    """Recover Failed Webhooks
+) -> Response[EndpointSecretOut]:
+    """Get Endpoint Secret
 
-     Resend all failed messages since a given time.
+     Get the endpoint's signing secret.
+
+    This is used to verify the authenticity of the webhook.
+    For more information please refer to [the consuming webhooks docs](https://docs.svix.com/consuming-
+    webhooks/).
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
-        idempotency_key (Union[Unset, str]):
-        json_body (RecoverIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        RecoverOut
+        Response[EndpointSecretOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: RecoverIn,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> RecoverOut:
-    """Recover Failed Webhooks
+) -> EndpointSecretOut:
+    """Get Endpoint Secret
+
+     Get the endpoint's signing secret.
 
-     Resend all failed messages since a given time.
+    This is used to verify the authenticity of the webhook.
+    For more information please refer to [the consuming webhooks docs](https://docs.svix.com/consuming-
+    webhooks/).
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
-        idempotency_key (Union[Unset, str]):
-        json_body (RecoverIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        RecoverOut
+        EndpointSecretOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        endpoint_id=endpoint_id,
-        client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            endpoint_id=endpoint_id,
+            client=client,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_replay.py` & `svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_transformation_partial_update.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,227 +1,231 @@
 import random
 from http import HTTPStatus
 from time import sleep
-from typing import Any, Dict, Union
+from typing import Any, Dict, cast
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.endpoint_transformation_in import EndpointTransformationIn
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...models.replay_in import ReplayIn
-from ...models.replay_out import ReplayOut
-from ...types import UNSET, Unset
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: ReplayIn,
-    idempotency_key: Union[Unset, str] = UNSET,
+    json_body: EndpointTransformationIn,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/app/{app_id}/endpoint/{endpoint_id}/replay-missing/".format(
+    url = "{}/api/v1/app/{app_id}/endpoint/{endpoint_id}/transformation/".format(
         client.base_url, app_id=app_id, endpoint_id=endpoint_id
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    if not isinstance(idempotency_key, Unset):
-        headers["idempotency-key"] = idempotency_key
-
     json_json_body = json_body.to_dict()
 
     return {
-        "method": "post",
+        "method": "patch",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> ReplayOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> Any:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_202 = ReplayOut.from_dict(response.json())
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
-    return response_202
 
-
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[None]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: ReplayIn,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> ReplayOut:
-    """Replay Missing Webhooks
+    json_body: EndpointTransformationIn,
+) -> Response[None]:
+    """Set Endpoint Transformation
 
-     Replays messages to the endpoint. Only messages that were created after `since` will be sent.
-    Messages that were previously sent to the endpoint are not resent.
+     Set or unset the transformation code associated with this endpoint
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
-        idempotency_key (Union[Unset, str]):
-        json_body (ReplayIn):
+        json_body (EndpointTransformationIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ReplayOut
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
-        idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: ReplayIn,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> ReplayOut:
-    """Replay Missing Webhooks
+    json_body: EndpointTransformationIn,
+) -> None:
+    """Set Endpoint Transformation
 
-     Replays messages to the endpoint. Only messages that were created after `since` will be sent.
-    Messages that were previously sent to the endpoint are not resent.
+     Set or unset the transformation code associated with this endpoint
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
-        idempotency_key (Union[Unset, str]):
-        json_body (ReplayIn):
+        json_body (EndpointTransformationIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ReplayOut
+        None
     """
 
     return sync_detailed(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
-        idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: ReplayIn,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> ReplayOut:
-    """Replay Missing Webhooks
+    json_body: EndpointTransformationIn,
+) -> Response[None]:
+    """Set Endpoint Transformation
 
-     Replays messages to the endpoint. Only messages that were created after `since` will be sent.
-    Messages that were previously sent to the endpoint are not resent.
+     Set or unset the transformation code associated with this endpoint
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
-        idempotency_key (Union[Unset, str]):
-        json_body (ReplayIn):
+        json_body (EndpointTransformationIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ReplayOut
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
-        idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: ReplayIn,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> ReplayOut:
-    """Replay Missing Webhooks
+    json_body: EndpointTransformationIn,
+) -> None:
+    """Set Endpoint Transformation
 
-     Replays messages to the endpoint. Only messages that were created after `since` will be sent.
-    Messages that were previously sent to the endpoint are not resent.
+     Set or unset the transformation code associated with this endpoint
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
-        idempotency_key (Union[Unset, str]):
-        json_body (ReplayIn):
+        json_body (EndpointTransformationIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ReplayOut
+        None
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        endpoint_id=endpoint_id,
-        client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            endpoint_id=endpoint_id,
+            client=client,
+            json_body=json_body,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_rotate_secret.py` & `svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_rotate_secret.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import random
 from http import HTTPStatus
 from time import sleep
-from typing import Any, Dict, Union
+from typing import Any, Dict, Union, cast
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.endpoint_secret_rotate_in import EndpointSecretRotateIn
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -34,86 +38,97 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> None:
+def _parse_response(*, client: Client, response: httpx.Response) -> Any:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_204 = None
-    return response_204
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[None]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
     json_body: EndpointSecretRotateIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> None:
+) -> Response[None]:
     """Rotate Endpoint Secret
 
      Rotates the endpoint's signing secret.  The previous secret will be valid for the next 24 hours.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (EndpointSecretRotateIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        None
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -126,72 +141,77 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (EndpointSecretRotateIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         None
     """
 
     return sync_detailed(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
     json_body: EndpointSecretRotateIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> None:
+) -> Response[None]:
     """Rotate Endpoint Secret
 
      Rotates the endpoint's signing secret.  The previous secret will be valid for the next 24 hours.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (EndpointSecretRotateIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        None
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -204,18 +224,24 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (EndpointSecretRotateIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         None
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        endpoint_id=endpoint_id,
-        client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            endpoint_id=endpoint_id,
+            client=client,
+            json_body=json_body,
+            idempotency_key=idempotency_key,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_send_example.py` & `svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_send_example.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.event_example_in import EventExampleIn
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_out import MessageOut
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -35,87 +39,98 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> MessageOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> MessageOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = MessageOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = MessageOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[MessageOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
     json_body: EventExampleIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> MessageOut:
+) -> Response[MessageOut]:
     """Send Event Type Example Message
 
      Send an example message for event
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (EventExampleIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        MessageOut
+        Response[MessageOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -128,72 +143,77 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (EventExampleIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         MessageOut
     """
 
     return sync_detailed(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
     json_body: EventExampleIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> MessageOut:
+) -> Response[MessageOut]:
     """Send Event Type Example Message
 
      Send an example message for event
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (EventExampleIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        MessageOut
+        Response[MessageOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -206,18 +226,24 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (EventExampleIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         MessageOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        endpoint_id=endpoint_id,
-        client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            endpoint_id=endpoint_id,
+            client=client,
+            json_body=json_body,
+            idempotency_key=idempotency_key,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_transformation_get.py` & `svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_transformation_get.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.endpoint_transformation_out import EndpointTransformationOut
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -26,80 +31,91 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> EndpointTransformationOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> EndpointTransformationOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = EndpointTransformationOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = EndpointTransformationOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[EndpointTransformationOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-) -> EndpointTransformationOut:
+) -> Response[EndpointTransformationOut]:
     """Get Endpoint Transformation
 
      Get the transformation code associated with this endpoint
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        EndpointTransformationOut
+        Response[EndpointTransformationOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -108,64 +124,69 @@
 
      Get the transformation code associated with this endpoint
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         EndpointTransformationOut
     """
 
     return sync_detailed(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-) -> EndpointTransformationOut:
+) -> Response[EndpointTransformationOut]:
     """Get Endpoint Transformation
 
      Get the transformation code associated with this endpoint
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        EndpointTransformationOut
+        Response[EndpointTransformationOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -174,16 +195,22 @@
 
      Get the transformation code associated with this endpoint
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         EndpointTransformationOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        endpoint_id=endpoint_id,
-        client=client,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            endpoint_id=endpoint_id,
+            client=client,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_transformation_simulate.py` & `svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_transformation_simulate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.endpoint_transformation_simulate_in import EndpointTransformationSimulateIn
 from ...models.endpoint_transformation_simulate_out import EndpointTransformationSimulateOut
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -35,87 +39,98 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> EndpointTransformationSimulateOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> EndpointTransformationSimulateOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = EndpointTransformationSimulateOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = EndpointTransformationSimulateOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[EndpointTransformationSimulateOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
     json_body: EndpointTransformationSimulateIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> EndpointTransformationSimulateOut:
+) -> Response[EndpointTransformationSimulateOut]:
     """Simulate
 
      Simulate running the transformation on the payload and code
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (EndpointTransformationSimulateIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        EndpointTransformationSimulateOut
+        Response[EndpointTransformationSimulateOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -128,72 +143,77 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (EndpointTransformationSimulateIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         EndpointTransformationSimulateOut
     """
 
     return sync_detailed(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
     json_body: EndpointTransformationSimulateIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> EndpointTransformationSimulateOut:
+) -> Response[EndpointTransformationSimulateOut]:
     """Simulate
 
      Simulate running the transformation on the payload and code
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (EndpointTransformationSimulateIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        EndpointTransformationSimulateOut
+        Response[EndpointTransformationSimulateOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -206,18 +226,24 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (EndpointTransformationSimulateIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         EndpointTransformationSimulateOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        endpoint_id=endpoint_id,
-        client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            endpoint_id=endpoint_id,
+            client=client,
+            json_body=json_body,
+            idempotency_key=idempotency_key,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/endpoint/v1_endpoint_update_headers.py` & `svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_patch_headers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,204 +1,231 @@
 import random
 from http import HTTPStatus
 from time import sleep
-from typing import Any, Dict
+from typing import Any, Dict, cast
 
 import httpx
 
-from ...client import AuthenticatedClient
-from ...models.endpoint_headers_in import EndpointHeadersIn
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.endpoint_headers_patch_in import EndpointHeadersPatchIn
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: EndpointHeadersIn,
+    json_body: EndpointHeadersPatchIn,
 ) -> Dict[str, Any]:
     url = "{}/api/v1/app/{app_id}/endpoint/{endpoint_id}/headers/".format(
         client.base_url, app_id=app_id, endpoint_id=endpoint_id
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
-        "method": "put",
+        "method": "patch",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> None:
+def _parse_response(*, client: Client, response: httpx.Response) -> Any:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_204 = None
-    return response_204
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[None]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: EndpointHeadersIn,
-) -> None:
-    """Update Endpoint Headers
+    json_body: EndpointHeadersPatchIn,
+) -> Response[None]:
+    """Patch Endpoint Headers
 
-     Set the additional headers to be sent with the webhook
+     Partially set the additional headers to be sent with the webhook
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
-        json_body (EndpointHeadersIn):
+        json_body (EndpointHeadersPatchIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        None
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: EndpointHeadersIn,
+    json_body: EndpointHeadersPatchIn,
 ) -> None:
-    """Update Endpoint Headers
+    """Patch Endpoint Headers
 
-     Set the additional headers to be sent with the webhook
+     Partially set the additional headers to be sent with the webhook
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
-        json_body (EndpointHeadersIn):
+        json_body (EndpointHeadersPatchIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         None
     """
 
     return sync_detailed(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: EndpointHeadersIn,
-) -> None:
-    """Update Endpoint Headers
+    json_body: EndpointHeadersPatchIn,
+) -> Response[None]:
+    """Patch Endpoint Headers
 
-     Set the additional headers to be sent with the webhook
+     Partially set the additional headers to be sent with the webhook
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
-        json_body (EndpointHeadersIn):
+        json_body (EndpointHeadersPatchIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        None
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: EndpointHeadersIn,
+    json_body: EndpointHeadersPatchIn,
 ) -> None:
-    """Update Endpoint Headers
+    """Patch Endpoint Headers
 
-     Set the additional headers to be sent with the webhook
+     Partially set the additional headers to be sent with the webhook
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
-        json_body (EndpointHeadersIn):
+        json_body (EndpointHeadersPatchIn):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         None
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        endpoint_id=endpoint_id,
-        client=client,
-        json_body=json_body,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            endpoint_id=endpoint_id,
+            client=client,
+            json_body=json_body,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/environment/v1_environment_export.py` & `svix-1.5.0/svix/internal/openapi_client/api/environment/v1_environment_export.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.environment_out import EnvironmentOut
 from ...models.export_environment_in import ExportEnvironmentIn
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
     json_body: ExportEnvironmentIn,
     idempotency_key: Union[Unset, str] = UNSET,
@@ -31,81 +35,92 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> EnvironmentOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> EnvironmentOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = EnvironmentOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = EnvironmentOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[EnvironmentOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
     json_body: ExportEnvironmentIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> EnvironmentOut:
+) -> Response[EnvironmentOut]:
     """Export Environment Configuration
 
      Download a JSON file containing all org-settings and event types
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (ExportEnvironmentIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        EnvironmentOut
+        Response[EnvironmentOut]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
     json_body: ExportEnvironmentIn,
     idempotency_key: Union[Unset, str] = UNSET,
@@ -114,64 +129,69 @@
 
      Download a JSON file containing all org-settings and event types
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (ExportEnvironmentIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         EnvironmentOut
     """
 
     return sync_detailed(
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
     json_body: ExportEnvironmentIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> EnvironmentOut:
+) -> Response[EnvironmentOut]:
     """Export Environment Configuration
 
      Download a JSON file containing all org-settings and event types
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (ExportEnvironmentIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        EnvironmentOut
+        Response[EnvironmentOut]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
     json_body: ExportEnvironmentIn,
     idempotency_key: Union[Unset, str] = UNSET,
@@ -180,16 +200,22 @@
 
      Download a JSON file containing all org-settings and event types
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (ExportEnvironmentIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         EnvironmentOut
     """
 
-    return await asyncio_detailed(
-        client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            client=client,
+            json_body=json_body,
+            idempotency_key=idempotency_key,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/environment/v1_environment_import.py` & `svix-1.5.0/svix/internal/openapi_client/api/environment/v1_environment_import.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import random
 from http import HTTPStatus
 from time import sleep
-from typing import Any, Dict, Union
+from typing import Any, Dict, Union, cast
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.environment_in import EnvironmentIn
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
     json_body: EnvironmentIn,
     idempotency_key: Union[Unset, str] = UNSET,
@@ -30,81 +34,92 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> None:
+def _parse_response(*, client: Client, response: httpx.Response) -> Any:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_204 = None
-    return response_204
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[None]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
     json_body: EnvironmentIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> None:
+) -> Response[None]:
     """Import Environment Configuration
 
      Import a configuration into the active organization.
     It doesn't delete anything, only adds/updates what was passed to it.
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (EnvironmentIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        None
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
     json_body: EnvironmentIn,
     idempotency_key: Union[Unset, str] = UNSET,
@@ -114,65 +129,70 @@
      Import a configuration into the active organization.
     It doesn't delete anything, only adds/updates what was passed to it.
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (EnvironmentIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         None
     """
 
     return sync_detailed(
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
     json_body: EnvironmentIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> None:
+) -> Response[None]:
     """Import Environment Configuration
 
      Import a configuration into the active organization.
     It doesn't delete anything, only adds/updates what was passed to it.
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (EnvironmentIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        None
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
     json_body: EnvironmentIn,
     idempotency_key: Union[Unset, str] = UNSET,
@@ -182,16 +202,22 @@
      Import a configuration into the active organization.
     It doesn't delete anything, only adds/updates what was passed to it.
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (EnvironmentIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         None
     """
 
-    return await asyncio_detailed(
-        client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            client=client,
+            json_body=json_body,
+            idempotency_key=idempotency_key,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/environment_settings/v1_environment_get_settings.py` & `svix-1.5.0/svix/internal/openapi_client/api/environment_settings/v1_environment_get_settings.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.environment_settings_out import EnvironmentSettingsOut
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/api/v1/environment/settings/".format(client.base_url)
@@ -22,132 +27,154 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> EnvironmentSettingsOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> EnvironmentSettingsOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = EnvironmentSettingsOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = EnvironmentSettingsOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[EnvironmentSettingsOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
-) -> EnvironmentSettingsOut:
+) -> Response[EnvironmentSettingsOut]:
     """Get Org Settings
 
      Get the environment's settings
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        EnvironmentSettingsOut
+        Response[EnvironmentSettingsOut]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
 ) -> EnvironmentSettingsOut:
     """Get Org Settings
 
      Get the environment's settings
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         EnvironmentSettingsOut
     """
 
     return sync_detailed(
         client=client,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
-) -> EnvironmentSettingsOut:
+) -> Response[EnvironmentSettingsOut]:
     """Get Org Settings
 
      Get the environment's settings
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        EnvironmentSettingsOut
+        Response[EnvironmentSettingsOut]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
 ) -> EnvironmentSettingsOut:
     """Get Org Settings
 
      Get the environment's settings
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         EnvironmentSettingsOut
     """
 
-    return await asyncio_detailed(
-        client=client,
-    )
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/event_type/patch_event_type.py` & `svix-1.5.0/svix/internal/openapi_client/api/event_type/patch_event_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.event_type_out import EventTypeOut
 from ...models.event_type_patch import EventTypePatch
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     event_type_name: str,
     *,
     client: AuthenticatedClient,
     json_body: EventTypePatch,
@@ -27,81 +32,92 @@
 
     return {
         "method": "patch",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> EventTypeOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> EventTypeOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = EventTypeOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = EventTypeOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[EventTypeOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     event_type_name: str,
     *,
     client: AuthenticatedClient,
     json_body: EventTypePatch,
-) -> EventTypeOut:
+) -> Response[EventTypeOut]:
     """Patch Event Type
 
      Partially update an event type.
 
     Args:
         event_type_name (str): The event type's name Example: user.signup.
         json_body (EventTypePatch):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        EventTypeOut
+        Response[EventTypeOut]
     """
 
     kwargs = _get_kwargs(
         event_type_name=event_type_name,
         client=client,
         json_body=json_body,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     event_type_name: str,
     *,
     client: AuthenticatedClient,
     json_body: EventTypePatch,
@@ -110,64 +126,69 @@
 
      Partially update an event type.
 
     Args:
         event_type_name (str): The event type's name Example: user.signup.
         json_body (EventTypePatch):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         EventTypeOut
     """
 
     return sync_detailed(
         event_type_name=event_type_name,
         client=client,
         json_body=json_body,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     event_type_name: str,
     *,
     client: AuthenticatedClient,
     json_body: EventTypePatch,
-) -> EventTypeOut:
+) -> Response[EventTypeOut]:
     """Patch Event Type
 
      Partially update an event type.
 
     Args:
         event_type_name (str): The event type's name Example: user.signup.
         json_body (EventTypePatch):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        EventTypeOut
+        Response[EventTypeOut]
     """
 
     kwargs = _get_kwargs(
         event_type_name=event_type_name,
         client=client,
         json_body=json_body,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     event_type_name: str,
     *,
     client: AuthenticatedClient,
     json_body: EventTypePatch,
@@ -176,16 +197,22 @@
 
      Partially update an event type.
 
     Args:
         event_type_name (str): The event type's name Example: user.signup.
         json_body (EventTypePatch):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         EventTypeOut
     """
 
-    return await asyncio_detailed(
-        event_type_name=event_type_name,
-        client=client,
-        json_body=json_body,
-    )
+    return (
+        await asyncio_detailed(
+            event_type_name=event_type_name,
+            client=client,
+            json_body=json_body,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/event_type/v1_event_type_create.py` & `svix-1.5.0/svix/internal/openapi_client/api/event_type/v1_event_type_create.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.event_type_in import EventTypeIn
 from ...models.event_type_out import EventTypeOut
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
     json_body: EventTypeIn,
     idempotency_key: Union[Unset, str] = UNSET,
@@ -31,85 +35,96 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> EventTypeOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> EventTypeOut:
+    if response.status_code == HTTPStatus.CREATED:
+        response_201 = EventTypeOut.from_dict(response.json())
+
+        return response_201
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_201 = EventTypeOut.from_dict(response.json())
-
-    return response_201
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[EventTypeOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
     json_body: EventTypeIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> EventTypeOut:
+) -> Response[EventTypeOut]:
     """Create Event Type
 
      Create new or unarchive existing event type.
 
     Unarchiving an event type will allow endpoints to filter on it and messages to be sent with it.
     Endpoints filtering on the event type before archival will continue to filter on it.
     This operation does not preserve the description and schemas.
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (EventTypeIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        EventTypeOut
+        Response[EventTypeOut]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
     json_body: EventTypeIn,
     idempotency_key: Union[Unset, str] = UNSET,
@@ -122,68 +137,73 @@
     Endpoints filtering on the event type before archival will continue to filter on it.
     This operation does not preserve the description and schemas.
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (EventTypeIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         EventTypeOut
     """
 
     return sync_detailed(
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
     json_body: EventTypeIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> EventTypeOut:
+) -> Response[EventTypeOut]:
     """Create Event Type
 
      Create new or unarchive existing event type.
 
     Unarchiving an event type will allow endpoints to filter on it and messages to be sent with it.
     Endpoints filtering on the event type before archival will continue to filter on it.
     This operation does not preserve the description and schemas.
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (EventTypeIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        EventTypeOut
+        Response[EventTypeOut]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
     json_body: EventTypeIn,
     idempotency_key: Union[Unset, str] = UNSET,
@@ -196,16 +216,22 @@
     Endpoints filtering on the event type before archival will continue to filter on it.
     This operation does not preserve the description and schemas.
 
     Args:
         idempotency_key (Union[Unset, str]):
         json_body (EventTypeIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         EventTypeOut
     """
 
-    return await asyncio_detailed(
-        client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            client=client,
+            json_body=json_body,
+            idempotency_key=idempotency_key,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/event_type/v1_event_type_delete.py` & `svix-1.5.0/svix/internal/openapi_client/api/event_type/v1_event_type_delete.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import random
 from http import HTTPStatus
 from time import sleep
-from typing import Any, Dict, Union
+from typing import Any, Dict, Union, cast
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     event_type_name: str,
     *,
     client: AuthenticatedClient,
     expunge: Union[Unset, None, bool] = False,
@@ -29,85 +33,96 @@
 
     return {
         "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> None:
+def _parse_response(*, client: Client, response: httpx.Response) -> Any:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_204 = None
-    return response_204
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[None]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     event_type_name: str,
     *,
     client: AuthenticatedClient,
     expunge: Union[Unset, None, bool] = False,
-) -> None:
+) -> Response[None]:
     """Delete Event Type
 
      Archive an event type.
 
     Endpoints already configured to filter on an event type will continue to do so after archival.
     However, new messages can not be sent with it and endpoints can not filter on it.
     An event type can be unarchived with the
     [create operation](#operation/create_event_type_api_v1_event_type__post).
 
     Args:
         event_type_name (str): The event type's name Example: user.signup.
         expunge (Union[Unset, None, bool]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        None
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         event_type_name=event_type_name,
         client=client,
         expunge=expunge,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     event_type_name: str,
     *,
     client: AuthenticatedClient,
     expunge: Union[Unset, None, bool] = False,
@@ -121,69 +136,74 @@
     An event type can be unarchived with the
     [create operation](#operation/create_event_type_api_v1_event_type__post).
 
     Args:
         event_type_name (str): The event type's name Example: user.signup.
         expunge (Union[Unset, None, bool]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         None
     """
 
     return sync_detailed(
         event_type_name=event_type_name,
         client=client,
         expunge=expunge,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     event_type_name: str,
     *,
     client: AuthenticatedClient,
     expunge: Union[Unset, None, bool] = False,
-) -> None:
+) -> Response[None]:
     """Delete Event Type
 
      Archive an event type.
 
     Endpoints already configured to filter on an event type will continue to do so after archival.
     However, new messages can not be sent with it and endpoints can not filter on it.
     An event type can be unarchived with the
     [create operation](#operation/create_event_type_api_v1_event_type__post).
 
     Args:
         event_type_name (str): The event type's name Example: user.signup.
         expunge (Union[Unset, None, bool]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        None
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         event_type_name=event_type_name,
         client=client,
         expunge=expunge,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     event_type_name: str,
     *,
     client: AuthenticatedClient,
     expunge: Union[Unset, None, bool] = False,
@@ -197,16 +217,22 @@
     An event type can be unarchived with the
     [create operation](#operation/create_event_type_api_v1_event_type__post).
 
     Args:
         event_type_name (str): The event type's name Example: user.signup.
         expunge (Union[Unset, None, bool]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         None
     """
 
-    return await asyncio_detailed(
-        event_type_name=event_type_name,
-        client=client,
-        expunge=expunge,
-    )
+    return (
+        await asyncio_detailed(
+            event_type_name=event_type_name,
+            client=client,
+            expunge=expunge,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/event_type/v1_event_type_list.py` & `svix-1.5.0/svix/internal/openapi_client/api/event_type/v1_event_type_list.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.list_response_event_type_out import ListResponseEventTypeOut
 from ...models.ordering import Ordering
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
@@ -46,90 +50,101 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> ListResponseEventTypeOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> ListResponseEventTypeOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ListResponseEventTypeOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = ListResponseEventTypeOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ListResponseEventTypeOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     order: Union[Unset, None, Ordering] = UNSET,
     include_archived: Union[Unset, None, bool] = False,
     with_content: Union[Unset, None, bool] = False,
-) -> ListResponseEventTypeOut:
+) -> Response[ListResponseEventTypeOut]:
     """List Event Types
 
      Return the list of event types.
 
     Args:
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The event type's name Example: user.signup.
         order (Union[Unset, None, Ordering]): Defines the ordering in a listing of results.
         include_archived (Union[Unset, None, bool]):
         with_content (Union[Unset, None, bool]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseEventTypeOut
+        Response[ListResponseEventTypeOut]
     """
 
     kwargs = _get_kwargs(
         client=client,
         limit=limit,
         iterator=iterator,
         order=order,
         include_archived=include_archived,
         with_content=with_content,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
@@ -144,76 +159,81 @@
     Args:
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The event type's name Example: user.signup.
         order (Union[Unset, None, Ordering]): Defines the ordering in a listing of results.
         include_archived (Union[Unset, None, bool]):
         with_content (Union[Unset, None, bool]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseEventTypeOut
     """
 
     return sync_detailed(
         client=client,
         limit=limit,
         iterator=iterator,
         order=order,
         include_archived=include_archived,
         with_content=with_content,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     order: Union[Unset, None, Ordering] = UNSET,
     include_archived: Union[Unset, None, bool] = False,
     with_content: Union[Unset, None, bool] = False,
-) -> ListResponseEventTypeOut:
+) -> Response[ListResponseEventTypeOut]:
     """List Event Types
 
      Return the list of event types.
 
     Args:
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The event type's name Example: user.signup.
         order (Union[Unset, None, Ordering]): Defines the ordering in a listing of results.
         include_archived (Union[Unset, None, bool]):
         with_content (Union[Unset, None, bool]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseEventTypeOut
+        Response[ListResponseEventTypeOut]
     """
 
     kwargs = _get_kwargs(
         client=client,
         limit=limit,
         iterator=iterator,
         order=order,
         include_archived=include_archived,
         with_content=with_content,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
@@ -228,19 +248,25 @@
     Args:
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The event type's name Example: user.signup.
         order (Union[Unset, None, Ordering]): Defines the ordering in a listing of results.
         include_archived (Union[Unset, None, bool]):
         with_content (Union[Unset, None, bool]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseEventTypeOut
     """
 
-    return await asyncio_detailed(
-        client=client,
-        limit=limit,
-        iterator=iterator,
-        order=order,
-        include_archived=include_archived,
-        with_content=with_content,
-    )
+    return (
+        await asyncio_detailed(
+            client=client,
+            limit=limit,
+            iterator=iterator,
+            order=order,
+            include_archived=include_archived,
+            with_content=with_content,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/integration/v1_integration_create.py` & `svix-1.5.0/svix/internal/openapi_client/api/endpoint/v1_endpoint_delete.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,208 +1,214 @@
 import random
 from http import HTTPStatus
 from time import sleep
-from typing import Any, Dict, Union
+from typing import Any, Dict, cast
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...models.integration_in import IntegrationIn
-from ...models.integration_out import IntegrationOut
-from ...types import UNSET, Unset
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
+    endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: IntegrationIn,
-    idempotency_key: Union[Unset, str] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/app/{app_id}/integration/".format(client.base_url, app_id=app_id)
+    url = "{}/api/v1/app/{app_id}/endpoint/{endpoint_id}/".format(
+        client.base_url, app_id=app_id, endpoint_id=endpoint_id
+    )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    if not isinstance(idempotency_key, Unset):
-        headers["idempotency-key"] = idempotency_key
-
-    json_json_body = json_body.to_dict()
-
     return {
-        "method": "post",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "json": json_json_body,
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> IntegrationOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> Any:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = IntegrationOut.from_dict(response.json())
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
-    return response_200
 
-
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[None]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
+    endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: IntegrationIn,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> IntegrationOut:
-    """Create Integration
+) -> Response[None]:
+    """Delete Endpoint
 
-     Create an integration.
+     Delete an endpoint.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        idempotency_key (Union[Unset, str]):
-        json_body (IntegrationIn):
+        endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        IntegrationOut
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
+        endpoint_id=endpoint_id,
         client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
+    endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: IntegrationIn,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> IntegrationOut:
-    """Create Integration
+) -> None:
+    """Delete Endpoint
 
-     Create an integration.
+     Delete an endpoint.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        idempotency_key (Union[Unset, str]):
-        json_body (IntegrationIn):
+        endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        IntegrationOut
+        None
     """
 
     return sync_detailed(
         app_id=app_id,
+        endpoint_id=endpoint_id,
         client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
+    endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: IntegrationIn,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> IntegrationOut:
-    """Create Integration
+) -> Response[None]:
+    """Delete Endpoint
 
-     Create an integration.
+     Delete an endpoint.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        idempotency_key (Union[Unset, str]):
-        json_body (IntegrationIn):
+        endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        IntegrationOut
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
+        endpoint_id=endpoint_id,
         client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
+    endpoint_id: str,
     *,
     client: AuthenticatedClient,
-    json_body: IntegrationIn,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> IntegrationOut:
-    """Create Integration
+) -> None:
+    """Delete Endpoint
 
-     Create an integration.
+     Delete an endpoint.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        idempotency_key (Union[Unset, str]):
-        json_body (IntegrationIn):
+        endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        IntegrationOut
+        None
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            endpoint_id=endpoint_id,
+            client=client,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/integration/v1_integration_get_key.py` & `svix-1.5.0/svix/internal/openapi_client/api/integration/v1_integration_get_key.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.integration_key_out import IntegrationKeyOut
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     integ_id: str,
     *,
     client: AuthenticatedClient,
@@ -24,80 +29,91 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> IntegrationKeyOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> IntegrationKeyOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = IntegrationKeyOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = IntegrationKeyOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[IntegrationKeyOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     integ_id: str,
     *,
     client: AuthenticatedClient,
-) -> IntegrationKeyOut:
+) -> Response[IntegrationKeyOut]:
     """Get Integration Key
 
      Get an integration's key.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         integ_id (str): The integ's ID Example: integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        IntegrationKeyOut
+        Response[IntegrationKeyOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         integ_id=integ_id,
         client=client,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     integ_id: str,
     *,
     client: AuthenticatedClient,
@@ -106,64 +122,69 @@
 
      Get an integration's key.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         integ_id (str): The integ's ID Example: integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         IntegrationKeyOut
     """
 
     return sync_detailed(
         app_id=app_id,
         integ_id=integ_id,
         client=client,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     integ_id: str,
     *,
     client: AuthenticatedClient,
-) -> IntegrationKeyOut:
+) -> Response[IntegrationKeyOut]:
     """Get Integration Key
 
      Get an integration's key.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         integ_id (str): The integ's ID Example: integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        IntegrationKeyOut
+        Response[IntegrationKeyOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         integ_id=integ_id,
         client=client,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     integ_id: str,
     *,
     client: AuthenticatedClient,
@@ -172,16 +193,22 @@
 
      Get an integration's key.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         integ_id (str): The integ's ID Example: integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         IntegrationKeyOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        integ_id=integ_id,
-        client=client,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            integ_id=integ_id,
+            client=client,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/integration/v1_integration_list.py` & `svix-1.5.0/svix/internal/openapi_client/api/integration/v1_integration_delete.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,213 +1,212 @@
 import random
 from http import HTTPStatus
 from time import sleep
-from typing import Any, Dict, Union
+from typing import Any, Dict, cast
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...models.list_response_integration_out import ListResponseIntegrationOut
-from ...types import UNSET, Unset
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
+    integ_id: str,
     *,
     client: AuthenticatedClient,
-    limit: Union[Unset, None, int] = UNSET,
-    iterator: Union[Unset, None, str] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/app/{app_id}/integration/".format(client.base_url, app_id=app_id)
+    url = "{}/api/v1/app/{app_id}/integration/{integ_id}/".format(client.base_url, app_id=app_id, integ_id=integ_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    params: Dict[str, Any] = {}
-    params["limit"] = limit
-
-    params["iterator"] = iterator
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
     return {
-        "method": "get",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "params": params,
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> ListResponseIntegrationOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> Any:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = ListResponseIntegrationOut.from_dict(response.json())
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
-    return response_200
 
-
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[None]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
+    integ_id: str,
     *,
     client: AuthenticatedClient,
-    limit: Union[Unset, None, int] = UNSET,
-    iterator: Union[Unset, None, str] = UNSET,
-) -> ListResponseIntegrationOut:
-    """List Integrations
+) -> Response[None]:
+    """Delete Integration
 
-     List the application's integrations.
+     Delete an integration.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        limit (Union[Unset, None, int]):
-        iterator (Union[Unset, None, str]): The integ's ID Example:
-            integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
+        integ_id (str): The integ's ID Example: integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ListResponseIntegrationOut
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
+        integ_id=integ_id,
         client=client,
-        limit=limit,
-        iterator=iterator,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
+    integ_id: str,
     *,
     client: AuthenticatedClient,
-    limit: Union[Unset, None, int] = UNSET,
-    iterator: Union[Unset, None, str] = UNSET,
-) -> ListResponseIntegrationOut:
-    """List Integrations
+) -> None:
+    """Delete Integration
 
-     List the application's integrations.
+     Delete an integration.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        limit (Union[Unset, None, int]):
-        iterator (Union[Unset, None, str]): The integ's ID Example:
-            integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
+        integ_id (str): The integ's ID Example: integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ListResponseIntegrationOut
+        None
     """
 
     return sync_detailed(
         app_id=app_id,
+        integ_id=integ_id,
         client=client,
-        limit=limit,
-        iterator=iterator,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
+    integ_id: str,
     *,
     client: AuthenticatedClient,
-    limit: Union[Unset, None, int] = UNSET,
-    iterator: Union[Unset, None, str] = UNSET,
-) -> ListResponseIntegrationOut:
-    """List Integrations
+) -> Response[None]:
+    """Delete Integration
 
-     List the application's integrations.
+     Delete an integration.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        limit (Union[Unset, None, int]):
-        iterator (Union[Unset, None, str]): The integ's ID Example:
-            integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
+        integ_id (str): The integ's ID Example: integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ListResponseIntegrationOut
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
+        integ_id=integ_id,
         client=client,
-        limit=limit,
-        iterator=iterator,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
+    integ_id: str,
     *,
     client: AuthenticatedClient,
-    limit: Union[Unset, None, int] = UNSET,
-    iterator: Union[Unset, None, str] = UNSET,
-) -> ListResponseIntegrationOut:
-    """List Integrations
+) -> None:
+    """Delete Integration
 
-     List the application's integrations.
+     Delete an integration.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        limit (Union[Unset, None, int]):
-        iterator (Union[Unset, None, str]): The integ's ID Example:
-            integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
+        integ_id (str): The integ's ID Example: integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ListResponseIntegrationOut
+        None
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        client=client,
-        limit=limit,
-        iterator=iterator,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            integ_id=integ_id,
+            client=client,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/integration/v1_integration_rotate_key.py` & `svix-1.5.0/svix/internal/openapi_client/api/integration/v1_integration_get.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,206 +1,214 @@
 import random
 from http import HTTPStatus
 from time import sleep
-from typing import Any, Dict, Union
+from typing import Any, Dict
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...models.integration_key_out import IntegrationKeyOut
-from ...types import UNSET, Unset
+from ...models.integration_out import IntegrationOut
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     integ_id: str,
     *,
     client: AuthenticatedClient,
-    idempotency_key: Union[Unset, str] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/app/{app_id}/integration/{integ_id}/key/rotate/".format(
-        client.base_url, app_id=app_id, integ_id=integ_id
-    )
+    url = "{}/api/v1/app/{app_id}/integration/{integ_id}/".format(client.base_url, app_id=app_id, integ_id=integ_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    if not isinstance(idempotency_key, Unset):
-        headers["idempotency-key"] = idempotency_key
-
     return {
-        "method": "post",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> IntegrationKeyOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> IntegrationOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = IntegrationOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = IntegrationKeyOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[IntegrationOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     integ_id: str,
     *,
     client: AuthenticatedClient,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> IntegrationKeyOut:
-    """Rotate Integration Key
+) -> Response[IntegrationOut]:
+    """Get Integration
 
-     Rotate the integration's key. The previous key will be immediately revoked.
+     Get an integration.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         integ_id (str): The integ's ID Example: integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
-        idempotency_key (Union[Unset, str]):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        IntegrationKeyOut
+        Response[IntegrationOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         integ_id=integ_id,
         client=client,
-        idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     integ_id: str,
     *,
     client: AuthenticatedClient,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> IntegrationKeyOut:
-    """Rotate Integration Key
+) -> IntegrationOut:
+    """Get Integration
 
-     Rotate the integration's key. The previous key will be immediately revoked.
+     Get an integration.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         integ_id (str): The integ's ID Example: integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
-        idempotency_key (Union[Unset, str]):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        IntegrationKeyOut
+        IntegrationOut
     """
 
     return sync_detailed(
         app_id=app_id,
         integ_id=integ_id,
         client=client,
-        idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     integ_id: str,
     *,
     client: AuthenticatedClient,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> IntegrationKeyOut:
-    """Rotate Integration Key
+) -> Response[IntegrationOut]:
+    """Get Integration
 
-     Rotate the integration's key. The previous key will be immediately revoked.
+     Get an integration.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         integ_id (str): The integ's ID Example: integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
-        idempotency_key (Union[Unset, str]):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        IntegrationKeyOut
+        Response[IntegrationOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         integ_id=integ_id,
         client=client,
-        idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     integ_id: str,
     *,
     client: AuthenticatedClient,
-    idempotency_key: Union[Unset, str] = UNSET,
-) -> IntegrationKeyOut:
-    """Rotate Integration Key
+) -> IntegrationOut:
+    """Get Integration
 
-     Rotate the integration's key. The previous key will be immediately revoked.
+     Get an integration.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         integ_id (str): The integ's ID Example: integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
-        idempotency_key (Union[Unset, str]):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        IntegrationKeyOut
+        IntegrationOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        integ_id=integ_id,
-        client=client,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            integ_id=integ_id,
+            client=client,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/integration/v1_integration_update.py` & `svix-1.5.0/svix/internal/openapi_client/api/integration/v1_integration_update.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.integration_out import IntegrationOut
 from ...models.integration_update import IntegrationUpdate
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     integ_id: str,
     *,
     client: AuthenticatedClient,
@@ -28,84 +33,95 @@
 
     return {
         "method": "put",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> IntegrationOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> IntegrationOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = IntegrationOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = IntegrationOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[IntegrationOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     integ_id: str,
     *,
     client: AuthenticatedClient,
     json_body: IntegrationUpdate,
-) -> IntegrationOut:
+) -> Response[IntegrationOut]:
     """Update Integration
 
      Update an integration.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         integ_id (str): The integ's ID Example: integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         json_body (IntegrationUpdate):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        IntegrationOut
+        Response[IntegrationOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         integ_id=integ_id,
         client=client,
         json_body=json_body,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     integ_id: str,
     *,
     client: AuthenticatedClient,
@@ -116,68 +132,73 @@
      Update an integration.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         integ_id (str): The integ's ID Example: integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         json_body (IntegrationUpdate):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         IntegrationOut
     """
 
     return sync_detailed(
         app_id=app_id,
         integ_id=integ_id,
         client=client,
         json_body=json_body,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     integ_id: str,
     *,
     client: AuthenticatedClient,
     json_body: IntegrationUpdate,
-) -> IntegrationOut:
+) -> Response[IntegrationOut]:
     """Update Integration
 
      Update an integration.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         integ_id (str): The integ's ID Example: integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         json_body (IntegrationUpdate):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        IntegrationOut
+        Response[IntegrationOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         integ_id=integ_id,
         client=client,
         json_body=json_body,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     integ_id: str,
     *,
     client: AuthenticatedClient,
@@ -188,17 +209,23 @@
      Update an integration.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         integ_id (str): The integ's ID Example: integ_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         json_body (IntegrationUpdate):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         IntegrationOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        integ_id=integ_id,
-        client=client,
-        json_body=json_body,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            integ_id=integ_id,
+            client=client,
+            json_body=json_body,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/message/create_message_attempt_for_endpoint.py` & `svix-1.5.0/svix/internal/openapi_client/api/message/create_message_attempt_for_endpoint.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_attempt_out import MessageAttemptOut
 from ...models.message_in import MessageIn
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -35,90 +39,101 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> MessageAttemptOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> MessageAttemptOut:
+    if response.status_code == HTTPStatus.CREATED:
+        response_201 = MessageAttemptOut.from_dict(response.json())
+
+        return response_201
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_201 = MessageAttemptOut.from_dict(response.json())
-
-    return response_201
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[MessageAttemptOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
     json_body: MessageIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> MessageAttemptOut:
+) -> Response[MessageAttemptOut]:
     """Create Message Attempt For Endpoint
 
      Creates and sends a message to the specified endpoint. The message attempt and response from the
     endpoint is returned.
     FIXME: use MessageIn for expediency, even though the `application` parameter is unused. Since this
     endpoint isn't publicly documented anyway, it should be fine
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (MessageIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        MessageAttemptOut
+        Response[MessageAttemptOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -134,75 +149,80 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (MessageIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         MessageAttemptOut
     """
 
     return sync_detailed(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
     json_body: MessageIn,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> MessageAttemptOut:
+) -> Response[MessageAttemptOut]:
     """Create Message Attempt For Endpoint
 
      Creates and sends a message to the specified endpoint. The message attempt and response from the
     endpoint is returned.
     FIXME: use MessageIn for expediency, even though the `application` parameter is unused. Since this
     endpoint isn't publicly documented anyway, it should be fine
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (MessageIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        MessageAttemptOut
+        Response[MessageAttemptOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         json_body=json_body,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -218,18 +238,24 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
         json_body (MessageIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         MessageAttemptOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        endpoint_id=endpoint_id,
-        client=client,
-        json_body=json_body,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            endpoint_id=endpoint_id,
+            client=client,
+            json_body=json_body,
+            idempotency_key=idempotency_key,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/message/v1_message_create.py` & `svix-1.5.0/svix/internal/openapi_client/api/message/v1_message_create.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_in import MessageIn
 from ...models.message_out import MessageOut
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     *,
     client: AuthenticatedClient,
     json_body: MessageIn,
@@ -38,49 +42,59 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "json": json_json_body,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> MessageOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> MessageOut:
+    if response.status_code == HTTPStatus.ACCEPTED:
+        response_202 = MessageOut.from_dict(response.json())
+
+        return response_202
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_202 = MessageOut.from_dict(response.json())
-
-    return response_202
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[MessageOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     *,
     client: AuthenticatedClient,
     json_body: MessageIn,
     with_content: Union[Unset, None, bool] = True,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> MessageOut:
+) -> Response[MessageOut]:
     """Create Message
 
      Creates a new message and dispatches it to all of the application's endpoints.
 
     The `eventId` is an optional custom unique ID. It's verified to be unique only up to a day, after
     that no verification will be made.
     If a message with the same `eventId` already exists for any application in your environment, a 409
@@ -98,43 +112,44 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         with_content (Union[Unset, None, bool]):  Default: True.
         idempotency_key (Union[Unset, str]):
         json_body (MessageIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        MessageOut
+        Response[MessageOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         client=client,
         json_body=json_body,
         with_content=with_content,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     *,
     client: AuthenticatedClient,
     json_body: MessageIn,
@@ -162,35 +177,39 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         with_content (Union[Unset, None, bool]):  Default: True.
         idempotency_key (Union[Unset, str]):
         json_body (MessageIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         MessageOut
     """
 
     return sync_detailed(
         app_id=app_id,
         client=client,
         json_body=json_body,
         with_content=with_content,
         idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     *,
     client: AuthenticatedClient,
     json_body: MessageIn,
     with_content: Union[Unset, None, bool] = True,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> MessageOut:
+) -> Response[MessageOut]:
     """Create Message
 
      Creates a new message and dispatches it to all of the application's endpoints.
 
     The `eventId` is an optional custom unique ID. It's verified to be unique only up to a day, after
     that no verification will be made.
     If a message with the same `eventId` already exists for any application in your environment, a 409
@@ -208,41 +227,42 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         with_content (Union[Unset, None, bool]):  Default: True.
         idempotency_key (Union[Unset, str]):
         json_body (MessageIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        MessageOut
+        Response[MessageOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         client=client,
         json_body=json_body,
         with_content=with_content,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     *,
     client: AuthenticatedClient,
     json_body: MessageIn,
@@ -270,18 +290,24 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         with_content (Union[Unset, None, bool]):  Default: True.
         idempotency_key (Union[Unset, str]):
         json_body (MessageIn):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         MessageOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        client=client,
-        json_body=json_body,
-        with_content=with_content,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            client=client,
+            json_body=json_body,
+            with_content=with_content,
+            idempotency_key=idempotency_key,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/message/v1_message_expunge_content.py` & `svix-1.5.0/svix/internal/openapi_client/api/message/v1_message_expunge_content.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import random
 from http import HTTPStatus
 from time import sleep
-from typing import Any, Dict
+from typing import Any, Dict, cast
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     msg_id: str,
     *,
     client: AuthenticatedClient,
@@ -23,82 +28,93 @@
 
     return {
         "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> None:
+def _parse_response(*, client: Client, response: httpx.Response) -> Any:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_204 = None
-    return response_204
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[None]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     msg_id: str,
     *,
     client: AuthenticatedClient,
-) -> None:
+) -> Response[None]:
     """Delete message payload
 
      Delete the given message's payload. Useful in cases when a message was accidentally sent with
     sensitive content.
 
     The message can't be replayed or resent once its payload has been deleted or expired.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        None
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         msg_id=msg_id,
         client=client,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     msg_id: str,
     *,
     client: AuthenticatedClient,
@@ -110,67 +126,72 @@
 
     The message can't be replayed or resent once its payload has been deleted or expired.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         None
     """
 
     return sync_detailed(
         app_id=app_id,
         msg_id=msg_id,
         client=client,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     msg_id: str,
     *,
     client: AuthenticatedClient,
-) -> None:
+) -> Response[None]:
     """Delete message payload
 
      Delete the given message's payload. Useful in cases when a message was accidentally sent with
     sensitive content.
 
     The message can't be replayed or resent once its payload has been deleted or expired.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        None
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         msg_id=msg_id,
         client=client,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     msg_id: str,
     *,
     client: AuthenticatedClient,
@@ -182,16 +203,22 @@
 
     The message can't be replayed or resent once its payload has been deleted or expired.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         None
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        msg_id=msg_id,
-        client=client,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            msg_id=msg_id,
+            client=client,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/message/v1_message_get.py` & `svix-1.5.0/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_expunge_content.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,207 +1,231 @@
 import random
 from http import HTTPStatus
 from time import sleep
-from typing import Any, Dict, Union
+from typing import Any, Dict, cast
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...models.message_out import MessageOut
-from ...types import UNSET, Unset
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     msg_id: str,
+    attempt_id: str,
     *,
     client: AuthenticatedClient,
-    with_content: Union[Unset, None, bool] = True,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/app/{app_id}/msg/{msg_id}/".format(client.base_url, app_id=app_id, msg_id=msg_id)
+    url = "{}/api/v1/app/{app_id}/msg/{msg_id}/attempt/{attempt_id}/content/".format(
+        client.base_url, app_id=app_id, msg_id=msg_id, attempt_id=attempt_id
+    )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    params: Dict[str, Any] = {}
-    params["with_content"] = with_content
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
     return {
-        "method": "get",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "params": params,
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> MessageOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> Any:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = cast(Any, None)
+        return response_204
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = MessageOut.from_dict(response.json())
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
-    return response_200
 
-
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[None]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     msg_id: str,
+    attempt_id: str,
     *,
     client: AuthenticatedClient,
-    with_content: Union[Unset, None, bool] = True,
-) -> MessageOut:
-    """Get Message
+) -> Response[None]:
+    """Delete attempt response body
 
-     Get a message by its ID or eventID.
+     Deletes the given attempt's response body. Useful when an endpoint accidentally returned sensitive
+    content.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
-        with_content (Union[Unset, None, bool]):  Default: True.
+        attempt_id (str): The attempt's ID Example: atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        MessageOut
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         msg_id=msg_id,
+        attempt_id=attempt_id,
         client=client,
-        with_content=with_content,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     msg_id: str,
+    attempt_id: str,
     *,
     client: AuthenticatedClient,
-    with_content: Union[Unset, None, bool] = True,
-) -> MessageOut:
-    """Get Message
+) -> None:
+    """Delete attempt response body
 
-     Get a message by its ID or eventID.
+     Deletes the given attempt's response body. Useful when an endpoint accidentally returned sensitive
+    content.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
-        with_content (Union[Unset, None, bool]):  Default: True.
+        attempt_id (str): The attempt's ID Example: atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        MessageOut
+        None
     """
 
     return sync_detailed(
         app_id=app_id,
         msg_id=msg_id,
+        attempt_id=attempt_id,
         client=client,
-        with_content=with_content,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     msg_id: str,
+    attempt_id: str,
     *,
     client: AuthenticatedClient,
-    with_content: Union[Unset, None, bool] = True,
-) -> MessageOut:
-    """Get Message
+) -> Response[None]:
+    """Delete attempt response body
 
-     Get a message by its ID or eventID.
+     Deletes the given attempt's response body. Useful when an endpoint accidentally returned sensitive
+    content.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
-        with_content (Union[Unset, None, bool]):  Default: True.
+        attempt_id (str): The attempt's ID Example: atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        MessageOut
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         msg_id=msg_id,
+        attempt_id=attempt_id,
         client=client,
-        with_content=with_content,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     msg_id: str,
+    attempt_id: str,
     *,
     client: AuthenticatedClient,
-    with_content: Union[Unset, None, bool] = True,
-) -> MessageOut:
-    """Get Message
+) -> None:
+    """Delete attempt response body
 
-     Get a message by its ID or eventID.
+     Deletes the given attempt's response body. Useful when an endpoint accidentally returned sensitive
+    content.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
-        with_content (Union[Unset, None, bool]):  Default: True.
+        attempt_id (str): The attempt's ID Example: atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        MessageOut
+        None
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        msg_id=msg_id,
-        client=client,
-        with_content=with_content,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            msg_id=msg_id,
+            attempt_id=attempt_id,
+            client=client,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/message/v1_message_list.py` & `svix-1.5.0/svix/internal/openapi_client/api/message/v1_message_list.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, List, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.list_response_message_out import ListResponseMessageOut
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
@@ -64,52 +68,62 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> ListResponseMessageOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> ListResponseMessageOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ListResponseMessageOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = ListResponseMessageOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ListResponseMessageOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     channel: Union[Unset, None, str] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     with_content: Union[Unset, None, bool] = False,
     event_types: Union[Unset, None, List[str]] = UNSET,
-) -> ListResponseMessageOut:
+) -> Response[ListResponseMessageOut]:
     """List Messages
 
      List all of the application's messages.
 
     The `before` and `after` parameters let you filter all items created before or after a certain date.
     These can be used alongside an iterator to paginate over results
     within a certain window.
@@ -120,16 +134,20 @@
         iterator (Union[Unset, None, str]): The msg's ID Example: msg_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         channel (Union[Unset, None, str]):  Example: project_1337.
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         with_content (Union[Unset, None, bool]):
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseMessageOut
+        Response[ListResponseMessageOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         client=client,
         limit=limit,
         iterator=iterator,
@@ -138,29 +156,26 @@
         after=after,
         with_content=with_content,
         event_types=event_types,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
@@ -185,43 +200,47 @@
         iterator (Union[Unset, None, str]): The msg's ID Example: msg_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         channel (Union[Unset, None, str]):  Example: project_1337.
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         with_content (Union[Unset, None, bool]):
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseMessageOut
     """
 
     return sync_detailed(
         app_id=app_id,
         client=client,
         limit=limit,
         iterator=iterator,
         channel=channel,
         before=before,
         after=after,
         with_content=with_content,
         event_types=event_types,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     channel: Union[Unset, None, str] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     with_content: Union[Unset, None, bool] = False,
     event_types: Union[Unset, None, List[str]] = UNSET,
-) -> ListResponseMessageOut:
+) -> Response[ListResponseMessageOut]:
     """List Messages
 
      List all of the application's messages.
 
     The `before` and `after` parameters let you filter all items created before or after a certain date.
     These can be used alongside an iterator to paginate over results
     within a certain window.
@@ -232,16 +251,20 @@
         iterator (Union[Unset, None, str]): The msg's ID Example: msg_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         channel (Union[Unset, None, str]):  Example: project_1337.
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         with_content (Union[Unset, None, bool]):
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseMessageOut
+        Response[ListResponseMessageOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         client=client,
         limit=limit,
         iterator=iterator,
@@ -251,26 +274,23 @@
         with_content=with_content,
         event_types=event_types,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
@@ -295,22 +315,28 @@
         iterator (Union[Unset, None, str]): The msg's ID Example: msg_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         channel (Union[Unset, None, str]):  Example: project_1337.
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         with_content (Union[Unset, None, bool]):
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseMessageOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        client=client,
-        limit=limit,
-        iterator=iterator,
-        channel=channel,
-        before=before,
-        after=after,
-        with_content=with_content,
-        event_types=event_types,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            client=client,
+            limit=limit,
+            iterator=iterator,
+            channel=channel,
+            before=before,
+            after=after,
+            with_content=with_content,
+            event_types=event_types,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_expunge_content.py` & `svix-1.5.0/svix/internal/openapi_client/api/application/patch_application.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,204 +1,218 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
+from ...models.application_out import ApplicationOut
+from ...models.application_patch import ApplicationPatch
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
-    msg_id: str,
-    attempt_id: str,
     *,
     client: AuthenticatedClient,
+    json_body: ApplicationPatch,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/app/{app_id}/msg/{msg_id}/attempt/{attempt_id}/content/".format(
-        client.base_url, app_id=app_id, msg_id=msg_id, attempt_id=attempt_id
-    )
+    url = "{}/api/v1/app/{app_id}/".format(client.base_url, app_id=app_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
+    json_json_body = json_body.to_dict()
+
     return {
-        "method": "delete",
+        "method": "patch",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> None:
+def _parse_response(*, client: Client, response: httpx.Response) -> ApplicationOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ApplicationOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_204 = None
-    return response_204
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ApplicationOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
-    msg_id: str,
-    attempt_id: str,
     *,
     client: AuthenticatedClient,
-) -> None:
-    """Delete attempt response body
+    json_body: ApplicationPatch,
+) -> Response[ApplicationOut]:
+    """Patch Application
 
-     Deletes the given attempt's response body. Useful when an endpoint accidentally returned sensitive
-    content.
+     Partially update an application.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
-        attempt_id (str): The attempt's ID Example: atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
+        json_body (ApplicationPatch):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        None
+        Response[ApplicationOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
-        msg_id=msg_id,
-        attempt_id=attempt_id,
         client=client,
+        json_body=json_body,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
-    msg_id: str,
-    attempt_id: str,
     *,
     client: AuthenticatedClient,
-) -> None:
-    """Delete attempt response body
+    json_body: ApplicationPatch,
+) -> ApplicationOut:
+    """Patch Application
 
-     Deletes the given attempt's response body. Useful when an endpoint accidentally returned sensitive
-    content.
+     Partially update an application.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
-        attempt_id (str): The attempt's ID Example: atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
+        json_body (ApplicationPatch):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        None
+        ApplicationOut
     """
 
     return sync_detailed(
         app_id=app_id,
-        msg_id=msg_id,
-        attempt_id=attempt_id,
         client=client,
-    )
+        json_body=json_body,
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
-    msg_id: str,
-    attempt_id: str,
     *,
     client: AuthenticatedClient,
-) -> None:
-    """Delete attempt response body
+    json_body: ApplicationPatch,
+) -> Response[ApplicationOut]:
+    """Patch Application
 
-     Deletes the given attempt's response body. Useful when an endpoint accidentally returned sensitive
-    content.
+     Partially update an application.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
-        attempt_id (str): The attempt's ID Example: atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
+        json_body (ApplicationPatch):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        None
+        Response[ApplicationOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
-        msg_id=msg_id,
-        attempt_id=attempt_id,
         client=client,
+        json_body=json_body,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
-    msg_id: str,
-    attempt_id: str,
     *,
     client: AuthenticatedClient,
-) -> None:
-    """Delete attempt response body
+    json_body: ApplicationPatch,
+) -> ApplicationOut:
+    """Patch Application
 
-     Deletes the given attempt's response body. Useful when an endpoint accidentally returned sensitive
-    content.
+     Partially update an application.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
-        attempt_id (str): The attempt's ID Example: atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
+        json_body (ApplicationPatch):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        None
+        ApplicationOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        msg_id=msg_id,
-        attempt_id=attempt_id,
-        client=client,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            client=client,
+            json_body=json_body,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_get_headers.py` & `svix-1.5.0/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_get_headers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.message_attempt_headers_out import MessageAttemptHeadersOut
+from ...types import Response
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     msg_id: str,
     attempt_id: str,
     *,
@@ -27,83 +32,94 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> MessageAttemptHeadersOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> MessageAttemptHeadersOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = MessageAttemptHeadersOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = MessageAttemptHeadersOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[MessageAttemptHeadersOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     msg_id: str,
     attempt_id: str,
     *,
     client: AuthenticatedClient,
-) -> MessageAttemptHeadersOut:
+) -> Response[MessageAttemptHeadersOut]:
     """Get Attempt Headers
 
      Calculate and return headers used on a given message attempt
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
         attempt_id (str): The attempt's ID Example: atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        MessageAttemptHeadersOut
+        Response[MessageAttemptHeadersOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         msg_id=msg_id,
         attempt_id=attempt_id,
         client=client,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     msg_id: str,
     attempt_id: str,
     *,
@@ -114,68 +130,73 @@
      Calculate and return headers used on a given message attempt
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
         attempt_id (str): The attempt's ID Example: atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         MessageAttemptHeadersOut
     """
 
     return sync_detailed(
         app_id=app_id,
         msg_id=msg_id,
         attempt_id=attempt_id,
         client=client,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     msg_id: str,
     attempt_id: str,
     *,
     client: AuthenticatedClient,
-) -> MessageAttemptHeadersOut:
+) -> Response[MessageAttemptHeadersOut]:
     """Get Attempt Headers
 
      Calculate and return headers used on a given message attempt
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
         attempt_id (str): The attempt's ID Example: atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        MessageAttemptHeadersOut
+        Response[MessageAttemptHeadersOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         msg_id=msg_id,
         attempt_id=attempt_id,
         client=client,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     msg_id: str,
     attempt_id: str,
     *,
@@ -186,17 +207,23 @@
      Calculate and return headers used on a given message attempt
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
         attempt_id (str): The attempt's ID Example: atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         MessageAttemptHeadersOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        msg_id=msg_id,
-        attempt_id=attempt_id,
-        client=client,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            msg_id=msg_id,
+            attempt_id=attempt_id,
+            client=client,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_attempted_destinations.py` & `svix-1.5.0/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_attempted_destinations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.list_response_message_endpoint_out import ListResponseMessageEndpointOut
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     msg_id: str,
     *,
     client: AuthenticatedClient,
@@ -34,87 +38,98 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> ListResponseMessageEndpointOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> ListResponseMessageEndpointOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ListResponseMessageEndpointOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = ListResponseMessageEndpointOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ListResponseMessageEndpointOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     msg_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
-) -> ListResponseMessageEndpointOut:
+) -> Response[ListResponseMessageEndpointOut]:
     """List Attempted Destinations
 
      `msg_id`: Use a message id or a message `eventId`
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseMessageEndpointOut
+        Response[ListResponseMessageEndpointOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         msg_id=msg_id,
         client=client,
         limit=limit,
         iterator=iterator,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     msg_id: str,
     *,
     client: AuthenticatedClient,
@@ -127,72 +142,77 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseMessageEndpointOut
     """
 
     return sync_detailed(
         app_id=app_id,
         msg_id=msg_id,
         client=client,
         limit=limit,
         iterator=iterator,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     msg_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
-) -> ListResponseMessageEndpointOut:
+) -> Response[ListResponseMessageEndpointOut]:
     """List Attempted Destinations
 
      `msg_id`: Use a message id or a message `eventId`
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseMessageEndpointOut
+        Response[ListResponseMessageEndpointOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         msg_id=msg_id,
         client=client,
         limit=limit,
         iterator=iterator,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     msg_id: str,
     *,
     client: AuthenticatedClient,
@@ -205,18 +225,24 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseMessageEndpointOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        msg_id=msg_id,
-        client=client,
-        limit=limit,
-        iterator=iterator,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            msg_id=msg_id,
+            client=client,
+            limit=limit,
+            iterator=iterator,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_attempted_messages.py` & `svix-1.5.0/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_attempted_messages.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,24 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.list_response_endpoint_message_out import ListResponseEndpointMessageOut
 from ...models.message_status import MessageStatus
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -65,53 +69,63 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> ListResponseEndpointMessageOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> ListResponseEndpointMessageOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ListResponseEndpointMessageOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = ListResponseEndpointMessageOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ListResponseEndpointMessageOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     channel: Union[Unset, None, str] = UNSET,
     status: Union[Unset, None, MessageStatus] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     with_content: Union[Unset, None, bool] = False,
-) -> ListResponseEndpointMessageOut:
+) -> Response[ListResponseEndpointMessageOut]:
     """List Attempted Messages
 
      List messages for a particular endpoint. Additionally includes metadata about the latest message
     attempt.
 
     The `before` parameter lets you filter all items created before a certain date and is ignored if an
     iterator is passed.
@@ -127,16 +141,20 @@
             - Pending = 1
             - Fail = 2
             - Sending = 3
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         with_content (Union[Unset, None, bool]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseEndpointMessageOut
+        Response[ListResponseEndpointMessageOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         limit=limit,
@@ -146,29 +164,26 @@
         before=before,
         after=after,
         with_content=with_content,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -199,14 +214,18 @@
             - Pending = 1
             - Fail = 2
             - Sending = 3
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         with_content (Union[Unset, None, bool]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseEndpointMessageOut
     """
 
     return sync_detailed(
         app_id=app_id,
         endpoint_id=endpoint_id,
@@ -214,30 +233,30 @@
         limit=limit,
         iterator=iterator,
         channel=channel,
         status=status,
         before=before,
         after=after,
         with_content=with_content,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     channel: Union[Unset, None, str] = UNSET,
     status: Union[Unset, None, MessageStatus] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     with_content: Union[Unset, None, bool] = False,
-) -> ListResponseEndpointMessageOut:
+) -> Response[ListResponseEndpointMessageOut]:
     """List Attempted Messages
 
      List messages for a particular endpoint. Additionally includes metadata about the latest message
     attempt.
 
     The `before` parameter lets you filter all items created before a certain date and is ignored if an
     iterator is passed.
@@ -253,16 +272,20 @@
             - Pending = 1
             - Fail = 2
             - Sending = 3
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         with_content (Union[Unset, None, bool]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseEndpointMessageOut
+        Response[ListResponseEndpointMessageOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         limit=limit,
@@ -273,26 +296,23 @@
         after=after,
         with_content=with_content,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -323,23 +343,29 @@
             - Pending = 1
             - Fail = 2
             - Sending = 3
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         with_content (Union[Unset, None, bool]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseEndpointMessageOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        endpoint_id=endpoint_id,
-        client=client,
-        limit=limit,
-        iterator=iterator,
-        channel=channel,
-        status=status,
-        before=before,
-        after=after,
-        with_content=with_content,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            endpoint_id=endpoint_id,
+            client=client,
+            limit=limit,
+            iterator=iterator,
+            channel=channel,
+            status=status,
+            before=before,
+            after=after,
+            with_content=with_content,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_by_endpoint.py` & `svix-1.5.0/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_by_msg.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,40 +2,43 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, List, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.list_response_message_attempt_out import ListResponseMessageAttemptOut
 from ...models.message_status import MessageStatus
 from ...models.status_code_class import StatusCodeClass
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
-    endpoint_id: str,
+    msg_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     status: Union[Unset, None, MessageStatus] = UNSET,
     status_code_class: Union[Unset, None, StatusCodeClass] = UNSET,
     channel: Union[Unset, None, str] = UNSET,
+    endpoint_id: Union[Unset, None, str] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     event_types: Union[Unset, None, List[str]] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/app/{app_id}/attempt/endpoint/{endpoint_id}/".format(
-        client.base_url, app_id=app_id, endpoint_id=endpoint_id
-    )
+    url = "{}/api/v1/app/{app_id}/attempt/msg/{msg_id}/".format(client.base_url, app_id=app_id, msg_id=msg_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["limit"] = limit
 
@@ -51,14 +54,16 @@
     if not isinstance(status_code_class, Unset):
         json_status_code_class = status_code_class.value if status_code_class else None
 
     params["status_code_class"] = json_status_code_class
 
     params["channel"] = channel
 
+    params["endpoint_id"] = endpoint_id
+
     json_before: Union[Unset, None, str] = UNSET
     if not isinstance(before, Unset):
         json_before = before.isoformat() if before else None
 
     params["before"] = json_before
 
     json_after: Union[Unset, None, str] = UNSET
@@ -80,61 +85,72 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> ListResponseMessageAttemptOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> ListResponseMessageAttemptOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ListResponseMessageAttemptOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = ListResponseMessageAttemptOut.from_dict(response.json())
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
-    return response_200
 
-
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ListResponseMessageAttemptOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
-    endpoint_id: str,
+    msg_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     status: Union[Unset, None, MessageStatus] = UNSET,
     status_code_class: Union[Unset, None, StatusCodeClass] = UNSET,
     channel: Union[Unset, None, str] = UNSET,
+    endpoint_id: Union[Unset, None, str] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     event_types: Union[Unset, None, List[str]] = UNSET,
-) -> ListResponseMessageAttemptOut:
-    """List Attempts By Endpoint
+) -> Response[ListResponseMessageAttemptOut]:
+    """List Attempts By Msg
 
-     List attempts by endpoint id
+     List attempts by message id
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
+        msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The attempt's ID Example:
             atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         status (Union[Unset, None, MessageStatus]): The sending status of the message:
             - Success = 0
             - Pending = 1
             - Fail = 2
@@ -144,76 +160,80 @@
             - CodeNone = 0
             - Code1xx = 100
             - Code2xx = 200
             - Code3xx = 300
             - Code4xx = 400
             - Code5xx = 500
         channel (Union[Unset, None, str]):  Example: project_1337.
+        endpoint_id (Union[Unset, None, str]): The ep's ID or UID Example: unique-ep-identifier.
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseMessageAttemptOut
+        Response[ListResponseMessageAttemptOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
-        endpoint_id=endpoint_id,
+        msg_id=msg_id,
         client=client,
         limit=limit,
         iterator=iterator,
         status=status,
         status_code_class=status_code_class,
         channel=channel,
+        endpoint_id=endpoint_id,
         before=before,
         after=after,
         event_types=event_types,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
-    endpoint_id: str,
+    msg_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     status: Union[Unset, None, MessageStatus] = UNSET,
     status_code_class: Union[Unset, None, StatusCodeClass] = UNSET,
     channel: Union[Unset, None, str] = UNSET,
+    endpoint_id: Union[Unset, None, str] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     event_types: Union[Unset, None, List[str]] = UNSET,
 ) -> ListResponseMessageAttemptOut:
-    """List Attempts By Endpoint
+    """List Attempts By Msg
 
-     List attempts by endpoint id
+     List attempts by message id
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
+        msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The attempt's ID Example:
             atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         status (Union[Unset, None, MessageStatus]): The sending status of the message:
             - Success = 0
             - Pending = 1
             - Fail = 2
@@ -223,58 +243,65 @@
             - CodeNone = 0
             - Code1xx = 100
             - Code2xx = 200
             - Code3xx = 300
             - Code4xx = 400
             - Code5xx = 500
         channel (Union[Unset, None, str]):  Example: project_1337.
+        endpoint_id (Union[Unset, None, str]): The ep's ID or UID Example: unique-ep-identifier.
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseMessageAttemptOut
     """
 
     return sync_detailed(
         app_id=app_id,
-        endpoint_id=endpoint_id,
+        msg_id=msg_id,
         client=client,
         limit=limit,
         iterator=iterator,
         status=status,
         status_code_class=status_code_class,
         channel=channel,
+        endpoint_id=endpoint_id,
         before=before,
         after=after,
         event_types=event_types,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
-    endpoint_id: str,
+    msg_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     status: Union[Unset, None, MessageStatus] = UNSET,
     status_code_class: Union[Unset, None, StatusCodeClass] = UNSET,
     channel: Union[Unset, None, str] = UNSET,
+    endpoint_id: Union[Unset, None, str] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     event_types: Union[Unset, None, List[str]] = UNSET,
-) -> ListResponseMessageAttemptOut:
-    """List Attempts By Endpoint
+) -> Response[ListResponseMessageAttemptOut]:
+    """List Attempts By Msg
 
-     List attempts by endpoint id
+     List attempts by message id
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
+        msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The attempt's ID Example:
             atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         status (Union[Unset, None, MessageStatus]): The sending status of the message:
             - Success = 0
             - Pending = 1
             - Fail = 2
@@ -284,74 +311,78 @@
             - CodeNone = 0
             - Code1xx = 100
             - Code2xx = 200
             - Code3xx = 300
             - Code4xx = 400
             - Code5xx = 500
         channel (Union[Unset, None, str]):  Example: project_1337.
+        endpoint_id (Union[Unset, None, str]): The ep's ID or UID Example: unique-ep-identifier.
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseMessageAttemptOut
+        Response[ListResponseMessageAttemptOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
-        endpoint_id=endpoint_id,
+        msg_id=msg_id,
         client=client,
         limit=limit,
         iterator=iterator,
         status=status,
         status_code_class=status_code_class,
         channel=channel,
+        endpoint_id=endpoint_id,
         before=before,
         after=after,
         event_types=event_types,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
-    endpoint_id: str,
+    msg_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     status: Union[Unset, None, MessageStatus] = UNSET,
     status_code_class: Union[Unset, None, StatusCodeClass] = UNSET,
     channel: Union[Unset, None, str] = UNSET,
+    endpoint_id: Union[Unset, None, str] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     event_types: Union[Unset, None, List[str]] = UNSET,
 ) -> ListResponseMessageAttemptOut:
-    """List Attempts By Endpoint
+    """List Attempts By Msg
 
-     List attempts by endpoint id
+     List attempts by message id
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
+        msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The attempt's ID Example:
             atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         status (Union[Unset, None, MessageStatus]): The sending status of the message:
             - Success = 0
             - Pending = 1
             - Fail = 2
@@ -361,28 +392,36 @@
             - CodeNone = 0
             - Code1xx = 100
             - Code2xx = 200
             - Code3xx = 300
             - Code4xx = 400
             - Code5xx = 500
         channel (Union[Unset, None, str]):  Example: project_1337.
+        endpoint_id (Union[Unset, None, str]): The ep's ID or UID Example: unique-ep-identifier.
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseMessageAttemptOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        endpoint_id=endpoint_id,
-        client=client,
-        limit=limit,
-        iterator=iterator,
-        status=status,
-        status_code_class=status_code_class,
-        channel=channel,
-        before=before,
-        after=after,
-        event_types=event_types,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            msg_id=msg_id,
+            client=client,
+            limit=limit,
+            iterator=iterator,
+            status=status,
+            status_code_class=status_code_class,
+            channel=channel,
+            endpoint_id=endpoint_id,
+            before=before,
+            after=after,
+            event_types=event_types,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_by_endpoint_deprecated.py` & `svix-1.5.0/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_by_endpoint_deprecated.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,24 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, List, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.list_response_message_attempt_endpoint_out import ListResponseMessageAttemptEndpointOut
 from ...models.message_status import MessageStatus
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     msg_id: str,
     endpoint_id: str,
     *,
@@ -73,38 +77,48 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> ListResponseMessageAttemptEndpointOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> ListResponseMessageAttemptEndpointOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ListResponseMessageAttemptEndpointOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = ListResponseMessageAttemptEndpointOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ListResponseMessageAttemptEndpointOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     msg_id: str,
     endpoint_id: str,
     *,
@@ -112,15 +126,15 @@
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     channel: Union[Unset, None, str] = UNSET,
     status: Union[Unset, None, MessageStatus] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     event_types: Union[Unset, None, List[str]] = UNSET,
-) -> ListResponseMessageAttemptEndpointOut:
+) -> Response[ListResponseMessageAttemptEndpointOut]:
     """List Attempts For Endpoint
 
      DEPRECATED: please use list_attempts with endpoint_id as a query parameter instead.
 
     List the message attempts for a particular endpoint.
 
     Returning the endpoint.
@@ -141,16 +155,20 @@
             - Pending = 1
             - Fail = 2
             - Sending = 3
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseMessageAttemptEndpointOut
+        Response[ListResponseMessageAttemptEndpointOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         msg_id=msg_id,
         endpoint_id=endpoint_id,
         client=client,
@@ -161,29 +179,26 @@
         before=before,
         after=after,
         event_types=event_types,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     msg_id: str,
     endpoint_id: str,
     *,
@@ -220,14 +235,18 @@
             - Pending = 1
             - Fail = 2
             - Sending = 3
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseMessageAttemptEndpointOut
     """
 
     return sync_detailed(
         app_id=app_id,
         msg_id=msg_id,
@@ -236,15 +255,15 @@
         limit=limit,
         iterator=iterator,
         channel=channel,
         status=status,
         before=before,
         after=after,
         event_types=event_types,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     msg_id: str,
     endpoint_id: str,
     *,
@@ -252,15 +271,15 @@
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     channel: Union[Unset, None, str] = UNSET,
     status: Union[Unset, None, MessageStatus] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     event_types: Union[Unset, None, List[str]] = UNSET,
-) -> ListResponseMessageAttemptEndpointOut:
+) -> Response[ListResponseMessageAttemptEndpointOut]:
     """List Attempts For Endpoint
 
      DEPRECATED: please use list_attempts with endpoint_id as a query parameter instead.
 
     List the message attempts for a particular endpoint.
 
     Returning the endpoint.
@@ -281,16 +300,20 @@
             - Pending = 1
             - Fail = 2
             - Sending = 3
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseMessageAttemptEndpointOut
+        Response[ListResponseMessageAttemptEndpointOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         msg_id=msg_id,
         endpoint_id=endpoint_id,
         client=client,
@@ -302,26 +325,23 @@
         after=after,
         event_types=event_types,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     msg_id: str,
     endpoint_id: str,
     *,
@@ -358,24 +378,30 @@
             - Pending = 1
             - Fail = 2
             - Sending = 3
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseMessageAttemptEndpointOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        msg_id=msg_id,
-        endpoint_id=endpoint_id,
-        client=client,
-        limit=limit,
-        iterator=iterator,
-        channel=channel,
-        status=status,
-        before=before,
-        after=after,
-        event_types=event_types,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            msg_id=msg_id,
+            endpoint_id=endpoint_id,
+            client=client,
+            limit=limit,
+            iterator=iterator,
+            channel=channel,
+            status=status,
+            before=before,
+            after=after,
+            event_types=event_types,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_by_msg.py` & `svix-1.5.0/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_by_endpoint.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,39 +2,44 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, List, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.list_response_message_attempt_out import ListResponseMessageAttemptOut
 from ...models.message_status import MessageStatus
 from ...models.status_code_class import StatusCodeClass
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
-    msg_id: str,
+    endpoint_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     status: Union[Unset, None, MessageStatus] = UNSET,
     status_code_class: Union[Unset, None, StatusCodeClass] = UNSET,
     channel: Union[Unset, None, str] = UNSET,
-    endpoint_id: Union[Unset, None, str] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     event_types: Union[Unset, None, List[str]] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/app/{app_id}/attempt/msg/{msg_id}/".format(client.base_url, app_id=app_id, msg_id=msg_id)
+    url = "{}/api/v1/app/{app_id}/attempt/endpoint/{endpoint_id}/".format(
+        client.base_url, app_id=app_id, endpoint_id=endpoint_id
+    )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["limit"] = limit
 
@@ -50,16 +55,14 @@
     if not isinstance(status_code_class, Unset):
         json_status_code_class = status_code_class.value if status_code_class else None
 
     params["status_code_class"] = json_status_code_class
 
     params["channel"] = channel
 
-    params["endpoint_id"] = endpoint_id
-
     json_before: Union[Unset, None, str] = UNSET
     if not isinstance(before, Unset):
         json_before = before.isoformat() if before else None
 
     params["before"] = json_before
 
     json_after: Union[Unset, None, str] = UNSET
@@ -81,62 +84,71 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> ListResponseMessageAttemptOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> ListResponseMessageAttemptOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ListResponseMessageAttemptOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = ListResponseMessageAttemptOut.from_dict(response.json())
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
-    return response_200
 
-
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ListResponseMessageAttemptOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
-    msg_id: str,
+    endpoint_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     status: Union[Unset, None, MessageStatus] = UNSET,
     status_code_class: Union[Unset, None, StatusCodeClass] = UNSET,
     channel: Union[Unset, None, str] = UNSET,
-    endpoint_id: Union[Unset, None, str] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     event_types: Union[Unset, None, List[str]] = UNSET,
-) -> ListResponseMessageAttemptOut:
-    """List Attempts By Msg
+) -> Response[ListResponseMessageAttemptOut]:
+    """List Attempts By Endpoint
 
-     List attempts by message id
+     List attempts by endpoint id
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
+        endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The attempt's ID Example:
             atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         status (Union[Unset, None, MessageStatus]): The sending status of the message:
             - Success = 0
             - Pending = 1
             - Fail = 2
@@ -146,79 +158,77 @@
             - CodeNone = 0
             - Code1xx = 100
             - Code2xx = 200
             - Code3xx = 300
             - Code4xx = 400
             - Code5xx = 500
         channel (Union[Unset, None, str]):  Example: project_1337.
-        endpoint_id (Union[Unset, None, str]): The ep's ID or UID Example: unique-ep-identifier.
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseMessageAttemptOut
+        Response[ListResponseMessageAttemptOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
-        msg_id=msg_id,
+        endpoint_id=endpoint_id,
         client=client,
         limit=limit,
         iterator=iterator,
         status=status,
         status_code_class=status_code_class,
         channel=channel,
-        endpoint_id=endpoint_id,
         before=before,
         after=after,
         event_types=event_types,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
-    msg_id: str,
+    endpoint_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     status: Union[Unset, None, MessageStatus] = UNSET,
     status_code_class: Union[Unset, None, StatusCodeClass] = UNSET,
     channel: Union[Unset, None, str] = UNSET,
-    endpoint_id: Union[Unset, None, str] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     event_types: Union[Unset, None, List[str]] = UNSET,
 ) -> ListResponseMessageAttemptOut:
-    """List Attempts By Msg
+    """List Attempts By Endpoint
 
-     List attempts by message id
+     List attempts by endpoint id
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
+        endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The attempt's ID Example:
             atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         status (Union[Unset, None, MessageStatus]): The sending status of the message:
             - Success = 0
             - Pending = 1
             - Fail = 2
@@ -228,61 +238,62 @@
             - CodeNone = 0
             - Code1xx = 100
             - Code2xx = 200
             - Code3xx = 300
             - Code4xx = 400
             - Code5xx = 500
         channel (Union[Unset, None, str]):  Example: project_1337.
-        endpoint_id (Union[Unset, None, str]): The ep's ID or UID Example: unique-ep-identifier.
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseMessageAttemptOut
     """
 
     return sync_detailed(
         app_id=app_id,
-        msg_id=msg_id,
+        endpoint_id=endpoint_id,
         client=client,
         limit=limit,
         iterator=iterator,
         status=status,
         status_code_class=status_code_class,
         channel=channel,
-        endpoint_id=endpoint_id,
         before=before,
         after=after,
         event_types=event_types,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
-    msg_id: str,
+    endpoint_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     status: Union[Unset, None, MessageStatus] = UNSET,
     status_code_class: Union[Unset, None, StatusCodeClass] = UNSET,
     channel: Union[Unset, None, str] = UNSET,
-    endpoint_id: Union[Unset, None, str] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     event_types: Union[Unset, None, List[str]] = UNSET,
-) -> ListResponseMessageAttemptOut:
-    """List Attempts By Msg
+) -> Response[ListResponseMessageAttemptOut]:
+    """List Attempts By Endpoint
 
-     List attempts by message id
+     List attempts by endpoint id
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
+        endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The attempt's ID Example:
             atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         status (Union[Unset, None, MessageStatus]): The sending status of the message:
             - Success = 0
             - Pending = 1
             - Fail = 2
@@ -292,77 +303,75 @@
             - CodeNone = 0
             - Code1xx = 100
             - Code2xx = 200
             - Code3xx = 300
             - Code4xx = 400
             - Code5xx = 500
         channel (Union[Unset, None, str]):  Example: project_1337.
-        endpoint_id (Union[Unset, None, str]): The ep's ID or UID Example: unique-ep-identifier.
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseMessageAttemptOut
+        Response[ListResponseMessageAttemptOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
-        msg_id=msg_id,
+        endpoint_id=endpoint_id,
         client=client,
         limit=limit,
         iterator=iterator,
         status=status,
         status_code_class=status_code_class,
         channel=channel,
-        endpoint_id=endpoint_id,
         before=before,
         after=after,
         event_types=event_types,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
-    msg_id: str,
+    endpoint_id: str,
     *,
     client: AuthenticatedClient,
     limit: Union[Unset, None, int] = UNSET,
     iterator: Union[Unset, None, str] = UNSET,
     status: Union[Unset, None, MessageStatus] = UNSET,
     status_code_class: Union[Unset, None, StatusCodeClass] = UNSET,
     channel: Union[Unset, None, str] = UNSET,
-    endpoint_id: Union[Unset, None, str] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     event_types: Union[Unset, None, List[str]] = UNSET,
 ) -> ListResponseMessageAttemptOut:
-    """List Attempts By Msg
+    """List Attempts By Endpoint
 
-     List attempts by message id
+     List attempts by endpoint id
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
-        msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
+        endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         limit (Union[Unset, None, int]):
         iterator (Union[Unset, None, str]): The attempt's ID Example:
             atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         status (Union[Unset, None, MessageStatus]): The sending status of the message:
             - Success = 0
             - Pending = 1
             - Fail = 2
@@ -372,30 +381,34 @@
             - CodeNone = 0
             - Code1xx = 100
             - Code2xx = 200
             - Code3xx = 300
             - Code4xx = 400
             - Code5xx = 500
         channel (Union[Unset, None, str]):  Example: project_1337.
-        endpoint_id (Union[Unset, None, str]): The ep's ID or UID Example: unique-ep-identifier.
         before (Union[Unset, None, datetime.datetime]):
         after (Union[Unset, None, datetime.datetime]):
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseMessageAttemptOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        msg_id=msg_id,
-        client=client,
-        limit=limit,
-        iterator=iterator,
-        status=status,
-        status_code_class=status_code_class,
-        channel=channel,
-        endpoint_id=endpoint_id,
-        before=before,
-        after=after,
-        event_types=event_types,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            endpoint_id=endpoint_id,
+            client=client,
+            limit=limit,
+            iterator=iterator,
+            status=status,
+            status_code_class=status_code_class,
+            channel=channel,
+            before=before,
+            after=after,
+            event_types=event_types,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_by_msg_deprecated.py` & `svix-1.5.0/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_list_by_msg_deprecated.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, List, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
 from ...models.list_response_message_attempt_out import ListResponseMessageAttemptOut
 from ...models.message_status import MessageStatus
 from ...models.status_code_class import StatusCodeClass
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     msg_id: str,
     *,
     client: AuthenticatedClient,
@@ -81,38 +85,48 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> ListResponseMessageAttemptOut:
+def _parse_response(*, client: Client, response: httpx.Response) -> ListResponseMessageAttemptOut:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ListResponseMessageAttemptOut.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = ListResponseMessageAttemptOut.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ListResponseMessageAttemptOut]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     msg_id: str,
     *,
     client: AuthenticatedClient,
@@ -121,16 +135,16 @@
     endpoint_id: Union[Unset, None, str] = UNSET,
     channel: Union[Unset, None, str] = UNSET,
     status: Union[Unset, None, MessageStatus] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     status_code_class: Union[Unset, None, StatusCodeClass] = UNSET,
     event_types: Union[Unset, None, List[str]] = UNSET,
-) -> ListResponseMessageAttemptOut:
-    """List Attempts
+) -> Response[ListResponseMessageAttemptOut]:
+    r"""List Attempts
 
      Deprecated: Please use \"List Attempts by Endpoint\" and \"List Attempts by Msg\" instead.
 
     `msg_id`: Use a message id or a message `eventId`
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
@@ -153,16 +167,20 @@
             - Code1xx = 100
             - Code2xx = 200
             - Code3xx = 300
             - Code4xx = 400
             - Code5xx = 500
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseMessageAttemptOut
+        Response[ListResponseMessageAttemptOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         msg_id=msg_id,
         client=client,
         limit=limit,
@@ -174,29 +192,26 @@
         after=after,
         status_code_class=status_code_class,
         event_types=event_types,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     msg_id: str,
     *,
     client: AuthenticatedClient,
@@ -206,15 +221,15 @@
     channel: Union[Unset, None, str] = UNSET,
     status: Union[Unset, None, MessageStatus] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     status_code_class: Union[Unset, None, StatusCodeClass] = UNSET,
     event_types: Union[Unset, None, List[str]] = UNSET,
 ) -> ListResponseMessageAttemptOut:
-    """List Attempts
+    r"""List Attempts
 
      Deprecated: Please use \"List Attempts by Endpoint\" and \"List Attempts by Msg\" instead.
 
     `msg_id`: Use a message id or a message `eventId`
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
@@ -237,14 +252,18 @@
             - Code1xx = 100
             - Code2xx = 200
             - Code3xx = 300
             - Code4xx = 400
             - Code5xx = 500
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseMessageAttemptOut
     """
 
     return sync_detailed(
         app_id=app_id,
         msg_id=msg_id,
@@ -254,15 +273,15 @@
         endpoint_id=endpoint_id,
         channel=channel,
         status=status,
         before=before,
         after=after,
         status_code_class=status_code_class,
         event_types=event_types,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     msg_id: str,
     *,
     client: AuthenticatedClient,
@@ -271,16 +290,16 @@
     endpoint_id: Union[Unset, None, str] = UNSET,
     channel: Union[Unset, None, str] = UNSET,
     status: Union[Unset, None, MessageStatus] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     status_code_class: Union[Unset, None, StatusCodeClass] = UNSET,
     event_types: Union[Unset, None, List[str]] = UNSET,
-) -> ListResponseMessageAttemptOut:
-    """List Attempts
+) -> Response[ListResponseMessageAttemptOut]:
+    r"""List Attempts
 
      Deprecated: Please use \"List Attempts by Endpoint\" and \"List Attempts by Msg\" instead.
 
     `msg_id`: Use a message id or a message `eventId`
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
@@ -303,16 +322,20 @@
             - Code1xx = 100
             - Code2xx = 200
             - Code3xx = 300
             - Code4xx = 400
             - Code5xx = 500
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        ListResponseMessageAttemptOut
+        Response[ListResponseMessageAttemptOut]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         msg_id=msg_id,
         client=client,
         limit=limit,
@@ -325,26 +348,23 @@
         status_code_class=status_code_class,
         event_types=event_types,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     msg_id: str,
     *,
     client: AuthenticatedClient,
@@ -354,15 +374,15 @@
     channel: Union[Unset, None, str] = UNSET,
     status: Union[Unset, None, MessageStatus] = UNSET,
     before: Union[Unset, None, datetime.datetime] = UNSET,
     after: Union[Unset, None, datetime.datetime] = UNSET,
     status_code_class: Union[Unset, None, StatusCodeClass] = UNSET,
     event_types: Union[Unset, None, List[str]] = UNSET,
 ) -> ListResponseMessageAttemptOut:
-    """List Attempts
+    r"""List Attempts
 
      Deprecated: Please use \"List Attempts by Endpoint\" and \"List Attempts by Msg\" instead.
 
     `msg_id`: Use a message id or a message `eventId`
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
@@ -385,25 +405,31 @@
             - Code1xx = 100
             - Code2xx = 200
             - Code3xx = 300
             - Code4xx = 400
             - Code5xx = 500
         event_types (Union[Unset, None, List[str]]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         ListResponseMessageAttemptOut
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        msg_id=msg_id,
-        client=client,
-        limit=limit,
-        iterator=iterator,
-        endpoint_id=endpoint_id,
-        channel=channel,
-        status=status,
-        before=before,
-        after=after,
-        status_code_class=status_code_class,
-        event_types=event_types,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            msg_id=msg_id,
+            client=client,
+            limit=limit,
+            iterator=iterator,
+            endpoint_id=endpoint_id,
+            channel=channel,
+            status=status,
+            before=before,
+            after=after,
+            status_code_class=status_code_class,
+            event_types=event_types,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_resend.py` & `svix-1.5.0/svix/internal/openapi_client/api/message_attempt/v1_message_attempt_resend.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import random
 from http import HTTPStatus
 from time import sleep
-from typing import Any, Dict, Union
+from typing import Any, Dict, Union, cast
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     msg_id: str,
     endpoint_id: str,
     *,
@@ -31,85 +35,96 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> None:
+def _parse_response(*, client: Client, response: httpx.Response) -> Any:
+    if response.status_code == HTTPStatus.ACCEPTED:
+        response_202 = cast(Any, None)
+        return response_202
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_202 = None
-    return response_202
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[None]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     msg_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> None:
+) -> Response[None]:
     """Resend Webhook
 
      Resend a message to the specified endpoint.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        None
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         msg_id=msg_id,
         endpoint_id=endpoint_id,
         client=client,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     msg_id: str,
     endpoint_id: str,
     *,
@@ -122,72 +137,77 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         None
     """
 
     return sync_detailed(
         app_id=app_id,
         msg_id=msg_id,
         endpoint_id=endpoint_id,
         client=client,
         idempotency_key=idempotency_key,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     msg_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
     idempotency_key: Union[Unset, str] = UNSET,
-) -> None:
+) -> Response[None]:
     """Resend Webhook
 
      Resend a message to the specified endpoint.
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        None
+        Response[None]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         msg_id=msg_id,
         endpoint_id=endpoint_id,
         client=client,
         idempotency_key=idempotency_key,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     msg_id: str,
     endpoint_id: str,
     *,
@@ -200,18 +220,24 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         msg_id (str): The msg's ID or UID Example: unique-msg-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         idempotency_key (Union[Unset, str]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         None
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        msg_id=msg_id,
-        endpoint_id=endpoint_id,
-        client=client,
-        idempotency_key=idempotency_key,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            msg_id=msg_id,
+            endpoint_id=endpoint_id,
+            client=client,
+            idempotency_key=idempotency_key,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/statistics/v1_stats_app_attempts.py` & `svix-1.5.0/svix/internal/openapi_client/api/statistics/v1_stats_app_attempts.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.attempt_statistics_response import AttemptStatisticsResponse
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     *,
     client: AuthenticatedClient,
     start_date: Union[Unset, None, datetime.datetime] = UNSET,
@@ -42,84 +46,95 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> AttemptStatisticsResponse:
+def _parse_response(*, client: Client, response: httpx.Response) -> AttemptStatisticsResponse:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = AttemptStatisticsResponse.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = AttemptStatisticsResponse.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[AttemptStatisticsResponse]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     *,
     client: AuthenticatedClient,
     start_date: Union[Unset, None, datetime.datetime] = UNSET,
     end_date: Union[Unset, None, datetime.datetime] = UNSET,
-) -> AttemptStatisticsResponse:
+) -> Response[AttemptStatisticsResponse]:
     """Get App Attempt Stats
 
      Returns application-level statistics on message attempts
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         start_date (Union[Unset, None, datetime.datetime]):
         end_date (Union[Unset, None, datetime.datetime]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        AttemptStatisticsResponse
+        Response[AttemptStatisticsResponse]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         client=client,
         start_date=start_date,
         end_date=end_date,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     *,
     client: AuthenticatedClient,
     start_date: Union[Unset, None, datetime.datetime] = UNSET,
@@ -130,68 +145,73 @@
      Returns application-level statistics on message attempts
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         start_date (Union[Unset, None, datetime.datetime]):
         end_date (Union[Unset, None, datetime.datetime]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         AttemptStatisticsResponse
     """
 
     return sync_detailed(
         app_id=app_id,
         client=client,
         start_date=start_date,
         end_date=end_date,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     *,
     client: AuthenticatedClient,
     start_date: Union[Unset, None, datetime.datetime] = UNSET,
     end_date: Union[Unset, None, datetime.datetime] = UNSET,
-) -> AttemptStatisticsResponse:
+) -> Response[AttemptStatisticsResponse]:
     """Get App Attempt Stats
 
      Returns application-level statistics on message attempts
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         start_date (Union[Unset, None, datetime.datetime]):
         end_date (Union[Unset, None, datetime.datetime]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        AttemptStatisticsResponse
+        Response[AttemptStatisticsResponse]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         client=client,
         start_date=start_date,
         end_date=end_date,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     *,
     client: AuthenticatedClient,
     start_date: Union[Unset, None, datetime.datetime] = UNSET,
@@ -202,17 +222,23 @@
      Returns application-level statistics on message attempts
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         start_date (Union[Unset, None, datetime.datetime]):
         end_date (Union[Unset, None, datetime.datetime]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         AttemptStatisticsResponse
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        client=client,
-        start_date=start_date,
-        end_date=end_date,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            client=client,
+            start_date=start_date,
+            end_date=end_date,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/api/statistics/v1_stats_endpoint_attempts.py` & `svix-1.5.0/svix/internal/openapi_client/api/statistics/v1_stats_endpoint_attempts.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 import random
 from http import HTTPStatus
 from time import sleep
 from typing import Any, Dict, Union
 
 import httpx
 
-from ...client import AuthenticatedClient
+from ... import errors
+from ...client import AuthenticatedClient, Client
 from ...models.attempt_statistics_response import AttemptStatisticsResponse
 from ...models.http_error import HttpError
 from ...models.http_validation_error import HTTPValidationError
-from ...types import UNSET, Unset
+from ...types import UNSET, Response, Unset
+
+SLEEP_TIME = 0.05
+NUM_RETRIES = 3
 
 
 def _get_kwargs(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -45,87 +49,98 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
+        "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> AttemptStatisticsResponse:
+def _parse_response(*, client: Client, response: httpx.Response) -> AttemptStatisticsResponse:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = AttemptStatisticsResponse.from_dict(response.json())
+
+        return response_200
+    if response.status_code == HTTPStatus.BAD_REQUEST:
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.FORBIDDEN:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.NOT_FOUND:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.CONFLICT:
-        raise HttpError(response.json(), response.status_code)
+        raise HttpError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
-        raise HTTPValidationError(response.json(), response.status_code)
+        raise HTTPValidationError.init_exception(response.json(), response.status_code)
     if response.status_code == HTTPStatus.TOO_MANY_REQUESTS:
-        raise HttpError(response.json(), response.status_code)
-    response_200 = AttemptStatisticsResponse.from_dict(response.json())
-
-    return response_200
+        raise HttpError.init_exception(response.json(), response.status_code)
+    raise errors.UnexpectedStatus(response.status_code, response.content)
 
 
-sleep_time = 0.05
-num_retries = 3
+def _build_response(*, client: Client, response: httpx.Response) -> Response[AttemptStatisticsResponse]:
+    return Response(
+        status_code=HTTPStatus(response.status_code),
+        content=response.content,
+        headers=response.headers,
+        parsed=_parse_response(client=client, response=response),
+    )
 
 
 def sync_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
     start_date: Union[Unset, None, datetime.datetime] = UNSET,
     end_date: Union[Unset, None, datetime.datetime] = UNSET,
-) -> AttemptStatisticsResponse:
+) -> Response[AttemptStatisticsResponse]:
     """Get Ep Stats
 
      Returns endpoint-level statistics on message attempts
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         start_date (Union[Unset, None, datetime.datetime]):
         end_date (Union[Unset, None, datetime.datetime]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        AttemptStatisticsResponse
+        Response[AttemptStatisticsResponse]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         start_date=start_date,
         end_date=end_date,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
-    retry_count = 0
-    for retry in range(num_retries):
+    for retry_count in range(NUM_RETRIES):
         response = httpx.request(
             verify=client.verify_ssl,
             **kwargs,
         )
-        if response.status_code >= 500 and retry < num_retries:
-            retry_count += 1
+        if response.status_code >= 500:
             kwargs["headers"]["svix-retry-count"] = str(retry_count)
-            sleep(sleep_time)
-            sleep_time * 2
+            sleep(SLEEP_TIME * (2**retry_count))
         else:
             break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 def sync(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -138,72 +153,77 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         start_date (Union[Unset, None, datetime.datetime]):
         end_date (Union[Unset, None, datetime.datetime]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         AttemptStatisticsResponse
     """
 
     return sync_detailed(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         start_date=start_date,
         end_date=end_date,
-    )
+    ).parsed
 
 
 async def asyncio_detailed(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
     start_date: Union[Unset, None, datetime.datetime] = UNSET,
     end_date: Union[Unset, None, datetime.datetime] = UNSET,
-) -> AttemptStatisticsResponse:
+) -> Response[AttemptStatisticsResponse]:
     """Get Ep Stats
 
      Returns endpoint-level statistics on message attempts
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         start_date (Union[Unset, None, datetime.datetime]):
         end_date (Union[Unset, None, datetime.datetime]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
-        AttemptStatisticsResponse
+        Response[AttemptStatisticsResponse]
     """
 
     kwargs = _get_kwargs(
         app_id=app_id,
         endpoint_id=endpoint_id,
         client=client,
         start_date=start_date,
         end_date=end_date,
     )
 
     kwargs["headers"] = {"svix-req-id": f"{random.getrandbits(32)}", **kwargs["headers"]}
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        retry_count = 0
-        for retry in range(num_retries):
+        for retry_count in range(NUM_RETRIES):
             response = await _client.request(**kwargs)
-            if response.status_code >= 500 and retry < num_retries:
-                retry_count += 1
+            if response.status_code >= 500:
                 kwargs["headers"]["svix-retry-count"] = str(retry_count)
-                sleep(sleep_time)
-                sleep_time * 2
+                sleep(SLEEP_TIME * (2**retry_count))
             else:
                 break
 
-    return _parse_response(response=response)
+    return _build_response(client=client, response=response)
 
 
 async def asyncio(
     app_id: str,
     endpoint_id: str,
     *,
     client: AuthenticatedClient,
@@ -216,18 +236,24 @@
 
     Args:
         app_id (str): The app's ID or UID Example: unique-app-identifier.
         endpoint_id (str): The ep's ID or UID Example: unique-ep-identifier.
         start_date (Union[Unset, None, datetime.datetime]):
         end_date (Union[Unset, None, datetime.datetime]):
 
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
     Returns:
         AttemptStatisticsResponse
     """
 
-    return await asyncio_detailed(
-        app_id=app_id,
-        endpoint_id=endpoint_id,
-        client=client,
-        start_date=start_date,
-        end_date=end_date,
-    )
+    return (
+        await asyncio_detailed(
+            app_id=app_id,
+            endpoint_id=endpoint_id,
+            client=client,
+            start_date=start_date,
+            end_date=end_date,
+        )
+    ).parsed
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/client.py` & `svix-1.5.0/svix/internal/openapi_client/client.py`

 * *Files identical despite different names*

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/__init__.py` & `svix-1.5.0/svix/internal/openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/app_portal_access_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/app_portal_access_in.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,22 +28,22 @@
         if feature_flags is not UNSET:
             field_dict["featureFlags"] = feature_flags
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        feature_flags = cast(List[str], dict_copy.pop("featureFlags", UNSET))
+        d = src_dict.copy()
+        feature_flags = cast(List[str], d.pop("featureFlags", UNSET))
 
         app_portal_access_in = cls(
             feature_flags=feature_flags,
         )
 
-        app_portal_access_in.additional_properties = dict_copy
+        app_portal_access_in.additional_properties = d
         return app_portal_access_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/app_portal_access_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/app_portal_access_out.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,25 +30,25 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        token = dict_copy.pop("token")
+        d = src_dict.copy()
+        token = d.pop("token")
 
-        url = dict_copy.pop("url")
+        url = d.pop("url")
 
         app_portal_access_out = cls(
             token=token,
             url=url,
         )
 
-        app_portal_access_out.additional_properties = dict_copy
+        app_portal_access_out.additional_properties = d
         return app_portal_access_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/app_usage_stats_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/app_usage_stats_in.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,28 +46,28 @@
         if app_ids is not UNSET:
             field_dict["appIds"] = app_ids
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        since = isoparse(dict_copy.pop("since"))
+        d = src_dict.copy()
+        since = isoparse(d.pop("since"))
 
-        until = isoparse(dict_copy.pop("until"))
+        until = isoparse(d.pop("until"))
 
-        app_ids = cast(List[str], dict_copy.pop("appIds", UNSET))
+        app_ids = cast(List[str], d.pop("appIds", UNSET))
 
         app_usage_stats_in = cls(
             since=since,
             until=until,
             app_ids=app_ids,
         )
 
-        app_usage_stats_in.additional_properties = dict_copy
+        app_usage_stats_in.additional_properties = d
         return app_usage_stats_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/app_usage_stats_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/app_usage_stats_out.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,28 +38,28 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        id = dict_copy.pop("id")
+        d = src_dict.copy()
+        id = d.pop("id")
 
-        status = BackgroundTaskStatus(dict_copy.pop("status"))
+        status = BackgroundTaskStatus(d.pop("status"))
 
-        task = BackgroundTaskType(dict_copy.pop("task"))
+        task = BackgroundTaskType(d.pop("task"))
 
         app_usage_stats_out = cls(
             id=id,
             status=status,
             task=task,
         )
 
-        app_usage_stats_out.additional_properties = dict_copy
+        app_usage_stats_out.additional_properties = d
         return app_usage_stats_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/application_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/application_in.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,31 +47,31 @@
         if uid is not UNSET:
             field_dict["uid"] = uid
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        name = dict_copy.pop("name")
+        d = src_dict.copy()
+        name = d.pop("name")
 
-        metadata = dict_copy.pop("metadata", UNSET)
+        metadata = d.pop("metadata", UNSET)
 
-        rate_limit = dict_copy.pop("rateLimit", UNSET)
+        rate_limit = d.pop("rateLimit", UNSET)
 
-        uid = dict_copy.pop("uid", UNSET)
+        uid = d.pop("uid", UNSET)
 
         application_in = cls(
             name=name,
             metadata=metadata,
             rate_limit=rate_limit,
             uid=uid,
         )
 
-        application_in.additional_properties = dict_copy
+        application_in.additional_properties = d
         return application_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/application_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/application_out.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,40 +62,40 @@
         if uid is not UNSET:
             field_dict["uid"] = uid
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        created_at = isoparse(dict_copy.pop("createdAt"))
+        d = src_dict.copy()
+        created_at = isoparse(d.pop("createdAt"))
 
-        id = dict_copy.pop("id")
+        id = d.pop("id")
 
-        metadata = dict_copy.pop("metadata")
+        metadata = d.pop("metadata")
 
-        name = dict_copy.pop("name")
+        name = d.pop("name")
 
-        updated_at = isoparse(dict_copy.pop("updatedAt"))
+        updated_at = isoparse(d.pop("updatedAt"))
 
-        rate_limit = dict_copy.pop("rateLimit", UNSET)
+        rate_limit = d.pop("rateLimit", UNSET)
 
-        uid = dict_copy.pop("uid", UNSET)
+        uid = d.pop("uid", UNSET)
 
         application_out = cls(
             created_at=created_at,
             id=id,
             metadata=metadata,
             name=name,
             updated_at=updated_at,
             rate_limit=rate_limit,
             uid=uid,
         )
 
-        application_out.additional_properties = dict_copy
+        application_out.additional_properties = d
         return application_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/application_patch.py` & `svix-1.5.0/svix/internal/openapi_client/models/application_patch.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,31 +45,31 @@
         if uid is not UNSET:
             field_dict["uid"] = uid
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        metadata = dict_copy.pop("metadata", UNSET)
+        d = src_dict.copy()
+        metadata = d.pop("metadata", UNSET)
 
-        name = dict_copy.pop("name", UNSET)
+        name = d.pop("name", UNSET)
 
-        rate_limit = dict_copy.pop("rateLimit", UNSET)
+        rate_limit = d.pop("rateLimit", UNSET)
 
-        uid = dict_copy.pop("uid", UNSET)
+        uid = d.pop("uid", UNSET)
 
         application_patch = cls(
             metadata=metadata,
             name=name,
             rate_limit=rate_limit,
             uid=uid,
         )
 
-        application_patch.additional_properties = dict_copy
+        application_patch.additional_properties = d
         return application_patch
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/application_stats.py` & `svix-1.5.0/svix/internal/openapi_client/models/application_stats.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,28 +37,28 @@
         if app_uid is not UNSET:
             field_dict["appUid"] = app_uid
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        app_id = dict_copy.pop("appId")
+        d = src_dict.copy()
+        app_id = d.pop("appId")
 
-        message_destinations = dict_copy.pop("messageDestinations")
+        message_destinations = d.pop("messageDestinations")
 
-        app_uid = dict_copy.pop("appUid", UNSET)
+        app_uid = d.pop("appUid", UNSET)
 
         application_stats = cls(
             app_id=app_id,
             message_destinations=message_destinations,
             app_uid=app_uid,
         )
 
-        application_stats.additional_properties = dict_copy
+        application_stats.additional_properties = d
         return application_stats
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/application_token_expire_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/application_token_expire_in.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,22 +26,22 @@
         if expiry is not UNSET:
             field_dict["expiry"] = expiry
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        expiry = dict_copy.pop("expiry", UNSET)
+        d = src_dict.copy()
+        expiry = d.pop("expiry", UNSET)
 
         application_token_expire_in = cls(
             expiry=expiry,
         )
 
-        application_token_expire_in.additional_properties = dict_copy
+        application_token_expire_in.additional_properties = d
         return application_token_expire_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/attempt_statistics_data.py` & `svix-1.5.0/svix/internal/openapi_client/models/attempt_statistics_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,25 +42,25 @@
         if success_count is not UNSET:
             field_dict["successCount"] = success_count
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        failure_count = cast(List[int], dict_copy.pop("failureCount", UNSET))
+        d = src_dict.copy()
+        failure_count = cast(List[int], d.pop("failureCount", UNSET))
 
-        success_count = cast(List[int], dict_copy.pop("successCount", UNSET))
+        success_count = cast(List[int], d.pop("successCount", UNSET))
 
         attempt_statistics_data = cls(
             failure_count=failure_count,
             success_count=success_count,
         )
 
-        attempt_statistics_data.additional_properties = dict_copy
+        attempt_statistics_data.additional_properties = d
         return attempt_statistics_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/attempt_statistics_response.py` & `svix-1.5.0/svix/internal/openapi_client/models/attempt_statistics_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,31 +49,33 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        data = AttemptStatisticsData.from_dict(dict_copy.pop("data"))
+        from ..models.attempt_statistics_data import AttemptStatisticsData
 
-        end_date = isoparse(dict_copy.pop("endDate"))
+        d = src_dict.copy()
+        data = AttemptStatisticsData.from_dict(d.pop("data"))
 
-        period = StatisticsPeriod(dict_copy.pop("period"))
+        end_date = isoparse(d.pop("endDate"))
 
-        start_date = isoparse(dict_copy.pop("startDate"))
+        period = StatisticsPeriod(d.pop("period"))
+
+        start_date = isoparse(d.pop("startDate"))
 
         attempt_statistics_response = cls(
             data=data,
             end_date=end_date,
             period=period,
             start_date=start_date,
         )
 
-        attempt_statistics_response.additional_properties = dict_copy
+        attempt_statistics_response.additional_properties = d
         return attempt_statistics_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/background_task_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/background_task_out.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,31 +46,31 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        data = dict_copy.pop("data")
+        d = src_dict.copy()
+        data = d.pop("data")
 
-        id = dict_copy.pop("id")
+        id = d.pop("id")
 
-        status = BackgroundTaskStatus(dict_copy.pop("status"))
+        status = BackgroundTaskStatus(d.pop("status"))
 
-        task = BackgroundTaskType(dict_copy.pop("task"))
+        task = BackgroundTaskType(d.pop("task"))
 
         background_task_out = cls(
             data=data,
             id=id,
             status=status,
             task=task,
         )
 
-        background_task_out.additional_properties = dict_copy
+        background_task_out.additional_properties = d
         return background_task_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/border_radius_config.py` & `svix-1.5.0/svix/internal/openapi_client/models/border_radius_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,43 +45,43 @@
         if input_ is not UNSET:
             field_dict["input"] = input_
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        _button = dict_copy.pop("button", UNSET)
+        d = src_dict.copy()
+        _button = d.pop("button", UNSET)
         button: Union[Unset, BorderRadiusEnum]
         if isinstance(_button, Unset):
             button = UNSET
         else:
             button = BorderRadiusEnum(_button)
 
-        _card = dict_copy.pop("card", UNSET)
+        _card = d.pop("card", UNSET)
         card: Union[Unset, BorderRadiusEnum]
         if isinstance(_card, Unset):
             card = UNSET
         else:
             card = BorderRadiusEnum(_card)
 
-        _input_ = dict_copy.pop("input", UNSET)
+        _input_ = d.pop("input", UNSET)
         input_: Union[Unset, BorderRadiusEnum]
         if isinstance(_input_, Unset):
             input_ = UNSET
         else:
             input_ = BorderRadiusEnum(_input_)
 
         border_radius_config = cls(
             button=button,
             card=card,
             input_=input_,
         )
 
-        border_radius_config.additional_properties = dict_copy
+        border_radius_config.additional_properties = d
         return border_radius_config
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/custom_color_palette.py` & `svix-1.5.0/svix/internal/openapi_client/models/custom_color_palette.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,37 +51,37 @@
         if text_primary is not UNSET:
             field_dict["textPrimary"] = text_primary
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        background_hover = dict_copy.pop("backgroundHover", UNSET)
+        d = src_dict.copy()
+        background_hover = d.pop("backgroundHover", UNSET)
 
-        background_primary = dict_copy.pop("backgroundPrimary", UNSET)
+        background_primary = d.pop("backgroundPrimary", UNSET)
 
-        background_secondary = dict_copy.pop("backgroundSecondary", UNSET)
+        background_secondary = d.pop("backgroundSecondary", UNSET)
 
-        interactive_accent = dict_copy.pop("interactiveAccent", UNSET)
+        interactive_accent = d.pop("interactiveAccent", UNSET)
 
-        text_danger = dict_copy.pop("textDanger", UNSET)
+        text_danger = d.pop("textDanger", UNSET)
 
-        text_primary = dict_copy.pop("textPrimary", UNSET)
+        text_primary = d.pop("textPrimary", UNSET)
 
         custom_color_palette = cls(
             background_hover=background_hover,
             background_primary=background_primary,
             background_secondary=background_secondary,
             interactive_accent=interactive_accent,
             text_danger=text_danger,
             text_primary=text_primary,
         )
 
-        custom_color_palette.additional_properties = dict_copy
+        custom_color_palette.additional_properties = d
         return custom_color_palette
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/custom_theme_override.py` & `svix-1.5.0/svix/internal/openapi_client/models/custom_theme_override.py`

 * *Files 21% similar despite different names*

```diff
@@ -41,35 +41,38 @@
         if font_size is not UNSET:
             field_dict["fontSize"] = font_size
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        _border_radius = dict_copy.pop("borderRadius", UNSET)
+        from ..models.border_radius_config import BorderRadiusConfig
+        from ..models.font_size_config import FontSizeConfig
+
+        d = src_dict.copy()
+        _border_radius = d.pop("borderRadius", UNSET)
         border_radius: Union[Unset, BorderRadiusConfig]
         if isinstance(_border_radius, Unset):
             border_radius = UNSET
         else:
             border_radius = BorderRadiusConfig.from_dict(_border_radius)
 
-        _font_size = dict_copy.pop("fontSize", UNSET)
+        _font_size = d.pop("fontSize", UNSET)
         font_size: Union[Unset, FontSizeConfig]
         if isinstance(_font_size, Unset):
             font_size = UNSET
         else:
             font_size = FontSizeConfig.from_dict(_font_size)
 
         custom_theme_override = cls(
             border_radius=border_radius,
             font_size=font_size,
         )
 
-        custom_theme_override.additional_properties = dict_copy
+        custom_theme_override.additional_properties = d
         return custom_theme_override
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/dashboard_access_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/dashboard_access_out.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,25 +30,25 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        token = dict_copy.pop("token")
+        d = src_dict.copy()
+        token = d.pop("token")
 
-        url = dict_copy.pop("url")
+        url = d.pop("url")
 
         dashboard_access_out = cls(
             token=token,
             url=url,
         )
 
-        dashboard_access_out.additional_properties = dict_copy
+        dashboard_access_out.additional_properties = d
         return dashboard_access_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_created_event.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_created_event.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,25 +38,27 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        data = EndpointCreatedEventData.from_dict(dict_copy.pop("data"))
+        from ..models.endpoint_created_event_data import EndpointCreatedEventData
 
-        type = EndpointCreatedEventType(dict_copy.pop("type"))
+        d = src_dict.copy()
+        data = EndpointCreatedEventData.from_dict(d.pop("data"))
+
+        type = EndpointCreatedEventType(d.pop("type"))
 
         endpoint_created_event = cls(
             data=data,
             type=type,
         )
 
-        endpoint_created_event.additional_properties = dict_copy
+        endpoint_created_event.additional_properties = d
         return endpoint_created_event
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_created_event_data.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_deleted_event_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="EndpointCreatedEventData")
+T = TypeVar("T", bound="EndpointDeletedEventData")
 
 
 @attr.s(auto_attribs=True)
-class EndpointCreatedEventData:
+class EndpointDeletedEventData:
     """
     Attributes:
         app_id (str): The app's ID Example: app_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         endpoint_id (str): The ep's ID Example: ep_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         app_uid (Union[Unset, None, str]): The app's UID Example: unique-app-identifier.
         endpoint_uid (Union[Unset, None, str]): The ep's UID Example: unique-ep-identifier.
     """
@@ -42,32 +42,32 @@
         if endpoint_uid is not UNSET:
             field_dict["endpointUid"] = endpoint_uid
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        app_id = dict_copy.pop("appId")
+        d = src_dict.copy()
+        app_id = d.pop("appId")
 
-        endpoint_id = dict_copy.pop("endpointId")
+        endpoint_id = d.pop("endpointId")
 
-        app_uid = dict_copy.pop("appUid", UNSET)
+        app_uid = d.pop("appUid", UNSET)
 
-        endpoint_uid = dict_copy.pop("endpointUid", UNSET)
+        endpoint_uid = d.pop("endpointUid", UNSET)
 
-        endpoint_created_event_data = cls(
+        endpoint_deleted_event_data = cls(
             app_id=app_id,
             endpoint_id=endpoint_id,
             app_uid=app_uid,
             endpoint_uid=endpoint_uid,
         )
 
-        endpoint_created_event_data.additional_properties = dict_copy
-        return endpoint_created_event_data
+        endpoint_deleted_event_data.additional_properties = d
+        return endpoint_deleted_event_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_deleted_event.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_deleted_event.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,25 +38,27 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        data = EndpointDeletedEventData.from_dict(dict_copy.pop("data"))
+        from ..models.endpoint_deleted_event_data import EndpointDeletedEventData
 
-        type = EndpointDeletedEventType(dict_copy.pop("type"))
+        d = src_dict.copy()
+        data = EndpointDeletedEventData.from_dict(d.pop("data"))
+
+        type = EndpointDeletedEventType(d.pop("type"))
 
         endpoint_deleted_event = cls(
             data=data,
             type=type,
         )
 
-        endpoint_deleted_event.additional_properties = dict_copy
+        endpoint_deleted_event.additional_properties = d
         return endpoint_deleted_event
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_deleted_event_data.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_created_event_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="EndpointDeletedEventData")
+T = TypeVar("T", bound="EndpointCreatedEventData")
 
 
 @attr.s(auto_attribs=True)
-class EndpointDeletedEventData:
+class EndpointCreatedEventData:
     """
     Attributes:
         app_id (str): The app's ID Example: app_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         endpoint_id (str): The ep's ID Example: ep_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         app_uid (Union[Unset, None, str]): The app's UID Example: unique-app-identifier.
         endpoint_uid (Union[Unset, None, str]): The ep's UID Example: unique-ep-identifier.
     """
@@ -42,32 +42,32 @@
         if endpoint_uid is not UNSET:
             field_dict["endpointUid"] = endpoint_uid
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        app_id = dict_copy.pop("appId")
+        d = src_dict.copy()
+        app_id = d.pop("appId")
 
-        endpoint_id = dict_copy.pop("endpointId")
+        endpoint_id = d.pop("endpointId")
 
-        app_uid = dict_copy.pop("appUid", UNSET)
+        app_uid = d.pop("appUid", UNSET)
 
-        endpoint_uid = dict_copy.pop("endpointUid", UNSET)
+        endpoint_uid = d.pop("endpointUid", UNSET)
 
-        endpoint_deleted_event_data = cls(
+        endpoint_created_event_data = cls(
             app_id=app_id,
             endpoint_id=endpoint_id,
             app_uid=app_uid,
             endpoint_uid=endpoint_uid,
         )
 
-        endpoint_deleted_event_data.additional_properties = dict_copy
-        return endpoint_deleted_event_data
+        endpoint_created_event_data.additional_properties = d
+        return endpoint_created_event_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_disabled_event.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_disabled_event.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,25 +39,27 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        data = EndpointDisabledEventData.from_dict(dict_copy.pop("data"))
+        from ..models.endpoint_disabled_event_data import EndpointDisabledEventData
 
-        type = EndpointDisabledEventType(dict_copy.pop("type"))
+        d = src_dict.copy()
+        data = EndpointDisabledEventData.from_dict(d.pop("data"))
+
+        type = EndpointDisabledEventType(d.pop("type"))
 
         endpoint_disabled_event = cls(
             data=data,
             type=type,
         )
 
-        endpoint_disabled_event.additional_properties = dict_copy
+        endpoint_disabled_event.additional_properties = d
         return endpoint_disabled_event
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_disabled_event_data.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_disabled_event_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,34 +50,34 @@
         if endpoint_uid is not UNSET:
             field_dict["endpointUid"] = endpoint_uid
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        app_id = dict_copy.pop("appId")
+        d = src_dict.copy()
+        app_id = d.pop("appId")
 
-        endpoint_id = dict_copy.pop("endpointId")
+        endpoint_id = d.pop("endpointId")
 
-        fail_since = isoparse(dict_copy.pop("failSince"))
+        fail_since = isoparse(d.pop("failSince"))
 
-        app_uid = dict_copy.pop("appUid", UNSET)
+        app_uid = d.pop("appUid", UNSET)
 
-        endpoint_uid = dict_copy.pop("endpointUid", UNSET)
+        endpoint_uid = d.pop("endpointUid", UNSET)
 
         endpoint_disabled_event_data = cls(
             app_id=app_id,
             endpoint_id=endpoint_id,
             fail_since=fail_since,
             app_uid=app_uid,
             endpoint_uid=endpoint_uid,
         )
 
-        endpoint_disabled_event_data.additional_properties = dict_copy
+        endpoint_disabled_event_data.additional_properties = d
         return endpoint_disabled_event_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_headers_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/integration_key_out.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,48 @@
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-if TYPE_CHECKING:
-    from ..models.endpoint_headers_in_headers import EndpointHeadersInHeaders
-
-
-T = TypeVar("T", bound="EndpointHeadersIn")
+T = TypeVar("T", bound="IntegrationKeyOut")
 
 
 @attr.s(auto_attribs=True)
-class EndpointHeadersIn:
+class IntegrationKeyOut:
     """
     Attributes:
-        headers (EndpointHeadersInHeaders):  Example: {'X-Example': '123', 'X-Foobar': 'Bar'}.
+        key (str):  Example: integsk_kV3ts5tKPNJN4Dl25cMTfUNdmabxbX0O.
     """
 
-    headers: "EndpointHeadersInHeaders"
+    key: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        headers = self.headers
+        key = self.key
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "headers": headers,
+                "key": key,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        headers = dict_copy.pop("headers")
+        d = src_dict.copy()
+        key = d.pop("key")
 
-        endpoint_headers_in = cls(
-            headers=headers,
+        integration_key_out = cls(
+            key=key,
         )
 
-        endpoint_headers_in.additional_properties = dict_copy
-        return endpoint_headers_in
+        integration_key_out.additional_properties = d
+        return integration_key_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_headers_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_headers_out.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,25 +37,25 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        headers = dict_copy.pop("headers")
+        d = src_dict.copy()
+        headers = d.pop("headers")
 
-        sensitive = cast(List[str], dict_copy.pop("sensitive"))
+        sensitive = cast(List[str], d.pop("sensitive"))
 
         endpoint_headers_out = cls(
             headers=headers,
             sensitive=sensitive,
         )
 
-        endpoint_headers_out.additional_properties = dict_copy
+        endpoint_headers_out.additional_properties = d
         return endpoint_headers_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_headers_patch_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_headers_patch_in.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,22 +30,22 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        headers = dict_copy.pop("headers")
+        d = src_dict.copy()
+        headers = d.pop("headers")
 
         endpoint_headers_patch_in = cls(
             headers=headers,
         )
 
-        endpoint_headers_patch_in.additional_properties = dict_copy
+        endpoint_headers_patch_in.additional_properties = d
         return endpoint_headers_patch_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_out.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,140 +1,153 @@
+import datetime
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
+from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.endpoint_in_metadata import EndpointInMetadata
+    from ..models.endpoint_out_metadata import EndpointOutMetadata
 
 
-T = TypeVar("T", bound="EndpointIn")
+T = TypeVar("T", bound="EndpointOut")
 
 
 @attr.s(auto_attribs=True)
-class EndpointIn:
+class EndpointOut:
     """
     Attributes:
+        created_at (datetime.datetime):
+        description (str): An example endpoint name
+        id (str): The ep's ID Example: ep_1srOrx2ZWZBpBUvZwXKQmoEYga2.
+        metadata (EndpointOutMetadata):
+        updated_at (datetime.datetime):
         url (str):  Example: https://example.com/webhook/.
         version (int):  Example: 1.
         channels (Union[Unset, None, List[str]]): List of message channels this endpoint listens to (omit for all)
             Example: ['project_123', 'group_2'].
-        description (Union[Unset, str]):  Default: ''. Example: An example endpoint name.
         disabled (Union[Unset, bool]):
         filter_types (Union[Unset, None, List[str]]):  Example: ['user.signup', 'user.deleted'].
-        metadata (Union[Unset, EndpointInMetadata]):
         rate_limit (Union[Unset, None, int]):
-        secret (Union[Unset, None, str]): The endpoint's verification secret. If `null` is passed, a secret is
-            automatically generated. Format: `base64` encoded random bytes optionally prefixed with `whsec_`. Recommended
-            size: 24. Example: whsec_C2FVsBQIhrscChlQIMV+b5sSYspob7oD.
         uid (Union[Unset, None, str]): Optional unique identifier for the endpoint Example: unique-ep-identifier.
     """
 
+    created_at: datetime.datetime
+    description: str
+    id: str
+    metadata: "EndpointOutMetadata"
+    updated_at: datetime.datetime
     url: str
     version: int
     channels: Union[Unset, None, List[str]] = UNSET
-    description: Union[Unset, str] = ""
     disabled: Union[Unset, bool] = False
     filter_types: Union[Unset, None, List[str]] = UNSET
-    metadata: Union[Unset, "EndpointInMetadata"] = UNSET
     rate_limit: Union[Unset, None, int] = UNSET
-    secret: Union[Unset, None, str] = UNSET
     uid: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        created_at = self.created_at.isoformat()
+
+        description = self.description
+        id = self.id
+        metadata = self.metadata
+        updated_at = self.updated_at.isoformat()
+
         url = self.url
         version = self.version
         channels: Union[Unset, None, List[str]] = UNSET
         if not isinstance(self.channels, Unset):
             if self.channels is None:
                 channels = None
             else:
                 channels = self.channels
 
-        description = self.description
         disabled = self.disabled
         filter_types: Union[Unset, None, List[str]] = UNSET
         if not isinstance(self.filter_types, Unset):
             if self.filter_types is None:
                 filter_types = None
             else:
                 filter_types = self.filter_types
 
-        metadata = self.metadata
         rate_limit = self.rate_limit
-        secret = self.secret
         uid = self.uid
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
+                "createdAt": created_at,
+                "description": description,
+                "id": id,
+                "metadata": metadata,
+                "updatedAt": updated_at,
                 "url": url,
                 "version": version,
             }
         )
         if channels is not UNSET:
             field_dict["channels"] = channels
-        if description is not UNSET:
-            field_dict["description"] = description
         if disabled is not UNSET:
             field_dict["disabled"] = disabled
         if filter_types is not UNSET:
             field_dict["filterTypes"] = filter_types
-        if metadata is not UNSET:
-            field_dict["metadata"] = metadata
         if rate_limit is not UNSET:
             field_dict["rateLimit"] = rate_limit
-        if secret is not UNSET:
-            field_dict["secret"] = secret
         if uid is not UNSET:
             field_dict["uid"] = uid
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        url = dict_copy.pop("url")
+        d = src_dict.copy()
+        created_at = isoparse(d.pop("createdAt"))
 
-        version = dict_copy.pop("version")
+        description = d.pop("description")
 
-        channels = cast(List[str], dict_copy.pop("channels", UNSET))
+        id = d.pop("id")
 
-        description = dict_copy.pop("description", UNSET)
+        metadata = d.pop("metadata")
 
-        disabled = dict_copy.pop("disabled", UNSET)
+        updated_at = isoparse(d.pop("updatedAt"))
 
-        filter_types = cast(List[str], dict_copy.pop("filterTypes", UNSET))
+        url = d.pop("url")
 
-        metadata = dict_copy.pop("metadata", UNSET)
+        version = d.pop("version")
 
-        rate_limit = dict_copy.pop("rateLimit", UNSET)
+        channels = cast(List[str], d.pop("channels", UNSET))
 
-        secret = dict_copy.pop("secret", UNSET)
+        disabled = d.pop("disabled", UNSET)
 
-        uid = dict_copy.pop("uid", UNSET)
+        filter_types = cast(List[str], d.pop("filterTypes", UNSET))
 
-        endpoint_in = cls(
+        rate_limit = d.pop("rateLimit", UNSET)
+
+        uid = d.pop("uid", UNSET)
+
+        endpoint_out = cls(
+            created_at=created_at,
+            description=description,
+            id=id,
+            metadata=metadata,
+            updated_at=updated_at,
             url=url,
             version=version,
             channels=channels,
-            description=description,
             disabled=disabled,
             filter_types=filter_types,
-            metadata=metadata,
             rate_limit=rate_limit,
-            secret=secret,
             uid=uid,
         )
 
-        endpoint_in.additional_properties = dict_copy
-        return endpoint_in
+        endpoint_out.additional_properties = d
+        return endpoint_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_message_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_message_out.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,30 +82,30 @@
         if next_attempt is not UNSET:
             field_dict["nextAttempt"] = next_attempt
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        event_type = dict_copy.pop("eventType")
+        d = src_dict.copy()
+        event_type = d.pop("eventType")
 
-        id = dict_copy.pop("id")
+        id = d.pop("id")
 
-        payload = dict_copy.pop("payload")
+        payload = d.pop("payload")
 
-        status = MessageStatus(dict_copy.pop("status"))
+        status = MessageStatus(d.pop("status"))
 
-        timestamp = isoparse(dict_copy.pop("timestamp"))
+        timestamp = isoparse(d.pop("timestamp"))
 
-        channels = cast(List[str], dict_copy.pop("channels", UNSET))
+        channels = cast(List[str], d.pop("channels", UNSET))
 
-        event_id = dict_copy.pop("eventId", UNSET)
+        event_id = d.pop("eventId", UNSET)
 
-        _next_attempt = dict_copy.pop("nextAttempt", UNSET)
+        _next_attempt = d.pop("nextAttempt", UNSET)
         next_attempt: Union[Unset, None, datetime.datetime]
         if _next_attempt is None:
             next_attempt = None
         elif isinstance(_next_attempt, Unset):
             next_attempt = UNSET
         else:
             next_attempt = isoparse(_next_attempt)
@@ -117,15 +117,15 @@
             status=status,
             timestamp=timestamp,
             channels=channels,
             event_id=event_id,
             next_attempt=next_attempt,
         )
 
-        endpoint_message_out.additional_properties = dict_copy
+        endpoint_message_out.additional_properties = d
         return endpoint_message_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/message_endpoint_out.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 import datetime
-from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 from dateutil.parser import isoparse
 
+from ..models.message_status import MessageStatus
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.endpoint_out_metadata import EndpointOutMetadata
-
-
-T = TypeVar("T", bound="EndpointOut")
+T = TypeVar("T", bound="MessageEndpointOut")
 
 
 @attr.s(auto_attribs=True)
-class EndpointOut:
+class MessageEndpointOut:
     """
     Attributes:
         created_at (datetime.datetime):
         description (str): An example endpoint name
         id (str): The ep's ID Example: ep_1srOrx2ZWZBpBUvZwXKQmoEYga2.
-        metadata (EndpointOutMetadata):
+        status (MessageStatus): The sending status of the message:
+            - Success = 0
+            - Pending = 1
+            - Fail = 2
+            - Sending = 3
         updated_at (datetime.datetime):
         url (str):  Example: https://example.com/webhook/.
         version (int):  Example: 1.
         channels (Union[Unset, None, List[str]]): List of message channels this endpoint listens to (omit for all)
             Example: ['project_123', 'group_2'].
         disabled (Union[Unset, bool]):
         filter_types (Union[Unset, None, List[str]]):  Example: ['user.signup', 'user.deleted'].
+        next_attempt (Union[Unset, None, datetime.datetime]):
         rate_limit (Union[Unset, None, int]):
         uid (Union[Unset, None, str]): Optional unique identifier for the endpoint Example: unique-ep-identifier.
     """
 
     created_at: datetime.datetime
     description: str
     id: str
-    metadata: "EndpointOutMetadata"
+    status: MessageStatus
     updated_at: datetime.datetime
     url: str
     version: int
     channels: Union[Unset, None, List[str]] = UNSET
     disabled: Union[Unset, bool] = False
     filter_types: Union[Unset, None, List[str]] = UNSET
+    next_attempt: Union[Unset, None, datetime.datetime] = UNSET
     rate_limit: Union[Unset, None, int] = UNSET
     uid: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         created_at = self.created_at.isoformat()
 
         description = self.description
         id = self.id
-        metadata = self.metadata
+        status = self.status.value
+
         updated_at = self.updated_at.isoformat()
 
         url = self.url
         version = self.version
         channels: Union[Unset, None, List[str]] = UNSET
         if not isinstance(self.channels, Unset):
             if self.channels is None:
@@ -67,87 +71,103 @@
         filter_types: Union[Unset, None, List[str]] = UNSET
         if not isinstance(self.filter_types, Unset):
             if self.filter_types is None:
                 filter_types = None
             else:
                 filter_types = self.filter_types
 
+        next_attempt: Union[Unset, None, str] = UNSET
+        if not isinstance(self.next_attempt, Unset):
+            next_attempt = self.next_attempt.isoformat() if self.next_attempt else None
+
         rate_limit = self.rate_limit
         uid = self.uid
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "createdAt": created_at,
                 "description": description,
                 "id": id,
-                "metadata": metadata,
+                "status": status,
                 "updatedAt": updated_at,
                 "url": url,
                 "version": version,
             }
         )
         if channels is not UNSET:
             field_dict["channels"] = channels
         if disabled is not UNSET:
             field_dict["disabled"] = disabled
         if filter_types is not UNSET:
             field_dict["filterTypes"] = filter_types
+        if next_attempt is not UNSET:
+            field_dict["nextAttempt"] = next_attempt
         if rate_limit is not UNSET:
             field_dict["rateLimit"] = rate_limit
         if uid is not UNSET:
             field_dict["uid"] = uid
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        created_at = isoparse(dict_copy.pop("createdAt"))
+        d = src_dict.copy()
+        created_at = isoparse(d.pop("createdAt"))
+
+        description = d.pop("description")
 
-        description = dict_copy.pop("description")
+        id = d.pop("id")
 
-        id = dict_copy.pop("id")
+        status = MessageStatus(d.pop("status"))
 
-        metadata = dict_copy.pop("metadata")
+        updated_at = isoparse(d.pop("updatedAt"))
 
-        updated_at = isoparse(dict_copy.pop("updatedAt"))
+        url = d.pop("url")
 
-        url = dict_copy.pop("url")
+        version = d.pop("version")
 
-        version = dict_copy.pop("version")
+        channels = cast(List[str], d.pop("channels", UNSET))
 
-        channels = cast(List[str], dict_copy.pop("channels", UNSET))
+        disabled = d.pop("disabled", UNSET)
 
-        disabled = dict_copy.pop("disabled", UNSET)
+        filter_types = cast(List[str], d.pop("filterTypes", UNSET))
 
-        filter_types = cast(List[str], dict_copy.pop("filterTypes", UNSET))
+        _next_attempt = d.pop("nextAttempt", UNSET)
+        next_attempt: Union[Unset, None, datetime.datetime]
+        if _next_attempt is None:
+            next_attempt = None
+        elif isinstance(_next_attempt, Unset):
+            next_attempt = UNSET
+        else:
+            next_attempt = isoparse(_next_attempt)
 
-        rate_limit = dict_copy.pop("rateLimit", UNSET)
+        rate_limit = d.pop("rateLimit", UNSET)
 
-        uid = dict_copy.pop("uid", UNSET)
+        uid = d.pop("uid", UNSET)
 
-        endpoint_out = cls(
+        message_endpoint_out = cls(
             created_at=created_at,
             description=description,
             id=id,
-            metadata=metadata,
+            status=status,
             updated_at=updated_at,
             url=url,
             version=version,
             channels=channels,
             disabled=disabled,
             filter_types=filter_types,
+            next_attempt=next_attempt,
             rate_limit=rate_limit,
             uid=uid,
         )
 
-        endpoint_out.additional_properties = dict_copy
-        return endpoint_out
+        message_endpoint_out.additional_properties = d
+        return message_endpoint_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_patch.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_patch.py`

 * *Files 10% similar despite different names*

```diff
@@ -89,49 +89,49 @@
         if version is not UNSET:
             field_dict["version"] = version
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        channels = cast(List[str], dict_copy.pop("channels", UNSET))
+        d = src_dict.copy()
+        channels = cast(List[str], d.pop("channels", UNSET))
 
-        description = dict_copy.pop("description", UNSET)
+        description = d.pop("description", UNSET)
 
-        disabled = dict_copy.pop("disabled", UNSET)
+        disabled = d.pop("disabled", UNSET)
 
-        filter_types = cast(List[str], dict_copy.pop("filterTypes", UNSET))
+        filter_types = cast(List[str], d.pop("filterTypes", UNSET))
 
-        metadata = dict_copy.pop("metadata", UNSET)
+        metadata = d.pop("metadata", UNSET)
 
-        rate_limit = dict_copy.pop("rateLimit", UNSET)
+        rate_limit = d.pop("rateLimit", UNSET)
 
-        secret = dict_copy.pop("secret", UNSET)
+        secret = d.pop("secret", UNSET)
 
-        uid = dict_copy.pop("uid", UNSET)
+        uid = d.pop("uid", UNSET)
 
-        url = dict_copy.pop("url", UNSET)
+        url = d.pop("url", UNSET)
 
-        version = dict_copy.pop("version", UNSET)
+        version = d.pop("version", UNSET)
 
         endpoint_patch = cls(
             channels=channels,
             description=description,
             disabled=disabled,
             filter_types=filter_types,
             metadata=metadata,
             rate_limit=rate_limit,
             secret=secret,
             uid=uid,
             url=url,
             version=version,
         )
 
-        endpoint_patch.additional_properties = dict_copy
+        endpoint_patch.additional_properties = d
         return endpoint_patch
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_secret_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_secret_out.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,22 +28,22 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        key = dict_copy.pop("key")
+        d = src_dict.copy()
+        key = d.pop("key")
 
         endpoint_secret_out = cls(
             key=key,
         )
 
-        endpoint_secret_out.additional_properties = dict_copy
+        endpoint_secret_out.additional_properties = d
         return endpoint_secret_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_secret_rotate_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_secret_rotate_in.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,22 +28,22 @@
         if key is not UNSET:
             field_dict["key"] = key
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        key = dict_copy.pop("key", UNSET)
+        d = src_dict.copy()
+        key = d.pop("key", UNSET)
 
         endpoint_secret_rotate_in = cls(
             key=key,
         )
 
-        endpoint_secret_rotate_in.additional_properties = dict_copy
+        endpoint_secret_rotate_in.additional_properties = d
         return endpoint_secret_rotate_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_stats.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,31 +38,31 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        fail = dict_copy.pop("fail")
+        d = src_dict.copy()
+        fail = d.pop("fail")
 
-        pending = dict_copy.pop("pending")
+        pending = d.pop("pending")
 
-        sending = dict_copy.pop("sending")
+        sending = d.pop("sending")
 
-        success = dict_copy.pop("success")
+        success = d.pop("success")
 
         endpoint_stats = cls(
             fail=fail,
             pending=pending,
             sending=sending,
             success=success,
         )
 
-        endpoint_stats.additional_properties = dict_copy
+        endpoint_stats.additional_properties = d
         return endpoint_stats
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_transformation_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_transformation_in.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,25 +31,25 @@
         if enabled is not UNSET:
             field_dict["enabled"] = enabled
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        code = dict_copy.pop("code", UNSET)
+        d = src_dict.copy()
+        code = d.pop("code", UNSET)
 
-        enabled = dict_copy.pop("enabled", UNSET)
+        enabled = d.pop("enabled", UNSET)
 
         endpoint_transformation_in = cls(
             code=code,
             enabled=enabled,
         )
 
-        endpoint_transformation_in.additional_properties = dict_copy
+        endpoint_transformation_in.additional_properties = d
         return endpoint_transformation_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_transformation_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_transformation_out.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,25 +31,25 @@
         if enabled is not UNSET:
             field_dict["enabled"] = enabled
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        code = dict_copy.pop("code", UNSET)
+        d = src_dict.copy()
+        code = d.pop("code", UNSET)
 
-        enabled = dict_copy.pop("enabled", UNSET)
+        enabled = d.pop("enabled", UNSET)
 
         endpoint_transformation_out = cls(
             code=code,
             enabled=enabled,
         )
 
-        endpoint_transformation_out.additional_properties = dict_copy
+        endpoint_transformation_out.additional_properties = d
         return endpoint_transformation_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_transformation_simulate_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_transformation_simulate_in.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,31 +50,31 @@
         if channels is not UNSET:
             field_dict["channels"] = channels
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        code = dict_copy.pop("code")
+        d = src_dict.copy()
+        code = d.pop("code")
 
-        event_type = dict_copy.pop("eventType")
+        event_type = d.pop("eventType")
 
-        payload = dict_copy.pop("payload")
+        payload = d.pop("payload")
 
-        channels = cast(List[str], dict_copy.pop("channels", UNSET))
+        channels = cast(List[str], d.pop("channels", UNSET))
 
         endpoint_transformation_simulate_in = cls(
             code=code,
             event_type=event_type,
             payload=payload,
             channels=channels,
         )
 
-        endpoint_transformation_simulate_in.additional_properties = dict_copy
+        endpoint_transformation_simulate_in.additional_properties = d
         return endpoint_transformation_simulate_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_transformation_simulate_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_transformation_simulate_out.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,33 +40,33 @@
         if method is not UNSET:
             field_dict["method"] = method
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        payload = dict_copy.pop("payload")
+        d = src_dict.copy()
+        payload = d.pop("payload")
 
-        url = dict_copy.pop("url")
+        url = d.pop("url")
 
-        _method = dict_copy.pop("method", UNSET)
+        _method = d.pop("method", UNSET)
         method: Union[Unset, TransformationHttpMethod]
         if isinstance(_method, Unset):
             method = UNSET
         else:
             method = TransformationHttpMethod(_method)
 
         endpoint_transformation_simulate_out = cls(
             payload=payload,
             url=url,
             method=method,
         )
 
-        endpoint_transformation_simulate_out.additional_properties = dict_copy
+        endpoint_transformation_simulate_out.additional_properties = d
         return endpoint_transformation_simulate_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_update.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_in.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.endpoint_update_metadata import EndpointUpdateMetadata
+    from ..models.endpoint_in_metadata import EndpointInMetadata
 
 
-T = TypeVar("T", bound="EndpointUpdate")
+T = TypeVar("T", bound="EndpointIn")
 
 
 @attr.s(auto_attribs=True)
-class EndpointUpdate:
+class EndpointIn:
     """
     Attributes:
         url (str):  Example: https://example.com/webhook/.
         version (int):  Example: 1.
         channels (Union[Unset, None, List[str]]): List of message channels this endpoint listens to (omit for all)
             Example: ['project_123', 'group_2'].
         description (Union[Unset, str]):  Default: ''. Example: An example endpoint name.
         disabled (Union[Unset, bool]):
         filter_types (Union[Unset, None, List[str]]):  Example: ['user.signup', 'user.deleted'].
-        metadata (Union[Unset, EndpointUpdateMetadata]):
+        metadata (Union[Unset, EndpointInMetadata]):
         rate_limit (Union[Unset, None, int]):
+        secret (Union[Unset, None, str]): The endpoint's verification secret. If `null` is passed, a secret is
+            automatically generated. Format: `base64` encoded random bytes optionally prefixed with `whsec_`. Recommended
+            size: 24. Example: whsec_C2FVsBQIhrscChlQIMV+b5sSYspob7oD.
         uid (Union[Unset, None, str]): Optional unique identifier for the endpoint Example: unique-ep-identifier.
     """
 
     url: str
     version: int
     channels: Union[Unset, None, List[str]] = UNSET
     description: Union[Unset, str] = ""
     disabled: Union[Unset, bool] = False
     filter_types: Union[Unset, None, List[str]] = UNSET
-    metadata: Union[Unset, "EndpointUpdateMetadata"] = UNSET
+    metadata: Union[Unset, "EndpointInMetadata"] = UNSET
     rate_limit: Union[Unset, None, int] = UNSET
+    secret: Union[Unset, None, str] = UNSET
     uid: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         url = self.url
         version = self.version
         channels: Union[Unset, None, List[str]] = UNSET
@@ -55,14 +59,15 @@
             if self.filter_types is None:
                 filter_types = None
             else:
                 filter_types = self.filter_types
 
         metadata = self.metadata
         rate_limit = self.rate_limit
+        secret = self.secret
         uid = self.uid
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "url": url,
@@ -77,54 +82,59 @@
             field_dict["disabled"] = disabled
         if filter_types is not UNSET:
             field_dict["filterTypes"] = filter_types
         if metadata is not UNSET:
             field_dict["metadata"] = metadata
         if rate_limit is not UNSET:
             field_dict["rateLimit"] = rate_limit
+        if secret is not UNSET:
+            field_dict["secret"] = secret
         if uid is not UNSET:
             field_dict["uid"] = uid
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        url = dict_copy.pop("url")
+        d = src_dict.copy()
+        url = d.pop("url")
 
-        version = dict_copy.pop("version")
+        version = d.pop("version")
 
-        channels = cast(List[str], dict_copy.pop("channels", UNSET))
+        channels = cast(List[str], d.pop("channels", UNSET))
 
-        description = dict_copy.pop("description", UNSET)
+        description = d.pop("description", UNSET)
 
-        disabled = dict_copy.pop("disabled", UNSET)
+        disabled = d.pop("disabled", UNSET)
 
-        filter_types = cast(List[str], dict_copy.pop("filterTypes", UNSET))
+        filter_types = cast(List[str], d.pop("filterTypes", UNSET))
 
-        metadata = dict_copy.pop("metadata", UNSET)
+        metadata = d.pop("metadata", UNSET)
 
-        rate_limit = dict_copy.pop("rateLimit", UNSET)
+        rate_limit = d.pop("rateLimit", UNSET)
 
-        uid = dict_copy.pop("uid", UNSET)
+        secret = d.pop("secret", UNSET)
 
-        endpoint_update = cls(
+        uid = d.pop("uid", UNSET)
+
+        endpoint_in = cls(
             url=url,
             version=version,
             channels=channels,
             description=description,
             disabled=disabled,
             filter_types=filter_types,
             metadata=metadata,
             rate_limit=rate_limit,
+            secret=secret,
             uid=uid,
         )
 
-        endpoint_update.additional_properties = dict_copy
-        return endpoint_update
+        endpoint_in.additional_properties = d
+        return endpoint_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_updated_event.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_updated_event.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,25 +38,27 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        data = EndpointUpdatedEventData.from_dict(dict_copy.pop("data"))
+        from ..models.endpoint_updated_event_data import EndpointUpdatedEventData
 
-        type = EndpointUpdatedEventType(dict_copy.pop("type"))
+        d = src_dict.copy()
+        data = EndpointUpdatedEventData.from_dict(d.pop("data"))
+
+        type = EndpointUpdatedEventType(d.pop("type"))
 
         endpoint_updated_event = cls(
             data=data,
             type=type,
         )
 
-        endpoint_updated_event.additional_properties = dict_copy
+        endpoint_updated_event.additional_properties = d
         return endpoint_updated_event
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/endpoint_updated_event_data.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_updated_event_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,31 +42,31 @@
         if endpoint_uid is not UNSET:
             field_dict["endpointUid"] = endpoint_uid
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        app_id = dict_copy.pop("appId")
+        d = src_dict.copy()
+        app_id = d.pop("appId")
 
-        endpoint_id = dict_copy.pop("endpointId")
+        endpoint_id = d.pop("endpointId")
 
-        app_uid = dict_copy.pop("appUid", UNSET)
+        app_uid = d.pop("appUid", UNSET)
 
-        endpoint_uid = dict_copy.pop("endpointUid", UNSET)
+        endpoint_uid = d.pop("endpointUid", UNSET)
 
         endpoint_updated_event_data = cls(
             app_id=app_id,
             endpoint_id=endpoint_id,
             app_uid=app_uid,
             endpoint_uid=endpoint_uid,
         )
 
-        endpoint_updated_event_data.additional_properties = dict_copy
+        endpoint_updated_event_data.additional_properties = d
         return endpoint_updated_event_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/environment_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/environment_in.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,41 +62,44 @@
         if settings is not UNSET:
             field_dict["settings"] = settings
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        created_at = isoparse(dict_copy.pop("createdAt"))
+        from ..models.event_type_in import EventTypeIn
+        from ..models.settings_in import SettingsIn
 
-        version = dict_copy.pop("version")
+        d = src_dict.copy()
+        created_at = isoparse(d.pop("createdAt"))
+
+        version = d.pop("version")
 
         event_types = []
-        _event_types = dict_copy.pop("eventTypes", UNSET)
+        _event_types = d.pop("eventTypes", UNSET)
         for event_types_item_data in _event_types or []:
             event_types_item = EventTypeIn.from_dict(event_types_item_data)
 
             event_types.append(event_types_item)
 
-        _settings = dict_copy.pop("settings", UNSET)
+        _settings = d.pop("settings", UNSET)
         settings: Union[Unset, SettingsIn]
         if isinstance(_settings, Unset):
             settings = UNSET
         else:
             settings = SettingsIn.from_dict(_settings)
 
         environment_in = cls(
             created_at=created_at,
             version=version,
             event_types=event_types,
             settings=settings,
         )
 
-        environment_in.additional_properties = dict_copy
+        environment_in.additional_properties = d
         return environment_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/environment_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/environment_out.py`

 * *Files 13% similar despite different names*

```diff
@@ -58,41 +58,44 @@
         if version is not UNSET:
             field_dict["version"] = version
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        created_at = isoparse(dict_copy.pop("createdAt"))
+        from ..models.event_type_out import EventTypeOut
+        from ..models.settings_out import SettingsOut
+
+        d = src_dict.copy()
+        created_at = isoparse(d.pop("createdAt"))
 
         event_types = []
-        _event_types = dict_copy.pop("eventTypes")
+        _event_types = d.pop("eventTypes")
         for event_types_item_data in _event_types:
             event_types_item = EventTypeOut.from_dict(event_types_item_data)
 
             event_types.append(event_types_item)
 
-        _settings = dict_copy.pop("settings", UNSET)
+        _settings = d.pop("settings", UNSET)
         settings: Union[Unset, SettingsOut]
         if isinstance(_settings, Unset):
             settings = UNSET
         else:
             settings = SettingsOut.from_dict(_settings)
 
-        version = dict_copy.pop("version", UNSET)
+        version = d.pop("version", UNSET)
 
         environment_out = cls(
             created_at=created_at,
             event_types=event_types,
             settings=settings,
             version=version,
         )
 
-        environment_out.additional_properties = dict_copy
+        environment_out.additional_properties = d
         return environment_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/environment_settings_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/environment_settings_out.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,61 +80,64 @@
         if enable_transformations is not UNSET:
             field_dict["enableTransformations"] = enable_transformations
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        _color_palette_dark = dict_copy.pop("colorPaletteDark", UNSET)
+        from ..models.custom_color_palette import CustomColorPalette
+        from ..models.custom_theme_override import CustomThemeOverride
+
+        d = src_dict.copy()
+        _color_palette_dark = d.pop("colorPaletteDark", UNSET)
         color_palette_dark: Union[Unset, CustomColorPalette]
         if isinstance(_color_palette_dark, Unset):
             color_palette_dark = UNSET
         else:
             color_palette_dark = CustomColorPalette.from_dict(_color_palette_dark)
 
-        _color_palette_light = dict_copy.pop("colorPaletteLight", UNSET)
+        _color_palette_light = d.pop("colorPaletteLight", UNSET)
         color_palette_light: Union[Unset, CustomColorPalette]
         if isinstance(_color_palette_light, Unset):
             color_palette_light = UNSET
         else:
             color_palette_light = CustomColorPalette.from_dict(_color_palette_light)
 
-        custom_color = dict_copy.pop("customColor", UNSET)
+        custom_color = d.pop("customColor", UNSET)
 
-        custom_font_family = dict_copy.pop("customFontFamily", UNSET)
+        custom_font_family = d.pop("customFontFamily", UNSET)
 
-        custom_logo_url = dict_copy.pop("customLogoUrl", UNSET)
+        custom_logo_url = d.pop("customLogoUrl", UNSET)
 
-        _custom_theme_override = dict_copy.pop("customThemeOverride", UNSET)
+        _custom_theme_override = d.pop("customThemeOverride", UNSET)
         custom_theme_override: Union[Unset, CustomThemeOverride]
         if isinstance(_custom_theme_override, Unset):
             custom_theme_override = UNSET
         else:
             custom_theme_override = CustomThemeOverride.from_dict(_custom_theme_override)
 
-        enable_channels = dict_copy.pop("enableChannels", UNSET)
+        enable_channels = d.pop("enableChannels", UNSET)
 
-        enable_integration_management = dict_copy.pop("enableIntegrationManagement", UNSET)
+        enable_integration_management = d.pop("enableIntegrationManagement", UNSET)
 
-        enable_transformations = dict_copy.pop("enableTransformations", UNSET)
+        enable_transformations = d.pop("enableTransformations", UNSET)
 
         environment_settings_out = cls(
             color_palette_dark=color_palette_dark,
             color_palette_light=color_palette_light,
             custom_color=custom_color,
             custom_font_family=custom_font_family,
             custom_logo_url=custom_logo_url,
             custom_theme_override=custom_theme_override,
             enable_channels=enable_channels,
             enable_integration_management=enable_integration_management,
             enable_transformations=enable_transformations,
         )
 
-        environment_settings_out.additional_properties = dict_copy
+        environment_settings_out.additional_properties = d
         return environment_settings_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/event_example_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/event_example_in.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,22 +26,22 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        event_type = dict_copy.pop("eventType")
+        d = src_dict.copy()
+        event_type = d.pop("eventType")
 
         event_example_in = cls(
             event_type=event_type,
         )
 
-        event_example_in.additional_properties = dict_copy
+        event_example_in.additional_properties = d
         return event_example_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/event_type_example_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/event_type_example_out.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,22 +31,22 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        example = dict_copy.pop("example")
+        d = src_dict.copy()
+        example = d.pop("example")
 
         event_type_example_out = cls(
             example=example,
         )
 
-        event_type_example_out.additional_properties = dict_copy
+        event_type_example_out.additional_properties = d
         return event_type_example_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/event_type_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/event_type_in.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,34 +54,34 @@
         if schemas is not UNSET:
             field_dict["schemas"] = schemas
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        description = dict_copy.pop("description")
+        d = src_dict.copy()
+        description = d.pop("description")
 
-        name = dict_copy.pop("name")
+        name = d.pop("name")
 
-        archived = dict_copy.pop("archived", UNSET)
+        archived = d.pop("archived", UNSET)
 
-        feature_flag = dict_copy.pop("featureFlag", UNSET)
+        feature_flag = d.pop("featureFlag", UNSET)
 
-        schemas = dict_copy.pop("schemas", UNSET)
+        schemas = d.pop("schemas", UNSET)
 
         event_type_in = cls(
             description=description,
             name=name,
             archived=archived,
             feature_flag=feature_flag,
             schemas=schemas,
         )
 
-        event_type_in.additional_properties = dict_copy
+        event_type_in.additional_properties = d
         return event_type_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/event_type_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/event_type_out.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,40 +66,40 @@
         if schemas is not UNSET:
             field_dict["schemas"] = schemas
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        created_at = isoparse(dict_copy.pop("createdAt"))
+        d = src_dict.copy()
+        created_at = isoparse(d.pop("createdAt"))
 
-        description = dict_copy.pop("description")
+        description = d.pop("description")
 
-        name = dict_copy.pop("name")
+        name = d.pop("name")
 
-        updated_at = isoparse(dict_copy.pop("updatedAt"))
+        updated_at = isoparse(d.pop("updatedAt"))
 
-        archived = dict_copy.pop("archived", UNSET)
+        archived = d.pop("archived", UNSET)
 
-        feature_flag = dict_copy.pop("featureFlag", UNSET)
+        feature_flag = d.pop("featureFlag", UNSET)
 
-        schemas = dict_copy.pop("schemas", UNSET)
+        schemas = d.pop("schemas", UNSET)
 
         event_type_out = cls(
             created_at=created_at,
             description=description,
             name=name,
             updated_at=updated_at,
             archived=archived,
             feature_flag=feature_flag,
             schemas=schemas,
         )
 
-        event_type_out.additional_properties = dict_copy
+        event_type_out.additional_properties = d
         return event_type_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/event_type_patch.py` & `svix-1.5.0/svix/internal/openapi_client/models/event_type_patch.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,31 +48,31 @@
         if schemas is not UNSET:
             field_dict["schemas"] = schemas
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        archived = dict_copy.pop("archived", UNSET)
+        d = src_dict.copy()
+        archived = d.pop("archived", UNSET)
 
-        description = dict_copy.pop("description", UNSET)
+        description = d.pop("description", UNSET)
 
-        feature_flag = dict_copy.pop("featureFlag", UNSET)
+        feature_flag = d.pop("featureFlag", UNSET)
 
-        schemas = dict_copy.pop("schemas", UNSET)
+        schemas = d.pop("schemas", UNSET)
 
         event_type_patch = cls(
             archived=archived,
             description=description,
             feature_flag=feature_flag,
             schemas=schemas,
         )
 
-        event_type_patch.additional_properties = dict_copy
+        event_type_patch.additional_properties = d
         return event_type_patch
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/event_type_schema_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/event_type_schema_in.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,22 +32,22 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        schema = dict_copy.pop("schema")
+        d = src_dict.copy()
+        schema = d.pop("schema")
 
         event_type_schema_in = cls(
             schema=schema,
         )
 
-        event_type_schema_in.additional_properties = dict_copy
+        event_type_schema_in.additional_properties = d
         return event_type_schema_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/event_type_update.py` & `svix-1.5.0/svix/internal/openapi_client/models/event_type_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,31 +50,31 @@
         if schemas is not UNSET:
             field_dict["schemas"] = schemas
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        description = dict_copy.pop("description")
+        d = src_dict.copy()
+        description = d.pop("description")
 
-        archived = dict_copy.pop("archived", UNSET)
+        archived = d.pop("archived", UNSET)
 
-        feature_flag = dict_copy.pop("featureFlag", UNSET)
+        feature_flag = d.pop("featureFlag", UNSET)
 
-        schemas = dict_copy.pop("schemas", UNSET)
+        schemas = d.pop("schemas", UNSET)
 
         event_type_update = cls(
             description=description,
             archived=archived,
             feature_flag=feature_flag,
             schemas=schemas,
         )
 
-        event_type_update.additional_properties = dict_copy
+        event_type_update.additional_properties = d
         return event_type_update
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/font_size_config.py` & `svix-1.5.0/svix/internal/openapi_client/models/font_size_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,22 +26,22 @@
         if base is not UNSET:
             field_dict["base"] = base
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        base = dict_copy.pop("base", UNSET)
+        d = src_dict.copy()
+        base = d.pop("base", UNSET)
 
         font_size_config = cls(
             base=base,
         )
 
-        font_size_config.additional_properties = dict_copy
+        font_size_config.additional_properties = d
         return font_size_config
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/integration_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/integration_in.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,22 +26,22 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        name = dict_copy.pop("name")
+        d = src_dict.copy()
+        name = d.pop("name")
 
         integration_in = cls(
             name=name,
         )
 
-        integration_in.additional_properties = dict_copy
+        integration_in.additional_properties = d
         return integration_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/integration_key_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/integration_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="IntegrationKeyOut")
+T = TypeVar("T", bound="IntegrationUpdate")
 
 
 @attr.s(auto_attribs=True)
-class IntegrationKeyOut:
+class IntegrationUpdate:
     """
     Attributes:
-        key (str):  Example: integsk_kV3ts5tKPNJN4Dl25cMTfUNdmabxbX0O.
+        name (str):  Example: Example Integration.
     """
 
-    key: str
+    name: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        key = self.key
+        name = self.name
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "key": key,
+                "name": name,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        key = dict_copy.pop("key")
+        d = src_dict.copy()
+        name = d.pop("name")
 
-        integration_key_out = cls(
-            key=key,
+        integration_update = cls(
+            name=name,
         )
 
-        integration_key_out.additional_properties = dict_copy
-        return integration_key_out
+        integration_update.additional_properties = d
+        return integration_update
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/integration_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/integration_out.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,31 +41,31 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        created_at = isoparse(dict_copy.pop("createdAt"))
+        d = src_dict.copy()
+        created_at = isoparse(d.pop("createdAt"))
 
-        id = dict_copy.pop("id")
+        id = d.pop("id")
 
-        name = dict_copy.pop("name")
+        name = d.pop("name")
 
-        updated_at = isoparse(dict_copy.pop("updatedAt"))
+        updated_at = isoparse(d.pop("updatedAt"))
 
         integration_out = cls(
             created_at=created_at,
             id=id,
             name=name,
             updated_at=updated_at,
         )
 
-        integration_out.additional_properties = dict_copy
+        integration_out.additional_properties = d
         return integration_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/integration_update.py` & `svix-1.5.0/svix/internal/openapi_client/models/one_time_token_out.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="IntegrationUpdate")
+T = TypeVar("T", bound="OneTimeTokenOut")
 
 
 @attr.s(auto_attribs=True)
-class IntegrationUpdate:
+class OneTimeTokenOut:
     """
     Attributes:
-        name (str):  Example: Example Integration.
+        token (str):
     """
 
-    name: str
+    token: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        name = self.name
+        token = self.token
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "name": name,
+                "token": token,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        name = dict_copy.pop("name")
+        d = src_dict.copy()
+        token = d.pop("token")
 
-        integration_update = cls(
-            name=name,
+        one_time_token_out = cls(
+            token=token,
         )
 
-        integration_update.additional_properties = dict_copy
-        return integration_update
+        one_time_token_out.additional_properties = d
+        return one_time_token_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/list_response_application_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/list_response_integration_out.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.application_out import ApplicationOut
+    from ..models.integration_out import IntegrationOut
 
 
-T = TypeVar("T", bound="ListResponseApplicationOut")
+T = TypeVar("T", bound="ListResponseIntegrationOut")
 
 
 @attr.s(auto_attribs=True)
-class ListResponseApplicationOut:
+class ListResponseIntegrationOut:
     """
     Attributes:
-        data (List['ApplicationOut']):
+        data (List['IntegrationOut']):
         done (bool):
         iterator (Union[Unset, None, str]):  Example: iterator.
         prev_iterator (Union[Unset, None, str]):  Example: -iterator.
     """
 
-    data: List["ApplicationOut"]
+    data: List["IntegrationOut"]
     done: bool
     iterator: Union[Unset, None, str] = UNSET
     prev_iterator: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         data = []
@@ -51,37 +51,39 @@
         if prev_iterator is not UNSET:
             field_dict["prevIterator"] = prev_iterator
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
+        from ..models.integration_out import IntegrationOut
+
+        d = src_dict.copy()
         data = []
-        _data = dict_copy.pop("data")
+        _data = d.pop("data")
         for data_item_data in _data:
-            data_item = ApplicationOut.from_dict(data_item_data)
+            data_item = IntegrationOut.from_dict(data_item_data)
 
             data.append(data_item)
 
-        done = dict_copy.pop("done")
+        done = d.pop("done")
 
-        iterator = dict_copy.pop("iterator", UNSET)
+        iterator = d.pop("iterator", UNSET)
 
-        prev_iterator = dict_copy.pop("prevIterator", UNSET)
+        prev_iterator = d.pop("prevIterator", UNSET)
 
-        list_response_application_out = cls(
+        list_response_integration_out = cls(
             data=data,
             done=done,
             iterator=iterator,
             prev_iterator=prev_iterator,
         )
 
-        list_response_application_out.additional_properties = dict_copy
-        return list_response_application_out
+        list_response_integration_out.additional_properties = d
+        return list_response_integration_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/list_response_application_stats.py` & `svix-1.5.0/svix/internal/openapi_client/models/list_response_application_stats.py`

 * *Files 13% similar despite different names*

```diff
@@ -51,36 +51,38 @@
         if prev_iterator is not UNSET:
             field_dict["prevIterator"] = prev_iterator
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
+        from ..models.application_stats import ApplicationStats
+
+        d = src_dict.copy()
         data = []
-        _data = dict_copy.pop("data")
+        _data = d.pop("data")
         for data_item_data in _data:
             data_item = ApplicationStats.from_dict(data_item_data)
 
             data.append(data_item)
 
-        done = dict_copy.pop("done")
+        done = d.pop("done")
 
-        iterator = dict_copy.pop("iterator", UNSET)
+        iterator = d.pop("iterator", UNSET)
 
-        prev_iterator = dict_copy.pop("prevIterator", UNSET)
+        prev_iterator = d.pop("prevIterator", UNSET)
 
         list_response_application_stats = cls(
             data=data,
             done=done,
             iterator=iterator,
             prev_iterator=prev_iterator,
         )
 
-        list_response_application_stats.additional_properties = dict_copy
+        list_response_application_stats.additional_properties = d
         return list_response_application_stats
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/list_response_background_task_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/list_response_endpoint_out.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.background_task_out import BackgroundTaskOut
+    from ..models.endpoint_out import EndpointOut
 
 
-T = TypeVar("T", bound="ListResponseBackgroundTaskOut")
+T = TypeVar("T", bound="ListResponseEndpointOut")
 
 
 @attr.s(auto_attribs=True)
-class ListResponseBackgroundTaskOut:
+class ListResponseEndpointOut:
     """
     Attributes:
-        data (List['BackgroundTaskOut']):
+        data (List['EndpointOut']):
         done (bool):
         iterator (Union[Unset, None, str]):  Example: iterator.
         prev_iterator (Union[Unset, None, str]):  Example: -iterator.
     """
 
-    data: List["BackgroundTaskOut"]
+    data: List["EndpointOut"]
     done: bool
     iterator: Union[Unset, None, str] = UNSET
     prev_iterator: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         data = []
@@ -51,37 +51,39 @@
         if prev_iterator is not UNSET:
             field_dict["prevIterator"] = prev_iterator
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
+        from ..models.endpoint_out import EndpointOut
+
+        d = src_dict.copy()
         data = []
-        _data = dict_copy.pop("data")
+        _data = d.pop("data")
         for data_item_data in _data:
-            data_item = BackgroundTaskOut.from_dict(data_item_data)
+            data_item = EndpointOut.from_dict(data_item_data)
 
             data.append(data_item)
 
-        done = dict_copy.pop("done")
+        done = d.pop("done")
 
-        iterator = dict_copy.pop("iterator", UNSET)
+        iterator = d.pop("iterator", UNSET)
 
-        prev_iterator = dict_copy.pop("prevIterator", UNSET)
+        prev_iterator = d.pop("prevIterator", UNSET)
 
-        list_response_background_task_out = cls(
+        list_response_endpoint_out = cls(
             data=data,
             done=done,
             iterator=iterator,
             prev_iterator=prev_iterator,
         )
 
-        list_response_background_task_out.additional_properties = dict_copy
-        return list_response_background_task_out
+        list_response_endpoint_out.additional_properties = d
+        return list_response_endpoint_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/list_response_endpoint_message_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/list_response_message_attempt_endpoint_out.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.endpoint_message_out import EndpointMessageOut
+    from ..models.message_attempt_endpoint_out import MessageAttemptEndpointOut
 
 
-T = TypeVar("T", bound="ListResponseEndpointMessageOut")
+T = TypeVar("T", bound="ListResponseMessageAttemptEndpointOut")
 
 
 @attr.s(auto_attribs=True)
-class ListResponseEndpointMessageOut:
+class ListResponseMessageAttemptEndpointOut:
     """
     Attributes:
-        data (List['EndpointMessageOut']):
+        data (List['MessageAttemptEndpointOut']):
         done (bool):
         iterator (Union[Unset, None, str]):  Example: iterator.
         prev_iterator (Union[Unset, None, str]):  Example: -iterator.
     """
 
-    data: List["EndpointMessageOut"]
+    data: List["MessageAttemptEndpointOut"]
     done: bool
     iterator: Union[Unset, None, str] = UNSET
     prev_iterator: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         data = []
@@ -51,37 +51,39 @@
         if prev_iterator is not UNSET:
             field_dict["prevIterator"] = prev_iterator
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
+        from ..models.message_attempt_endpoint_out import MessageAttemptEndpointOut
+
+        d = src_dict.copy()
         data = []
-        _data = dict_copy.pop("data")
+        _data = d.pop("data")
         for data_item_data in _data:
-            data_item = EndpointMessageOut.from_dict(data_item_data)
+            data_item = MessageAttemptEndpointOut.from_dict(data_item_data)
 
             data.append(data_item)
 
-        done = dict_copy.pop("done")
+        done = d.pop("done")
 
-        iterator = dict_copy.pop("iterator", UNSET)
+        iterator = d.pop("iterator", UNSET)
 
-        prev_iterator = dict_copy.pop("prevIterator", UNSET)
+        prev_iterator = d.pop("prevIterator", UNSET)
 
-        list_response_endpoint_message_out = cls(
+        list_response_message_attempt_endpoint_out = cls(
             data=data,
             done=done,
             iterator=iterator,
             prev_iterator=prev_iterator,
         )
 
-        list_response_endpoint_message_out.additional_properties = dict_copy
-        return list_response_endpoint_message_out
+        list_response_message_attempt_endpoint_out.additional_properties = d
+        return list_response_message_attempt_endpoint_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/list_response_endpoint_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/list_response_application_out.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.endpoint_out import EndpointOut
+    from ..models.application_out import ApplicationOut
 
 
-T = TypeVar("T", bound="ListResponseEndpointOut")
+T = TypeVar("T", bound="ListResponseApplicationOut")
 
 
 @attr.s(auto_attribs=True)
-class ListResponseEndpointOut:
+class ListResponseApplicationOut:
     """
     Attributes:
-        data (List['EndpointOut']):
+        data (List['ApplicationOut']):
         done (bool):
         iterator (Union[Unset, None, str]):  Example: iterator.
         prev_iterator (Union[Unset, None, str]):  Example: -iterator.
     """
 
-    data: List["EndpointOut"]
+    data: List["ApplicationOut"]
     done: bool
     iterator: Union[Unset, None, str] = UNSET
     prev_iterator: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         data = []
@@ -51,37 +51,39 @@
         if prev_iterator is not UNSET:
             field_dict["prevIterator"] = prev_iterator
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
+        from ..models.application_out import ApplicationOut
+
+        d = src_dict.copy()
         data = []
-        _data = dict_copy.pop("data")
+        _data = d.pop("data")
         for data_item_data in _data:
-            data_item = EndpointOut.from_dict(data_item_data)
+            data_item = ApplicationOut.from_dict(data_item_data)
 
             data.append(data_item)
 
-        done = dict_copy.pop("done")
+        done = d.pop("done")
 
-        iterator = dict_copy.pop("iterator", UNSET)
+        iterator = d.pop("iterator", UNSET)
 
-        prev_iterator = dict_copy.pop("prevIterator", UNSET)
+        prev_iterator = d.pop("prevIterator", UNSET)
 
-        list_response_endpoint_out = cls(
+        list_response_application_out = cls(
             data=data,
             done=done,
             iterator=iterator,
             prev_iterator=prev_iterator,
         )
 
-        list_response_endpoint_out.additional_properties = dict_copy
-        return list_response_endpoint_out
+        list_response_application_out.additional_properties = d
+        return list_response_application_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/list_response_event_type_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/list_response_event_type_out.py`

 * *Files 16% similar despite different names*

```diff
@@ -51,36 +51,38 @@
         if prev_iterator is not UNSET:
             field_dict["prevIterator"] = prev_iterator
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
+        from ..models.event_type_out import EventTypeOut
+
+        d = src_dict.copy()
         data = []
-        _data = dict_copy.pop("data")
+        _data = d.pop("data")
         for data_item_data in _data:
             data_item = EventTypeOut.from_dict(data_item_data)
 
             data.append(data_item)
 
-        done = dict_copy.pop("done")
+        done = d.pop("done")
 
-        iterator = dict_copy.pop("iterator", UNSET)
+        iterator = d.pop("iterator", UNSET)
 
-        prev_iterator = dict_copy.pop("prevIterator", UNSET)
+        prev_iterator = d.pop("prevIterator", UNSET)
 
         list_response_event_type_out = cls(
             data=data,
             done=done,
             iterator=iterator,
             prev_iterator=prev_iterator,
         )
 
-        list_response_event_type_out.additional_properties = dict_copy
+        list_response_event_type_out.additional_properties = d
         return list_response_event_type_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/list_response_integration_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/list_response_message_endpoint_out.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.integration_out import IntegrationOut
+    from ..models.message_endpoint_out import MessageEndpointOut
 
 
-T = TypeVar("T", bound="ListResponseIntegrationOut")
+T = TypeVar("T", bound="ListResponseMessageEndpointOut")
 
 
 @attr.s(auto_attribs=True)
-class ListResponseIntegrationOut:
+class ListResponseMessageEndpointOut:
     """
     Attributes:
-        data (List['IntegrationOut']):
+        data (List['MessageEndpointOut']):
         done (bool):
         iterator (Union[Unset, None, str]):  Example: iterator.
         prev_iterator (Union[Unset, None, str]):  Example: -iterator.
     """
 
-    data: List["IntegrationOut"]
+    data: List["MessageEndpointOut"]
     done: bool
     iterator: Union[Unset, None, str] = UNSET
     prev_iterator: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         data = []
@@ -51,37 +51,39 @@
         if prev_iterator is not UNSET:
             field_dict["prevIterator"] = prev_iterator
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
+        from ..models.message_endpoint_out import MessageEndpointOut
+
+        d = src_dict.copy()
         data = []
-        _data = dict_copy.pop("data")
+        _data = d.pop("data")
         for data_item_data in _data:
-            data_item = IntegrationOut.from_dict(data_item_data)
+            data_item = MessageEndpointOut.from_dict(data_item_data)
 
             data.append(data_item)
 
-        done = dict_copy.pop("done")
+        done = d.pop("done")
 
-        iterator = dict_copy.pop("iterator", UNSET)
+        iterator = d.pop("iterator", UNSET)
 
-        prev_iterator = dict_copy.pop("prevIterator", UNSET)
+        prev_iterator = d.pop("prevIterator", UNSET)
 
-        list_response_integration_out = cls(
+        list_response_message_endpoint_out = cls(
             data=data,
             done=done,
             iterator=iterator,
             prev_iterator=prev_iterator,
         )
 
-        list_response_integration_out.additional_properties = dict_copy
-        return list_response_integration_out
+        list_response_message_endpoint_out.additional_properties = d
+        return list_response_message_endpoint_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/list_response_message_attempt_endpoint_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/list_response_endpoint_message_out.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.message_attempt_endpoint_out import MessageAttemptEndpointOut
+    from ..models.endpoint_message_out import EndpointMessageOut
 
 
-T = TypeVar("T", bound="ListResponseMessageAttemptEndpointOut")
+T = TypeVar("T", bound="ListResponseEndpointMessageOut")
 
 
 @attr.s(auto_attribs=True)
-class ListResponseMessageAttemptEndpointOut:
+class ListResponseEndpointMessageOut:
     """
     Attributes:
-        data (List['MessageAttemptEndpointOut']):
+        data (List['EndpointMessageOut']):
         done (bool):
         iterator (Union[Unset, None, str]):  Example: iterator.
         prev_iterator (Union[Unset, None, str]):  Example: -iterator.
     """
 
-    data: List["MessageAttemptEndpointOut"]
+    data: List["EndpointMessageOut"]
     done: bool
     iterator: Union[Unset, None, str] = UNSET
     prev_iterator: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         data = []
@@ -51,37 +51,39 @@
         if prev_iterator is not UNSET:
             field_dict["prevIterator"] = prev_iterator
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
+        from ..models.endpoint_message_out import EndpointMessageOut
+
+        d = src_dict.copy()
         data = []
-        _data = dict_copy.pop("data")
+        _data = d.pop("data")
         for data_item_data in _data:
-            data_item = MessageAttemptEndpointOut.from_dict(data_item_data)
+            data_item = EndpointMessageOut.from_dict(data_item_data)
 
             data.append(data_item)
 
-        done = dict_copy.pop("done")
+        done = d.pop("done")
 
-        iterator = dict_copy.pop("iterator", UNSET)
+        iterator = d.pop("iterator", UNSET)
 
-        prev_iterator = dict_copy.pop("prevIterator", UNSET)
+        prev_iterator = d.pop("prevIterator", UNSET)
 
-        list_response_message_attempt_endpoint_out = cls(
+        list_response_endpoint_message_out = cls(
             data=data,
             done=done,
             iterator=iterator,
             prev_iterator=prev_iterator,
         )
 
-        list_response_message_attempt_endpoint_out.additional_properties = dict_copy
-        return list_response_message_attempt_endpoint_out
+        list_response_endpoint_message_out.additional_properties = d
+        return list_response_endpoint_message_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/list_response_message_attempt_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/list_response_message_attempt_out.py`

 * *Files 18% similar despite different names*

```diff
@@ -51,36 +51,38 @@
         if prev_iterator is not UNSET:
             field_dict["prevIterator"] = prev_iterator
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
+        from ..models.message_attempt_out import MessageAttemptOut
+
+        d = src_dict.copy()
         data = []
-        _data = dict_copy.pop("data")
+        _data = d.pop("data")
         for data_item_data in _data:
             data_item = MessageAttemptOut.from_dict(data_item_data)
 
             data.append(data_item)
 
-        done = dict_copy.pop("done")
+        done = d.pop("done")
 
-        iterator = dict_copy.pop("iterator", UNSET)
+        iterator = d.pop("iterator", UNSET)
 
-        prev_iterator = dict_copy.pop("prevIterator", UNSET)
+        prev_iterator = d.pop("prevIterator", UNSET)
 
         list_response_message_attempt_out = cls(
             data=data,
             done=done,
             iterator=iterator,
             prev_iterator=prev_iterator,
         )
 
-        list_response_message_attempt_out.additional_properties = dict_copy
+        list_response_message_attempt_out.additional_properties = d
         return list_response_message_attempt_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/list_response_message_endpoint_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/list_response_message_out.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.message_endpoint_out import MessageEndpointOut
+    from ..models.message_out import MessageOut
 
 
-T = TypeVar("T", bound="ListResponseMessageEndpointOut")
+T = TypeVar("T", bound="ListResponseMessageOut")
 
 
 @attr.s(auto_attribs=True)
-class ListResponseMessageEndpointOut:
+class ListResponseMessageOut:
     """
     Attributes:
-        data (List['MessageEndpointOut']):
+        data (List['MessageOut']):
         done (bool):
         iterator (Union[Unset, None, str]):  Example: iterator.
         prev_iterator (Union[Unset, None, str]):  Example: -iterator.
     """
 
-    data: List["MessageEndpointOut"]
+    data: List["MessageOut"]
     done: bool
     iterator: Union[Unset, None, str] = UNSET
     prev_iterator: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         data = []
@@ -51,37 +51,39 @@
         if prev_iterator is not UNSET:
             field_dict["prevIterator"] = prev_iterator
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
+        from ..models.message_out import MessageOut
+
+        d = src_dict.copy()
         data = []
-        _data = dict_copy.pop("data")
+        _data = d.pop("data")
         for data_item_data in _data:
-            data_item = MessageEndpointOut.from_dict(data_item_data)
+            data_item = MessageOut.from_dict(data_item_data)
 
             data.append(data_item)
 
-        done = dict_copy.pop("done")
+        done = d.pop("done")
 
-        iterator = dict_copy.pop("iterator", UNSET)
+        iterator = d.pop("iterator", UNSET)
 
-        prev_iterator = dict_copy.pop("prevIterator", UNSET)
+        prev_iterator = d.pop("prevIterator", UNSET)
 
-        list_response_message_endpoint_out = cls(
+        list_response_message_out = cls(
             data=data,
             done=done,
             iterator=iterator,
             prev_iterator=prev_iterator,
         )
 
-        list_response_message_endpoint_out.additional_properties = dict_copy
-        return list_response_message_endpoint_out
+        list_response_message_out.additional_properties = d
+        return list_response_message_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/list_response_message_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/list_response_background_task_out.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.message_out import MessageOut
+    from ..models.background_task_out import BackgroundTaskOut
 
 
-T = TypeVar("T", bound="ListResponseMessageOut")
+T = TypeVar("T", bound="ListResponseBackgroundTaskOut")
 
 
 @attr.s(auto_attribs=True)
-class ListResponseMessageOut:
+class ListResponseBackgroundTaskOut:
     """
     Attributes:
-        data (List['MessageOut']):
+        data (List['BackgroundTaskOut']):
         done (bool):
         iterator (Union[Unset, None, str]):  Example: iterator.
         prev_iterator (Union[Unset, None, str]):  Example: -iterator.
     """
 
-    data: List["MessageOut"]
+    data: List["BackgroundTaskOut"]
     done: bool
     iterator: Union[Unset, None, str] = UNSET
     prev_iterator: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         data = []
@@ -51,37 +51,39 @@
         if prev_iterator is not UNSET:
             field_dict["prevIterator"] = prev_iterator
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
+        from ..models.background_task_out import BackgroundTaskOut
+
+        d = src_dict.copy()
         data = []
-        _data = dict_copy.pop("data")
+        _data = d.pop("data")
         for data_item_data in _data:
-            data_item = MessageOut.from_dict(data_item_data)
+            data_item = BackgroundTaskOut.from_dict(data_item_data)
 
             data.append(data_item)
 
-        done = dict_copy.pop("done")
+        done = d.pop("done")
 
-        iterator = dict_copy.pop("iterator", UNSET)
+        iterator = d.pop("iterator", UNSET)
 
-        prev_iterator = dict_copy.pop("prevIterator", UNSET)
+        prev_iterator = d.pop("prevIterator", UNSET)
 
-        list_response_message_out = cls(
+        list_response_background_task_out = cls(
             data=data,
             done=done,
             iterator=iterator,
             prev_iterator=prev_iterator,
         )
 
-        list_response_message_out.additional_properties = dict_copy
-        return list_response_message_out
+        list_response_background_task_out.additional_properties = d
+        return list_response_background_task_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/message_attempt_endpoint_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/message_attempt_out.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.message_attempt_trigger_type import MessageAttemptTriggerType
 from ..models.message_status import MessageStatus
 
-T = TypeVar("T", bound="MessageAttemptEndpointOut")
+T = TypeVar("T", bound="MessageAttemptOut")
 
 
 @attr.s(auto_attribs=True)
-class MessageAttemptEndpointOut:
+class MessageAttemptOut:
     """
     Attributes:
         endpoint_id (str): The ep's ID Example: ep_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         id (str): The attempt's ID Example: atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         msg_id (str): The msg's ID Example: msg_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         response (str):  Example: {}.
         response_status_code (int):  Example: 200.
@@ -72,47 +72,47 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        endpoint_id = dict_copy.pop("endpointId")
+        d = src_dict.copy()
+        endpoint_id = d.pop("endpointId")
 
-        id = dict_copy.pop("id")
+        id = d.pop("id")
 
-        msg_id = dict_copy.pop("msgId")
+        msg_id = d.pop("msgId")
 
-        response = dict_copy.pop("response")
+        response = d.pop("response")
 
-        response_status_code = dict_copy.pop("responseStatusCode")
+        response_status_code = d.pop("responseStatusCode")
 
-        status = MessageStatus(dict_copy.pop("status"))
+        status = MessageStatus(d.pop("status"))
 
-        timestamp = isoparse(dict_copy.pop("timestamp"))
+        timestamp = isoparse(d.pop("timestamp"))
 
-        trigger_type = MessageAttemptTriggerType(dict_copy.pop("triggerType"))
+        trigger_type = MessageAttemptTriggerType(d.pop("triggerType"))
 
-        url = dict_copy.pop("url")
+        url = d.pop("url")
 
-        message_attempt_endpoint_out = cls(
+        message_attempt_out = cls(
             endpoint_id=endpoint_id,
             id=id,
             msg_id=msg_id,
             response=response,
             response_status_code=response_status_code,
             status=status,
             timestamp=timestamp,
             trigger_type=trigger_type,
             url=url,
         )
 
-        message_attempt_endpoint_out.additional_properties = dict_copy
-        return message_attempt_endpoint_out
+        message_attempt_out.additional_properties = d
+        return message_attempt_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/message_attempt_exhausted_event.py` & `svix-1.5.0/svix/internal/openapi_client/models/message_attempt_exhausted_event.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,25 +40,27 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        data = MessageAttemptExhaustedEventData.from_dict(dict_copy.pop("data"))
+        from ..models.message_attempt_exhausted_event_data import MessageAttemptExhaustedEventData
 
-        type = MessageAttemptExhaustedEventType(dict_copy.pop("type"))
+        d = src_dict.copy()
+        data = MessageAttemptExhaustedEventData.from_dict(d.pop("data"))
+
+        type = MessageAttemptExhaustedEventType(d.pop("type"))
 
         message_attempt_exhausted_event = cls(
             data=data,
             type=type,
         )
 
-        message_attempt_exhausted_event.additional_properties = dict_copy
+        message_attempt_exhausted_event.additional_properties = d
         return message_attempt_exhausted_event
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/message_attempt_exhausted_event_data.py` & `svix-1.5.0/svix/internal/openapi_client/models/message_attempt_exhausted_event_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,37 +57,39 @@
         if msg_event_id is not UNSET:
             field_dict["msgEventId"] = msg_event_id
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        app_id = dict_copy.pop("appId")
+        from ..models.message_attempt_failed_data import MessageAttemptFailedData
 
-        endpoint_id = dict_copy.pop("endpointId")
+        d = src_dict.copy()
+        app_id = d.pop("appId")
 
-        last_attempt = MessageAttemptFailedData.from_dict(dict_copy.pop("lastAttempt"))
+        endpoint_id = d.pop("endpointId")
 
-        msg_id = dict_copy.pop("msgId")
+        last_attempt = MessageAttemptFailedData.from_dict(d.pop("lastAttempt"))
 
-        app_uid = dict_copy.pop("appUid", UNSET)
+        msg_id = d.pop("msgId")
 
-        msg_event_id = dict_copy.pop("msgEventId", UNSET)
+        app_uid = d.pop("appUid", UNSET)
+
+        msg_event_id = d.pop("msgEventId", UNSET)
 
         message_attempt_exhausted_event_data = cls(
             app_id=app_id,
             endpoint_id=endpoint_id,
             last_attempt=last_attempt,
             msg_id=msg_id,
             app_uid=app_uid,
             msg_event_id=msg_event_id,
         )
 
-        message_attempt_exhausted_event_data.additional_properties = dict_copy
+        message_attempt_exhausted_event_data.additional_properties = d
         return message_attempt_exhausted_event_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/message_attempt_failed_data.py` & `svix-1.5.0/svix/internal/openapi_client/models/message_attempt_failed_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,28 +36,28 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        id = dict_copy.pop("id")
+        d = src_dict.copy()
+        id = d.pop("id")
 
-        response_status_code = dict_copy.pop("responseStatusCode")
+        response_status_code = d.pop("responseStatusCode")
 
-        timestamp = isoparse(dict_copy.pop("timestamp"))
+        timestamp = isoparse(d.pop("timestamp"))
 
         message_attempt_failed_data = cls(
             id=id,
             response_status_code=response_status_code,
             timestamp=timestamp,
         )
 
-        message_attempt_failed_data.additional_properties = dict_copy
+        message_attempt_failed_data.additional_properties = d
         return message_attempt_failed_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/message_attempt_failing_event.py` & `svix-1.5.0/svix/internal/openapi_client/models/message_attempt_failing_event.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,25 +41,27 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        data = MessageAttemptFailingEventData.from_dict(dict_copy.pop("data"))
+        from ..models.message_attempt_failing_event_data import MessageAttemptFailingEventData
 
-        type = MessageAttemptFailingEventType(dict_copy.pop("type"))
+        d = src_dict.copy()
+        data = MessageAttemptFailingEventData.from_dict(d.pop("data"))
+
+        type = MessageAttemptFailingEventType(d.pop("type"))
 
         message_attempt_failing_event = cls(
             data=data,
             type=type,
         )
 
-        message_attempt_failing_event.additional_properties = dict_copy
+        message_attempt_failing_event.additional_properties = d
         return message_attempt_failing_event
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/message_attempt_failing_event_data.py` & `svix-1.5.0/svix/internal/openapi_client/models/message_attempt_failing_event_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,37 +57,39 @@
         if msg_event_id is not UNSET:
             field_dict["msgEventId"] = msg_event_id
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        app_id = dict_copy.pop("appId")
+        from ..models.message_attempt_failed_data import MessageAttemptFailedData
 
-        endpoint_id = dict_copy.pop("endpointId")
+        d = src_dict.copy()
+        app_id = d.pop("appId")
 
-        last_attempt = MessageAttemptFailedData.from_dict(dict_copy.pop("lastAttempt"))
+        endpoint_id = d.pop("endpointId")
 
-        msg_id = dict_copy.pop("msgId")
+        last_attempt = MessageAttemptFailedData.from_dict(d.pop("lastAttempt"))
 
-        app_uid = dict_copy.pop("appUid", UNSET)
+        msg_id = d.pop("msgId")
 
-        msg_event_id = dict_copy.pop("msgEventId", UNSET)
+        app_uid = d.pop("appUid", UNSET)
+
+        msg_event_id = d.pop("msgEventId", UNSET)
 
         message_attempt_failing_event_data = cls(
             app_id=app_id,
             endpoint_id=endpoint_id,
             last_attempt=last_attempt,
             msg_id=msg_id,
             app_uid=app_uid,
             msg_event_id=msg_event_id,
         )
 
-        message_attempt_failing_event_data.additional_properties = dict_copy
+        message_attempt_failing_event_data.additional_properties = d
         return message_attempt_failing_event_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/message_attempt_headers_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/message_attempt_headers_out.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,25 +35,25 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        sensitive = cast(List[str], dict_copy.pop("sensitive"))
+        d = src_dict.copy()
+        sensitive = cast(List[str], d.pop("sensitive"))
 
-        sent_headers = dict_copy.pop("sentHeaders")
+        sent_headers = d.pop("sentHeaders")
 
         message_attempt_headers_out = cls(
             sensitive=sensitive,
             sent_headers=sent_headers,
         )
 
-        message_attempt_headers_out.additional_properties = dict_copy
+        message_attempt_headers_out.additional_properties = d
         return message_attempt_headers_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/message_attempt_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/message_attempt_endpoint_out.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.message_attempt_trigger_type import MessageAttemptTriggerType
 from ..models.message_status import MessageStatus
 
-T = TypeVar("T", bound="MessageAttemptOut")
+T = TypeVar("T", bound="MessageAttemptEndpointOut")
 
 
 @attr.s(auto_attribs=True)
-class MessageAttemptOut:
+class MessageAttemptEndpointOut:
     """
     Attributes:
         endpoint_id (str): The ep's ID Example: ep_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         id (str): The attempt's ID Example: atmpt_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         msg_id (str): The msg's ID Example: msg_1srOrx2ZWZBpBUvZwXKQmoEYga2.
         response (str):  Example: {}.
         response_status_code (int):  Example: 200.
@@ -72,47 +72,47 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        endpoint_id = dict_copy.pop("endpointId")
+        d = src_dict.copy()
+        endpoint_id = d.pop("endpointId")
 
-        id = dict_copy.pop("id")
+        id = d.pop("id")
 
-        msg_id = dict_copy.pop("msgId")
+        msg_id = d.pop("msgId")
 
-        response = dict_copy.pop("response")
+        response = d.pop("response")
 
-        response_status_code = dict_copy.pop("responseStatusCode")
+        response_status_code = d.pop("responseStatusCode")
 
-        status = MessageStatus(dict_copy.pop("status"))
+        status = MessageStatus(d.pop("status"))
 
-        timestamp = isoparse(dict_copy.pop("timestamp"))
+        timestamp = isoparse(d.pop("timestamp"))
 
-        trigger_type = MessageAttemptTriggerType(dict_copy.pop("triggerType"))
+        trigger_type = MessageAttemptTriggerType(d.pop("triggerType"))
 
-        url = dict_copy.pop("url")
+        url = d.pop("url")
 
-        message_attempt_out = cls(
+        message_attempt_endpoint_out = cls(
             endpoint_id=endpoint_id,
             id=id,
             msg_id=msg_id,
             response=response,
             response_status_code=response_status_code,
             status=status,
             timestamp=timestamp,
             trigger_type=trigger_type,
             url=url,
         )
 
-        message_attempt_out.additional_properties = dict_copy
-        return message_attempt_out
+        message_attempt_endpoint_out.additional_properties = d
+        return message_attempt_endpoint_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/message_broadcast_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/message_broadcast_in.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,34 +58,34 @@
         if payload_retention_period is not UNSET:
             field_dict["payloadRetentionPeriod"] = payload_retention_period
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        event_type = dict_copy.pop("eventType")
+        d = src_dict.copy()
+        event_type = d.pop("eventType")
 
-        payload = dict_copy.pop("payload")
+        payload = d.pop("payload")
 
-        channels = cast(List[str], dict_copy.pop("channels", UNSET))
+        channels = cast(List[str], d.pop("channels", UNSET))
 
-        event_id = dict_copy.pop("eventId", UNSET)
+        event_id = d.pop("eventId", UNSET)
 
-        payload_retention_period = dict_copy.pop("payloadRetentionPeriod", UNSET)
+        payload_retention_period = d.pop("payloadRetentionPeriod", UNSET)
 
         message_broadcast_in = cls(
             event_type=event_type,
             payload=payload,
             channels=channels,
             event_id=event_id,
             payload_retention_period=payload_retention_period,
         )
 
-        message_broadcast_in.additional_properties = dict_copy
+        message_broadcast_in.additional_properties = d
         return message_broadcast_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/message_broadcast_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/message_broadcast_out.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,28 +38,28 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        id = dict_copy.pop("id")
+        d = src_dict.copy()
+        id = d.pop("id")
 
-        status = BackgroundTaskStatus(dict_copy.pop("status"))
+        status = BackgroundTaskStatus(d.pop("status"))
 
-        task = BackgroundTaskType(dict_copy.pop("task"))
+        task = BackgroundTaskType(d.pop("task"))
 
         message_broadcast_out = cls(
             id=id,
             status=status,
             task=task,
         )
 
-        message_broadcast_out.additional_properties = dict_copy
+        message_broadcast_out.additional_properties = d
         return message_broadcast_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/message_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/message_in.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,42 +67,44 @@
         if payload_retention_period is not UNSET:
             field_dict["payloadRetentionPeriod"] = payload_retention_period
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        event_type = dict_copy.pop("eventType")
+        from ..models.application_in import ApplicationIn
 
-        payload = dict_copy.pop("payload")
+        d = src_dict.copy()
+        event_type = d.pop("eventType")
 
-        _application = dict_copy.pop("application", UNSET)
+        payload = d.pop("payload")
+
+        _application = d.pop("application", UNSET)
         application: Union[Unset, ApplicationIn]
         if isinstance(_application, Unset):
             application = UNSET
         else:
             application = ApplicationIn.from_dict(_application)
 
-        channels = cast(List[str], dict_copy.pop("channels", UNSET))
+        channels = cast(List[str], d.pop("channels", UNSET))
 
-        event_id = dict_copy.pop("eventId", UNSET)
+        event_id = d.pop("eventId", UNSET)
 
-        payload_retention_period = dict_copy.pop("payloadRetentionPeriod", UNSET)
+        payload_retention_period = d.pop("payloadRetentionPeriod", UNSET)
 
         message_in = cls(
             event_type=event_type,
             payload=payload,
             application=application,
             channels=channels,
             event_id=event_id,
             payload_retention_period=payload_retention_period,
         )
 
-        message_in.additional_properties = dict_copy
+        message_in.additional_properties = d
         return message_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/message_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/message_out.py`

 * *Files 11% similar despite different names*

```diff
@@ -64,37 +64,37 @@
         if event_id is not UNSET:
             field_dict["eventId"] = event_id
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        event_type = dict_copy.pop("eventType")
+        d = src_dict.copy()
+        event_type = d.pop("eventType")
 
-        id = dict_copy.pop("id")
+        id = d.pop("id")
 
-        payload = dict_copy.pop("payload")
+        payload = d.pop("payload")
 
-        timestamp = isoparse(dict_copy.pop("timestamp"))
+        timestamp = isoparse(d.pop("timestamp"))
 
-        channels = cast(List[str], dict_copy.pop("channels", UNSET))
+        channels = cast(List[str], d.pop("channels", UNSET))
 
-        event_id = dict_copy.pop("eventId", UNSET)
+        event_id = d.pop("eventId", UNSET)
 
         message_out = cls(
             event_type=event_type,
             id=id,
             payload=payload,
             timestamp=timestamp,
             channels=channels,
             event_id=event_id,
         )
 
-        message_out.additional_properties = dict_copy
+        message_out.additional_properties = d
         return message_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/one_time_token_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/one_time_token_in.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,22 +26,22 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        one_time_token = dict_copy.pop("oneTimeToken")
+        d = src_dict.copy()
+        one_time_token = d.pop("oneTimeToken")
 
         one_time_token_in = cls(
             one_time_token=one_time_token,
         )
 
-        one_time_token_in.additional_properties = dict_copy
+        one_time_token_in.additional_properties = d
         return one_time_token_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/one_time_token_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/endpoint_headers_in.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,52 @@
-from typing import Any, Dict, List, Type, TypeVar
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="OneTimeTokenOut")
+if TYPE_CHECKING:
+    from ..models.endpoint_headers_in_headers import EndpointHeadersInHeaders
+
+
+T = TypeVar("T", bound="EndpointHeadersIn")
 
 
 @attr.s(auto_attribs=True)
-class OneTimeTokenOut:
+class EndpointHeadersIn:
     """
     Attributes:
-        token (str):
+        headers (EndpointHeadersInHeaders):  Example: {'X-Example': '123', 'X-Foobar': 'Bar'}.
     """
 
-    token: str
+    headers: "EndpointHeadersInHeaders"
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        token = self.token
+        headers = self.headers
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "token": token,
+                "headers": headers,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        token = dict_copy.pop("token")
+        d = src_dict.copy()
+        headers = d.pop("headers")
 
-        one_time_token_out = cls(
-            token=token,
+        endpoint_headers_in = cls(
+            headers=headers,
         )
 
-        one_time_token_out.additional_properties = dict_copy
-        return one_time_token_out
+        endpoint_headers_in.additional_properties = d
+        return endpoint_headers_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/recover_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/recover_in.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,32 +38,32 @@
         if until is not UNSET:
             field_dict["until"] = until
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        since = isoparse(dict_copy.pop("since"))
+        d = src_dict.copy()
+        since = isoparse(d.pop("since"))
 
-        _until = dict_copy.pop("until", UNSET)
+        _until = d.pop("until", UNSET)
         until: Union[Unset, None, datetime.datetime]
         if _until is None:
             until = None
         elif isinstance(_until, Unset):
             until = UNSET
         else:
             until = isoparse(_until)
 
         recover_in = cls(
             since=since,
             until=until,
         )
 
-        recover_in.additional_properties = dict_copy
+        recover_in.additional_properties = d
         return recover_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/recover_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/replay_out.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
 from ..models.background_task_status import BackgroundTaskStatus
 from ..models.background_task_type import BackgroundTaskType
 
-T = TypeVar("T", bound="RecoverOut")
+T = TypeVar("T", bound="ReplayOut")
 
 
 @attr.s(auto_attribs=True)
-class RecoverOut:
+class ReplayOut:
     """
     Attributes:
         id (str):
         status (BackgroundTaskStatus):
         task (BackgroundTaskType):
     """
 
@@ -38,29 +38,29 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        id = dict_copy.pop("id")
+        d = src_dict.copy()
+        id = d.pop("id")
 
-        status = BackgroundTaskStatus(dict_copy.pop("status"))
+        status = BackgroundTaskStatus(d.pop("status"))
 
-        task = BackgroundTaskType(dict_copy.pop("task"))
+        task = BackgroundTaskType(d.pop("task"))
 
-        recover_out = cls(
+        replay_out = cls(
             id=id,
             status=status,
             task=task,
         )
 
-        recover_out.additional_properties = dict_copy
-        return recover_out
+        replay_out.additional_properties = d
+        return replay_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/replay_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/replay_in.py`

 * *Files 14% similar despite different names*

```diff
@@ -38,32 +38,32 @@
         if until is not UNSET:
             field_dict["until"] = until
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        since = isoparse(dict_copy.pop("since"))
+        d = src_dict.copy()
+        since = isoparse(d.pop("since"))
 
-        _until = dict_copy.pop("until", UNSET)
+        _until = d.pop("until", UNSET)
         until: Union[Unset, None, datetime.datetime]
         if _until is None:
             until = None
         elif isinstance(_until, Unset):
             until = UNSET
         else:
             until = isoparse(_until)
 
         replay_in = cls(
             since=since,
             until=until,
         )
 
-        replay_in.additional_properties = dict_copy
+        replay_in.additional_properties = d
         return replay_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/replay_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/recover_out.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
 from ..models.background_task_status import BackgroundTaskStatus
 from ..models.background_task_type import BackgroundTaskType
 
-T = TypeVar("T", bound="ReplayOut")
+T = TypeVar("T", bound="RecoverOut")
 
 
 @attr.s(auto_attribs=True)
-class ReplayOut:
+class RecoverOut:
     """
     Attributes:
         id (str):
         status (BackgroundTaskStatus):
         task (BackgroundTaskType):
     """
 
@@ -38,29 +38,29 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        id = dict_copy.pop("id")
+        d = src_dict.copy()
+        id = d.pop("id")
 
-        status = BackgroundTaskStatus(dict_copy.pop("status"))
+        status = BackgroundTaskStatus(d.pop("status"))
 
-        task = BackgroundTaskType(dict_copy.pop("task"))
+        task = BackgroundTaskType(d.pop("task"))
 
-        replay_out = cls(
+        recover_out = cls(
             id=id,
             status=status,
             task=task,
         )
 
-        replay_out.additional_properties = dict_copy
-        return replay_out
+        recover_out.additional_properties = d
+        return recover_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/settings_in.py` & `svix-1.5.0/svix/internal/openapi_client/models/settings_out.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.custom_color_palette import CustomColorPalette
     from ..models.custom_theme_override import CustomThemeOverride
 
 
-T = TypeVar("T", bound="SettingsIn")
+T = TypeVar("T", bound="SettingsOut")
 
 
 @attr.s(auto_attribs=True)
-class SettingsIn:
+class SettingsOut:
     """
     Attributes:
         color_palette_dark (Union[Unset, CustomColorPalette]):
         color_palette_light (Union[Unset, CustomColorPalette]):
         custom_base_font_size (Union[Unset, None, int]):
         custom_color (Union[Unset, None, str]):
         custom_font_family (Union[Unset, None, str]):  Example: Open Sans.
@@ -110,61 +110,64 @@
         if read_only is not UNSET:
             field_dict["readOnly"] = read_only
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        _color_palette_dark = dict_copy.pop("colorPaletteDark", UNSET)
+        from ..models.custom_color_palette import CustomColorPalette
+        from ..models.custom_theme_override import CustomThemeOverride
+
+        d = src_dict.copy()
+        _color_palette_dark = d.pop("colorPaletteDark", UNSET)
         color_palette_dark: Union[Unset, CustomColorPalette]
         if isinstance(_color_palette_dark, Unset):
             color_palette_dark = UNSET
         else:
             color_palette_dark = CustomColorPalette.from_dict(_color_palette_dark)
 
-        _color_palette_light = dict_copy.pop("colorPaletteLight", UNSET)
+        _color_palette_light = d.pop("colorPaletteLight", UNSET)
         color_palette_light: Union[Unset, CustomColorPalette]
         if isinstance(_color_palette_light, Unset):
             color_palette_light = UNSET
         else:
             color_palette_light = CustomColorPalette.from_dict(_color_palette_light)
 
-        custom_base_font_size = dict_copy.pop("customBaseFontSize", UNSET)
+        custom_base_font_size = d.pop("customBaseFontSize", UNSET)
 
-        custom_color = dict_copy.pop("customColor", UNSET)
+        custom_color = d.pop("customColor", UNSET)
 
-        custom_font_family = dict_copy.pop("customFontFamily", UNSET)
+        custom_font_family = d.pop("customFontFamily", UNSET)
 
-        custom_logo_url = dict_copy.pop("customLogoUrl", UNSET)
+        custom_logo_url = d.pop("customLogoUrl", UNSET)
 
-        _custom_theme_override = dict_copy.pop("customThemeOverride", UNSET)
+        _custom_theme_override = d.pop("customThemeOverride", UNSET)
         custom_theme_override: Union[Unset, CustomThemeOverride]
         if isinstance(_custom_theme_override, Unset):
             custom_theme_override = UNSET
         else:
             custom_theme_override = CustomThemeOverride.from_dict(_custom_theme_override)
 
-        disable_endpoint_on_failure = dict_copy.pop("disableEndpointOnFailure", UNSET)
+        disable_endpoint_on_failure = d.pop("disableEndpointOnFailure", UNSET)
 
-        display_name = dict_copy.pop("displayName", UNSET)
+        display_name = d.pop("displayName", UNSET)
 
-        enable_channels = dict_copy.pop("enableChannels", UNSET)
+        enable_channels = d.pop("enableChannels", UNSET)
 
-        enable_integration_management = dict_copy.pop("enableIntegrationManagement", UNSET)
+        enable_integration_management = d.pop("enableIntegrationManagement", UNSET)
 
-        enable_transformations = dict_copy.pop("enableTransformations", UNSET)
+        enable_transformations = d.pop("enableTransformations", UNSET)
 
-        enforce_https = dict_copy.pop("enforceHttps", UNSET)
+        enforce_https = d.pop("enforceHttps", UNSET)
 
-        event_catalog_published = dict_copy.pop("eventCatalogPublished", UNSET)
+        event_catalog_published = d.pop("eventCatalogPublished", UNSET)
 
-        read_only = dict_copy.pop("readOnly", UNSET)
+        read_only = d.pop("readOnly", UNSET)
 
-        settings_in = cls(
+        settings_out = cls(
             color_palette_dark=color_palette_dark,
             color_palette_light=color_palette_light,
             custom_base_font_size=custom_base_font_size,
             custom_color=custom_color,
             custom_font_family=custom_font_family,
             custom_logo_url=custom_logo_url,
             custom_theme_override=custom_theme_override,
@@ -174,16 +177,16 @@
             enable_integration_management=enable_integration_management,
             enable_transformations=enable_transformations,
             enforce_https=enforce_https,
             event_catalog_published=event_catalog_published,
             read_only=read_only,
         )
 
-        settings_in.additional_properties = dict_copy
-        return settings_in
+        settings_out.additional_properties = d
+        return settings_out
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/models/settings_out.py` & `svix-1.5.0/svix/internal/openapi_client/models/settings_in.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.custom_color_palette import CustomColorPalette
     from ..models.custom_theme_override import CustomThemeOverride
 
 
-T = TypeVar("T", bound="SettingsOut")
+T = TypeVar("T", bound="SettingsIn")
 
 
 @attr.s(auto_attribs=True)
-class SettingsOut:
+class SettingsIn:
     """
     Attributes:
         color_palette_dark (Union[Unset, CustomColorPalette]):
         color_palette_light (Union[Unset, CustomColorPalette]):
         custom_base_font_size (Union[Unset, None, int]):
         custom_color (Union[Unset, None, str]):
         custom_font_family (Union[Unset, None, str]):  Example: Open Sans.
@@ -110,61 +110,64 @@
         if read_only is not UNSET:
             field_dict["readOnly"] = read_only
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        dict_copy = src_dict.copy()
-        _color_palette_dark = dict_copy.pop("colorPaletteDark", UNSET)
+        from ..models.custom_color_palette import CustomColorPalette
+        from ..models.custom_theme_override import CustomThemeOverride
+
+        d = src_dict.copy()
+        _color_palette_dark = d.pop("colorPaletteDark", UNSET)
         color_palette_dark: Union[Unset, CustomColorPalette]
         if isinstance(_color_palette_dark, Unset):
             color_palette_dark = UNSET
         else:
             color_palette_dark = CustomColorPalette.from_dict(_color_palette_dark)
 
-        _color_palette_light = dict_copy.pop("colorPaletteLight", UNSET)
+        _color_palette_light = d.pop("colorPaletteLight", UNSET)
         color_palette_light: Union[Unset, CustomColorPalette]
         if isinstance(_color_palette_light, Unset):
             color_palette_light = UNSET
         else:
             color_palette_light = CustomColorPalette.from_dict(_color_palette_light)
 
-        custom_base_font_size = dict_copy.pop("customBaseFontSize", UNSET)
+        custom_base_font_size = d.pop("customBaseFontSize", UNSET)
 
-        custom_color = dict_copy.pop("customColor", UNSET)
+        custom_color = d.pop("customColor", UNSET)
 
-        custom_font_family = dict_copy.pop("customFontFamily", UNSET)
+        custom_font_family = d.pop("customFontFamily", UNSET)
 
-        custom_logo_url = dict_copy.pop("customLogoUrl", UNSET)
+        custom_logo_url = d.pop("customLogoUrl", UNSET)
 
-        _custom_theme_override = dict_copy.pop("customThemeOverride", UNSET)
+        _custom_theme_override = d.pop("customThemeOverride", UNSET)
         custom_theme_override: Union[Unset, CustomThemeOverride]
         if isinstance(_custom_theme_override, Unset):
             custom_theme_override = UNSET
         else:
             custom_theme_override = CustomThemeOverride.from_dict(_custom_theme_override)
 
-        disable_endpoint_on_failure = dict_copy.pop("disableEndpointOnFailure", UNSET)
+        disable_endpoint_on_failure = d.pop("disableEndpointOnFailure", UNSET)
 
-        display_name = dict_copy.pop("displayName", UNSET)
+        display_name = d.pop("displayName", UNSET)
 
-        enable_channels = dict_copy.pop("enableChannels", UNSET)
+        enable_channels = d.pop("enableChannels", UNSET)
 
-        enable_integration_management = dict_copy.pop("enableIntegrationManagement", UNSET)
+        enable_integration_management = d.pop("enableIntegrationManagement", UNSET)
 
-        enable_transformations = dict_copy.pop("enableTransformations", UNSET)
+        enable_transformations = d.pop("enableTransformations", UNSET)
 
-        enforce_https = dict_copy.pop("enforceHttps", UNSET)
+        enforce_https = d.pop("enforceHttps", UNSET)
 
-        event_catalog_published = dict_copy.pop("eventCatalogPublished", UNSET)
+        event_catalog_published = d.pop("eventCatalogPublished", UNSET)
 
-        read_only = dict_copy.pop("readOnly", UNSET)
+        read_only = d.pop("readOnly", UNSET)
 
-        settings_out = cls(
+        settings_in = cls(
             color_palette_dark=color_palette_dark,
             color_palette_light=color_palette_light,
             custom_base_font_size=custom_base_font_size,
             custom_color=custom_color,
             custom_font_family=custom_font_family,
             custom_logo_url=custom_logo_url,
             custom_theme_override=custom_theme_override,
@@ -174,16 +177,16 @@
             enable_integration_management=enable_integration_management,
             enable_transformations=enable_transformations,
             enforce_https=enforce_https,
             event_catalog_published=event_catalog_published,
             read_only=read_only,
         )
 
-        settings_out.additional_properties = dict_copy
-        return settings_out
+        settings_in.additional_properties = d
+        return settings_in
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `svix-1.4.12/svix/internal/openapi_client/types.py` & `svix-1.5.0/svix/internal/openapi_client/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,11 +34,11 @@
 @attr.s(auto_attribs=True)
 class Response(Generic[T]):
     """A response from an endpoint"""
 
     status_code: HTTPStatus
     content: bytes
     headers: MutableMapping[str, str]
-    parsed: Optional[T]
+    parsed: T
 
 
 __all__ = ["File", "Response", "FileJsonType"]
```

### Comparing `svix-1.4.12/svix/webhooks.py` & `svix-1.5.0/svix/webhooks.py`

 * *Files identical despite different names*

### Comparing `svix-1.4.12/svix.egg-info/SOURCES.txt` & `svix-1.5.0/svix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `svix-1.4.12/tests/test_webhooks.py` & `svix-1.5.0/tests/test_webhooks.py`

 * *Files identical despite different names*

