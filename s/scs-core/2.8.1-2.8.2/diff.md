# Comparing `tmp/scs-core-2.8.1.tar.gz` & `tmp/scs-core-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs-core-2.8.1.tar", last modified: Mon Jun 26 09:34:13 2023, max compression
+gzip compressed data, was "scs-core-2.8.2.tar", last modified: Mon Jun 26 13:24:09 2023, max compression
```

## Comparing `scs-core-2.8.1.tar` & `scs-core-2.8.2.tar`

### file list

```diff
@@ -1,419 +1,419 @@
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.050926 scs-core-2.8.1/
--rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:27.000000 scs-core-2.8.1/LICENSE
--rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:27.000000 scs-core-2.8.1/MANIFEST.in
--rw-rw-r--   0 jade      (1002) jade      (1002)     2059 2023-06-26 09:34:13.050926 scs-core-2.8.1/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)     1404 2023-06-26 09:33:48.000000 scs-core-2.8.1/README.md
--rw-rw-r--   0 jade      (1002) jade      (1002)       41 2022-08-17 09:53:27.000000 scs-core-2.8.1/README.rst
--rw-rw-r--   0 jade      (1002) jade      (1002)      124 2023-02-06 14:01:57.000000 scs-core-2.8.1/requirements.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-06-26 09:34:13.050926 scs-core-2.8.1/setup.cfg
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1996 2022-08-17 09:53:27.000000 scs-core-2.8.1/setup.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.010926 scs-core-2.8.1/src/
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.014926 scs-core-2.8.1/src/scs_core/
--rw-rw-r--   0 jade      (1002) jade      (1002)      183 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.014926 scs-core-2.8.1/src/scs_core/aqcsv/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.018926 scs-core-2.8.1/src/scs_core/aqcsv/conf/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/conf/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2617 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/conf/airnow_site_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1034 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/conf/airnow_uploader_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.018926 scs-core-2.8.1/src/scs_core/aqcsv/connector/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/connector/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10203 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/aqcsv/connector/airnow_mapping_task.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6655 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/connector/datum_mapping.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5042 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/connector/source_mapping.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.018926 scs-core-2.8.1/src/scs_core/aqcsv/data/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/data/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3750 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/data/aqcsv_datetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    13723 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/data/aqcsv_record.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3033 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/data/aqcsv_site.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.018926 scs-core-2.8.1/src/scs_core/aqcsv/specification/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2824 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/agency.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2728 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/country.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1163 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/country_iso.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1175 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/country_numeric.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     9800 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/method.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3765 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/mpc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3453 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/parameter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2855 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/qc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3732 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/qualifier.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2879 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/unit.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.018926 scs-core-2.8.1/src/scs_core/aws/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.018926 scs-core-2.8.1/src/scs_core/aws/client/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/client/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3585 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/client/access_key.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2332 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/client/api_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2113 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/client/api_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1217 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/client/client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5103 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/client/client_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1281 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/client/device_control_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3294 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/client/email_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3361 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/client/monitor_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5891 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/aws/client/mqtt_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3856 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/client/rest_client.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.018926 scs-core-2.8.1/src/scs_core/aws/config/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/config/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      744 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/config/aws.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4471 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/aws/config/project.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.022926 scs-core-2.8.1/src/scs_core/aws/data/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/data/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    16736 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/data/alert.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     9320 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/data/byline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1792 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/data/byline_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4640 2023-04-17 09:22:53.000000 scs-core-2.8.1/src/scs_core/aws/data/dataset.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3550 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/data/deployment.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3337 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/data/device_monitor_email_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    12653 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/data/device_monitor_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3313 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/data/device_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4032 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/aws/data/email_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2859 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/data/http_response.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3175 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/data/message.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1776 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/data/power_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1820 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/data/runtime_record.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1795 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/data/status_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2884 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/data/upload_interval.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1793 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/data/uptime_list.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.022926 scs-core-2.8.1/src/scs_core/aws/greengrass/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/greengrass/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1998 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/greengrass/aws_deployer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3017 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/aws/greengrass/aws_deployment_reporter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     9610 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/greengrass/aws_group.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    16440 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/aws/greengrass/aws_group_configuration.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    11557 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/greengrass/aws_identity.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      440 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/greengrass/gg_errors.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.026926 scs-core-2.8.1/src/scs_core/aws/manager/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/manager/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8285 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/alert_specification_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7269 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/alert_status_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3950 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/byline_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7269 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/configuration_check_finder.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3256 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/configuration_check_requester.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10816 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/configuration_finder.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2248 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/device_monitor_specification_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1497 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/device_monitor_status_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10307 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/dynamo_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3551 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/manager/ec2_message_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6470 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/lambda_bylines.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    15996 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/aws/manager/lambda_message_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    18045 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/aws/manager/s3_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4295 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/manager/sagemaker_model_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7802 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/manager/sagemaker_trial_manager.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.026926 scs-core-2.8.1/src/scs_core/aws/security/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/security/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1372 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/access_key_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5114 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_client_credentials.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7498 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_device.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1527 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_device_creator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3111 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_device_finder.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1911 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_device_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10555 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_login_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2181 2023-04-17 09:22:53.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_membership.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2314 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_password_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    11499 2023-04-17 09:22:53.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_user.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3227 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_user_finder.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3540 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_user_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3175 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/device_whitelist_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1947 2023-04-17 09:22:53.000000 scs-core-2.8.1/src/scs_core/aws/security/opr_membership.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    22905 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/organisation.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     9601 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/organisation_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1752 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/path_filter.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.026926 scs-core-2.8.1/src/scs_core/client/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/client/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4470 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/client/http_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6933 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/client/http_exception.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      497 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/client/http_status.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2831 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/client/network.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1415 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/client/resource_unavailable_exception.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2638 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/client/sftp_client_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.030926 scs-core-2.8.1/src/scs_core/climate/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/climate/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1407 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/climate/absolute_humidity.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1418 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/climate/icp10101_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3081 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/climate/mpl115a2_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2911 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/climate/mpl115a2_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2290 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/climate/pressure_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2188 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/climate/pressure_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3156 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/climate/sht_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1844 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/climate/sht_datum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.030926 scs-core-2.8.1/src/scs_core/comms/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/comms/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3125 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/comms/mqtt_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2395 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/comms/uds_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1552 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/comms/uds_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2350 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/comms/uds_server.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1614 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/comms/uds_writer.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.030926 scs-core-2.8.1/src/scs_core/control/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/control/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4918 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/control/command.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4896 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/control/control_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3792 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/control/control_handler.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4737 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/control/control_receipt.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.030926 scs-core-2.8.1/src/scs_core/csv/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/csv/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1979 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/csv/csv_archive.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7484 2023-04-17 09:22:53.000000 scs-core-2.8.1/src/scs_core/csv/csv_dict.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5996 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/csv/csv_log.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8594 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/csv/csv_log_cursor_queue.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8574 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/csv/csv_log_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8240 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/csv/csv_logger.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3323 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/csv/csv_logger_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5347 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/csv/csv_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4503 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/csv/csv_writer.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.034926 scs-core-2.8.1/src/scs_core/data/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4802 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/aggregate.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1947 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/data/array_dict.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2415 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/average.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2158 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/categorical_regression.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8964 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/data/checkpoint_generator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1008 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/crc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2092 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/crypt.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    19704 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/data/datetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6448 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/data/datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2634 2023-04-17 09:22:53.000000 scs-core-2.8.1/src/scs_core/data/duplicates.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3809 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/data/histogram.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1747 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/interval.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5951 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/join.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    14204 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/data/json.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3274 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/lin_regress.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5364 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/linear_regression.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1372 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/low_pass_filter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1628 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/median_filter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1892 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/min_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5682 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/data/model_delta.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8334 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/data/path_dict.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1291 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/precision.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3466 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/publication.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4181 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/data/queue_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8858 2023-04-17 09:22:53.000000 scs-core-2.8.1/src/scs_core/data/recurring_period.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1265 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/regression.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4348 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/data/rtc_datetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2249 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/data/sample_delta.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10713 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/stats.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1280 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/str.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7391 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/timedelta.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2185 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/tokens.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7456 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/data/topic_path.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.034926 scs-core-2.8.1/src/scs_core/display/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/display/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3786 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/display/display_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.034926 scs-core-2.8.1/src/scs_core/email/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/email/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2131 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/email/email_queue.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2420 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/email/email_queue_manager.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.034926 scs-core-2.8.1/src/scs_core/estate/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/estate/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6202 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/estate/baseline_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    33022 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/estate/configuration.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4521 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/estate/configuration_check.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5221 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/estate/git_pull.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3621 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/estate/git_pull_check.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6675 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/estate/mqtt_device_poller.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2450 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/estate/mqtt_peer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6563 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/estate/package_version.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.034926 scs-core-2.8.1/src/scs_core/exegesis/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/exegesis/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.034926 scs-core-2.8.1/src/scs_core/exegesis/gas/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/exegesis/gas/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      693 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/exegesis/gas/exegete_catalogue.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1345 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/exegesis/gas/exegete_collection.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.034926 scs-core-2.8.1/src/scs_core/exegesis/particulate/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/exegesis/particulate/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      701 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/exegesis/particulate/exegete_catalogue.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1353 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/exegesis/particulate/exegete_collection.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2248 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/exegesis/particulate/text.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/gas/
--rw-rw-r--   0 jade      (1002) jade      (1002)      292 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/gas/a4/
--rw-rw-r--   0 jade      (1002) jade      (1002)      410 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/a4/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3700 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/gas/a4/a4.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10274 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/gas/a4/a4_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5667 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4131 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum_v1.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3932 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum_vA.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5191 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum_vB.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5557 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum_vC.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4662 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/a4/a4_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6990 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/a4/a4_temp_comp.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/gas/afe/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/afe/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1542 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/afe/afe_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3242 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/afe/pt1000_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2445 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/afe/pt1000_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3600 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/afe_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    11555 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/gas/afe_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6742 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/afe_id.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/gas/d4/
--rw-rw-r--   0 jade      (1002) jade      (1002)      130 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/d4/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3710 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/d4/d4_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3106 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/gas/dsi_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4204 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/gas.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/gas/isi/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/isi/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1373 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/isi/isi_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7366 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/gas/minimum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/gas/ndir/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/ndir/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1777 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/ndir/ndir.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2723 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/ndir/ndir_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3350 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/ndir/ndir_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3649 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/ndir/ndir_version.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3065 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/ndir/ndir_voltages.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/gas/pid/
--rw-rw-r--   0 jade      (1002) jade      (1002)      378 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/pid/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4106 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/pid/pid.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4196 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/gas/pid/pid_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4028 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/pid/pid_calibrated_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3730 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/pid/pid_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3694 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/pid/pid_temp_comp.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/gas/scd30/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/scd30/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2538 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/scd30/scd30_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2804 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/scd30/scd30_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2866 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/scd30/scd30_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3556 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/gas/sensor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6165 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/gas/sensor_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3043 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/gas/sensor_calib.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/gps/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gps/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4077 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gps/gps_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/interface/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/interface/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2271 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/interface/interface_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/led/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/led/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      870 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/led/led.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2343 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/led/led_state.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/location/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/location/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2992 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/location/timezone.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3708 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/location/timezone_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2379 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/location/timezone_offset.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/model/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/model/catalogue/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/catalogue/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    11042 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/model/catalogue/model_compendium.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4774 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/catalogue/model_compendium_group.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5220 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/catalogue/term.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2038 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/catalogue/training_period.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/model/gas/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3349 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1354 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/gas_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1545 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/gas_inference_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2932 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/gas_model_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/model/gas/s1/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/s1/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2704 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/s1/gas_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3344 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/s1/s1_gas_inference_client.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/model/gas/vB/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/vB/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2702 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/vB/gas_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3120 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/vB/vb_gas_inference_client.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/model/gas/vE/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/vE/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3535 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/vE/gas_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4409 2022-10-03 10:46:58.000000 scs-core-2.8.1/src/scs_core/model/gas/vE/ve_gas_inference_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1218 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/vcal_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3488 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/model/model_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/model/pmx/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/pmx/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1549 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/pmx/pmx_inference_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1609 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/pmx/pmx_model_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/model/pmx/s1/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/pmx/s1/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2215 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/pmx/s1/pmx_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2051 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/monitor/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/monitor/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1558 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/monitor/monitor_error.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1557 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/monitor/monitor_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1395 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/monitor/monitor_response.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/particulate/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/particulate/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4558 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/particulate/opc_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5142 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/particulate/opc_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2610 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/particulate/opc_version.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2103 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/particulate/pmx_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6405 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/particulate/sps_datum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/position/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4062 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/position/gps_datum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/position/nmea/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1578 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/gpdatetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4215 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/gpgga.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2685 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/gpgll.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3410 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/gpgsa.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3850 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/gpgsv.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2500 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/gploc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4056 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/gprmc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1318 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/gptime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2685 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/gpvtg.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2535 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/nmea_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      782 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/nmea_sentence.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3884 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/position/position.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.046925 scs-core-2.8.1/src/scs_core/psu/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/psu/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2320 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/psu/psu.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4543 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/psu/psu_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1733 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/psu/psu_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1728 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/psu/psu_uptime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5663 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/psu/psu_version.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.046925 scs-core-2.8.1/src/scs_core/sample/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sample/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3421 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/sample/climate_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    12029 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/sample/configuration_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5262 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/sample/gases_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3724 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/sample/particulates_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2872 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/sample/pressure_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4034 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/sample/sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5876 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/sample/status_sample.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.046925 scs-core-2.8.1/src/scs_core/sampler/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sampler/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1263 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sampler/sampler.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.046925 scs-core-2.8.1/src/scs_core/sync/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sync/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2168 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sync/interval_timer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1681 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sync/line_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      606 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sync/runner.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6819 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/sync/schedule.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1811 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sync/synchronised_process.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1724 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sync/timed_runner.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.050926 scs-core-2.8.1/src/scs_core/sys/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1791 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/sys/command.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4443 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/disk_usage.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5191 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/disk_volume.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2399 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/eeprom_image.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2622 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/exception_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6991 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/sys/filesystem.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1994 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/ipv4_address.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1167 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/sys/logging.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1297 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/sys/memory.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    17409 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/sys/modem.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5733 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/network.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5974 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/sys/node.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3851 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/persistence_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2318 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/sys/platform.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      834 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/process_comms.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4919 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/sys/ps_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3284 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/serial.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2405 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/shared_secret.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2506 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/signalled_exit.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2244 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/subprocess.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5730 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/sys/system_id.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2013 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/sys/system_temp.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6610 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/sys/tail.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1409 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/timeout.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1192 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/sys/timer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1784 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/trace_entry.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5602 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/sys/uptime_datum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.014926 scs-core-2.8.1/src/scs_core.egg-info/
--rw-rw-r--   0 jade      (1002) jade      (1002)     2059 2023-06-26 09:34:12.000000 scs-core-2.8.1/src/scs_core.egg-info/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)    13337 2023-06-26 09:34:13.000000 scs-core-2.8.1/src/scs_core.egg-info/SOURCES.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-06-26 09:34:12.000000 scs-core-2.8.1/src/scs_core.egg-info/dependency_links.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)      124 2023-06-26 09:34:12.000000 scs-core-2.8.1/src/scs_core.egg-info/requires.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)        9 2023-06-26 09:34:12.000000 scs-core-2.8.1/src/scs_core.egg-info/top_level.txt
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.770826 scs-core-2.8.2/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:27.000000 scs-core-2.8.2/LICENSE
+-rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:27.000000 scs-core-2.8.2/MANIFEST.in
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2059 2023-06-26 13:24:09.770826 scs-core-2.8.2/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1404 2023-06-26 09:33:48.000000 scs-core-2.8.2/README.md
+-rw-rw-r--   0 jade      (1002) jade      (1002)       41 2022-08-17 09:53:27.000000 scs-core-2.8.2/README.rst
+-rw-rw-r--   0 jade      (1002) jade      (1002)      124 2023-02-06 14:01:57.000000 scs-core-2.8.2/requirements.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-06-26 13:24:09.770826 scs-core-2.8.2/setup.cfg
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1996 2022-08-17 09:53:27.000000 scs-core-2.8.2/setup.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.738826 scs-core-2.8.2/src/
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.742826 scs-core-2.8.2/src/scs_core/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      183 2023-06-26 13:23:15.000000 scs-core-2.8.2/src/scs_core/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.742826 scs-core-2.8.2/src/scs_core/aqcsv/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.742826 scs-core-2.8.2/src/scs_core/aqcsv/conf/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/conf/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2617 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/conf/airnow_site_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1034 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/conf/airnow_uploader_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.742826 scs-core-2.8.2/src/scs_core/aqcsv/connector/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/connector/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10203 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/aqcsv/connector/airnow_mapping_task.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6655 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/connector/datum_mapping.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5042 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/connector/source_mapping.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.742826 scs-core-2.8.2/src/scs_core/aqcsv/data/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/data/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3750 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/data/aqcsv_datetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    13723 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/data/aqcsv_record.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3033 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/data/aqcsv_site.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.742826 scs-core-2.8.2/src/scs_core/aqcsv/specification/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2824 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/agency.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2728 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/country.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1163 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/country_iso.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1175 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/country_numeric.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9800 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/method.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3765 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/mpc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3453 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/parameter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2855 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/qc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3732 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/qualifier.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2879 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aqcsv/specification/unit.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.742826 scs-core-2.8.2/src/scs_core/aws/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.746826 scs-core-2.8.2/src/scs_core/aws/client/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/client/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3585 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/client/access_key.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2332 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/client/api_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2113 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/client/api_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1217 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/client/client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5103 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/client/client_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1281 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/client/device_control_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3294 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/client/email_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3361 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/client/monitor_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5891 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/aws/client/mqtt_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3856 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/client/rest_client.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.746826 scs-core-2.8.2/src/scs_core/aws/config/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/config/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      744 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/config/aws.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4471 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/aws/config/project.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.746826 scs-core-2.8.2/src/scs_core/aws/data/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/data/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    16736 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/data/alert.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9320 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/data/byline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1792 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/data/byline_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4640 2023-04-17 09:22:53.000000 scs-core-2.8.2/src/scs_core/aws/data/dataset.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3550 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/data/deployment.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3337 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/data/device_monitor_email_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    12653 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/data/device_monitor_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3313 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/data/device_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4032 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/aws/data/email_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2859 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/data/http_response.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3175 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/data/message.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1776 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/data/power_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1820 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/data/runtime_record.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1795 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/data/status_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2884 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/data/upload_interval.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1793 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/data/uptime_list.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.746826 scs-core-2.8.2/src/scs_core/aws/greengrass/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/greengrass/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1998 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/greengrass/aws_deployer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3017 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/aws/greengrass/aws_deployment_reporter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9610 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/greengrass/aws_group.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    16440 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/aws/greengrass/aws_group_configuration.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    11557 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/greengrass/aws_identity.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      440 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/greengrass/gg_errors.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.750826 scs-core-2.8.2/src/scs_core/aws/manager/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/manager/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8285 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/alert_specification_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7269 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/alert_status_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3950 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/byline_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7269 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/configuration_check_finder.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3256 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/configuration_check_requester.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10816 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/configuration_finder.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2248 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/device_monitor_specification_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1497 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/device_monitor_status_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10307 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/dynamo_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3551 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/manager/ec2_message_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6470 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/manager/lambda_bylines.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    15996 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/aws/manager/lambda_message_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    18045 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/aws/manager/s3_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4295 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/manager/sagemaker_model_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7802 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/manager/sagemaker_trial_manager.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.750826 scs-core-2.8.2/src/scs_core/aws/security/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/aws/security/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1372 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/access_key_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5114 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_client_credentials.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7498 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_device.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1527 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_device_creator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3111 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_device_finder.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1911 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_device_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10555 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_login_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2181 2023-04-17 09:22:53.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_membership.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2314 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_password_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    11840 2023-06-26 13:23:15.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_user.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3227 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_user_finder.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3540 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/cognito_user_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3175 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/device_whitelist_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1947 2023-04-17 09:22:53.000000 scs-core-2.8.2/src/scs_core/aws/security/opr_membership.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    22905 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/organisation.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9601 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/organisation_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1752 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/aws/security/path_filter.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.750826 scs-core-2.8.2/src/scs_core/client/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/client/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4470 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/client/http_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6933 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/client/http_exception.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      497 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/client/http_status.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2831 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/client/network.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1415 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/client/resource_unavailable_exception.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2638 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/client/sftp_client_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.750826 scs-core-2.8.2/src/scs_core/climate/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/climate/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1407 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/climate/absolute_humidity.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1418 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/climate/icp10101_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3081 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/climate/mpl115a2_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2911 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/climate/mpl115a2_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2290 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/climate/pressure_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2188 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/climate/pressure_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3156 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/climate/sht_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1844 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/climate/sht_datum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.750826 scs-core-2.8.2/src/scs_core/comms/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/comms/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3125 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/comms/mqtt_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2395 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/comms/uds_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1552 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/comms/uds_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2350 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/comms/uds_server.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1614 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/comms/uds_writer.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.750826 scs-core-2.8.2/src/scs_core/control/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/control/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4918 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/control/command.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4896 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/control/control_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3792 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/control/control_handler.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4737 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/control/control_receipt.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.754826 scs-core-2.8.2/src/scs_core/csv/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/csv/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1979 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/csv/csv_archive.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7484 2023-04-17 09:22:53.000000 scs-core-2.8.2/src/scs_core/csv/csv_dict.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5996 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/csv/csv_log.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8594 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/csv/csv_log_cursor_queue.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8574 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/csv/csv_log_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8240 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/csv/csv_logger.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3323 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/csv/csv_logger_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5347 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/csv/csv_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4503 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/csv/csv_writer.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.754826 scs-core-2.8.2/src/scs_core/data/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4802 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/aggregate.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1947 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/data/array_dict.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2415 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/average.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2158 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/categorical_regression.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8964 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/data/checkpoint_generator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1008 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/crc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2092 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/crypt.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    19704 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/data/datetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6448 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/data/datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2634 2023-04-17 09:22:53.000000 scs-core-2.8.2/src/scs_core/data/duplicates.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3809 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/data/histogram.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1747 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/interval.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5951 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/join.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    14204 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/data/json.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3274 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/lin_regress.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5364 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/linear_regression.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1372 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/low_pass_filter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1628 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/median_filter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1892 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/min_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5682 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/data/model_delta.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8334 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/data/path_dict.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1291 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/precision.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3466 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/publication.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4181 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/data/queue_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8858 2023-04-17 09:22:53.000000 scs-core-2.8.2/src/scs_core/data/recurring_period.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1265 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/regression.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4348 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/data/rtc_datetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2249 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/data/sample_delta.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10713 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/stats.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1280 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/str.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7391 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/timedelta.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2185 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/data/tokens.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7456 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/data/topic_path.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.754826 scs-core-2.8.2/src/scs_core/display/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/display/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3786 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/display/display_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.754826 scs-core-2.8.2/src/scs_core/email/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/email/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2131 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/email/email_queue.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2420 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/email/email_queue_manager.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.758826 scs-core-2.8.2/src/scs_core/estate/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/estate/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6202 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/estate/baseline_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    33022 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/estate/configuration.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4521 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/estate/configuration_check.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5221 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/estate/git_pull.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3621 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/estate/git_pull_check.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6675 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/estate/mqtt_device_poller.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2450 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/estate/mqtt_peer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6563 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/estate/package_version.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.758826 scs-core-2.8.2/src/scs_core/exegesis/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/exegesis/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.758826 scs-core-2.8.2/src/scs_core/exegesis/gas/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/exegesis/gas/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      693 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/exegesis/gas/exegete_catalogue.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1345 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/exegesis/gas/exegete_collection.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.758826 scs-core-2.8.2/src/scs_core/exegesis/particulate/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/exegesis/particulate/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      701 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/exegesis/particulate/exegete_catalogue.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1353 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/exegesis/particulate/exegete_collection.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2248 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/exegesis/particulate/text.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.758826 scs-core-2.8.2/src/scs_core/gas/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      292 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.758826 scs-core-2.8.2/src/scs_core/gas/a4/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      410 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/a4/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3700 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/gas/a4/a4.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10274 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/gas/a4/a4_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5667 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4131 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum_v1.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3932 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum_vA.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5191 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum_vB.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5557 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum_vC.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4662 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/a4/a4_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6990 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/a4/a4_temp_comp.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.758826 scs-core-2.8.2/src/scs_core/gas/afe/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/afe/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1542 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/afe/afe_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3242 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/afe/pt1000_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2445 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/afe/pt1000_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3600 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/afe_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    11555 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/gas/afe_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6742 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/afe_id.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.758826 scs-core-2.8.2/src/scs_core/gas/d4/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      130 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/d4/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3710 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/d4/d4_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3106 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/gas/dsi_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4204 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/gas.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.758826 scs-core-2.8.2/src/scs_core/gas/isi/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/isi/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1373 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/isi/isi_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7366 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/gas/minimum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/gas/ndir/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/ndir/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1777 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/ndir/ndir.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2723 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/ndir/ndir_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3350 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/ndir/ndir_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3649 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/ndir/ndir_version.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3065 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/ndir/ndir_voltages.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/gas/pid/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      378 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/pid/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4106 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/pid/pid.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4196 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/gas/pid/pid_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4028 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/pid/pid_calibrated_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3730 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/pid/pid_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3694 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/pid/pid_temp_comp.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/gas/scd30/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/scd30/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2538 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/scd30/scd30_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2804 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/scd30/scd30_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2866 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gas/scd30/scd30_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3556 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/gas/sensor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6165 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/gas/sensor_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3043 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/gas/sensor_calib.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/gps/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gps/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4077 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/gps/gps_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/interface/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/interface/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2271 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/interface/interface_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/led/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/led/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      870 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/led/led.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2343 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/led/led_state.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/location/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/location/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2992 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/location/timezone.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3708 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/location/timezone_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2379 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/location/timezone_offset.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/model/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/model/catalogue/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/catalogue/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    11042 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/model/catalogue/model_compendium.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4774 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/catalogue/model_compendium_group.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5220 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/catalogue/term.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2038 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/catalogue/training_period.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/model/gas/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3349 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1354 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/gas_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1545 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/gas_inference_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2932 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/gas_model_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/model/gas/s1/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/s1/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2704 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/s1/gas_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3344 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/s1/s1_gas_inference_client.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/model/gas/vB/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/vB/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2702 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/vB/gas_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3120 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/vB/vb_gas_inference_client.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/model/gas/vE/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/vE/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3535 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/vE/gas_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4409 2022-10-03 10:46:58.000000 scs-core-2.8.2/src/scs_core/model/gas/vE/ve_gas_inference_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1218 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/gas/vcal_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3488 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/model/model_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.762826 scs-core-2.8.2/src/scs_core/model/pmx/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/pmx/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1549 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/pmx/pmx_inference_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1609 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/pmx/pmx_model_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.766826 scs-core-2.8.2/src/scs_core/model/pmx/s1/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/pmx/s1/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2215 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/pmx/s1/pmx_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2051 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.766826 scs-core-2.8.2/src/scs_core/monitor/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/monitor/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1558 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/monitor/monitor_error.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1557 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/monitor/monitor_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1395 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/monitor/monitor_response.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.766826 scs-core-2.8.2/src/scs_core/particulate/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/particulate/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4558 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/particulate/opc_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5142 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/particulate/opc_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2610 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/particulate/opc_version.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2103 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/particulate/pmx_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6405 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/particulate/sps_datum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.766826 scs-core-2.8.2/src/scs_core/position/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4062 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/position/gps_datum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.766826 scs-core-2.8.2/src/scs_core/position/nmea/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1578 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/gpdatetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4215 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/gpgga.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2685 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/gpgll.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3410 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/gpgsa.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3850 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/gpgsv.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2500 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/gploc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4056 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/gprmc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1318 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/gptime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2685 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/gpvtg.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2535 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/nmea_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      782 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/position/nmea/nmea_sentence.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3884 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/position/position.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.766826 scs-core-2.8.2/src/scs_core/psu/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/psu/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2320 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/psu/psu.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4543 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/psu/psu_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1733 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/psu/psu_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1728 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/psu/psu_uptime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5663 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/psu/psu_version.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.766826 scs-core-2.8.2/src/scs_core/sample/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sample/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3421 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/sample/climate_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    12029 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/sample/configuration_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5262 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/sample/gases_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3724 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/sample/particulates_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2872 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/sample/pressure_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4034 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/sample/sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5876 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/sample/status_sample.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.766826 scs-core-2.8.2/src/scs_core/sampler/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sampler/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1263 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sampler/sampler.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.766826 scs-core-2.8.2/src/scs_core/sync/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sync/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2168 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sync/interval_timer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1681 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sync/line_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      606 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sync/runner.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6819 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/sync/schedule.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1811 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sync/synchronised_process.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1724 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sync/timed_runner.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.770826 scs-core-2.8.2/src/scs_core/sys/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1791 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/sys/command.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4443 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/disk_usage.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5191 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/disk_volume.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2399 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/eeprom_image.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2622 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/exception_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6991 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/sys/filesystem.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1994 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/ipv4_address.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1167 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/sys/logging.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1297 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/sys/memory.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    17409 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/sys/modem.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5733 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/network.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5974 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/sys/node.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3851 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/persistence_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2318 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/sys/platform.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      834 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/process_comms.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4919 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/sys/ps_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3284 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/serial.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2405 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/shared_secret.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2506 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/signalled_exit.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2244 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/subprocess.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5730 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/sys/system_id.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2013 2023-06-26 09:33:48.000000 scs-core-2.8.2/src/scs_core/sys/system_temp.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6610 2023-03-20 10:12:25.000000 scs-core-2.8.2/src/scs_core/sys/tail.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1409 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/timeout.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1192 2023-02-06 14:01:57.000000 scs-core-2.8.2/src/scs_core/sys/timer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1784 2022-08-17 09:53:27.000000 scs-core-2.8.2/src/scs_core/sys/trace_entry.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5602 2022-09-20 10:07:36.000000 scs-core-2.8.2/src/scs_core/sys/uptime_datum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 13:24:09.742826 scs-core-2.8.2/src/scs_core.egg-info/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2059 2023-06-26 13:24:09.000000 scs-core-2.8.2/src/scs_core.egg-info/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)    13337 2023-06-26 13:24:09.000000 scs-core-2.8.2/src/scs_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-06-26 13:24:09.000000 scs-core-2.8.2/src/scs_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)      124 2023-06-26 13:24:09.000000 scs-core-2.8.2/src/scs_core.egg-info/requires.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)        9 2023-06-26 13:24:09.000000 scs-core-2.8.2/src/scs_core.egg-info/top_level.txt
```

### Comparing `scs-core-2.8.1/LICENSE` & `scs-core-2.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/PKG-INFO` & `scs-core-2.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-core
-Version: 2.8.1
+Version: 2.8.2
 Summary: The root of all South Coast Science environmental monitoring applications.
 Home-page: https://github.com/south-coast-science/scs_core
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scs-core-2.8.1/README.md` & `scs-core-2.8.2/README.md`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/setup.py` & `scs-core-2.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aqcsv/conf/airnow_site_conf.py` & `scs-core-2.8.2/src/scs_core/aqcsv/conf/airnow_site_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aqcsv/conf/airnow_uploader_conf.py` & `scs-core-2.8.2/src/scs_core/aqcsv/conf/airnow_uploader_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aqcsv/connector/airnow_mapping_task.py` & `scs-core-2.8.2/src/scs_core/aqcsv/connector/airnow_mapping_task.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aqcsv/connector/datum_mapping.py` & `scs-core-2.8.2/src/scs_core/aqcsv/connector/datum_mapping.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aqcsv/connector/source_mapping.py` & `scs-core-2.8.2/src/scs_core/aqcsv/connector/source_mapping.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aqcsv/data/aqcsv_datetime.py` & `scs-core-2.8.2/src/scs_core/aqcsv/data/aqcsv_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aqcsv/data/aqcsv_record.py` & `scs-core-2.8.2/src/scs_core/aqcsv/data/aqcsv_record.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aqcsv/data/aqcsv_site.py` & `scs-core-2.8.2/src/scs_core/aqcsv/data/aqcsv_site.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aqcsv/specification/agency.py` & `scs-core-2.8.2/src/scs_core/aqcsv/specification/agency.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aqcsv/specification/country.py` & `scs-core-2.8.2/src/scs_core/aqcsv/specification/country.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aqcsv/specification/country_iso.py` & `scs-core-2.8.2/src/scs_core/aqcsv/specification/country_iso.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aqcsv/specification/country_numeric.py` & `scs-core-2.8.2/src/scs_core/aqcsv/specification/country_numeric.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aqcsv/specification/method.py` & `scs-core-2.8.2/src/scs_core/aqcsv/specification/method.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aqcsv/specification/mpc.py` & `scs-core-2.8.2/src/scs_core/aqcsv/specification/mpc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aqcsv/specification/parameter.py` & `scs-core-2.8.2/src/scs_core/aqcsv/specification/parameter.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aqcsv/specification/qc.py` & `scs-core-2.8.2/src/scs_core/aqcsv/specification/qc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aqcsv/specification/qualifier.py` & `scs-core-2.8.2/src/scs_core/aqcsv/specification/qualifier.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aqcsv/specification/unit.py` & `scs-core-2.8.2/src/scs_core/aqcsv/specification/unit.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/client/access_key.py` & `scs-core-2.8.2/src/scs_core/aws/client/access_key.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/client/api_auth.py` & `scs-core-2.8.2/src/scs_core/aws/client/api_auth.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/client/api_client.py` & `scs-core-2.8.2/src/scs_core/aws/client/api_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/client/client.py` & `scs-core-2.8.2/src/scs_core/aws/client/client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/client/client_auth.py` & `scs-core-2.8.2/src/scs_core/aws/client/client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/client/device_control_client.py` & `scs-core-2.8.2/src/scs_core/aws/client/device_control_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/client/email_client.py` & `scs-core-2.8.2/src/scs_core/aws/client/email_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/client/monitor_auth.py` & `scs-core-2.8.2/src/scs_core/aws/client/monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/client/mqtt_client.py` & `scs-core-2.8.2/src/scs_core/aws/client/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/client/rest_client.py` & `scs-core-2.8.2/src/scs_core/aws/client/rest_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/config/aws.py` & `scs-core-2.8.2/src/scs_core/aws/config/aws.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/config/project.py` & `scs-core-2.8.2/src/scs_core/aws/config/project.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/data/alert.py` & `scs-core-2.8.2/src/scs_core/aws/data/alert.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/data/byline.py` & `scs-core-2.8.2/src/scs_core/aws/data/byline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/data/byline_list.py` & `scs-core-2.8.2/src/scs_core/aws/data/byline_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/data/dataset.py` & `scs-core-2.8.2/src/scs_core/aws/data/dataset.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/data/deployment.py` & `scs-core-2.8.2/src/scs_core/aws/data/deployment.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/data/device_monitor_email_list.py` & `scs-core-2.8.2/src/scs_core/aws/data/device_monitor_email_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/data/device_monitor_report.py` & `scs-core-2.8.2/src/scs_core/aws/data/device_monitor_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/data/device_report.py` & `scs-core-2.8.2/src/scs_core/aws/data/device_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/data/email_list.py` & `scs-core-2.8.2/src/scs_core/aws/data/email_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/data/http_response.py` & `scs-core-2.8.2/src/scs_core/aws/data/http_response.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/data/message.py` & `scs-core-2.8.2/src/scs_core/aws/data/message.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/data/power_list.py` & `scs-core-2.8.2/src/scs_core/aws/data/power_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/data/runtime_record.py` & `scs-core-2.8.2/src/scs_core/aws/data/runtime_record.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/data/status_list.py` & `scs-core-2.8.2/src/scs_core/aws/data/status_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/data/upload_interval.py` & `scs-core-2.8.2/src/scs_core/aws/data/upload_interval.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/data/uptime_list.py` & `scs-core-2.8.2/src/scs_core/aws/data/uptime_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/greengrass/aws_deployer.py` & `scs-core-2.8.2/src/scs_core/aws/greengrass/aws_deployer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/greengrass/aws_deployment_reporter.py` & `scs-core-2.8.2/src/scs_core/aws/greengrass/aws_deployment_reporter.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/greengrass/aws_group.py` & `scs-core-2.8.2/src/scs_core/aws/greengrass/aws_group.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/greengrass/aws_group_configuration.py` & `scs-core-2.8.2/src/scs_core/aws/greengrass/aws_group_configuration.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/greengrass/aws_identity.py` & `scs-core-2.8.2/src/scs_core/aws/greengrass/aws_identity.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/manager/alert_specification_manager.py` & `scs-core-2.8.2/src/scs_core/aws/manager/alert_specification_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/manager/alert_status_manager.py` & `scs-core-2.8.2/src/scs_core/aws/manager/alert_status_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/manager/byline_manager.py` & `scs-core-2.8.2/src/scs_core/aws/manager/byline_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/manager/configuration_check_finder.py` & `scs-core-2.8.2/src/scs_core/aws/manager/configuration_check_finder.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/manager/configuration_check_requester.py` & `scs-core-2.8.2/src/scs_core/aws/manager/configuration_check_requester.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/manager/configuration_finder.py` & `scs-core-2.8.2/src/scs_core/aws/manager/configuration_finder.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/manager/device_monitor_specification_manager.py` & `scs-core-2.8.2/src/scs_core/aws/manager/device_monitor_specification_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/manager/device_monitor_status_manager.py` & `scs-core-2.8.2/src/scs_core/aws/manager/device_monitor_status_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/manager/dynamo_manager.py` & `scs-core-2.8.2/src/scs_core/aws/manager/dynamo_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/manager/ec2_message_manager.py` & `scs-core-2.8.2/src/scs_core/aws/manager/ec2_message_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/manager/lambda_bylines.py` & `scs-core-2.8.2/src/scs_core/aws/manager/lambda_bylines.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/manager/lambda_message_manager.py` & `scs-core-2.8.2/src/scs_core/aws/manager/lambda_message_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/manager/s3_manager.py` & `scs-core-2.8.2/src/scs_core/aws/manager/s3_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/manager/sagemaker_model_manager.py` & `scs-core-2.8.2/src/scs_core/aws/manager/sagemaker_model_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/manager/sagemaker_trial_manager.py` & `scs-core-2.8.2/src/scs_core/aws/manager/sagemaker_trial_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/security/access_key_manager.py` & `scs-core-2.8.2/src/scs_core/aws/security/access_key_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/security/cognito_client_credentials.py` & `scs-core-2.8.2/src/scs_core/aws/security/cognito_client_credentials.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/security/cognito_device.py` & `scs-core-2.8.2/src/scs_core/aws/security/cognito_device.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/security/cognito_device_creator.py` & `scs-core-2.8.2/src/scs_core/aws/security/cognito_device_creator.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/security/cognito_device_finder.py` & `scs-core-2.8.2/src/scs_core/aws/security/cognito_device_finder.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/security/cognito_device_manager.py` & `scs-core-2.8.2/src/scs_core/aws/security/cognito_device_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/security/cognito_login_manager.py` & `scs-core-2.8.2/src/scs_core/aws/security/cognito_login_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/security/cognito_membership.py` & `scs-core-2.8.2/src/scs_core/aws/security/cognito_membership.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/security/cognito_password_manager.py` & `scs-core-2.8.2/src/scs_core/aws/security/cognito_password_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/security/cognito_user.py` & `scs-core-2.8.2/src/scs_core/aws/security/cognito_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,39 +150,41 @@
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def construct_from_jdict(cls, jdict, skeleton=False):
         if not jdict:
-            return cls(None, None, None, None, None, None, None, None, None, None, None, None) if skeleton else None
+            return cls(None, None, None, None, None, None, None, None, None, None, None, None, None) if skeleton \
+                else None
 
         username = jdict.get('username')
         email = jdict.get('email')
         password = jdict.get('password')
         given_name = cls.int_name(jdict.get('given-name'))
         family_name = cls.int_name(jdict.get('family-name'))
 
         confirmation_status = jdict.get('confirmation-status')
         enabled = jdict.get('enabled')
         email_verified = jdict.get('email-verified')
         is_super = jdict.get('is-super')
         is_tester = jdict.get('is-tester')
+        is_financial = jdict.get('is-financial')
 
         created = LocalizedDatetime.construct_from_iso8601(jdict.get('created'))
         last_updated = LocalizedDatetime.construct_from_iso8601(jdict.get('last-updated'))
 
-        return cls(username, created, confirmation_status, enabled,
-                   email_verified, email, given_name, family_name, password, is_super, is_tester, last_updated)
+        return cls(username, created, confirmation_status, enabled, email_verified, email,
+                   given_name, family_name, password, is_super, is_tester, is_financial, last_updated)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, username, created, confirmation_status, enabled,
-                 email_verified, email, given_name, family_name, password, is_super, is_tester, last_updated):
+    def __init__(self, username, created, confirmation_status, enabled, email_verified, email,
+                 given_name, family_name, password, is_super, is_tester, is_financial, last_updated):
         """
         Constructor
         """
 
         self._username = username                                   # string email address or hash
         self._created = created                                     # LocalisedDatetime
         self.__confirmation_status = confirmation_status            # string
@@ -191,14 +193,15 @@
         self.__email_verified = bool(email_verified)                # bool
         self.__email = email                                        # string
         self.__given_name = given_name                              # string
         self.__family_name = family_name                            # string
         self.__password = password                                  # string
         self.__is_super = bool(is_super)                            # bool
         self.__is_tester = bool(is_tester)                          # bool
+        self.__is_financial = bool(is_financial)                    # bool
 
         self._last_updated = last_updated                           # LocalizedDatetime
 
 
     def __eq__(self, other):
         try:
             return self.username == other.username and self.confirmation_status == other.confirmation_status \
@@ -289,14 +292,15 @@
 
         if self.enabled is not None:
             jdict['enabled'] = self.enabled
 
         jdict['email-verified'] = self.email_verified
         jdict['is-super'] = self.is_super
         jdict['is-tester'] = self.is_tester
+        jdict['is-financial'] = self.is_financial
 
         if self.created is not None:
             jdict['created'] = self.created.as_iso8601()
 
         if self.last_updated is not None:
             jdict['last-updated'] = self.last_updated.as_iso8601()
 
@@ -357,20 +361,25 @@
 
     @property
     def is_tester(self):
         return self.__is_tester
 
 
     @property
+    def is_financial(self):
+        return self.__is_financial
+
+
+    @property
     def last_updated(self):
         return self._last_updated
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
         return self.__class__.__name__ + ":{username:%s, created:%s, confirmation_status:%s, enabled:%s, " \
                "email_verified:%s, email:%s, given_name:%s, family_name:%s, is_super:%s, is_tester:%s, " \
-               "last_updated:%s}" % \
+               "is_financial:%s, last_updated:%s}" % \
                (self.username, self.created, self.confirmation_status, self.enabled,
                 self.email_verified, self.email, self.given_name, self.family_name, self.is_super, self.is_tester,
-                self.last_updated)
+                self.is_financial, self.last_updated)
```

