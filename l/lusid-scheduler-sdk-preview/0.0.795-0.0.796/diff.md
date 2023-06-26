# Comparing `tmp/lusid-scheduler-sdk-preview-0.0.795.tar.gz` & `tmp/lusid-scheduler-sdk-preview-0.0.796.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-scheduler-sdk-preview-0.0.795.tar", last modified: Sat Jun 17 08:42:37 2023, max compression
+gzip compressed data, was "dist/lusid-scheduler-sdk-preview-0.0.796.tar", last modified: Mon Jun 26 08:57:46 2023, max compression
```

## Comparing `lusid-scheduler-sdk-preview-0.0.795.tar` & `lusid-scheduler-sdk-preview-0.0.796.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 08:42:37.000000 lusid-scheduler-sdk-preview-0.0.795/
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      367 2023-06-17 08:42:37.000000 lusid-scheduler-sdk-preview-0.0.795/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8886 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 08:42:37.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/
--rw-r--r--   0 root         (0) root         (0)     4369 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 08:42:37.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/api/
--rw-r--r--   0 root         (0) root         (0)      328 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6831 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    52333 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/api/images_api.py
--rw-r--r--   0 root         (0) root         (0)    74271 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/api/jobs_api.py
--rw-r--r--   0 root         (0) root         (0)    55693 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/api/schedules_api.py
--rw-r--r--   0 root         (0) root         (0)    27412 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16623 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5095 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 08:42:37.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/
--rw-r--r--   0 root         (0) root         (0)     3216 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7220 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     8983 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7224 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)    11992 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/argument_definition.py
--rw-r--r--   0 root         (0) root         (0)    24696 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/create_job_request.py
--rw-r--r--   0 root         (0) root         (0)    16506 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/create_schedule_request.py
--rw-r--r--   0 root         (0) root         (0)     8005 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9494 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     8718 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/image.py
--rw-r--r--   0 root         (0) root         (0)    10613 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/image_summary.py
--rw-r--r--   0 root         (0) root         (0)    18900 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/job_definition.py
--rw-r--r--   0 root         (0) root         (0)    18845 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/job_history.py
--rw-r--r--   0 root         (0) root         (0)    20106 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/job_run_result.py
--rw-r--r--   0 root         (0) root         (0)     6418 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9532 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10697 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     5844 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/notification.py
--rw-r--r--   0 root         (0) root         (0)    10271 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/repository.py
--rw-r--r--   0 root         (0) root         (0)     6408 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/required_resources.py
--rw-r--r--   0 root         (0) root         (0)     6592 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7743 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7407 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/resource_list_of_image_summary.py
--rw-r--r--   0 root         (0) root         (0)     7435 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/resource_list_of_job_definition.py
--rw-r--r--   0 root         (0) root         (0)     7351 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/resource_list_of_job_history.py
--rw-r--r--   0 root         (0) root         (0)     7351 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/resource_list_of_repository.py
--rw-r--r--   0 root         (0) root         (0)     7575 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/resource_list_of_schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     9669 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/scan_report.py
--rw-r--r--   0 root         (0) root         (0)     9993 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/scan_summary.py
--rw-r--r--   0 root         (0) root         (0)    12564 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     5226 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/start_job_request.py
--rw-r--r--   0 root         (0) root         (0)     6547 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/start_job_response.py
--rw-r--r--   0 root         (0) root         (0)     7564 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/start_schedule_response.py
--rw-r--r--   0 root         (0) root         (0)     7315 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/tag.py
--rw-r--r--   0 root         (0) root         (0)     6024 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/time_trigger.py
--rw-r--r--   0 root         (0) root         (0)     4068 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/trigger.py
--rw-r--r--   0 root         (0) root         (0)    22675 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/update_job_request.py
--rw-r--r--   0 root         (0) root         (0)    15546 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/update_schedule_request.py
--rw-r--r--   0 root         (0) root         (0)    14153 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/upload_image_instructions.py
--rw-r--r--   0 root         (0) root         (0)     5321 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/upload_image_request.py
--rw-r--r--   0 root         (0) root         (0)     9287 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/vulnerability.py
--rw-r--r--   0 root         (0) root         (0)    13553 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 08:42:37.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/utilities/
--rw-r--r--   0 root         (0) root         (0)       62 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1035 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 08:42:37.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      367 2023-06-17 08:42:37.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2624 2023-06-17 08:42:37.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 08:42:37.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-06-17 08:42:37.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-17 08:42:37.000000 lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-17 08:42:37.000000 lusid-scheduler-sdk-preview-0.0.795/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2275 2023-06-17 08:42:26.000000 lusid-scheduler-sdk-preview-0.0.795/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:57:46.000000 lusid-scheduler-sdk-preview-0.0.796/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      367 2023-06-26 08:57:46.000000 lusid-scheduler-sdk-preview-0.0.796/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8886 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:57:46.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/
+-rw-r--r--   0 root         (0) root         (0)     4369 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:57:46.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/api/
+-rw-r--r--   0 root         (0) root         (0)      328 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6831 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    52333 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/api/images_api.py
+-rw-r--r--   0 root         (0) root         (0)    74271 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/api/jobs_api.py
+-rw-r--r--   0 root         (0) root         (0)    55693 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/api/schedules_api.py
+-rw-r--r--   0 root         (0) root         (0)    27412 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16623 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5095 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:57:46.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7220 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     8983 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7224 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)    11992 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/argument_definition.py
+-rw-r--r--   0 root         (0) root         (0)    24696 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/create_job_request.py
+-rw-r--r--   0 root         (0) root         (0)    18889 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/create_schedule_request.py
+-rw-r--r--   0 root         (0) root         (0)     8005 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9494 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8718 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/image.py
+-rw-r--r--   0 root         (0) root         (0)    10613 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/image_summary.py
+-rw-r--r--   0 root         (0) root         (0)    18900 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    18845 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/job_history.py
+-rw-r--r--   0 root         (0) root         (0)    20106 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/job_run_result.py
+-rw-r--r--   0 root         (0) root         (0)     6418 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9532 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10697 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     5844 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)    10271 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/repository.py
+-rw-r--r--   0 root         (0) root         (0)     6408 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/required_resources.py
+-rw-r--r--   0 root         (0) root         (0)     6592 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7743 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7407 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/resource_list_of_image_summary.py
+-rw-r--r--   0 root         (0) root         (0)     7435 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/resource_list_of_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/resource_list_of_job_history.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/resource_list_of_repository.py
+-rw-r--r--   0 root         (0) root         (0)     7575 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/resource_list_of_schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9669 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/scan_report.py
+-rw-r--r--   0 root         (0) root         (0)     9993 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/scan_summary.py
+-rw-r--r--   0 root         (0) root         (0)    13684 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5226 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/start_job_request.py
+-rw-r--r--   0 root         (0) root         (0)     6547 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/start_job_response.py
+-rw-r--r--   0 root         (0) root         (0)     7564 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/start_schedule_response.py
+-rw-r--r--   0 root         (0) root         (0)     7315 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/tag.py
+-rw-r--r--   0 root         (0) root         (0)     6024 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/time_trigger.py
+-rw-r--r--   0 root         (0) root         (0)     4068 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/trigger.py
+-rw-r--r--   0 root         (0) root         (0)    22675 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/update_job_request.py
+-rw-r--r--   0 root         (0) root         (0)    17929 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/update_schedule_request.py
+-rw-r--r--   0 root         (0) root         (0)    14153 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/upload_image_instructions.py
+-rw-r--r--   0 root         (0) root         (0)     5321 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/upload_image_request.py
+-rw-r--r--   0 root         (0) root         (0)     9287 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/vulnerability.py
+-rw-r--r--   0 root         (0) root         (0)    13553 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:57:46.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/utilities/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 08:57:46.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      367 2023-06-26 08:57:46.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-06-26 08:57:46.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 08:57:46.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-06-26 08:57:46.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-26 08:57:46.000000 lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-26 08:57:46.000000 lusid-scheduler-sdk-preview-0.0.796/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2275 2023-06-26 08:55:20.000000 lusid-scheduler-sdk-preview-0.0.796/setup.py
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/README.md` & `lusid-scheduler-sdk-preview-0.0.796/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-scheduler-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.795
-- Package version: 0.0.795
+- API version: 0.0.796
+- Package version: 0.0.796
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/__init__.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.0.795"
+__version__ = "0.0.796"
 
 # import apis into sdk package
 from lusid_scheduler.api.application_metadata_api import ApplicationMetadataApi
 from lusid_scheduler.api.images_api import ImagesApi
 from lusid_scheduler.api.jobs_api import JobsApi
 from lusid_scheduler.api.schedules_api import SchedulesApi
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/api/application_metadata_api.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/api/application_metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/api/images_api.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/api/images_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -163,15 +163,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "str",
             400: "LusidValidationProblemDetails",