### Comparing `scs-core-2.8.1/src/scs_core/aws/security/cognito_user_finder.py` & `scs-core-2.8.2/src/scs_core/aws/security/cognito_user_finder.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/security/cognito_user_manager.py` & `scs-core-2.8.2/src/scs_core/aws/security/cognito_user_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/security/device_whitelist_manager.py` & `scs-core-2.8.2/src/scs_core/aws/security/device_whitelist_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/security/opr_membership.py` & `scs-core-2.8.2/src/scs_core/aws/security/opr_membership.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/security/organisation.py` & `scs-core-2.8.2/src/scs_core/aws/security/organisation.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/security/organisation_manager.py` & `scs-core-2.8.2/src/scs_core/aws/security/organisation_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/aws/security/path_filter.py` & `scs-core-2.8.2/src/scs_core/aws/security/path_filter.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/client/http_client.py` & `scs-core-2.8.2/src/scs_core/client/http_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/client/http_exception.py` & `scs-core-2.8.2/src/scs_core/client/http_exception.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/client/network.py` & `scs-core-2.8.2/src/scs_core/client/network.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/client/resource_unavailable_exception.py` & `scs-core-2.8.2/src/scs_core/client/resource_unavailable_exception.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/client/sftp_client_conf.py` & `scs-core-2.8.2/src/scs_core/client/sftp_client_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/climate/absolute_humidity.py` & `scs-core-2.8.2/src/scs_core/climate/absolute_humidity.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/climate/icp10101_datum.py` & `scs-core-2.8.2/src/scs_core/climate/icp10101_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/climate/mpl115a2_calib.py` & `scs-core-2.8.2/src/scs_core/climate/mpl115a2_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/climate/mpl115a2_datum.py` & `scs-core-2.8.2/src/scs_core/climate/mpl115a2_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/climate/pressure_conf.py` & `scs-core-2.8.2/src/scs_core/climate/pressure_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/climate/pressure_datum.py` & `scs-core-2.8.2/src/scs_core/climate/pressure_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/climate/sht_conf.py` & `scs-core-2.8.2/src/scs_core/climate/sht_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/climate/sht_datum.py` & `scs-core-2.8.2/src/scs_core/climate/sht_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/comms/mqtt_conf.py` & `scs-core-2.8.2/src/scs_core/comms/mqtt_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/comms/uds_client.py` & `scs-core-2.8.2/src/scs_core/comms/uds_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/comms/uds_reader.py` & `scs-core-2.8.2/src/scs_core/comms/uds_reader.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/comms/uds_server.py` & `scs-core-2.8.2/src/scs_core/comms/uds_server.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/comms/uds_writer.py` & `scs-core-2.8.2/src/scs_core/comms/uds_writer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/control/command.py` & `scs-core-2.8.2/src/scs_core/control/command.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/control/control_datum.py` & `scs-core-2.8.2/src/scs_core/control/control_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/control/control_handler.py` & `scs-core-2.8.2/src/scs_core/control/control_handler.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/control/control_receipt.py` & `scs-core-2.8.2/src/scs_core/control/control_receipt.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/csv/csv_archive.py` & `scs-core-2.8.2/src/scs_core/csv/csv_archive.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/csv/csv_dict.py` & `scs-core-2.8.2/src/scs_core/csv/csv_dict.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/csv/csv_log.py` & `scs-core-2.8.2/src/scs_core/csv/csv_log.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/csv/csv_log_cursor_queue.py` & `scs-core-2.8.2/src/scs_core/csv/csv_log_cursor_queue.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/csv/csv_log_reader.py` & `scs-core-2.8.2/src/scs_core/csv/csv_log_reader.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/csv/csv_logger.py` & `scs-core-2.8.2/src/scs_core/csv/csv_logger.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/csv/csv_logger_conf.py` & `scs-core-2.8.2/src/scs_core/csv/csv_logger_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/csv/csv_reader.py` & `scs-core-2.8.2/src/scs_core/csv/csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/csv/csv_writer.py` & `scs-core-2.8.2/src/scs_core/csv/csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/aggregate.py` & `scs-core-2.8.2/src/scs_core/data/aggregate.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/array_dict.py` & `scs-core-2.8.2/src/scs_core/data/array_dict.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/average.py` & `scs-core-2.8.2/src/scs_core/data/average.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/categorical_regression.py` & `scs-core-2.8.2/src/scs_core/data/categorical_regression.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/checkpoint_generator.py` & `scs-core-2.8.2/src/scs_core/data/checkpoint_generator.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/crc.py` & `scs-core-2.8.2/src/scs_core/data/crc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/crypt.py` & `scs-core-2.8.2/src/scs_core/data/crypt.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/datetime.py` & `scs-core-2.8.2/src/scs_core/data/datetime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/datum.py` & `scs-core-2.8.2/src/scs_core/data/datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/duplicates.py` & `scs-core-2.8.2/src/scs_core/data/duplicates.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/histogram.py` & `scs-core-2.8.2/src/scs_core/data/histogram.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/interval.py` & `scs-core-2.8.2/src/scs_core/data/interval.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/join.py` & `scs-core-2.8.2/src/scs_core/data/join.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/json.py` & `scs-core-2.8.2/src/scs_core/data/json.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/lin_regress.py` & `scs-core-2.8.2/src/scs_core/data/lin_regress.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/linear_regression.py` & `scs-core-2.8.2/src/scs_core/data/linear_regression.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/low_pass_filter.py` & `scs-core-2.8.2/src/scs_core/data/low_pass_filter.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/median_filter.py` & `scs-core-2.8.2/src/scs_core/data/median_filter.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/min_list.py` & `scs-core-2.8.2/src/scs_core/data/min_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/model_delta.py` & `scs-core-2.8.2/src/scs_core/data/model_delta.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/path_dict.py` & `scs-core-2.8.2/src/scs_core/data/path_dict.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/precision.py` & `scs-core-2.8.2/src/scs_core/data/precision.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/publication.py` & `scs-core-2.8.2/src/scs_core/data/publication.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/queue_report.py` & `scs-core-2.8.2/src/scs_core/data/queue_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/recurring_period.py` & `scs-core-2.8.2/src/scs_core/data/recurring_period.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/regression.py` & `scs-core-2.8.2/src/scs_core/data/regression.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/rtc_datetime.py` & `scs-core-2.8.2/src/scs_core/data/rtc_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/sample_delta.py` & `scs-core-2.8.2/src/scs_core/data/sample_delta.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/stats.py` & `scs-core-2.8.2/src/scs_core/data/stats.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/str.py` & `scs-core-2.8.2/src/scs_core/data/str.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/timedelta.py` & `scs-core-2.8.2/src/scs_core/data/timedelta.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/tokens.py` & `scs-core-2.8.2/src/scs_core/data/tokens.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/data/topic_path.py` & `scs-core-2.8.2/src/scs_core/data/topic_path.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/display/display_conf.py` & `scs-core-2.8.2/src/scs_core/display/display_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/email/email_queue.py` & `scs-core-2.8.2/src/scs_core/email/email_queue.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/email/email_queue_manager.py` & `scs-core-2.8.2/src/scs_core/email/email_queue_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/estate/baseline_conf.py` & `scs-core-2.8.2/src/scs_core/estate/baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/estate/configuration.py` & `scs-core-2.8.2/src/scs_core/estate/configuration.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/estate/configuration_check.py` & `scs-core-2.8.2/src/scs_core/estate/configuration_check.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/estate/git_pull.py` & `scs-core-2.8.2/src/scs_core/estate/git_pull.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/estate/git_pull_check.py` & `scs-core-2.8.2/src/scs_core/estate/git_pull_check.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/estate/mqtt_device_poller.py` & `scs-core-2.8.2/src/scs_core/estate/mqtt_device_poller.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/estate/mqtt_peer.py` & `scs-core-2.8.2/src/scs_core/estate/mqtt_peer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/estate/package_version.py` & `scs-core-2.8.2/src/scs_core/estate/package_version.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/exegesis/gas/exegete_catalogue.py` & `scs-core-2.8.2/src/scs_core/exegesis/gas/exegete_catalogue.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/exegesis/gas/exegete_collection.py` & `scs-core-2.8.2/src/scs_core/exegesis/gas/exegete_collection.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/exegesis/particulate/exegete_catalogue.py` & `scs-core-2.8.2/src/scs_core/exegesis/particulate/exegete_catalogue.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/exegesis/particulate/exegete_collection.py` & `scs-core-2.8.2/src/scs_core/exegesis/particulate/exegete_collection.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/exegesis/particulate/text.py` & `scs-core-2.8.2/src/scs_core/exegesis/particulate/text.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/a4/a4.py` & `scs-core-2.8.2/src/scs_core/gas/a4/a4.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/a4/a4_calib.py` & `scs-core-2.8.2/src/scs_core/gas/a4/a4_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum.py` & `scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum_v1.py` & `scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum_v1.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum_vA.py` & `scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum_vA.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum_vB.py` & `scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum_vB.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum_vC.py` & `scs-core-2.8.2/src/scs_core/gas/a4/a4_calibrated_datum_vC.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/a4/a4_datum.py` & `scs-core-2.8.2/src/scs_core/gas/a4/a4_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/a4/a4_temp_comp.py` & `scs-core-2.8.2/src/scs_core/gas/a4/a4_temp_comp.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/afe/afe_datum.py` & `scs-core-2.8.2/src/scs_core/gas/afe/afe_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/afe/pt1000_calib.py` & `scs-core-2.8.2/src/scs_core/gas/afe/pt1000_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/afe/pt1000_datum.py` & `scs-core-2.8.2/src/scs_core/gas/afe/pt1000_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/afe_baseline.py` & `scs-core-2.8.2/src/scs_core/gas/afe_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/afe_calib.py` & `scs-core-2.8.2/src/scs_core/gas/afe_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/afe_id.py` & `scs-core-2.8.2/src/scs_core/gas/afe_id.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/d4/d4_datum.py` & `scs-core-2.8.2/src/scs_core/gas/d4/d4_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/dsi_calib.py` & `scs-core-2.8.2/src/scs_core/gas/dsi_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/gas.py` & `scs-core-2.8.2/src/scs_core/gas/gas.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/isi/isi_datum.py` & `scs-core-2.8.2/src/scs_core/gas/isi/isi_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/minimum.py` & `scs-core-2.8.2/src/scs_core/gas/minimum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/ndir/ndir.py` & `scs-core-2.8.2/src/scs_core/gas/ndir/ndir.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/ndir/ndir_conf.py` & `scs-core-2.8.2/src/scs_core/gas/ndir/ndir_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/ndir/ndir_datum.py` & `scs-core-2.8.2/src/scs_core/gas/ndir/ndir_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/ndir/ndir_version.py` & `scs-core-2.8.2/src/scs_core/gas/ndir/ndir_version.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/ndir/ndir_voltages.py` & `scs-core-2.8.2/src/scs_core/gas/ndir/ndir_voltages.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/pid/pid.py` & `scs-core-2.8.2/src/scs_core/gas/pid/pid.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/pid/pid_calib.py` & `scs-core-2.8.2/src/scs_core/gas/pid/pid_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/pid/pid_calibrated_datum.py` & `scs-core-2.8.2/src/scs_core/gas/pid/pid_calibrated_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/pid/pid_datum.py` & `scs-core-2.8.2/src/scs_core/gas/pid/pid_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/pid/pid_temp_comp.py` & `scs-core-2.8.2/src/scs_core/gas/pid/pid_temp_comp.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/scd30/scd30_baseline.py` & `scs-core-2.8.2/src/scs_core/gas/scd30/scd30_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/scd30/scd30_conf.py` & `scs-core-2.8.2/src/scs_core/gas/scd30/scd30_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/scd30/scd30_datum.py` & `scs-core-2.8.2/src/scs_core/gas/scd30/scd30_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/sensor.py` & `scs-core-2.8.2/src/scs_core/gas/sensor.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/sensor_baseline.py` & `scs-core-2.8.2/src/scs_core/gas/sensor_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gas/sensor_calib.py` & `scs-core-2.8.2/src/scs_core/gas/sensor_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/gps/gps_conf.py` & `scs-core-2.8.2/src/scs_core/gps/gps_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/interface/interface_conf.py` & `scs-core-2.8.2/src/scs_core/interface/interface_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/led/led.py` & `scs-core-2.8.2/src/scs_core/led/led.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/led/led_state.py` & `scs-core-2.8.2/src/scs_core/led/led_state.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/location/timezone.py` & `scs-core-2.8.2/src/scs_core/location/timezone.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/location/timezone_conf.py` & `scs-core-2.8.2/src/scs_core/location/timezone_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/location/timezone_offset.py` & `scs-core-2.8.2/src/scs_core/location/timezone_offset.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/catalogue/model_compendium.py` & `scs-core-2.8.2/src/scs_core/model/catalogue/model_compendium.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/catalogue/model_compendium_group.py` & `scs-core-2.8.2/src/scs_core/model/catalogue/model_compendium_group.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/catalogue/term.py` & `scs-core-2.8.2/src/scs_core/model/catalogue/term.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/catalogue/training_period.py` & `scs-core-2.8.2/src/scs_core/model/catalogue/training_period.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/gas/baseline.py` & `scs-core-2.8.2/src/scs_core/model/gas/baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/gas/gas_baseline.py` & `scs-core-2.8.2/src/scs_core/model/gas/gas_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/gas/gas_inference_client.py` & `scs-core-2.8.2/src/scs_core/model/gas/gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/gas/gas_model_conf.py` & `scs-core-2.8.2/src/scs_core/model/gas/gas_model_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/gas/s1/gas_request.py` & `scs-core-2.8.2/src/scs_core/model/gas/s1/gas_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/gas/s1/s1_gas_inference_client.py` & `scs-core-2.8.2/src/scs_core/model/gas/s1/s1_gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/gas/vB/gas_request.py` & `scs-core-2.8.2/src/scs_core/model/gas/vB/gas_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/gas/vB/vb_gas_inference_client.py` & `scs-core-2.8.2/src/scs_core/model/gas/vB/vb_gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/gas/vE/gas_request.py` & `scs-core-2.8.2/src/scs_core/model/gas/vE/gas_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/gas/vE/ve_gas_inference_client.py` & `scs-core-2.8.2/src/scs_core/model/gas/vE/ve_gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/gas/vcal_baseline.py` & `scs-core-2.8.2/src/scs_core/model/gas/vcal_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/model_conf.py` & `scs-core-2.8.2/src/scs_core/model/model_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/pmx/pmx_inference_client.py` & `scs-core-2.8.2/src/scs_core/model/pmx/pmx_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/pmx/pmx_model_conf.py` & `scs-core-2.8.2/src/scs_core/model/pmx/pmx_model_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/pmx/s1/pmx_request.py` & `scs-core-2.8.2/src/scs_core/model/pmx/s1/pmx_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py` & `scs-core-2.8.2/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/monitor/monitor_error.py` & `scs-core-2.8.2/src/scs_core/monitor/monitor_error.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/monitor/monitor_request.py` & `scs-core-2.8.2/src/scs_core/monitor/monitor_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/monitor/monitor_response.py` & `scs-core-2.8.2/src/scs_core/monitor/monitor_response.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/particulate/opc_conf.py` & `scs-core-2.8.2/src/scs_core/particulate/opc_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/particulate/opc_datum.py` & `scs-core-2.8.2/src/scs_core/particulate/opc_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/particulate/opc_version.py` & `scs-core-2.8.2/src/scs_core/particulate/opc_version.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/particulate/pmx_datum.py` & `scs-core-2.8.2/src/scs_core/particulate/pmx_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/particulate/sps_datum.py` & `scs-core-2.8.2/src/scs_core/particulate/sps_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/position/gps_datum.py` & `scs-core-2.8.2/src/scs_core/position/gps_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/position/nmea/gpdatetime.py` & `scs-core-2.8.2/src/scs_core/position/nmea/gpdatetime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/position/nmea/gpgga.py` & `scs-core-2.8.2/src/scs_core/position/nmea/gpgga.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/position/nmea/gpgll.py` & `scs-core-2.8.2/src/scs_core/position/nmea/gpgll.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/position/nmea/gpgsa.py` & `scs-core-2.8.2/src/scs_core/position/nmea/gpgsa.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/position/nmea/gpgsv.py` & `scs-core-2.8.2/src/scs_core/position/nmea/gpgsv.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/position/nmea/gploc.py` & `scs-core-2.8.2/src/scs_core/position/nmea/gploc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/position/nmea/gprmc.py` & `scs-core-2.8.2/src/scs_core/position/nmea/gprmc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/position/nmea/gptime.py` & `scs-core-2.8.2/src/scs_core/position/nmea/gptime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/position/nmea/gpvtg.py` & `scs-core-2.8.2/src/scs_core/position/nmea/gpvtg.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/position/nmea/nmea_report.py` & `scs-core-2.8.2/src/scs_core/position/nmea/nmea_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/position/nmea/nmea_sentence.py` & `scs-core-2.8.2/src/scs_core/position/nmea/nmea_sentence.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/position/position.py` & `scs-core-2.8.2/src/scs_core/position/position.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/psu/psu.py` & `scs-core-2.8.2/src/scs_core/psu/psu.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/psu/psu_conf.py` & `scs-core-2.8.2/src/scs_core/psu/psu_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/psu/psu_report.py` & `scs-core-2.8.2/src/scs_core/psu/psu_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/psu/psu_uptime.py` & `scs-core-2.8.2/src/scs_core/psu/psu_uptime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/psu/psu_version.py` & `scs-core-2.8.2/src/scs_core/psu/psu_version.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sample/climate_sample.py` & `scs-core-2.8.2/src/scs_core/sample/climate_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sample/configuration_sample.py` & `scs-core-2.8.2/src/scs_core/sample/configuration_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sample/gases_sample.py` & `scs-core-2.8.2/src/scs_core/sample/gases_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sample/particulates_sample.py` & `scs-core-2.8.2/src/scs_core/sample/particulates_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sample/pressure_sample.py` & `scs-core-2.8.2/src/scs_core/sample/pressure_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sample/sample.py` & `scs-core-2.8.2/src/scs_core/sample/sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sample/status_sample.py` & `scs-core-2.8.2/src/scs_core/sample/status_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sampler/sampler.py` & `scs-core-2.8.2/src/scs_core/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sync/interval_timer.py` & `scs-core-2.8.2/src/scs_core/sync/interval_timer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sync/line_reader.py` & `scs-core-2.8.2/src/scs_core/sync/line_reader.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sync/runner.py` & `scs-core-2.8.2/src/scs_core/sync/runner.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sync/schedule.py` & `scs-core-2.8.2/src/scs_core/sync/schedule.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sync/synchronised_process.py` & `scs-core-2.8.2/src/scs_core/sync/synchronised_process.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sync/timed_runner.py` & `scs-core-2.8.2/src/scs_core/sync/timed_runner.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/command.py` & `scs-core-2.8.2/src/scs_core/sys/command.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/disk_usage.py` & `scs-core-2.8.2/src/scs_core/sys/disk_usage.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/disk_volume.py` & `scs-core-2.8.2/src/scs_core/sys/disk_volume.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/eeprom_image.py` & `scs-core-2.8.2/src/scs_core/sys/eeprom_image.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/exception_report.py` & `scs-core-2.8.2/src/scs_core/sys/exception_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/filesystem.py` & `scs-core-2.8.2/src/scs_core/sys/filesystem.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/ipv4_address.py` & `scs-core-2.8.2/src/scs_core/sys/ipv4_address.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/logging.py` & `scs-core-2.8.2/src/scs_core/sys/logging.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/memory.py` & `scs-core-2.8.2/src/scs_core/sys/memory.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/modem.py` & `scs-core-2.8.2/src/scs_core/sys/modem.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/network.py` & `scs-core-2.8.2/src/scs_core/sys/network.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/node.py` & `scs-core-2.8.2/src/scs_core/sys/node.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/persistence_manager.py` & `scs-core-2.8.2/src/scs_core/sys/persistence_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/platform.py` & `scs-core-2.8.2/src/scs_core/sys/platform.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/process_comms.py` & `scs-core-2.8.2/src/scs_core/sys/process_comms.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/ps_datum.py` & `scs-core-2.8.2/src/scs_core/sys/ps_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/serial.py` & `scs-core-2.8.2/src/scs_core/sys/serial.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/shared_secret.py` & `scs-core-2.8.2/src/scs_core/sys/shared_secret.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/signalled_exit.py` & `scs-core-2.8.2/src/scs_core/sys/signalled_exit.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/subprocess.py` & `scs-core-2.8.2/src/scs_core/sys/subprocess.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/system_id.py` & `scs-core-2.8.2/src/scs_core/sys/system_id.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/system_temp.py` & `scs-core-2.8.2/src/scs_core/sys/system_temp.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/tail.py` & `scs-core-2.8.2/src/scs_core/sys/tail.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/timeout.py` & `scs-core-2.8.2/src/scs_core/sys/timeout.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/timer.py` & `scs-core-2.8.2/src/scs_core/sys/timer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/trace_entry.py` & `scs-core-2.8.2/src/scs_core/sys/trace_entry.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core/sys/uptime_datum.py` & `scs-core-2.8.2/src/scs_core/sys/uptime_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.8.1/src/scs_core.egg-info/PKG-INFO` & `scs-core-2.8.2/src/scs_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-core
-Version: 2.8.1
+Version: 2.8.2
 Summary: The root of all South Coast Science environmental monitoring applications.
 Home-page: https://github.com/south-coast-science/scs_core
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scs-core-2.8.1/src/scs_core.egg-info/SOURCES.txt` & `scs-core-2.8.2/src/scs_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