@@ -306,15 +306,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "file",
             400: "LusidValidationProblemDetails",
@@ -456,15 +456,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Image",
             400: "LusidValidationProblemDetails",
@@ -656,15 +656,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfImageSummary",
             400: "LusidValidationProblemDetails",
@@ -845,15 +845,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfRepository",
             400: "LusidValidationProblemDetails",
@@ -992,15 +992,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "UploadImageInstructions",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/api/jobs_api.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/api/jobs_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -162,15 +162,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "JobDefinition",
             400: "LusidValidationProblemDetails",
@@ -315,15 +315,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfScheduleDefinition",
             400: "LusidValidationProblemDetails",
@@ -502,15 +502,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfJobHistory",
             400: "LusidValidationProblemDetails",
@@ -652,15 +652,15 @@
             ['text/plain', 'application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "str",
             400: "LusidValidationProblemDetails",
@@ -802,15 +802,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "JobRunResult",
             400: "LusidValidationProblemDetails",
@@ -955,15 +955,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfScheduleDefinition",
             400: "LusidValidationProblemDetails",
@@ -1144,15 +1144,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfJobDefinition",
             400: "LusidValidationProblemDetails",
@@ -1311,15 +1311,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             202: "StartJobResponse",
             400: "LusidValidationProblemDetails",
@@ -1478,15 +1478,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "JobDefinition",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/api/schedules_api.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/api/schedules_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -158,15 +158,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ScheduleDefinition",
             400: "LusidValidationProblemDetails",
@@ -311,15 +311,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -472,15 +472,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ScheduleDefinition",
             400: "LusidValidationProblemDetails",
@@ -625,15 +625,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ScheduleDefinition",
             400: "LusidValidationProblemDetails",
@@ -814,15 +814,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfScheduleDefinition",
             400: "LusidValidationProblemDetails",
@@ -967,15 +967,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             202: "StartScheduleResponse",
             400: "LusidValidationProblemDetails",
@@ -1134,15 +1134,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.795'
+        header_params['X-LUSID-SDK-Version'] = '0.0.796'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ScheduleDefinition",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/api_client.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.0.795/python'
+        self.user_agent = 'OpenAPI-Generator/0.0.796/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/configuration.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.0.795\n"\
-               "SDK Package Version: 0.0.795".\
+               "Version of the API: 0.0.796\n"\
+               "SDK Package Version: 0.0.796".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/exceptions.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/__init__.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/access_controlled_action.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/access_controlled_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/access_controlled_resource.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/action_id.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/action_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/argument_definition.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/argument_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/create_job_request.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/create_job_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/create_schedule_request.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/update_schedule_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_scheduler.configuration import Configuration
 
 
-class CreateScheduleRequest(object):
+class UpdateScheduleRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,170 +35,147 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'schedule_id': 'ResourceId',
         'job_id': 'ResourceId',
         'name': 'str',
         'description': 'str',
         'author': 'str',
         'owner': 'str',
         'arguments': 'dict(str, str)',
         'trigger': 'Trigger',
         'notifications': 'list[Notification]',
-        'enabled': 'bool'
+        'enabled': 'bool',
+        'use_as_auth': 'str'
     }
 
     attribute_map = {
-        'schedule_id': 'scheduleId',
         'job_id': 'jobId',
         'name': 'name',
         'description': 'description',
         'author': 'author',
         'owner': 'owner',
         'arguments': 'arguments',
         'trigger': 'trigger',
         'notifications': 'notifications',
-        'enabled': 'enabled'
+        'enabled': 'enabled',
+        'use_as_auth': 'useAsAuth'
     }
 
     required_map = {
-        'schedule_id': 'required',
         'job_id': 'required',
         'name': 'required',
         'description': 'required',
         'author': 'optional',
         'owner': 'optional',
         'arguments': 'optional',
         'trigger': 'optional',
         'notifications': 'required',
-        'enabled': 'optional'
+        'enabled': 'optional',
+        'use_as_auth': 'optional'
     }
 
-    def __init__(self, schedule_id=None, job_id=None, name=None, description=None, author=None, owner=None, arguments=None, trigger=None, notifications=None, enabled=None, local_vars_configuration=None):  # noqa: E501
-        """CreateScheduleRequest - a model defined in OpenAPI"
+    def __init__(self, job_id=None, name=None, description=None, author=None, owner=None, arguments=None, trigger=None, notifications=None, enabled=None, use_as_auth=None, local_vars_configuration=None):  # noqa: E501
+        """UpdateScheduleRequest - a model defined in OpenAPI"
         
-        :param schedule_id:  (required)
-        :type schedule_id: lusid_scheduler.ResourceId
         :param job_id:  (required)
         :type job_id: lusid_scheduler.ResourceId
-        :param name:  A display name for this Schedule (required)
+        :param name:  The updated name of the schedule (required)
         :type name: str
-        :param description:  A description of the Schedule (required)
+        :param description:  The updated description of the schedule (required)
         :type description: str
-        :param author:  Name of the author of this schedule
+        :param author:  The updated author of the schedule
         :type author: str
-        :param owner:  Name of owner of this schedule
+        :param owner:  The update owner of the schedule
         :type owner: str
-        :param arguments:  All arguments specified by this Schedule that will be passed in to the Job
+        :param arguments:  Updated arguments to be passed to the job  Note: The new arguments will completely replace old arguments
         :type arguments: dict(str, str)
         :param trigger: 
         :type trigger: lusid_scheduler.Trigger
-        :param notifications:  Notifications for this Schedule (required)
+        :param notifications:  Updated notifications for this schedule (required)
         :type notifications: list[lusid_scheduler.Notification]
         :param enabled:  Specify whether schedule is enabled or not  Defaults to true
         :type enabled: bool
+        :param use_as_auth:  Id of user associated with schedule. All calls to FINBOURNE services  as part of execution of this schedule will be authenticated as this   user. Can be null, in which case we'll default to that of the user   making this request
+        :type use_as_auth: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._schedule_id = None
         self._job_id = None
         self._name = None
         self._description = None
         self._author = None
         self._owner = None
         self._arguments = None
         self._trigger = None
         self._notifications = None
         self._enabled = None
+        self._use_as_auth = None
         self.discriminator = None
 
-        self.schedule_id = schedule_id
         self.job_id = job_id
         self.name = name
         self.description = description
         self.author = author
         self.owner = owner
         self.arguments = arguments
         if trigger is not None:
             self.trigger = trigger
         self.notifications = notifications
         if enabled is not None:
             self.enabled = enabled
-
-    @property
-    def schedule_id(self):
-        """Gets the schedule_id of this CreateScheduleRequest.  # noqa: E501
-
-
-        :return: The schedule_id of this CreateScheduleRequest.  # noqa: E501
-        :rtype: lusid_scheduler.ResourceId
-        """
-        return self._schedule_id
-
-    @schedule_id.setter
-    def schedule_id(self, schedule_id):
-        """Sets the schedule_id of this CreateScheduleRequest.
-
-
-        :param schedule_id: The schedule_id of this CreateScheduleRequest.  # noqa: E501
-        :type schedule_id: lusid_scheduler.ResourceId
-        """
-        if self.local_vars_configuration.client_side_validation and schedule_id is None:  # noqa: E501
-            raise ValueError("Invalid value for `schedule_id`, must not be `None`")  # noqa: E501
-
-        self._schedule_id = schedule_id
+        self.use_as_auth = use_as_auth
 
     @property
     def job_id(self):
-        """Gets the job_id of this CreateScheduleRequest.  # noqa: E501
+        """Gets the job_id of this UpdateScheduleRequest.  # noqa: E501
 
 
-        :return: The job_id of this CreateScheduleRequest.  # noqa: E501
+        :return: The job_id of this UpdateScheduleRequest.  # noqa: E501
         :rtype: lusid_scheduler.ResourceId
         """
         return self._job_id
 
     @job_id.setter
     def job_id(self, job_id):
-        """Sets the job_id of this CreateScheduleRequest.
+        """Sets the job_id of this UpdateScheduleRequest.
 
 
-        :param job_id: The job_id of this CreateScheduleRequest.  # noqa: E501
+        :param job_id: The job_id of this UpdateScheduleRequest.  # noqa: E501
         :type job_id: lusid_scheduler.ResourceId
         """
         if self.local_vars_configuration.client_side_validation and job_id is None:  # noqa: E501
             raise ValueError("Invalid value for `job_id`, must not be `None`")  # noqa: E501
 
         self._job_id = job_id
 
     @property
     def name(self):
-        """Gets the name of this CreateScheduleRequest.  # noqa: E501
+        """Gets the name of this UpdateScheduleRequest.  # noqa: E501
 
-        A display name for this Schedule  # noqa: E501
+        The updated name of the schedule  # noqa: E501
 
-        :return: The name of this CreateScheduleRequest.  # noqa: E501
+        :return: The name of this UpdateScheduleRequest.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this CreateScheduleRequest.
+        """Sets the name of this UpdateScheduleRequest.
 
-        A display name for this Schedule  # noqa: E501
+        The updated name of the schedule  # noqa: E501
 
-        :param name: The name of this CreateScheduleRequest.  # noqa: E501
+        :param name: The name of this UpdateScheduleRequest.  # noqa: E501
         :type name: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 name is not None and len(name) > 512):
             raise ValueError("Invalid value for `name`, length must be less than or equal to `512`")  # noqa: E501
@@ -209,30 +186,30 @@
                 name is not None and not re.search(r'^[\s\S]*$', name)):  # noqa: E501
             raise ValueError(r"Invalid value for `name`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
         self._name = name
 
     @property
     def description(self):
-        """Gets the description of this CreateScheduleRequest.  # noqa: E501
+        """Gets the description of this UpdateScheduleRequest.  # noqa: E501
 
-        A description of the Schedule  # noqa: E501
+        The updated description of the schedule  # noqa: E501
 
-        :return: The description of this CreateScheduleRequest.  # noqa: E501
+        :return: The description of this UpdateScheduleRequest.  # noqa: E501
         :rtype: str
         """
         return self._description
 
     @description.setter
     def description(self, description):
-        """Sets the description of this CreateScheduleRequest.
+        """Sets the description of this UpdateScheduleRequest.
 
-        A description of the Schedule  # noqa: E501
+        The updated description of the schedule  # noqa: E501
 
-        :param description: The description of this CreateScheduleRequest.  # noqa: E501
+        :param description: The description of this UpdateScheduleRequest.  # noqa: E501
         :type description: str
         """
         if self.local_vars_configuration.client_side_validation and description is None:  # noqa: E501
             raise ValueError("Invalid value for `description`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 description is not None and len(description) > 512):
             raise ValueError("Invalid value for `description`, length must be less than or equal to `512`")  # noqa: E501
@@ -243,30 +220,30 @@
                 description is not None and not re.search(r'^[\s\S]*$', description)):  # noqa: E501
             raise ValueError(r"Invalid value for `description`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
         self._description = description
 
     @property
     def author(self):
-        """Gets the author of this CreateScheduleRequest.  # noqa: E501
+        """Gets the author of this UpdateScheduleRequest.  # noqa: E501
 
-        Name of the author of this schedule  # noqa: E501
+        The updated author of the schedule  # noqa: E501
 
-        :return: The author of this CreateScheduleRequest.  # noqa: E501
+        :return: The author of this UpdateScheduleRequest.  # noqa: E501
         :rtype: str
         """
         return self._author
 
     @author.setter
     def author(self, author):
-        """Sets the author of this CreateScheduleRequest.
+        """Sets the author of this UpdateScheduleRequest.
 
-        Name of the author of this schedule  # noqa: E501
+        The updated author of the schedule  # noqa: E501
 
-        :param author: The author of this CreateScheduleRequest.  # noqa: E501
+        :param author: The author of this UpdateScheduleRequest.  # noqa: E501
         :type author: str
         """
         if (self.local_vars_configuration.client_side_validation and
                 author is not None and len(author) > 512):
             raise ValueError("Invalid value for `author`, length must be less than or equal to `512`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 author is not None and len(author) < 0):
@@ -275,30 +252,30 @@
                 author is not None and not re.search(r'^[\s\S]*$', author)):  # noqa: E501
             raise ValueError(r"Invalid value for `author`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
         self._author = author
 
     @property
     def owner(self):
-        """Gets the owner of this CreateScheduleRequest.  # noqa: E501
+        """Gets the owner of this UpdateScheduleRequest.  # noqa: E501
 
-        Name of owner of this schedule  # noqa: E501
+        The update owner of the schedule  # noqa: E501
 
-        :return: The owner of this CreateScheduleRequest.  # noqa: E501
+        :return: The owner of this UpdateScheduleRequest.  # noqa: E501
         :rtype: str
         """
         return self._owner
 
     @owner.setter
     def owner(self, owner):
-        """Sets the owner of this CreateScheduleRequest.
+        """Sets the owner of this UpdateScheduleRequest.
 
-        Name of owner of this schedule  # noqa: E501
+        The update owner of the schedule  # noqa: E501
 
-        :param owner: The owner of this CreateScheduleRequest.  # noqa: E501
+        :param owner: The owner of this UpdateScheduleRequest.  # noqa: E501
         :type owner: str
         """
         if (self.local_vars_configuration.client_side_validation and
                 owner is not None and len(owner) > 512):
             raise ValueError("Invalid value for `owner`, length must be less than or equal to `512`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 owner is not None and len(owner) < 0):
@@ -307,104 +284,136 @@
                 owner is not None and not re.search(r'^[\s\S]*$', owner)):  # noqa: E501
             raise ValueError(r"Invalid value for `owner`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
         self._owner = owner
 
     @property
     def arguments(self):
-        """Gets the arguments of this CreateScheduleRequest.  # noqa: E501
+        """Gets the arguments of this UpdateScheduleRequest.  # noqa: E501
 
-        All arguments specified by this Schedule that will be passed in to the Job  # noqa: E501
+        Updated arguments to be passed to the job  Note: The new arguments will completely replace old arguments  # noqa: E501
 
-        :return: The arguments of this CreateScheduleRequest.  # noqa: E501
+        :return: The arguments of this UpdateScheduleRequest.  # noqa: E501
         :rtype: dict(str, str)
         """
         return self._arguments
 
     @arguments.setter
     def arguments(self, arguments):
-        """Sets the arguments of this CreateScheduleRequest.
+        """Sets the arguments of this UpdateScheduleRequest.
 
-        All arguments specified by this Schedule that will be passed in to the Job  # noqa: E501
+        Updated arguments to be passed to the job  Note: The new arguments will completely replace old arguments  # noqa: E501
 
-        :param arguments: The arguments of this CreateScheduleRequest.  # noqa: E501
+        :param arguments: The arguments of this UpdateScheduleRequest.  # noqa: E501
         :type arguments: dict(str, str)
         """
 
         self._arguments = arguments
 
     @property
     def trigger(self):
-        """Gets the trigger of this CreateScheduleRequest.  # noqa: E501
+        """Gets the trigger of this UpdateScheduleRequest.  # noqa: E501
 
 
-        :return: The trigger of this CreateScheduleRequest.  # noqa: E501
+        :return: The trigger of this UpdateScheduleRequest.  # noqa: E501
         :rtype: lusid_scheduler.Trigger
         """
         return self._trigger
 
     @trigger.setter
     def trigger(self, trigger):
-        """Sets the trigger of this CreateScheduleRequest.
+        """Sets the trigger of this UpdateScheduleRequest.
 
 
-        :param trigger: The trigger of this CreateScheduleRequest.  # noqa: E501
+        :param trigger: The trigger of this UpdateScheduleRequest.  # noqa: E501
         :type trigger: lusid_scheduler.Trigger
         """
 
         self._trigger = trigger
 
     @property
     def notifications(self):
-        """Gets the notifications of this CreateScheduleRequest.  # noqa: E501
+        """Gets the notifications of this UpdateScheduleRequest.  # noqa: E501
 
-        Notifications for this Schedule  # noqa: E501
+        Updated notifications for this schedule  # noqa: E501
 
-        :return: The notifications of this CreateScheduleRequest.  # noqa: E501
+        :return: The notifications of this UpdateScheduleRequest.  # noqa: E501
         :rtype: list[lusid_scheduler.Notification]
         """
         return self._notifications
 
     @notifications.setter
     def notifications(self, notifications):
-        """Sets the notifications of this CreateScheduleRequest.
+        """Sets the notifications of this UpdateScheduleRequest.
 
-        Notifications for this Schedule  # noqa: E501
+        Updated notifications for this schedule  # noqa: E501
 
-        :param notifications: The notifications of this CreateScheduleRequest.  # noqa: E501
+        :param notifications: The notifications of this UpdateScheduleRequest.  # noqa: E501
         :type notifications: list[lusid_scheduler.Notification]
         """
         if self.local_vars_configuration.client_side_validation and notifications is None:  # noqa: E501
             raise ValueError("Invalid value for `notifications`, must not be `None`")  # noqa: E501
 
         self._notifications = notifications
 
     @property
     def enabled(self):
-        """Gets the enabled of this CreateScheduleRequest.  # noqa: E501
+        """Gets the enabled of this UpdateScheduleRequest.  # noqa: E501
 
         Specify whether schedule is enabled or not  Defaults to true  # noqa: E501
 
-        :return: The enabled of this CreateScheduleRequest.  # noqa: E501
+        :return: The enabled of this UpdateScheduleRequest.  # noqa: E501
         :rtype: bool
         """
         return self._enabled
 
     @enabled.setter
     def enabled(self, enabled):
-        """Sets the enabled of this CreateScheduleRequest.
+        """Sets the enabled of this UpdateScheduleRequest.
 
         Specify whether schedule is enabled or not  Defaults to true  # noqa: E501
 
-        :param enabled: The enabled of this CreateScheduleRequest.  # noqa: E501
+        :param enabled: The enabled of this UpdateScheduleRequest.  # noqa: E501
         :type enabled: bool
         """
 
         self._enabled = enabled
 
+    @property
+    def use_as_auth(self):
+        """Gets the use_as_auth of this UpdateScheduleRequest.  # noqa: E501
+
+        Id of user associated with schedule. All calls to FINBOURNE services  as part of execution of this schedule will be authenticated as this   user. Can be null, in which case we'll default to that of the user   making this request  # noqa: E501
+
+        :return: The use_as_auth of this UpdateScheduleRequest.  # noqa: E501
+        :rtype: str
+        """
+        return self._use_as_auth
+
+    @use_as_auth.setter
+    def use_as_auth(self, use_as_auth):
+        """Sets the use_as_auth of this UpdateScheduleRequest.
+
+        Id of user associated with schedule. All calls to FINBOURNE services  as part of execution of this schedule will be authenticated as this   user. Can be null, in which case we'll default to that of the user   making this request  # noqa: E501
+
+        :param use_as_auth: The use_as_auth of this UpdateScheduleRequest.  # noqa: E501
+        :type use_as_auth: str
+        """
+        if (self.local_vars_configuration.client_side_validation and
+                use_as_auth is not None and len(use_as_auth) > 64):
+            raise ValueError("Invalid value for `use_as_auth`, length must be less than or equal to `64`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                use_as_auth is not None and len(use_as_auth) < 1):
+            raise ValueError("Invalid value for `use_as_auth`, length must be greater than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                use_as_auth is not None and not re.search(r'^[a-zA-Z0-9\-_]+$', use_as_auth)):  # noqa: E501
+            raise ValueError(r"Invalid value for `use_as_auth`, must be a follow pattern or equal to `/^[a-zA-Z0-9\-_]+$/`")  # noqa: E501
+
+        self._use_as_auth = use_as_auth
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
@@ -439,18 +448,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, CreateScheduleRequest):
+        if not isinstance(other, UpdateScheduleRequest):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, CreateScheduleRequest):
+        if not isinstance(other, UpdateScheduleRequest):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/id_selector_definition.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/id_selector_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/identifier_part_schema.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/identifier_part_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/image.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/image_summary.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/image_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/job_definition.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/job_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/job_history.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/job_history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/job_run_result.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/job_run_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/link.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/lusid_problem_details.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/lusid_validation_problem_details.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/notification.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/repository.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/required_resources.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/required_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/resource_id.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/resource_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/resource_list_of_access_controlled_resource.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/resource_list_of_access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/resource_list_of_image_summary.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/resource_list_of_image_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/resource_list_of_job_definition.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/resource_list_of_job_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/resource_list_of_job_history.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/resource_list_of_job_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/resource_list_of_repository.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/resource_list_of_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/resource_list_of_schedule_definition.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/resource_list_of_schedule_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/scan_report.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/scan_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/scan_summary.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/scan_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/schedule_definition.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/schedule_definition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -41,61 +41,66 @@
     openapi_types = {
         'schedule_identifier': 'ResourceId',
         'job_id': 'ResourceId',
         'name': 'str',
         'description': 'str',
         'author': 'str',
         'owner': 'str',
+        'use_as_auth': 'str',
         'arguments': 'dict(str, str)',
         'trigger': 'Trigger',
         'notifications': 'list[Notification]',
         'enabled': 'bool'
     }
 
     attribute_map = {
         'schedule_identifier': 'scheduleIdentifier',
         'job_id': 'jobId',
         'name': 'name',
         'description': 'description',
         'author': 'author',
         'owner': 'owner',
+        'use_as_auth': 'useAsAuth',
         'arguments': 'arguments',
         'trigger': 'trigger',
         'notifications': 'notifications',
         'enabled': 'enabled'
     }
 
     required_map = {
         'schedule_identifier': 'required',
         'job_id': 'optional',
         'name': 'optional',
         'description': 'optional',
         'author': 'optional',
         'owner': 'optional',
+        'use_as_auth': 'optional',
         'arguments': 'optional',
         'trigger': 'optional',
         'notifications': 'optional',
         'enabled': 'optional'
     }
 
-    def __init__(self, schedule_identifier=None, job_id=None, name=None, description=None, author=None, owner=None, arguments=None, trigger=None, notifications=None, enabled=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, schedule_identifier=None, job_id=None, name=None, description=None, author=None, owner=None, use_as_auth=None, arguments=None, trigger=None, notifications=None, enabled=None, local_vars_configuration=None):  # noqa: E501
         """ScheduleDefinition - a model defined in OpenAPI"
         
         :param schedule_identifier:  (required)
         :type schedule_identifier: lusid_scheduler.ResourceId
         :param job_id: 
         :type job_id: lusid_scheduler.ResourceId
         :param name:  A display name for this Schedule
         :type name: str
         :param description:  A description of the Schedule
         :type description: str
         :param author:  Name of the author of this schedule
         :type author: str
         :param owner:  Name of owner of this schedule
         :type owner: str
+        :param use_as_auth:  User to runs schedule when automatically run and authenticates   requests in the schedule
+        :type use_as_auth: str
         :param arguments:  All arguments specified by this Schedule that will be passed in to the Job
         :type arguments: dict(str, str)
         :param trigger: 
         :type trigger: lusid_scheduler.Trigger
         :param notifications:  Notifications for this Schedule
         :type notifications: list[lusid_scheduler.Notification]
         :param enabled:  The status of this schedule
@@ -108,27 +113,29 @@
 
         self._schedule_identifier = None
         self._job_id = None
         self._name = None
         self._description = None
         self._author = None
         self._owner = None
+        self._use_as_auth = None
         self._arguments = None
         self._trigger = None
         self._notifications = None
         self._enabled = None
         self.discriminator = None
 
         self.schedule_identifier = schedule_identifier
         if job_id is not None:
             self.job_id = job_id
         self.name = name
         self.description = description
         self.author = author
         self.owner = owner
+        self.use_as_auth = use_as_auth
         self.arguments = arguments
         if trigger is not None:
             self.trigger = trigger
         self.notifications = notifications
         if enabled is not None:
             self.enabled = enabled
 
@@ -265,14 +272,37 @@
         :param owner: The owner of this ScheduleDefinition.  # noqa: E501
         :type owner: str
         """
 
         self._owner = owner
 
     @property
+    def use_as_auth(self):
+        """Gets the use_as_auth of this ScheduleDefinition.  # noqa: E501
+
+        User to runs schedule when automatically run and authenticates   requests in the schedule  # noqa: E501
+
+        :return: The use_as_auth of this ScheduleDefinition.  # noqa: E501
+        :rtype: str
+        """
+        return self._use_as_auth
+
+    @use_as_auth.setter
+    def use_as_auth(self, use_as_auth):
+        """Sets the use_as_auth of this ScheduleDefinition.
+
+        User to runs schedule when automatically run and authenticates   requests in the schedule  # noqa: E501
+
+        :param use_as_auth: The use_as_auth of this ScheduleDefinition.  # noqa: E501
+        :type use_as_auth: str
+        """
+
+        self._use_as_auth = use_as_auth
+
+    @property
     def arguments(self):
         """Gets the arguments of this ScheduleDefinition.  # noqa: E501
 
         All arguments specified by this Schedule that will be passed in to the Job  # noqa: E501
 
         :return: The arguments of this ScheduleDefinition.  # noqa: E501
         :rtype: dict(str, str)
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/start_job_request.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/start_job_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/start_job_response.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/start_job_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/start_schedule_response.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/start_schedule_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/tag.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/time_trigger.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/time_trigger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/trigger.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/trigger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/update_job_request.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/update_job_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/upload_image_instructions.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/upload_image_instructions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/upload_image_request.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/upload_image_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/models/vulnerability.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/models/vulnerability.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/rest.py` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.795
+    The version of the OpenAPI document: 0.0.796
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler/utilities/config_keys.json` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-scheduler-sdk-preview-0.0.795/lusid_scheduler_sdk_preview.egg-info/SOURCES.txt` & `lusid-scheduler-sdk-preview-0.0.796/lusid_scheduler_sdk_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lusid-scheduler-sdk-preview-0.0.795/setup.py` & `lusid-scheduler-sdk-preview-0.0.796/setup.py`

 * *Files identical despite different names*

