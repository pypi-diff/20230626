# Comparing `tmp/scs-core-2.4.6.tar.gz` & `tmp/scs-core-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs-core-2.4.6.tar", last modified: Mon Mar 20 10:15:26 2023, max compression
+gzip compressed data, was "scs-core-2.8.1.tar", last modified: Mon Jun 26 09:34:13 2023, max compression
```

## Comparing `scs-core-2.4.6.tar` & `scs-core-2.8.1.tar`

### file list

```diff
@@ -1,459 +1,419 @@
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.594678 scs-core-2.4.6/
--rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:27.000000 scs-core-2.4.6/LICENSE
--rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:27.000000 scs-core-2.4.6/MANIFEST.in
--rw-rw-r--   0 jade      (1002) jade      (1002)     1027 2023-03-20 10:15:26.594678 scs-core-2.4.6/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)      372 2022-08-17 09:53:27.000000 scs-core-2.4.6/README.md
--rw-rw-r--   0 jade      (1002) jade      (1002)       41 2022-08-17 09:53:27.000000 scs-core-2.4.6/README.rst
--rw-rw-r--   0 jade      (1002) jade      (1002)      124 2023-02-06 14:01:57.000000 scs-core-2.4.6/requirements.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-03-20 10:15:26.594678 scs-core-2.4.6/setup.cfg
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1996 2022-08-17 09:53:27.000000 scs-core-2.4.6/setup.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.558677 scs-core-2.4.6/src/
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.562677 scs-core-2.4.6/src/scs_core/
--rw-rw-r--   0 jade      (1002) jade      (1002)      183 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.562677 scs-core-2.4.6/src/scs_core/aqcsv/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.562677 scs-core-2.4.6/src/scs_core/aqcsv/conf/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/conf/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2617 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/conf/airnow_site_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1034 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/conf/airnow_uploader_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.566677 scs-core-2.4.6/src/scs_core/aqcsv/connector/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/connector/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10203 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aqcsv/connector/airnow_mapping_task.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6655 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/connector/datum_mapping.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5042 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/connector/source_mapping.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.566677 scs-core-2.4.6/src/scs_core/aqcsv/data/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/data/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3750 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/data/aqcsv_datetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    13723 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/data/aqcsv_record.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3033 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/data/aqcsv_site.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.566677 scs-core-2.4.6/src/scs_core/aqcsv/specification/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/specification/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2824 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/specification/agency.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2728 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/specification/country.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1163 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/specification/country_iso.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1175 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/specification/country_numeric.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     9800 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/specification/method.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3765 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/specification/mpc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3453 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/specification/parameter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2855 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/specification/qc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3732 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/specification/qualifier.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2879 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aqcsv/specification/unit.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.566677 scs-core-2.4.6/src/scs_core/aws/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.566677 scs-core-2.4.6/src/scs_core/aws/client/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/client/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3518 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/client/access_key.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2332 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/client/api_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1217 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/client/client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5103 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/client/client_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3294 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/client/email_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3361 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/client/monitor_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5891 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/client/mqtt_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3854 2022-11-09 12:09:25.000000 scs-core-2.4.6/src/scs_core/aws/client/rest_client.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.566677 scs-core-2.4.6/src/scs_core/aws/config/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/config/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      744 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/config/aws.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4471 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/config/project.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.566677 scs-core-2.4.6/src/scs_core/aws/data/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/data/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    13143 2022-09-20 10:07:36.000000 scs-core-2.4.6/src/scs_core/aws/data/alert.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     9028 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/data/byline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1792 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/data/byline_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4546 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/data/dataset.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3550 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/data/deployment.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3287 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/data/device_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4032 2022-09-20 10:07:36.000000 scs-core-2.4.6/src/scs_core/aws/data/email_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2857 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/data/http_response.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3175 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/data/message.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1776 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/data/power_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1820 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/data/runtime_record.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1795 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/data/status_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2884 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/data/upload_interval.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1793 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/data/uptime_list.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.566677 scs-core-2.4.6/src/scs_core/aws/greengrass/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/greengrass/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1998 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/greengrass/aws_deployer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3017 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/greengrass/aws_deployment_reporter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     9610 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/greengrass/aws_group.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    16440 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/greengrass/aws_group_configuration.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    11557 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/greengrass/aws_identity.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      440 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/greengrass/gg_errors.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.570677 scs-core-2.4.6/src/scs_core/aws/manager/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/manager/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7721 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/manager/alert_specification_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7109 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/manager/alert_status_finder.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3867 2022-11-09 12:09:25.000000 scs-core-2.4.6/src/scs_core/aws/manager/byline_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7661 2022-09-20 10:07:36.000000 scs-core-2.4.6/src/scs_core/aws/manager/configuration_check_finder.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3286 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/manager/configuration_check_requester.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10989 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/manager/configuration_finder.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     9506 2022-11-09 12:09:25.000000 scs-core-2.4.6/src/scs_core/aws/manager/dynamo_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3551 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/manager/ec2_message_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6467 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/manager/lambda_bylines.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    15996 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/aws/manager/lambda_message_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    18045 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/manager/s3_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4295 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/manager/sagemaker_model_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7802 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/manager/sagemaker_trial_manager.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.570677 scs-core-2.4.6/src/scs_core/aws/security/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/aws/security/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1343 2022-11-09 12:09:25.000000 scs-core-2.4.6/src/scs_core/aws/security/byline_filter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4838 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/security/cognito_device.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2877 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/security/cognito_device_finder.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2749 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/security/cognito_device_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10686 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/security/cognito_login_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2178 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/security/cognito_membership.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3791 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/security/cognito_password_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    14261 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/security/cognito_user.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4186 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/security/cognito_user_finder.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4325 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/security/cognito_user_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    22594 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/security/organisation.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10431 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/aws/security/organisation_manager.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.570677 scs-core-2.4.6/src/scs_core/client/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/client/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4403 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/client/http_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2746 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/client/network.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1415 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/client/resource_unavailable_exception.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2638 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/client/sftp_client_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.570677 scs-core-2.4.6/src/scs_core/climate/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/climate/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1407 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/climate/absolute_humidity.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1418 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/climate/icp10101_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3081 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/climate/mpl115a2_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2911 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/climate/mpl115a2_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2290 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/climate/pressure_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2188 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/climate/pressure_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3156 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/climate/sht_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1844 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/climate/sht_datum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.574677 scs-core-2.4.6/src/scs_core/comms/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/comms/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3125 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/comms/mqtt_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2395 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/comms/uds_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1552 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/comms/uds_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2350 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/comms/uds_server.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1614 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/comms/uds_writer.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.574677 scs-core-2.4.6/src/scs_core/control/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/control/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4918 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/control/command.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4896 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/control/control_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3792 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/control/control_handler.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4737 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/control/control_receipt.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.574677 scs-core-2.4.6/src/scs_core/csv/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/csv/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1979 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/csv/csv_archive.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7470 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/csv/csv_dict.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5996 2022-09-20 10:07:36.000000 scs-core-2.4.6/src/scs_core/csv/csv_log.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8594 2022-09-20 10:07:36.000000 scs-core-2.4.6/src/scs_core/csv/csv_log_cursor_queue.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8574 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/csv/csv_log_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8212 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/csv/csv_logger.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3323 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/csv/csv_logger_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5347 2022-09-20 10:07:36.000000 scs-core-2.4.6/src/scs_core/csv/csv_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4503 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/csv/csv_writer.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.578677 scs-core-2.4.6/src/scs_core/data/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4802 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/aggregate.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1947 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/data/array_dict.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2415 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/average.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2158 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/categorical_regression.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8964 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/data/checkpoint_generator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1008 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/crc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2092 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/crypt.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    19704 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/data/datetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6448 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/data/datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2374 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/duplicates.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3809 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/data/histogram.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1747 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/interval.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5951 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/join.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    14362 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/data/json.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3274 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/lin_regress.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5364 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/linear_regression.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1372 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/low_pass_filter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1628 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/median_filter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1892 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/min_list.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5682 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/data/model_delta.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8334 2022-09-20 10:07:36.000000 scs-core-2.4.6/src/scs_core/data/path_dict.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1291 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/precision.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3466 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/publication.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4181 2022-09-20 10:07:36.000000 scs-core-2.4.6/src/scs_core/data/queue_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8861 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/recurring_period.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1265 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/regression.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4348 2022-09-20 10:07:36.000000 scs-core-2.4.6/src/scs_core/data/rtc_datetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2249 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/data/sample_delta.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    10713 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/stats.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1280 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/str.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7391 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/timedelta.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2185 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/data/tokens.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7456 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/data/topic_path.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.578677 scs-core-2.4.6/src/scs_core/display/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/display/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3786 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/display/display_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.578677 scs-core-2.4.6/src/scs_core/email/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/email/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2131 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/email/email_queue.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2420 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/email/email_queue_manager.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.578677 scs-core-2.4.6/src/scs_core/estate/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/estate/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6202 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/estate/baseline_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    33840 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/estate/configuration.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4521 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/estate/configuration_check.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5221 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/estate/git_pull.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3621 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/estate/git_pull_check.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6613 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/estate/mqtt_device_poller.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6246 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/estate/mqtt_peer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6563 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/estate/package_version.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.578677 scs-core-2.4.6/src/scs_core/exegesis/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/exegesis/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.578677 scs-core-2.4.6/src/scs_core/exegesis/gas/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/exegesis/gas/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      693 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/exegesis/gas/exegete_catalogue.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1345 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/exegesis/gas/exegete_collection.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.578677 scs-core-2.4.6/src/scs_core/exegesis/particulate/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/exegesis/particulate/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      701 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/exegesis/particulate/exegete_catalogue.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1353 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/exegesis/particulate/exegete_collection.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2248 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/exegesis/particulate/text.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.578677 scs-core-2.4.6/src/scs_core/gas/
--rw-rw-r--   0 jade      (1002) jade      (1002)      292 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.578677 scs-core-2.4.6/src/scs_core/gas/a4/
--rw-rw-r--   0 jade      (1002) jade      (1002)      410 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/a4/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3684 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/a4/a4.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     8774 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/a4/a4_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5667 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/a4/a4_calibrated_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4131 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/a4/a4_calibrated_datum_v1.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3932 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/a4/a4_calibrated_datum_vA.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5191 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/a4/a4_calibrated_datum_vB.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5557 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/a4/a4_calibrated_datum_vC.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4662 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/a4/a4_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6990 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/a4/a4_temp_comp.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.582677 scs-core-2.4.6/src/scs_core/gas/afe/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/afe/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1542 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/afe/afe_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3242 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/afe/pt1000_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2445 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/afe/pt1000_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3600 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/afe_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    11350 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/afe_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6742 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/afe_id.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.582677 scs-core-2.4.6/src/scs_core/gas/d4/
--rw-rw-r--   0 jade      (1002) jade      (1002)      130 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/d4/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3710 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/d4/d4_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2899 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/dsi_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4204 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/gas.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.582677 scs-core-2.4.6/src/scs_core/gas/isi/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/isi/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1373 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/isi/isi_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7366 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/gas/minimum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.582677 scs-core-2.4.6/src/scs_core/gas/ndir/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/ndir/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1777 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/ndir/ndir.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2723 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/ndir/ndir_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3350 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/ndir/ndir_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3649 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/ndir/ndir_version.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3065 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/ndir/ndir_voltages.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.582677 scs-core-2.4.6/src/scs_core/gas/pid/
--rw-rw-r--   0 jade      (1002) jade      (1002)      378 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/pid/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4106 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/pid/pid.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3889 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/pid/pid_calib.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4028 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/pid/pid_calibrated_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3730 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/pid/pid_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3694 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/pid/pid_temp_comp.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.582677 scs-core-2.4.6/src/scs_core/gas/scd30/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/scd30/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2538 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/scd30/scd30_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2804 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/scd30/scd30_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2866 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/scd30/scd30_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3588 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/sensor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6165 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/gas/sensor_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2852 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gas/sensor_calib.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.582677 scs-core-2.4.6/src/scs_core/gps/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gps/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4077 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/gps/gps_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.582677 scs-core-2.4.6/src/scs_core/interface/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/interface/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2271 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/interface/interface_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.582677 scs-core-2.4.6/src/scs_core/led/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/led/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      870 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/led/led.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2343 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/led/led_state.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.582677 scs-core-2.4.6/src/scs_core/location/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/location/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2992 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/location/timezone.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3710 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/location/timezone_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2379 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/location/timezone_offset.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.582677 scs-core-2.4.6/src/scs_core/model/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.582677 scs-core-2.4.6/src/scs_core/model/catalogue/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/catalogue/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    11042 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/model/catalogue/model_compendium.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4774 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/catalogue/model_compendium_group.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5220 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/catalogue/term.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2038 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/catalogue/training_period.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.586678 scs-core-2.4.6/src/scs_core/model/gas/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/gas/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3349 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/gas/baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1354 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/gas/gas_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1545 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/gas/gas_inference_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2932 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/gas/gas_model_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.586678 scs-core-2.4.6/src/scs_core/model/gas/s1/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/gas/s1/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2704 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/gas/s1/gas_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3344 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/gas/s1/s1_gas_inference_client.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.586678 scs-core-2.4.6/src/scs_core/model/gas/vB/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/gas/vB/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2702 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/gas/vB/gas_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3120 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/gas/vB/vb_gas_inference_client.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.586678 scs-core-2.4.6/src/scs_core/model/gas/vE/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/gas/vE/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3535 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/gas/vE/gas_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4409 2022-10-03 10:46:58.000000 scs-core-2.4.6/src/scs_core/model/gas/vE/ve_gas_inference_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1218 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/gas/vcal_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3488 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/model/model_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.586678 scs-core-2.4.6/src/scs_core/model/pmx/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/pmx/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1549 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/pmx/pmx_inference_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1609 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/pmx/pmx_model_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.586678 scs-core-2.4.6/src/scs_core/model/pmx/s1/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/pmx/s1/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2215 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/pmx/s1/pmx_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2051 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.586678 scs-core-2.4.6/src/scs_core/monitor/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/monitor/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1558 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/monitor/monitor_error.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1557 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/monitor/monitor_request.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1395 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/monitor/monitor_response.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.586678 scs-core-2.4.6/src/scs_core/osio/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/__init__.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.586678 scs-core-2.4.6/src/scs_core/osio/client/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/client/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2101 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/client/api_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2755 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/client/client_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1777 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/client/client_exception.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1696 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/client/realtime_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4045 2022-11-09 12:09:25.000000 scs-core-2.4.6/src/scs_core/osio/client/rest_client.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.586678 scs-core-2.4.6/src/scs_core/osio/config/
--rw-rw-r--   0 jade      (1002) jade      (1002)      294 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/config/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4175 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/config/project.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1771 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/osio/config/project_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2528 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/config/project_source.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6328 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/config/project_topic.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.590678 scs-core-2.4.6/src/scs_core/osio/data/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1786 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/abstract_topic.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1629 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/derived_data.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3389 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/derived_topic.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4467 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/device.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3265 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/device_summary.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3548 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/device_topic.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1869 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/error.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2681 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/location.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2189 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/message.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1337 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/message_body.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2021 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/message_event.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2571 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/message_payload.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1498 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/message_response.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2619 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/message_tag.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2839 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/organisation.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2208 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/schema.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3050 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/topic.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2196 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/topic_contributor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2863 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/topic_info.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4500 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/topic_metadata.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3927 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/topic_stats.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3461 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/topic_summary.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3164 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/user.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3500 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/user_metadata.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3817 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/data/user_topic.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.590678 scs-core-2.4.6/src/scs_core/osio/manager/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/manager/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4395 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/manager/device_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2085 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/manager/message_event_subscriber.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4936 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/manager/message_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3226 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/manager/organisation_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1353 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/manager/schema_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6882 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/osio/manager/topic_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2289 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/osio/manager/user_manager.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.590678 scs-core-2.4.6/src/scs_core/particulate/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/particulate/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4856 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/particulate/opc_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5142 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/particulate/opc_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2610 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/particulate/opc_version.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2103 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/particulate/pmx_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6405 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/particulate/sps_datum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.590678 scs-core-2.4.6/src/scs_core/position/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/position/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4062 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/position/gps_datum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.590678 scs-core-2.4.6/src/scs_core/position/nmea/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/position/nmea/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1578 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/position/nmea/gpdatetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4215 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/position/nmea/gpgga.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2685 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/position/nmea/gpgll.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3410 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/position/nmea/gpgsa.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3850 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/position/nmea/gpgsv.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2500 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/position/nmea/gploc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4056 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/position/nmea/gprmc.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1318 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/position/nmea/gptime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2685 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/position/nmea/gpvtg.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2535 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/position/nmea/nmea_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      782 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/position/nmea/nmea_sentence.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3884 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/position/position.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.590678 scs-core-2.4.6/src/scs_core/psu/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/psu/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2320 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/psu/psu.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4543 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/psu/psu_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1733 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/psu/psu_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1728 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/psu/psu_uptime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5663 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/psu/psu_version.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.590678 scs-core-2.4.6/src/scs_core/sample/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sample/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3421 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/sample/climate_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    12082 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/sample/configuration_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5262 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/sample/gases_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3724 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/sample/particulates_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2872 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/sample/pressure_sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4034 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/sample/sample.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5876 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/sample/status_sample.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.590678 scs-core-2.4.6/src/scs_core/sampler/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sampler/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1263 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sampler/sampler.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.594678 scs-core-2.4.6/src/scs_core/sync/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sync/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2168 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sync/interval_timer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1681 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sync/line_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      606 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sync/runner.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6819 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/sync/schedule.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1811 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sync/synchronised_process.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1724 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sync/timed_runner.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.594678 scs-core-2.4.6/src/scs_core/sys/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sys/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1791 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/sys/command.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4443 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sys/disk_usage.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5191 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sys/disk_volume.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2399 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sys/eeprom_image.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2622 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sys/exception_report.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6991 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/sys/filesystem.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4904 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/sys/http_exception.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      497 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/sys/http_status.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1994 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sys/ipv4_address.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1167 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/sys/logging.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1297 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/sys/memory.py
--rw-rw-r--   0 jade      (1002) jade      (1002)    17409 2022-09-20 10:07:36.000000 scs-core-2.4.6/src/scs_core/sys/modem.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5733 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sys/network.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6095 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/sys/node.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3851 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sys/persistence_manager.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2318 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/sys/platform.py
--rw-rw-r--   0 jade      (1002) jade      (1002)      834 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sys/process_comms.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4919 2022-09-20 10:07:36.000000 scs-core-2.4.6/src/scs_core/sys/ps_datum.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3284 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sys/serial.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2405 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sys/shared_secret.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2506 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sys/signalled_exit.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2244 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sys/subprocess.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5663 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sys/system_id.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1951 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sys/system_temp.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6610 2023-03-20 10:12:25.000000 scs-core-2.4.6/src/scs_core/sys/tail.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1409 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sys/timeout.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1192 2023-02-06 14:01:57.000000 scs-core-2.4.6/src/scs_core/sys/timer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1784 2022-08-17 09:53:27.000000 scs-core-2.4.6/src/scs_core/sys/trace_entry.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5602 2022-09-20 10:07:36.000000 scs-core-2.4.6/src/scs_core/sys/uptime_datum.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-03-20 10:15:26.562677 scs-core-2.4.6/src/scs_core.egg-info/
--rw-rw-r--   0 jade      (1002) jade      (1002)     1027 2023-03-20 10:15:26.000000 scs-core-2.4.6/src/scs_core.egg-info/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)    14587 2023-03-20 10:15:26.000000 scs-core-2.4.6/src/scs_core.egg-info/SOURCES.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-03-20 10:15:26.000000 scs-core-2.4.6/src/scs_core.egg-info/dependency_links.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)      124 2023-03-20 10:15:26.000000 scs-core-2.4.6/src/scs_core.egg-info/requires.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)        9 2023-03-20 10:15:26.000000 scs-core-2.4.6/src/scs_core.egg-info/top_level.txt
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.050926 scs-core-2.8.1/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:27.000000 scs-core-2.8.1/LICENSE
+-rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:27.000000 scs-core-2.8.1/MANIFEST.in
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2059 2023-06-26 09:34:13.050926 scs-core-2.8.1/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1404 2023-06-26 09:33:48.000000 scs-core-2.8.1/README.md
+-rw-rw-r--   0 jade      (1002) jade      (1002)       41 2022-08-17 09:53:27.000000 scs-core-2.8.1/README.rst
+-rw-rw-r--   0 jade      (1002) jade      (1002)      124 2023-02-06 14:01:57.000000 scs-core-2.8.1/requirements.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-06-26 09:34:13.050926 scs-core-2.8.1/setup.cfg
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1996 2022-08-17 09:53:27.000000 scs-core-2.8.1/setup.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.010926 scs-core-2.8.1/src/
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.014926 scs-core-2.8.1/src/scs_core/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      183 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.014926 scs-core-2.8.1/src/scs_core/aqcsv/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.018926 scs-core-2.8.1/src/scs_core/aqcsv/conf/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/conf/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2617 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/conf/airnow_site_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1034 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/conf/airnow_uploader_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.018926 scs-core-2.8.1/src/scs_core/aqcsv/connector/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/connector/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10203 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/aqcsv/connector/airnow_mapping_task.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6655 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/connector/datum_mapping.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5042 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/connector/source_mapping.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.018926 scs-core-2.8.1/src/scs_core/aqcsv/data/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/data/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3750 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/data/aqcsv_datetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    13723 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/data/aqcsv_record.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3033 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/data/aqcsv_site.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.018926 scs-core-2.8.1/src/scs_core/aqcsv/specification/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2824 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/agency.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2728 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/country.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1163 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/country_iso.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1175 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/country_numeric.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9800 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/method.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3765 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/mpc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3453 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/parameter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2855 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/qc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3732 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/qualifier.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2879 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aqcsv/specification/unit.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.018926 scs-core-2.8.1/src/scs_core/aws/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.018926 scs-core-2.8.1/src/scs_core/aws/client/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/client/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3585 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/client/access_key.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2332 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/client/api_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2113 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/client/api_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1217 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/client/client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5103 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/client/client_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1281 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/client/device_control_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3294 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/client/email_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3361 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/client/monitor_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5891 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/aws/client/mqtt_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3856 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/client/rest_client.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.018926 scs-core-2.8.1/src/scs_core/aws/config/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/config/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      744 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/config/aws.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4471 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/aws/config/project.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.022926 scs-core-2.8.1/src/scs_core/aws/data/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/data/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    16736 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/data/alert.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9320 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/data/byline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1792 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/data/byline_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4640 2023-04-17 09:22:53.000000 scs-core-2.8.1/src/scs_core/aws/data/dataset.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3550 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/data/deployment.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3337 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/data/device_monitor_email_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    12653 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/data/device_monitor_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3313 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/data/device_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4032 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/aws/data/email_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2859 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/data/http_response.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3175 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/data/message.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1776 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/data/power_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1820 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/data/runtime_record.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1795 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/data/status_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2884 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/data/upload_interval.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1793 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/data/uptime_list.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.022926 scs-core-2.8.1/src/scs_core/aws/greengrass/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/greengrass/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1998 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/greengrass/aws_deployer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3017 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/aws/greengrass/aws_deployment_reporter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9610 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/greengrass/aws_group.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    16440 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/aws/greengrass/aws_group_configuration.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    11557 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/greengrass/aws_identity.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      440 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/greengrass/gg_errors.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.026926 scs-core-2.8.1/src/scs_core/aws/manager/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/manager/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8285 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/alert_specification_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7269 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/alert_status_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3950 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/byline_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7269 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/configuration_check_finder.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3256 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/configuration_check_requester.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10816 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/configuration_finder.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2248 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/device_monitor_specification_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1497 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/device_monitor_status_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10307 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/dynamo_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3551 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/manager/ec2_message_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6470 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/manager/lambda_bylines.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    15996 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/aws/manager/lambda_message_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    18045 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/aws/manager/s3_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4295 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/manager/sagemaker_model_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7802 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/manager/sagemaker_trial_manager.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.026926 scs-core-2.8.1/src/scs_core/aws/security/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/aws/security/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1372 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/access_key_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5114 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_client_credentials.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7498 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_device.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1527 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_device_creator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3111 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_device_finder.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1911 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_device_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10555 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_login_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2181 2023-04-17 09:22:53.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_membership.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2314 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_password_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    11499 2023-04-17 09:22:53.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_user.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3227 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_user_finder.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3540 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/cognito_user_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3175 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/device_whitelist_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1947 2023-04-17 09:22:53.000000 scs-core-2.8.1/src/scs_core/aws/security/opr_membership.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    22905 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/organisation.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9601 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/organisation_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1752 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/aws/security/path_filter.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.026926 scs-core-2.8.1/src/scs_core/client/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/client/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4470 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/client/http_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6933 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/client/http_exception.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      497 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/client/http_status.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2831 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/client/network.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1415 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/client/resource_unavailable_exception.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2638 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/client/sftp_client_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.030926 scs-core-2.8.1/src/scs_core/climate/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/climate/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1407 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/climate/absolute_humidity.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1418 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/climate/icp10101_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3081 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/climate/mpl115a2_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2911 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/climate/mpl115a2_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2290 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/climate/pressure_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2188 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/climate/pressure_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3156 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/climate/sht_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1844 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/climate/sht_datum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.030926 scs-core-2.8.1/src/scs_core/comms/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/comms/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3125 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/comms/mqtt_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2395 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/comms/uds_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1552 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/comms/uds_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2350 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/comms/uds_server.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1614 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/comms/uds_writer.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.030926 scs-core-2.8.1/src/scs_core/control/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/control/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4918 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/control/command.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4896 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/control/control_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3792 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/control/control_handler.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4737 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/control/control_receipt.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.030926 scs-core-2.8.1/src/scs_core/csv/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/csv/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1979 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/csv/csv_archive.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7484 2023-04-17 09:22:53.000000 scs-core-2.8.1/src/scs_core/csv/csv_dict.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5996 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/csv/csv_log.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8594 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/csv/csv_log_cursor_queue.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8574 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/csv/csv_log_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8240 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/csv/csv_logger.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3323 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/csv/csv_logger_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5347 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/csv/csv_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4503 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/csv/csv_writer.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.034926 scs-core-2.8.1/src/scs_core/data/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4802 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/aggregate.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1947 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/data/array_dict.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2415 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/average.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2158 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/categorical_regression.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8964 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/data/checkpoint_generator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1008 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/crc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2092 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/crypt.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    19704 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/data/datetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6448 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/data/datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2634 2023-04-17 09:22:53.000000 scs-core-2.8.1/src/scs_core/data/duplicates.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3809 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/data/histogram.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1747 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/interval.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5951 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/join.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    14204 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/data/json.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3274 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/lin_regress.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5364 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/linear_regression.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1372 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/low_pass_filter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1628 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/median_filter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1892 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/min_list.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5682 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/data/model_delta.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8334 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/data/path_dict.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1291 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/precision.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3466 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/publication.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4181 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/data/queue_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     8858 2023-04-17 09:22:53.000000 scs-core-2.8.1/src/scs_core/data/recurring_period.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1265 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/regression.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4348 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/data/rtc_datetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2249 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/data/sample_delta.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10713 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/stats.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1280 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/str.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7391 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/timedelta.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2185 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/data/tokens.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7456 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/data/topic_path.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.034926 scs-core-2.8.1/src/scs_core/display/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/display/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3786 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/display/display_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.034926 scs-core-2.8.1/src/scs_core/email/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/email/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2131 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/email/email_queue.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2420 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/email/email_queue_manager.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.034926 scs-core-2.8.1/src/scs_core/estate/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/estate/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6202 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/estate/baseline_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    33022 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/estate/configuration.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4521 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/estate/configuration_check.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5221 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/estate/git_pull.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3621 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/estate/git_pull_check.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6675 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/estate/mqtt_device_poller.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2450 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/estate/mqtt_peer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6563 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/estate/package_version.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.034926 scs-core-2.8.1/src/scs_core/exegesis/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/exegesis/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.034926 scs-core-2.8.1/src/scs_core/exegesis/gas/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/exegesis/gas/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      693 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/exegesis/gas/exegete_catalogue.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1345 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/exegesis/gas/exegete_collection.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.034926 scs-core-2.8.1/src/scs_core/exegesis/particulate/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/exegesis/particulate/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      701 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/exegesis/particulate/exegete_catalogue.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1353 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/exegesis/particulate/exegete_collection.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2248 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/exegesis/particulate/text.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/gas/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      292 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/gas/a4/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      410 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/a4/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3700 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/gas/a4/a4.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    10274 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/gas/a4/a4_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5667 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4131 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum_v1.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3932 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum_vA.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5191 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum_vB.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5557 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum_vC.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4662 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/a4/a4_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6990 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/a4/a4_temp_comp.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/gas/afe/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/afe/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1542 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/afe/afe_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3242 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/afe/pt1000_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2445 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/afe/pt1000_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3600 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/afe_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    11555 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/gas/afe_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6742 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/afe_id.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/gas/d4/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      130 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/d4/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3710 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/d4/d4_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3106 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/gas/dsi_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4204 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/gas.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/gas/isi/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/isi/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1373 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/isi/isi_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7366 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/gas/minimum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/gas/ndir/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/ndir/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1777 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/ndir/ndir.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2723 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/ndir/ndir_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3350 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/ndir/ndir_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3649 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/ndir/ndir_version.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3065 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/ndir/ndir_voltages.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/gas/pid/
+-rw-rw-r--   0 jade      (1002) jade      (1002)      378 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/pid/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4106 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/pid/pid.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4196 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/gas/pid/pid_calib.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4028 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/pid/pid_calibrated_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3730 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/pid/pid_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3694 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/pid/pid_temp_comp.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/gas/scd30/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/scd30/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2538 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/scd30/scd30_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2804 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/scd30/scd30_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2866 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gas/scd30/scd30_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3556 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/gas/sensor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6165 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/gas/sensor_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3043 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/gas/sensor_calib.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/gps/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gps/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4077 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/gps/gps_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/interface/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/interface/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2271 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/interface/interface_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/led/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/led/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      870 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/led/led.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2343 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/led/led_state.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.038926 scs-core-2.8.1/src/scs_core/location/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/location/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2992 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/location/timezone.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3708 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/location/timezone_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2379 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/location/timezone_offset.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/model/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/__init__.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/model/catalogue/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/catalogue/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    11042 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/model/catalogue/model_compendium.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4774 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/catalogue/model_compendium_group.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5220 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/catalogue/term.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2038 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/catalogue/training_period.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/model/gas/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3349 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1354 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/gas_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1545 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/gas_inference_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2932 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/gas_model_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/model/gas/s1/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/s1/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2704 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/s1/gas_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3344 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/s1/s1_gas_inference_client.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/model/gas/vB/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/vB/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2702 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/vB/gas_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3120 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/vB/vb_gas_inference_client.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/model/gas/vE/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/vE/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3535 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/vE/gas_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4409 2022-10-03 10:46:58.000000 scs-core-2.8.1/src/scs_core/model/gas/vE/ve_gas_inference_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1218 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/gas/vcal_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3488 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/model/model_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/model/pmx/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/pmx/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1549 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/pmx/pmx_inference_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1609 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/pmx/pmx_model_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/model/pmx/s1/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/pmx/s1/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2215 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/pmx/s1/pmx_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2051 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/monitor/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/monitor/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1558 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/monitor/monitor_error.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1557 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/monitor/monitor_request.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1395 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/monitor/monitor_response.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/particulate/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/particulate/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4558 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/particulate/opc_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5142 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/particulate/opc_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2610 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/particulate/opc_version.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2103 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/particulate/pmx_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6405 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/particulate/sps_datum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/position/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4062 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/position/gps_datum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.042925 scs-core-2.8.1/src/scs_core/position/nmea/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1578 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/gpdatetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4215 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/gpgga.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2685 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/gpgll.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3410 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/gpgsa.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3850 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/gpgsv.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2500 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/gploc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4056 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/gprmc.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1318 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/gptime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2685 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/gpvtg.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2535 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/nmea_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      782 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/position/nmea/nmea_sentence.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3884 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/position/position.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.046925 scs-core-2.8.1/src/scs_core/psu/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/psu/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2320 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/psu/psu.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4543 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/psu/psu_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1733 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/psu/psu_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1728 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/psu/psu_uptime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5663 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/psu/psu_version.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.046925 scs-core-2.8.1/src/scs_core/sample/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sample/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3421 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/sample/climate_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    12029 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/sample/configuration_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5262 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/sample/gases_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3724 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/sample/particulates_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2872 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/sample/pressure_sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4034 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/sample/sample.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5876 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/sample/status_sample.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.046925 scs-core-2.8.1/src/scs_core/sampler/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sampler/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1263 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sampler/sampler.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.046925 scs-core-2.8.1/src/scs_core/sync/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sync/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2168 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sync/interval_timer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1681 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sync/line_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      606 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sync/runner.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6819 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/sync/schedule.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1811 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sync/synchronised_process.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1724 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sync/timed_runner.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.050926 scs-core-2.8.1/src/scs_core/sys/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1791 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/sys/command.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4443 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/disk_usage.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5191 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/disk_volume.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2399 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/eeprom_image.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2622 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/exception_report.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6991 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/sys/filesystem.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1994 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/ipv4_address.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1167 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/sys/logging.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1297 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/sys/memory.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)    17409 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/sys/modem.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5733 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/network.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5974 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/sys/node.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3851 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/persistence_manager.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2318 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/sys/platform.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)      834 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/process_comms.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4919 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/sys/ps_datum.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3284 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/serial.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2405 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/shared_secret.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2506 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/signalled_exit.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2244 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/subprocess.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5730 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/sys/system_id.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2013 2023-06-26 09:33:48.000000 scs-core-2.8.1/src/scs_core/sys/system_temp.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6610 2023-03-20 10:12:25.000000 scs-core-2.8.1/src/scs_core/sys/tail.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1409 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/timeout.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1192 2023-02-06 14:01:57.000000 scs-core-2.8.1/src/scs_core/sys/timer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1784 2022-08-17 09:53:27.000000 scs-core-2.8.1/src/scs_core/sys/trace_entry.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5602 2022-09-20 10:07:36.000000 scs-core-2.8.1/src/scs_core/sys/uptime_datum.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:34:13.014926 scs-core-2.8.1/src/scs_core.egg-info/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2059 2023-06-26 09:34:12.000000 scs-core-2.8.1/src/scs_core.egg-info/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)    13337 2023-06-26 09:34:13.000000 scs-core-2.8.1/src/scs_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-06-26 09:34:12.000000 scs-core-2.8.1/src/scs_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)      124 2023-06-26 09:34:12.000000 scs-core-2.8.1/src/scs_core.egg-info/requires.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)        9 2023-06-26 09:34:12.000000 scs-core-2.8.1/src/scs_core.egg-info/top_level.txt
```

### Comparing `scs-core-2.4.6/LICENSE` & `scs-core-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/setup.py` & `scs-core-2.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aqcsv/conf/airnow_site_conf.py` & `scs-core-2.8.1/src/scs_core/aqcsv/conf/airnow_site_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aqcsv/conf/airnow_uploader_conf.py` & `scs-core-2.8.1/src/scs_core/aqcsv/conf/airnow_uploader_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aqcsv/connector/airnow_mapping_task.py` & `scs-core-2.8.1/src/scs_core/aqcsv/connector/airnow_mapping_task.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aqcsv/connector/datum_mapping.py` & `scs-core-2.8.1/src/scs_core/aqcsv/connector/datum_mapping.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aqcsv/connector/source_mapping.py` & `scs-core-2.8.1/src/scs_core/aqcsv/connector/source_mapping.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aqcsv/data/aqcsv_datetime.py` & `scs-core-2.8.1/src/scs_core/aqcsv/data/aqcsv_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aqcsv/data/aqcsv_record.py` & `scs-core-2.8.1/src/scs_core/aqcsv/data/aqcsv_record.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aqcsv/data/aqcsv_site.py` & `scs-core-2.8.1/src/scs_core/aqcsv/data/aqcsv_site.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aqcsv/specification/agency.py` & `scs-core-2.8.1/src/scs_core/aqcsv/specification/agency.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aqcsv/specification/country.py` & `scs-core-2.8.1/src/scs_core/aqcsv/specification/country.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aqcsv/specification/country_iso.py` & `scs-core-2.8.1/src/scs_core/aqcsv/specification/country_iso.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aqcsv/specification/country_numeric.py` & `scs-core-2.8.1/src/scs_core/aqcsv/specification/country_numeric.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aqcsv/specification/method.py` & `scs-core-2.8.1/src/scs_core/aqcsv/specification/method.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aqcsv/specification/mpc.py` & `scs-core-2.8.1/src/scs_core/aqcsv/specification/mpc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aqcsv/specification/parameter.py` & `scs-core-2.8.1/src/scs_core/aqcsv/specification/parameter.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aqcsv/specification/qc.py` & `scs-core-2.8.1/src/scs_core/aqcsv/specification/qc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aqcsv/specification/qualifier.py` & `scs-core-2.8.1/src/scs_core/aqcsv/specification/qualifier.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aqcsv/specification/unit.py` & `scs-core-2.8.1/src/scs_core/aqcsv/specification/unit.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/client/access_key.py` & `scs-core-2.8.1/src/scs_core/aws/client/access_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """
 Created on 16 Oct 2020
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 https://stackoverflow.com/questions/2520893/how-to-flush-the-input-stream-in-python
+
+document example:
+{"key-id": "ABC", "secret-key": "123"}
 """
 
 import json
 import os
 import sys
 import termios
 
@@ -50,15 +53,15 @@
 
         return cls(id, secret)
 
 
     @classmethod
     def from_user(cls):
         try:
-            termios.tcflush(sys.stdin, termios.TCIOFLUSH)  # flush stdin
+            termios.tcflush(sys.stdin, termios.TCIOFLUSH)           # flush stdin
         except termios.error:
             pass
 
         print("Enter AWS Access Key ID: ", end="", file=sys.stderr)
         id = input().strip()
 
         print("Enter AWS Secret Access Key: ", end="", file=sys.stderr)
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/client/api_auth.py` & `scs-core-2.8.1/src/scs_core/aws/client/api_auth.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/client/client.py` & `scs-core-2.8.1/src/scs_core/aws/client/client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/client/client_auth.py` & `scs-core-2.8.1/src/scs_core/aws/client/client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/client/email_client.py` & `scs-core-2.8.1/src/scs_core/aws/client/email_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/client/monitor_auth.py` & `scs-core-2.8.1/src/scs_core/aws/client/monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/client/mqtt_client.py` & `scs-core-2.8.1/src/scs_core/aws/client/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/client/rest_client.py` & `scs-core-2.8.1/src/scs_core/aws/client/rest_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,17 +13,16 @@
 """
 
 import json
 
 from scs_core.data.json import JSONify
 
 from scs_core.client.http_client import HTTPClient
-
-from scs_core.sys.http_exception import HTTPException
-from scs_core.sys.http_status import HTTPStatus
+from scs_core.client.http_exception import HTTPException
+from scs_core.client.http_status import HTTPStatus
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class RESTClient(object):
     """
     classdocs
@@ -58,23 +57,23 @@
         # print("RESTClient.get: path: %s params: %s headers:%s" % (path, params, self.__headers), file=sys.stderr)
 
         try:
             response_jstr = self.__http_client.get(path, params, self.__headers)
             # print("response_jstr: %s" % response_jstr, file=sys.stderr)
             # print("-", file=sys.stderr)
 
-        except HTTPException as exc:
+        except HTTPException as ex:
             # print("exc: %s" % exc, file=sys.stderr)
             # print("-", file=sys.stderr)
 
-            if exc.status == HTTPStatus.NOT_FOUND:
+            if ex.status == HTTPStatus.NOT_FOUND:
                 return None
 
             else:
-                raise exc
+                raise ex
 
         try:
             response = json.loads(response_jstr)
         except ValueError:
             response = None
 
         return response
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/config/aws.py` & `scs-core-2.8.1/src/scs_core/aws/config/aws.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/config/project.py` & `scs-core-2.8.1/src/scs_core/aws/config/project.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/data/alert.py` & `scs-core-2.8.1/src/scs_core/aws/data/alert.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 """
 Created on 17 Jun 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 Alert example:
-{"id": 77, "topic": "south-coast-science-dev/development/loc/1/gases", "field": "val.CO.cnc", "lower-threshold": null,
-"upper-threshold": 1000.0, "alert-on-none": true, "aggregation-period": {"interval": 1, "units": "M"},
-"test-interval": null, "creator-email-address": "authorization@southcoastscience.com",
-"to": "someone@me.com", "cc-list": [], "suspended": false}
+{"id": 88, "description": "warm", "topic": "south-coast-science-dev/development/loc/1/climate", "field": "val.tmp",
+"lower-threshold": null, "upper-threshold": 30.0, "alert-on-none": false,
+"aggregation-period": {"interval": 1, "units": "M"}, "test-interval": null, "json-message": false,
+"creator-email-address": "bruno.beloff@southcoastscience.com", "to": "bruno.beloff@southcoastscience.com",
+"cc-list": ["bbeloff@me.com", "jadempage@outlook.com"], "suspended": false}
 
 AlertStatus example:
-{"id": 77, "rec": "2021-09-07T11:40:00Z", "cause": null, "val": 589.6}
+{"id": 77, "rec": "2021-09-07T11:40:00Z", "cause": "OK", "val": 589.6}
 
 https://martinstapel.com/how-to-autoincrement-in-dynamo-db-if-you-really-need-to/
 https://stackoverflow.com/questions/37072341/how-to-use-auto-increment-for-primary-key-id-in-dynamodb
 """
 
 from collections import OrderedDict
 
-from scs_core.data.recurring_period import RecurringPeriod
 from scs_core.data.datetime import LocalizedDatetime
 from scs_core.data.datum import Datum
-from scs_core.data.json import JSONable
+from scs_core.data.json import JSONable, JSONify
+from scs_core.data.recurring_period import RecurringPeriod
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class AlertStatus(JSONable):
     """
     classdocs
     """
 
     BELOW_LOWER_THRESHOLD =     '<L'
     ABOVE_UPPER_THRESHOLD =     '>U'
     NULL_VALUE =                'NV'
-
+    OK =                        'OK'
 
     @classmethod
     def causes(cls):
-        return cls.BELOW_LOWER_THRESHOLD, cls.ABOVE_UPPER_THRESHOLD, cls.NULL_VALUE
+        return cls.BELOW_LOWER_THRESHOLD, cls.ABOVE_UPPER_THRESHOLD, cls.NULL_VALUE, cls.OK
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def construct_from_jdict(cls, jdict):
         if not jdict:
@@ -85,15 +86,15 @@
 
         return False
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_excursion(self):
-        return self.cause is not None
+        return self.cause != 'OK'
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         jdict = OrderedDict()
 
@@ -147,70 +148,84 @@
     @classmethod
     def construct_from_jdict(cls, jdict):
         if not jdict:
             return None
 
         id = jdict.get('id')
 
+        description = jdict.get('description', '')
+
         topic = jdict.get('topic')
         field = jdict.get('field')
 
         lower_threshold = jdict.get('lower-threshold')
         upper_threshold = jdict.get('upper-threshold')
         alert_on_none = jdict.get('alert-on-none')
 
         aggregation_period = RecurringPeriod.construct_from_jdict(jdict.get('aggregation-period'))
         test_interval = RecurringPeriod.construct_from_jdict(jdict.get('test-interval'))
 
+        json_message = jdict.get('json-message', False)
+
         creator_email_address = jdict.get('creator-email-address')
 
         to = jdict.get('to')
-        cc_list = jdict.get('cc-list')
+        cc_list = set(jdict.get('cc-list', []))
         suspended = jdict.get('suspended')
 
-        return cls(id, topic, field, lower_threshold, upper_threshold, alert_on_none,
-                   aggregation_period, test_interval, creator_email_address, to, cc_list, suspended)
+        return cls(id, description, topic, field, lower_threshold, upper_threshold, alert_on_none,
+                   aggregation_period, test_interval, json_message, creator_email_address, to, cc_list, suspended)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, id, topic, field, lower_threshold, upper_threshold, alert_on_none,
-                 aggregation_period, test_interval, creator_email_address, to, cc_list, suspended):
+    def __init__(self, id, description, topic, field, lower_threshold, upper_threshold, alert_on_none,
+                 aggregation_period, test_interval, json_message, creator_email_address, to, cc_list, suspended):
         """
         Constructor
         """
         self.__id = Datum.int(id)                                   # int
 
+        self.__description = description                            # string
+
         self.__topic = topic                                        # string topic
         self.__field = field                                        # string path
 
         self.__lower_threshold = Datum.float(lower_threshold)       # float                 updatable
         self.__upper_threshold = Datum.float(upper_threshold)       # float                 updatable
         self.__alert_on_none = bool(alert_on_none)                  # bool                  updatable
 
         self.__aggregation_period = aggregation_period              # RecurringPeriod       updatable
         self.__test_interval = test_interval                        # RecurringPeriod       updatable
 
+        self.__json_message = bool(json_message)                    # bool
+
         self.__creator_email_address = creator_email_address        # string
 
         self.__to = to                                              # string                updatable
-        self.__cc_list = cc_list                                    # array of string       updatable
+        self.__cc_list = cc_list                                    # set of string         updatable
         self.__suspended = bool(suspended)                          # bool                  updatable
 
 
     def __lt__(self, other):
         if self.topic < other.topic:
             return True
 
         if self.topic > other.topic:
             return False
 
         if self.field < other.field:
             return True
 
+        if self.description > other.description:
+            return False
+
+        if self.description < other.description:
+            return True
+
         if self.field > other.field:
             return False
 
         if self.creator_email_address < other.creator_email_address:
             return True
 
         if self.creator_email_address > other.creator_email_address:
@@ -224,16 +239,15 @@
 
         return False
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.topic is None or self.field is None or self.aggregation_period is None or \
-                self.creator_email_address is None or self.to is None:
+        if self.topic is None or self.field is None or self.aggregation_period is None or self.to is None:
             return False
 
         if not self.has_trigger():
             return False
 
         if not self.has_valid_thresholds():
             return False
@@ -309,32 +323,51 @@
 
 
     def end_datetime(self, origin: LocalizedDatetime):
         return self.aggregation_period.end_datetime(origin)
         # return self.test_interval.end_datetime(origin) if self.test_interval else \
         #     self.aggregation_period.end_datetime(origin)
 
+
+    # ----------------------------------------------------------------------------------------------------------------
+
+    def add_cc(self, cc):
+        self.__cc_list.add(cc)
+
+
+    def remove_cc(self, cc):
+        try:
+            self.__cc_list.remove(cc)
+        except KeyError:
+            pass
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         jdict = OrderedDict()
 
         jdict['id'] = self.id
 
+        jdict['description'] = self.description
+
         jdict['topic'] = self.topic
         jdict['field'] = self.field
 
         jdict['lower-threshold'] = self.lower_threshold
         jdict['upper-threshold'] = self.upper_threshold
         jdict['alert-on-none'] = self.alert_on_none
 
         jdict['aggregation-period'] = self.aggregation_period.as_json()
         jdict['test-interval'] = None if self.test_interval is None else self.test_interval.as_json()
 
-        jdict['creator-email-address'] = self.creator_email_address
+        jdict['json-message'] = self.json_message
+
+        if self.creator_email_address is not None:
+            jdict['creator-email-address'] = self.creator_email_address
 
         jdict['to'] = self.to
         jdict['cc-list'] = self.cc_list
         jdict['suspended'] = self.suspended
 
         return jdict
 
@@ -343,14 +376,19 @@
 
     @property
     def id(self):
         return self.__id
 
 
     @property
+    def description(self):
+        return self.__description
+
+
+    @property
     def topic(self):
         return self.__topic
 
 
     @property
     def field(self):
         return self.__field
@@ -378,26 +416,36 @@
 
     @property
     def test_interval(self):
         return self.__test_interval
 
 
     @property
+    def json_message(self):
+        return self.__json_message
+
+
+    @property
     def creator_email_address(self):
         return self.__creator_email_address
 
 
+    @creator_email_address.setter
+    def creator_email_address(self, creator_email_address):
+        self.__creator_email_address = creator_email_address
+
+
     @property
     def to(self):
         return self.__to
 
 
     @property
     def cc_list(self):
-        return self.__cc_list
+        return sorted(self.__cc_list)
 
 
     @property
     def suspended(self):
         return self.__suspended
 
 
@@ -421,13 +469,79 @@
 
         self.__cc_list.remove(cc)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "AlertSpecification:{id:%s, topic:%s, field:%s, lower_threshold:%s, upper_threshold:%s, " \
-               "alert_on_none:%s, aggregation_period:%s, test_interval:%s, creator_email_address:%s, " \
-               "to:%s, cc_list:%s, suspended:%s}" %  \
-               (self.id, self.topic, self.field, self.lower_threshold, self.upper_threshold,
-                self.alert_on_none, self.aggregation_period, self.test_interval, self.creator_email_address,
-                self.to, self.cc_list, self.suspended)
+        return "AlertSpecification:{id:%s, description:%s, topic:%s, field:%s, lower_threshold:%s, " \
+               "upper_threshold:%s, alert_on_none:%s, aggregation_period:%s, test_interval:%s, " \
+               "json_message:%s, creator_email_address:%s, to:%s, cc_list:%s, suspended:%s}" %  \
+               (self.id, self.description, self.topic, self.field, self.lower_threshold,
+                self.upper_threshold, self.alert_on_none, self.aggregation_period, self.test_interval,
+                self.json_message, self.creator_email_address, self.to, self.__cc_list, self.suspended)
+
+
+# --------------------------------------------------------------------------------------------------------------------
+
+class AlertMessage(JSONable):
+    """
+    classdocs
+    """
+
+    # ----------------------------------------------------------------------------------------------------------------
+
+    @classmethod
+    def construct_from_jdict(cls, jdict):
+        if not jdict:
+            return None
+
+        alert_specification = AlertSpecification.construct_from_jdict(jdict.get('specification'))
+        alert_status = AlertStatus.construct_from_jdict(jdict.get('status'))
+
+        return cls(alert_specification, alert_status)
+
+
+    # ----------------------------------------------------------------------------------------------------------------
+
+    def __init__(self, alert_specification: AlertSpecification, alert_status: AlertStatus):
+        """
+        Constructor
+        """
+        self.__alert_specification = alert_specification                    # AlertSpecification
+        self.__alert_status = alert_status                                  # AlertStatus
+
+
+    # ----------------------------------------------------------------------------------------------------------------
+
+    def as_json(self):
+        jdict = OrderedDict()
+
+        jdict['specification'] = self.alert_specification
+        jdict['status'] = self.alert_status
+
+        return jdict
+
+
+    # ----------------------------------------------------------------------------------------------------------------
+
+    def subject(self):
+        return JSONify.dumps(self.alert_status)
+
+
+    # ----------------------------------------------------------------------------------------------------------------
+
+    @property
+    def alert_specification(self):
+        return self.__alert_specification
+
+
+    @property
+    def alert_status(self):
+        return self.__alert_status
+
+
+    # ----------------------------------------------------------------------------------------------------------------
+
+    def __str__(self, *args, **kwargs):
+        return "AlertMessage:{alert_specification:%s, alert_status:%s}" %  \
+               (self.alert_specification, self.alert_status)
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/data/byline.py` & `scs-core-2.8.1/src/scs_core/aws/data/byline.py`

 * *Files 3% similar despite different names*

```diff
@@ -187,15 +187,25 @@
 
     def __len__(self):
         return len(list(self.bylines))
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def latest_topic(self, suffix):
+    def latest_byline(self, suffix=''):
+        latest_byline = None
+
+        for byline in self.bylines:
+            if byline.topic.endswith(suffix) and (latest_byline is None or byline.rec > latest_byline.rec):
+                latest_byline = byline
+
+        return latest_byline
+
+
+    def latest_topic(self, suffix=''):
         latest_rec = None
         topic = None
 
         for byline in self.bylines:
             if byline.topic.endswith(suffix) and (latest_rec is None or byline.rec > latest_rec):
                 latest_rec = byline.rec
                 topic = byline.topic
@@ -255,15 +265,15 @@
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def device(self):
         for device in self._device_bylines.keys():
-            return device                                       # return the first device
+            return device                                       # return the first device tag
 
         return None
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class TopicBylineGroup(BylineGroup):
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/data/byline_list.py` & `scs-core-2.8.1/src/scs_core/aws/data/byline_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/data/dataset.py` & `scs-core-2.8.1/src/scs_core/aws/data/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,24 +84,27 @@
 
 
     def extend(self, items):
         for item in items:
             self.add(item)
 
 
-    def update_with(self, item: DatasetItem):
+    def update_with(self, item: DatasetItem, insert_only=False):
         try:
             retrieved_item = self.__items[item.index]
 
+            if insert_only:
+                return
+
             # no changes...
             if item == retrieved_item:
                 return
 
             # AWS item is newer - ignore old-world item...
-            if retrieved_item.last_updated > self.latest_import:
+            if self.latest_import and retrieved_item.last_updated > self.latest_import:
                 self.__logger.info('WARNING: old-world item ignored: %s' % item)
                 return
 
             # old-world item is newer...
             item.copy_pk(retrieved_item)
 
             if not self.simulate:
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/data/deployment.py` & `scs-core-2.8.1/src/scs_core/aws/data/deployment.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/data/device_report.py` & `scs-core-2.8.1/src/scs_core/aws/data/device_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 
 from collections import OrderedDict
 
 from scs_core.data.json import JSONable
 
 
+# TODO: delete this class
 # --------------------------------------------------------------------------------------------------------------------
 
 class DeviceReport(JSONable):
 
     @classmethod
     def construct_from_jdict(cls, jdict):
         if not jdict:
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/data/email_list.py` & `scs-core-2.8.1/src/scs_core/aws/data/email_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/data/http_response.py` & `scs-core-2.8.1/src/scs_core/aws/data/http_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 https://docs.python.org/3/library/http.html
 https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS
 """
 
 from abc import ABC
 from http import HTTPStatus
 
+from scs_core.client.http_exception import HTTPException
 from scs_core.data.json import JSONable, JSONify
 
-from scs_core.sys.http_exception import HTTPException
-
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class HTTPResponse(JSONable, ABC):
     """
     classdocs
     """
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/data/message.py` & `scs-core-2.8.1/src/scs_core/aws/data/message.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/data/power_list.py` & `scs-core-2.8.1/src/scs_core/aws/data/power_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/data/runtime_record.py` & `scs-core-2.8.1/src/scs_core/aws/data/runtime_record.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/data/status_list.py` & `scs-core-2.8.1/src/scs_core/aws/data/status_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/data/upload_interval.py` & `scs-core-2.8.1/src/scs_core/aws/data/upload_interval.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/data/uptime_list.py` & `scs-core-2.8.1/src/scs_core/aws/data/uptime_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/greengrass/aws_deployer.py` & `scs-core-2.8.1/src/scs_core/aws/greengrass/aws_deployer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/greengrass/aws_deployment_reporter.py` & `scs-core-2.8.1/src/scs_core/aws/greengrass/aws_deployment_reporter.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/greengrass/aws_group.py` & `scs-core-2.8.1/src/scs_core/aws/greengrass/aws_group.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/greengrass/aws_group_configuration.py` & `scs-core-2.8.1/src/scs_core/aws/greengrass/aws_group_configuration.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/greengrass/aws_identity.py` & `scs-core-2.8.1/src/scs_core/aws/greengrass/aws_identity.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/manager/alert_specification_manager.py` & `scs-core-2.8.1/src/scs_core/aws/manager/alert_specification_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,122 +3,127 @@
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 from collections import OrderedDict
 from http import HTTPStatus
 
+from scs_core.aws.client.api_client import APIClient
 from scs_core.aws.data.alert import AlertSpecification
 from scs_core.aws.data.http_response import HTTPResponse
 
-from scs_core.data.str import Str
+from scs_core.client.http_exception import HTTPException
 
-from scs_core.sys.http_exception import HTTPException
+from scs_core.data.str import Str
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class AlertSpecificationManager(object):
+class AlertSpecificationManager(APIClient):
     """
     classdocs
     """
 
     __URL = "https://a066wbide8.execute-api.us-west-2.amazonaws.com/default/AlertSpecification"
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, http_client, auth):
-        self.__http_client = http_client                # requests package
-        self.__auth = auth
+    def __init__(self, http_client):
+        super().__init__(http_client)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def find(self, topic_filter, path_filter, creator_filter):
-        request = AlertSpecificationManagerRequest(topic_filter, path_filter, creator_filter)
-        headers = {'Authorization': self.__auth.email_address}
+    def find(self, token, description_filter, topic_filter, path_filter, creator_filter):
+        request = AlertSpecificationFindRequest(description_filter, topic_filter, path_filter, creator_filter)
 
-        response = self.__http_client.get(self.__URL, headers=headers, params=request.params())
+        response = self._http_client.get(self.__URL, headers=self._token_headers(token), params=request.params())
+        self._check_response(response)
 
-        return AlertSpecificationManagerResponse.construct_from_jdict(response.json())
+        return AlertSpecificationFindResponse.construct_from_jdict(response.json())
 
 
-    def retrieve(self, id):
+    def retrieve(self, token, id):
         url = '/'.join((self.__URL, str(id)))
-        headers = {'Authorization': self.__auth.email_address}
 
-        http_response = self.__http_client.get(url, headers=headers)
-        response = AlertSpecificationManagerResponse.construct_from_jdict(http_response.json())
+        http_response = self._http_client.get(url, headers=self._token_headers(token))
+        self._check_response(http_response)
+
+        response = AlertSpecificationFindResponse.construct_from_jdict(http_response.json())
 
         return response.alerts[0] if response.alerts else None
 
 
-    def create(self, alert):
-        headers = {'Authorization': self.__auth.email_address}
+    def create(self, token, alert):
+        http_response = self._http_client.post(self.__URL, headers=self._token_headers(token), json=alert.as_json())
+        self._check_response(http_response)
 
-        http_response = self.__http_client.post(self.__URL, headers=headers, json=alert.as_json())
-        response = AlertSpecificationManagerResponse.construct_from_jdict(http_response.json())
+        response = AlertSpecificationFindResponse.construct_from_jdict(http_response.json())
 
         return response.alerts[0] if response.alerts else None
 
 
-    def update(self, alert):
+    def update(self, token, alert):
         url = '/'.join((self.__URL, str(alert.id)))
-        headers = {'Authorization': self.__auth.email_address}
 
-        http_response = self.__http_client.post(url, headers=headers, json=alert.as_json())
-        response = AlertSpecificationManagerResponse.construct_from_jdict(http_response.json())
+        http_response = self._http_client.post(url, headers=self._token_headers(token), json=alert.as_json())
+        self._check_response(http_response)
+
+        response = AlertSpecificationFindResponse.construct_from_jdict(http_response.json())
 
         return response.alerts[0] if response.alerts else None
 
 
-    def delete(self, id):
+    def delete(self, token, id):
         url = '/'.join((self.__URL, str(id)))
-        headers = {'Authorization': self.__auth.email_address}
 
-        self.__http_client.delete(url, headers=headers)
+        http_response = self._http_client.delete(url, headers=self._token_headers(token))
+        self._check_response(http_response)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "AlertSpecificationManager:{auth:%s}" % self.__auth
+        return "AlertSpecificationManager:{}"
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class AlertSpecificationManagerRequest(object):
+class AlertSpecificationFindRequest(object):
     """
     classdocs
     """
 
+    DESCRIPTION_FILTER = 'description'
     TOPIC_FILTER = 'topic'
     PATH_FILTER = 'path'
     CREATOR_FILTER = 'creator'
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def construct_from_qsp(cls, qsp):
         if not qsp:
             return None
 
+        description_filter = qsp.get(cls.DESCRIPTION_FILTER)
         topic_filter = qsp.get(cls.TOPIC_FILTER)
         path_filter = qsp.get(cls.PATH_FILTER)
         creator_filter = qsp.get(cls.CREATOR_FILTER)
 
-        return cls(topic_filter, path_filter, creator_filter)
+        return cls(description_filter, topic_filter, path_filter, creator_filter)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, topic_filter, path_filter, creator_filter):
+    def __init__(self, description_filter, topic_filter, path_filter, creator_filter):
         """
         Constructor
         """
+        self.__description_filter = description_filter              # string
         self.__topic_filter = topic_filter                          # string
         self.__path_filter = path_filter                            # string
         self.__creator_filter = creator_filter                      # string
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
@@ -126,26 +131,34 @@
     def is_valid(cls):
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def params(self):
+        description_filter = self.description_filter if self.description_filter else None
+
         params = {
+            self.DESCRIPTION_FILTER: description_filter,
             self.TOPIC_FILTER: self.topic_filter,
             self.PATH_FILTER: self.path_filter,
             self.CREATOR_FILTER: self.creator_filter
         }
 
         return params
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
+    def description_filter(self):
+        return self.__description_filter
+
+
+    @property
     def topic_filter(self):
         return self.__topic_filter
 
 
     @property
     def path_filter(self):
         return self.__path_filter
@@ -155,21 +168,23 @@
     def creator_filter(self):
         return self.__creator_filter
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "AlertSpecificationManagerRequest:{topic_filter:%s, path_filter:%s, creator_filter:%s}" % \
-               (self.topic_filter, self.path_filter, self.creator_filter)
+        return "AlertSpecificationFindRequest:{description_filter:%s, topic_filter:%s, path_filter:%s, " \
+               "creator_filter:%s}" % \
+               (self.description_filter, self.topic_filter, self.path_filter,
+                self.creator_filter)
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class AlertSpecificationManagerResponse(HTTPResponse):
+class AlertSpecificationFindResponse(HTTPResponse):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
@@ -235,9 +250,9 @@
     def next_url(self):
         return self.__next_url
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "AlertSpecificationManagerResponse:{status:%s, alerts:%s, next_url:%s}" % \
+        return "AlertSpecificationFindResponse:{status:%s, alerts:%s, next_url:%s}" % \
                (self.status, Str.collection(self.alerts), self.next_url)
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/manager/alert_status_finder.py` & `scs-core-2.8.1/src/scs_core/aws/manager/alert_status_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,59 +4,66 @@
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 from collections import OrderedDict
 from enum import Enum
 from http import HTTPStatus
 
+from scs_core.aws.client.api_client import APIClient
 from scs_core.aws.data.alert import AlertStatus
 from scs_core.aws.data.http_response import HTTPResponse
 
+from scs_core.client.http_exception import HTTPException
+
 from scs_core.data.datum import Datum
 from scs_core.data.str import Str
 
-from scs_core.sys.http_exception import HTTPException
-
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class AlertStatusFinder(object):
+class AlertStatusManager(APIClient):
     """
     classdocs
     """
 
-    __URL = "https://nssnahspkj.execute-api.us-west-2.amazonaws.com/default/AlertHistoryLatestFinder"
+    __URL = "https://n0ctatmvjl.execute-api.us-west-2.amazonaws.com/default/AlertStatus"
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, http_client, auth):
-        self.__http_client = http_client                # requests package
-        self.__auth = auth
+    def __init__(self, http_client):
+        super().__init__(http_client)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def find(self, id_filter, cause_filter, response_mode):
-        request = AlertStatusFinderRequest(id_filter, cause_filter, response_mode)
-        headers = {'Authorization': self.__auth.email_address}
+    def find(self, token, id_filter, cause_filter, response_mode):
+        request = AlertStatusFindRequest(id_filter, cause_filter, response_mode)
+
+        response = self._http_client.get(self.__URL, headers=self._token_headers(token), params=request.params())
+        self._check_response(response)
+
+        return AlertStatusFindResponse.construct_from_jdict(response.json())
+
 
-        response = self.__http_client.get(self.__URL, headers=headers, params=request.params())
+    def delete(self, token, id):
+        url = '/'.join((self.__URL, str(id)))
 
-        return AlertStatusFinderResponse.construct_from_jdict(response.json())
+        http_response = self._http_client.delete(url, headers=self._token_headers(token))
+        self._check_response(http_response)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "AlertStatusFinder:{auth:%s}" % self.__auth
+        return "AlertStatusManager:{}"
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class AlertStatusFinderRequest(object):
+class AlertStatusFindRequest(object):
     """
     classdocs
     """
 
     class Mode(Enum):
         HISTORY = 1
         LATEST = 2
@@ -134,21 +141,21 @@
     def response_mode(self):
         return self.__response_mode
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "AlertStatusFinderRequest:{id_filter:%s, cause_filter:%s, response_mode:%s}" % \
+        return "AlertStatusFindRequest:{id_filter:%s, cause_filter:%s, response_mode:%s}" % \
                (self.id_filter, self.cause_filter, self.response_mode)
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class AlertStatusFinderResponse(HTTPResponse):
+class AlertStatusFindResponse(HTTPResponse):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
@@ -157,15 +164,15 @@
             return None
 
         status = HTTPStatus(jdict.get('statusCode'))
 
         if status != HTTPStatus.OK:
             raise HTTPException.construct(status.value, status.phrase, status.description)
 
-        mode = AlertStatusFinderRequest.Mode[jdict.get('mode')]
+        mode = AlertStatusFindRequest.Mode[jdict.get('mode')]
 
         alert_statuses = []
         if jdict.get('alert-statuses'):
             for alert_jdict in jdict.get('alert-statuses'):
                 alert_statuses.append(AlertStatus.construct_from_jdict(alert_jdict))
 
         next_url = jdict.get('next')
@@ -225,9 +232,9 @@
     def next_url(self):
         return self.__next_url
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "AlertStatusFinderResponse:{status:%s, mode:%s, alert_statuses:%s, next_url:%s}" % \
+        return "AlertStatusFindResponse:{status:%s, mode:%s, alert_statuses:%s, next_url:%s}" % \
                (self.status, self.mode, Str.collection(self.alert_statuses), self.next_url)
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/manager/byline_manager.py` & `scs-core-2.8.1/src/scs_core/aws/manager/byline_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,47 +6,46 @@
 Equivalent to cURLs:
 curl "https://aws.southcoastscience.com/device-topics?topic=south-coast-science-dev/alphasense/loc/303/gases"
 curl "https://aws.southcoastscience.com/device-topics?device=scs-bgx-303"
 """
 
 from urllib.parse import parse_qs, urlparse
 
+from scs_core.aws.client.api_client import APIClient
 from scs_core.aws.data.byline import Byline, DeviceBylineGroup, TopicBylineGroup
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class BylineManager(object):
+class BylineManager(APIClient):
     """
     classdocs
     """
 
     # __URL = 'https://aws.southcoastscience.com/device-topics'
     __URL = 'https://cxzne688y0.execute-api.us-west-2.amazonaws.com/default/Bylines'
 
     __DEVICE =      'device'
     __TOPIC =       'topic'
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, http_client, reporter=None):
-        """
-        Constructor
-        """
-        self.__http_client = http_client                        # requests package
+        super().__init__(http_client)
+
         self.__reporter = reporter                              # BatchDownloadReporter
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def find_latest_byline_for_topic(self, topic):
         params = {self.__TOPIC: topic}
 
-        response = self.__http_client.get(self.__URL, params=params)
+        response = self._http_client.get(self.__URL, params=params)
         jdict = response.json()
 
         # bylines...
         if jdict is None:
             return None
 
         latest_byline = None
@@ -61,15 +60,15 @@
 
 
     def find_bylines(self, excluded=None):
         params = {}
         items_jdict = []
 
         while True:
-            response = self.__http_client.get(self.__URL, params=params)
+            response = self._http_client.get(self.__URL, params=params)
             jdict = response.json()
 
             block = jdict.get('Items')
             items_jdict += block
 
             # report...
             if self.__reporter:
@@ -85,35 +84,41 @@
         # bylines...
         return TopicBylineGroup.construct_from_jdict(items_jdict, excluded=excluded, skeleton=True)
 
 
     def find_bylines_for_topic(self, topic, excluded=None):
         params = {self.__TOPIC: topic}
 
-        response = self.__http_client.get(self.__URL, params=params)
+        response = self._http_client.get(self.__URL, params=params)
+        self._check_response(response)
+
         jdict = response.json()
 
         # bylines...
         return TopicBylineGroup.construct_from_jdict(jdict, excluded=excluded, skeleton=True)
 
 
     def find_bylines_for_device(self, device, excluded=None):
         params = {self.__DEVICE: device}
 
-        response = self.__http_client.get(self.__URL, params=params)
+        response = self._http_client.get(self.__URL, params=params)
+        self._check_response(response)
+
         jdict = response.json()
 
         # bylines...
         return DeviceBylineGroup.construct_from_jdict(jdict, excluded=excluded, skeleton=True)
 
 
     def find_byline_for_device_topic(self, device, topic):
         params = {self.__DEVICE: device}
 
-        response = self.__http_client.get(self.__URL, params=params)
+        response = self._http_client.get(self.__URL, params=params)
+        self._check_response(response)
+
         jdict = response.json()
 
         # bylines...
         if jdict is None:
             return None
 
         for item in jdict:
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/manager/configuration_check_finder.py` & `scs-core-2.8.1/src/scs_core/aws/manager/configuration_check_finder.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,51 +6,52 @@
 https://stackoverflow.com/questions/36932/how-can-i-represent-an-enum-in-python
 """
 
 from collections import OrderedDict
 from enum import Enum
 from http import HTTPStatus
 
+from scs_core.aws.client.api_client import APIClient
 from scs_core.aws.data.http_response import HTTPResponse
+
+from scs_core.client.http_exception import HTTPException
 from scs_core.data.str import Str
 from scs_core.estate.configuration_check import ConfigurationCheck
-from scs_core.sys.http_exception import HTTPException
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class ConfigurationCheckFinder(object):
+class ConfigurationCheckFinder(APIClient):
     """
     classdocs
     """
 
     __URL = "https://p18hyi3w56.execute-api.us-west-2.amazonaws.com/default/ConfigurationCheckFinder"
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, http_client, auth):
-        self.__http_client = http_client                # requests package
-        self.__auth = auth
+    def __init__(self, http_client):
+        super().__init__(http_client)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def find(self, tag_filter, exact_match, result_code, response_mode):
-        request = ConfigurationCheckRequest(tag_filter, exact_match, result_code, response_mode)
-        headers = {'Authorization': self.__auth.email_address}
+    def find(self, token, tag_filter, exact_match, response_mode):
+        request = ConfigurationCheckRequest(tag_filter, exact_match, response_mode)
 
-        response = self.__http_client.get(self.__URL, headers=headers, params=request.params())
+        response = self._http_client.get(self.__URL, headers=self._token_headers(token), params=request.params())
+        self._check_response(response)
 
         return ConfigurationCheckResponse.construct_from_jdict(response.json())
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "ConfigurationCheckFinder:{auth:%s}" % self.__auth
+        return "ConfigurationCheckFinder:{}"
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class ConfigurationCheckRequest(object):
     """
     classdocs
@@ -58,46 +59,43 @@
 
     class Mode(Enum):
         FULL = 1
         TAGS_ONLY = 2
 
     TAG_FILTER = 'tagFilter'
     EXACT_MATCH = 'exactMatch'
-    RESULT_CODE = 'resultCode'
     RESPONSE_MODE = 'responseMode'
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def construct_from_qsp(cls, qsp):
         if not qsp:
             return None
 
         tag_filter = qsp.get(cls.TAG_FILTER)
         exact_match = qsp.get(cls.EXACT_MATCH, 'false').lower() == 'true'
-        result_code = qsp.get(cls.RESULT_CODE)
 
         try:
             response_mode = cls.Mode[qsp.get(cls.RESPONSE_MODE)]
         except KeyError:
             response_mode = None
 
-        return cls(tag_filter, exact_match, result_code, response_mode)
+        return cls(tag_filter, exact_match, response_mode)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, tag_filter, exact_match, result_code, response_mode):
+    def __init__(self, tag_filter, exact_match, response_mode):
         """
         Constructor
         """
         self.__tag_filter = tag_filter                          # string
         self.__exact_match = bool(exact_match)                  # bool
-        self.__result_code = result_code                        # string
         self.__response_mode = response_mode                    # MODE enum
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
         if self.response_mode is None:
@@ -112,15 +110,14 @@
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def params(self):
         params = {
             self.TAG_FILTER: self.tag_filter,
             self.EXACT_MATCH: self.exact_match,
-            self.RESULT_CODE: self.result_code,
             self.RESPONSE_MODE: self.response_mode.name
         }
 
         return params
 
 
     # ----------------------------------------------------------------------------------------------------------------
@@ -132,28 +129,23 @@
 
     @property
     def exact_match(self):
         return self.__exact_match
 
 
     @property
-    def result_code(self):
-        return self.__result_code
-
-
-    @property
     def response_mode(self):
         return self.__response_mode
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "ConfigurationCheckRequest:{tag_filter:%s, exact_match:%s, result_code:%s, response_mode:%s}" % \
-               (self.tag_filter, self.exact_match, self.result_code, self.response_mode)
+        return "ConfigurationCheckRequest:{tag_filter:%s, exact_match:%s, response_mode:%s}" % \
+               (self.tag_filter, self.exact_match, self.response_mode)
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class ConfigurationCheckResponse(HTTPResponse):
     """
     classdocs
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/manager/configuration_check_requester.py` & `scs-core-2.8.1/src/scs_core/aws/manager/configuration_check_requester.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,49 +5,50 @@
 
 https://stackoverflow.com/questions/36932/how-can-i-represent-an-enum-in-python
 """
 
 from collections import OrderedDict
 from http import HTTPStatus
 
+from scs_core.aws.client.api_client import APIClient
 from scs_core.aws.data.http_response import HTTPResponse
-from scs_core.sys.http_exception import HTTPException
+
+from scs_core.client.http_exception import HTTPException
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class ConfigurationCheckRequester(object):
+class ConfigurationCheckRequester(APIClient):
     """
     classdocs
     """
 
     __URL = "https://5nkrlhaq69.execute-api.us-west-2.amazonaws.com/default/MQTTConfigQueuer"
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, http_client, auth):
-        self.__http_client = http_client                # requests package
-        self.__auth = auth
+    def __init__(self, http_client):
+        super().__init__(http_client)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def request(self, tag):
+    def request(self, token, tag):
         params = {'tag': tag}
-        headers = {'Authorization': self.__auth.email_address}
 
-        response = self.__http_client.get(self.__URL, headers=headers, params=params)
+        response = self._http_client.get(self.__URL, headers=self._token_headers(token), params=params)
+        self._check_response(response)
 
         return ConfigurationCheckRequesterResponse.construct_from_jdict(response.json())
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "ConfigurationCheckRequester:{auth:%s}" % self.__auth
+        return "ConfigurationCheckRequester:{}"
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class ConfigurationCheckRequesterResponse(HTTPResponse):
     """
     classdocs
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/manager/configuration_finder.py` & `scs-core-2.8.1/src/scs_core/aws/manager/configuration_finder.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,64 +9,60 @@
 import json
 
 from collections import OrderedDict
 from enum import Enum
 from http import HTTPStatus
 from urllib.parse import parse_qs, urlparse
 
+from scs_core.aws.client.api_client import APIClient
 from scs_core.aws.data.http_response import HTTPResponse
 
+from scs_core.client.http_exception import HTTPException
+
 from scs_core.data.str import Str
 
 from scs_core.sample.configuration_sample import ConfigurationSample
 
-from scs_core.sys.http_exception import HTTPException
-from scs_core.sys.logging import Logging
-
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class ConfigurationFinder(object):
+class ConfigurationFinder(APIClient):
     """
     classdocs
     """
 
     __URL = "https://p18hyi3w56.execute-api.us-west-2.amazonaws.com/default/ConfigurationFinder"
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, http_client, auth, reporter=None):
-        self.__http_client = http_client                        # requests package
-        self.__auth = auth
-        self.__reporter = reporter                              # BatchDownloadReporter
+    def __init__(self, http_client, reporter=None):
+        super().__init__(http_client)
 
-        self.__logger = Logging.getLogger()
+        self.__reporter = reporter                              # BatchDownloadReporter
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def find(self, tag_filter, exact_match, response_mode):
+    def find(self, token, tag_filter, exact_match, response_mode):
         if self.__reporter:
             self.__reporter.reset()
 
         request = ConfigurationRequest(tag_filter, exact_match, response_mode)
-        headers = {'Authorization': self.__auth.email_address}
-
         params = request.params()
 
         while True:
-            self.__logger.debug("*** url: %s" % self.__URL)
-            self.__logger.debug("*** params: %s" % params)
+            self._logger.debug("*** url: %s" % self.__URL)
+            self._logger.debug("*** params: %s" % params)
 
-            response = self.__http_client.get(self.__URL, headers=headers, params=params)
-            self.__logger.debug(response.json())
+            response = self._http_client.get(self.__URL, headers=self._token_headers(token), params=params)
+            self._check_response(response)
 
             # messages...
             block = ConfigurationResponse.construct_from_jdict(response.json())
-            # self.__logger.debug(block)
+            # self._logger.debug(block)
 
             for item in block.items:
                 yield item
 
             # report...
             if self.__reporter:
                 self.__reporter.print(len(block))
@@ -78,15 +74,15 @@
             next_url = urlparse(block.next_url)
             params = parse_qs(next_url.query)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "ConfigurationFinder:{auth:%s}" % self.__auth
+        return "ConfigurationFinder:{}"
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class ConfigurationRequest(object):
     """
     classdocs
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/manager/dynamo_manager.py` & `scs-core-2.8.1/src/scs_core/aws/manager/dynamo_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 
 @author: Jade Page (jade.page@southcoastscience.com)
 
 https://stackoverflow.com/questions/36780856/complete-scan-of-dynamodb-with-boto3
 
 https://github.com/boto/botocore/issues/1688
 
+https://stackoverflow.com/questions/46616282/dynamodb-query-filterexpression-multiple-condition-chaining-python
+
 A single manager for all required dynamoDB related functions.
 
 """
 
-from boto3.dynamodb.conditions import Key, Attr
-
+from boto3.dynamodb.conditions import Key, Attr, And
+from functools import reduce
 
 # --------------------------------------------------------------------------------------------------------------------
 
 
 class DynamoManager(object):
     """
     classdocs
@@ -66,15 +68,15 @@
 
         return response
 
     def add_simple(self, table_name, pk, pk_val, sk=None, sk_val=None):
         table = self.__dynamo_resource.Table(table_name)
         if sk and sk_val:
             item = {pk: pk_val, sk: sk_val}
-        elif pk and pk_val and not sk and sk_val:
+        elif pk and pk_val and not sk and not sk_val:
             item = {pk: pk_val}
         else:
             return None
 
         response = table.put_item(
             Item=item
         )
@@ -121,18 +123,40 @@
 
         response = table.query(KeyConditionExpression=Key(sk).eq(filter_item),
                                IndexName=index_name)
         to_return = []
         to_return.extend(response['Items'])
         return to_return
 
+    def multi_scan(self, table_name, key_value_pairs, limited):
+        kwargs = {}
+
+        if not table_name:
+            return kwargs
+
+        table = self.__dynamo_resource.Table(table_name)
+
+        to_return = []
+        q = table.scan(FilterExpression=reduce(And, ([Key(k).eq(v) for k, v in key_value_pairs])))
+        to_return.extend(q['Items'])
+        if not limited:
+            while 'LastEvaluatedKey' in q:
+                esk = q['LastEvaluatedKey']
+                q = table.scan(FilterExpression=reduce(And, ([Key(k).eq(v) for k, v in key_value_pairs.items()])),
+                               ExclusiveStartKey=esk)
+                to_return.extend(q['Items'])
+        return to_return
+
     # ----------------------------------------------------------------------------------------------------------------
     # MAIN FUNCTIONALITY
     # ----------------------------------------------------------------------------------------------------------------
 
+
+
+
     @staticmethod
     def build_query(table_name, pk=None, pk_val=None, sk=None, sk_val=None, keys_only=False, exact=False,
                     limit=None, fosk=False):
 
         kwargs = {}
 
         if not table_name:
@@ -174,27 +198,27 @@
                 kwargs['ProjectionExpression'] = '#pk'
                 kwargs['ExpressionAttributeNames'] = {'#pk': pk}
 
             return kwargs
 
         # Filter on second key - filter on second key keys only - filter on second key batched
         if pk and sk and sk_val and fosk:
-            kwargs['ProjectionExpression'] = pk
             if exact:
-                kwargs['KeyConditionExpression'] = Key(sk).eq(sk_val)
+                kwargs['FilterExpression'] = Key(sk).eq(sk_val)
             else:
-                kwargs['KeyConditionExpression'] = Attr(sk).contains(sk_val)
+                kwargs['FilterExpression'] = Attr(sk).contains(sk_val)
             if limit:
                 kwargs['Limit'] = limit
             if keys_only:
                 kwargs['ProjectionExpression'] = '#pk'
                 kwargs['ExpressionAttributeNames'] = {'#pk': pk}
 
             return kwargs
 
+
     def do_query(self, table_name, query, limited=False):
         exact_match = False
         if "KeyConditionExpression" in query:
             exact_match = True
         table = self.__dynamo_resource.Table(table_name)
         to_return = []
         if exact_match:
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/manager/ec2_message_manager.py` & `scs-core-2.8.1/src/scs_core/aws/manager/ec2_message_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/manager/lambda_bylines.py` & `scs-core-2.8.1/src/scs_core/aws/manager/lambda_bylines.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import json
 
 from collections import OrderedDict
 from http import HTTPStatus
 
 from scs_core.aws.data.http_response import HTTPResponse
-from scs_core.sys.http_exception import HTTPException
+from scs_core.client.http_exception import HTTPException
 
 
 # ----------------------------------------------------------------------------------------------------------------
 
 class BylineExclusiveStartKey(object):
     """
     classdocs
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/manager/lambda_message_manager.py` & `scs-core-2.8.1/src/scs_core/aws/manager/lambda_message_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/manager/s3_manager.py` & `scs-core-2.8.1/src/scs_core/aws/manager/s3_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/manager/sagemaker_model_manager.py` & `scs-core-2.8.1/src/scs_core/aws/manager/sagemaker_model_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/manager/sagemaker_trial_manager.py` & `scs-core-2.8.1/src/scs_core/aws/manager/sagemaker_trial_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/aws/security/byline_filter.py` & `scs-core-2.8.1/src/scs_core/aws/security/path_filter.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 Created on 31 Oct 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 
 # --------------------------------------------------------------------------------------------------------------------
-
-class BylineFilter(object):
+class PathFilter(object):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, user_paths):
@@ -19,28 +18,44 @@
         Constructor
         """
         self.__user_paths = user_paths                  # array of string
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def filter(self, bylines):
+    def byline_filter(self, bylines):
         for byline in bylines:
             topic = byline['topic']
 
             for user_path in self.__user_paths:
                 if topic.startswith(user_path):
                     yield byline
                     break
 
 
+    def device_is_visible(self, pod):
+        for user_path in self.__user_paths:
+            if pod.device_path.startswith(user_path) or pod.location_path.startswith(user_path):
+                return True
+
+        return False
+
+
+    def path_is_visible(self, path):
+        for user_path in self.__user_paths:
+            if path.startswith(user_path):
+                return True
+
+        return False
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def user_paths(self):
         return self.__user_paths
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "BylineFilter:{user_paths:%s}" % self.user_paths
+        return "PathFilter:{user_paths:%s}" % self.user_paths
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/security/cognito_device.py` & `scs-core-2.8.1/src/scs_core/sys/disk_usage.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,166 +1,164 @@
 """
-Created on 5 Apr 2022
+Created on 16 Apr 2018
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-example document (credentials):
-{"username": "scs-opc-1", "password": "Ytzglk6oYpzJY0FB"}
+JSON example:
+{"path": "/srv/removable_data_storage", "free": 15423610880, "used": 329793536, "total": 15753404416,
+"is-available": true}
 
-example document (identity):
-{"username": "scs-ap1-343", "created": "2022-04-07T13:37:56Z"}
+https://www.geeksforgeeks.org/python-os-statvfs-method/
 """
 
+import os
+
 from collections import OrderedDict
 
-from scs_core.data.datetime import LocalizedDatetime
 from scs_core.data.json import JSONable
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CognitoDeviceCredentials(JSONable):
+class DiskUsage(JSONable):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    @staticmethod
-    def is_valid_password(password):
-        if not isinstance(password, str):
-            return False
+    @classmethod
+    def construct_from_statvfs(cls, path, statvfs):
+        free = statvfs.f_bfree * statvfs.f_bsize
+        total = statvfs.f_blocks * statvfs.f_bsize
+        used = total - free
 
-        return len(password) > 15
+        return cls(path, free, used, total)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, tag, shared_secret):
+    def __init__(self, path, free, used, total):
         """
         Constructor
         """
-        self._tag = tag                                # PK: string
-        self.__shared_secret = shared_secret            # string
+        self.__path = path                          # string
+
+        self.__free = int(free)                     # int bytes
+        self.__used = int(used)                     # int bytes
+        self.__total = int(total)                   # int bytes
+
+
+    # ----------------------------------------------------------------------------------------------------------------
+
+    def percent_used(self):
+        if not self.is_available:
+            return None
+
+        percent = self.used / self.total * 100
+
+        return round(percent, 1)
+
 
+    @property
+    def is_available(self):
+        try:
+            os.listdir(self.path)
+            return True
 
-    def __lt__(self, other):
-        return self.tag < other.tag
+        except OSError:
+            return False
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         jdict = OrderedDict()
 
-        jdict['username'] = self.tag
-        jdict['password'] = self.shared_secret
+        jdict['path'] = self.path
+
+        jdict['free'] = self.free
+        jdict['used'] = self.used
+        jdict['total'] = self.total
+
+        jdict['is-available'] = self.is_available
 
         return jdict
 
+
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def username(self):
-        return self.tag
+    def path(self):
+        return self.__path
 
 
     @property
-    def tag(self):
-        return self._tag
+    def free(self):
+        return self.__free
 
 
     @property
-    def shared_secret(self):
-        return self.__shared_secret
+    def used(self):
+        return self.__used
+
+
+    @property
+    def total(self):
+        return self.__total
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "CognitoDeviceCredentials:{tag:%s, shared_secret:%s}" % \
-               (self.tag, self.shared_secret)
+        return "DiskUsage:{path:%s, free:%s, used:%s, total:%s}" %  \
+               (self.path, self.free, self.used, self.total)
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CognitoDeviceIdentity(CognitoDeviceCredentials):
+class ReportedDiskUsage(DiskUsage):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
-    def construct_from_jdict(cls, jdict, skeleton=False):
+    def construct_from_jdict(cls, jdict):
         if not jdict:
-            return cls(None, None, None, None) if skeleton else None
+            return None
+
+        path = jdict.get('path')
+
+        free = jdict.get('free')
+        used = jdict.get('used')
+        total = jdict.get('total')
 
-        tag = jdict.get('username')
-        shared_secret = jdict.get('password')
-        created = LocalizedDatetime.construct_from_iso8601(jdict.get('created'))
-        last_updated = LocalizedDatetime.construct_from_iso8601(jdict.get('last-updated'))
+        is_available = jdict.get('is-available')
 
-        return cls(tag, shared_secret, created, last_updated)
+        return cls(path, free, used, total, is_available)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, tag, shared_secret, created, last_updated):
+    def __init__(self, path, free, used, total, is_available):
         """
         Constructor
         """
-        super().__init__(tag, shared_secret)
+        super().__init__(path, free, used, total)
 
-        self._created = created                                 # LocalisedDatetime
-        self._last_updated = last_updated                       # LocalizedDatetime
-
-
-    def __eq__(self, other):
-        try:
-            return self.tag == other.tag
-
-        except (TypeError, AttributeError):
-            return False
-
-
-    def __lt__(self, other):
-        return self.tag < other.tag
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    def as_json(self):
-        jdict = OrderedDict()
-
-        if self.tag is not None:
-            jdict['username'] = self.tag
-
-        if self.shared_secret is not None:
-            jdict['password'] = self.shared_secret
-
-        if self.created is not None:
-            jdict['created'] = self.created.as_iso8601()
-
-        if self.last_updated is not None:
-            jdict['last-updated'] = self.last_updated.as_iso8601()
-
-        return jdict
+        self.__is_available = is_available                      # bool
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def created(self):
-        return self._created
-
-
-    @property
-    def last_updated(self):
-        return self._last_updated
+    def is_available(self):
+        return self.__is_available
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return self.__class__.__name__ + ":{tag:%s, shared_secret:%s, created:%s, last_updated:%s}" % \
-               (self.tag, self.shared_secret, self.created, self.last_updated)
+        return "ReportedDiskUsage:{path:%s, free:%s, used:%s, total:%s, is_available:%s}" %  \
+               (self.path, self.free, self.used, self.total, self.is_available)
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/security/cognito_device_finder.py` & `scs-core-2.8.1/src/scs_core/aws/security/cognito_device_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,57 @@
 """
 Created on 5 Apr 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
-import json
-
-from http import HTTPStatus
-
+from scs_core.aws.client.api_client import APIClient
 from scs_core.aws.security.cognito_device import CognitoDeviceIdentity
 
-from scs_core.sys.http_exception import HTTPException
-from scs_core.sys.logging import Logging
+from scs_core.data.json import JSONify
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CognitoDeviceFinder(object):
+class CognitoDeviceManager(APIClient):
     """
     classdocs
     """
 
-    __URL = 'https://6c2sfqt656.execute-api.us-west-2.amazonaws.com/default/CognitoDevices/retrieve'
+    __URL = 'https://6c2sfqt656.execute-api.us-west-2.amazonaws.com/default/CognitoDevices'
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, http_client):
-        self.__http_client = http_client                    # requests package
-        self.__logger = Logging.getLogger()
+        super().__init__(http_client)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def find_all(self, token):
-        url = '/'.join((self.__URL, 'all'))
-
-        response = self.__http_client.get(url, headers=self.__headers(token))
-        self.__check_response(response)
-
-        # print("response: %s" % response.json())
-
-        return tuple(CognitoDeviceIdentity.construct_from_jdict(jdict) for jdict in response.json())
-
-
-    def find_by_tag(self, token, tag):
-        url = '/'.join((self.__URL, 'in'))
-        payload = json.dumps({"username": tag})
-
-        response = self.__http_client.get(url, data=payload, headers=self.__headers(token))
-        self.__check_response(response)
-
-        return tuple(CognitoDeviceIdentity.construct_from_jdict(jdict) for jdict in response.json())
-
-
-    def get_by_tag(self, token, tag):
-        url = '/'.join((self.__URL, 'exact'))
-        payload = json.dumps({"username": tag})
-
-        response = self.__http_client.get(url, data=payload, headers=self.__headers(token))
-        self.__check_response(response)
+    def create(self, token, identity):
+        response = self._http_client.post(self.__URL, headers=self._token_headers(token), data=JSONify.dumps(identity))
+        self._check_response(response)
 
         return CognitoDeviceIdentity.construct_from_jdict(response.json())
 
 
-    # ----------------------------------------------------------------------------------------------------------------
+    def update(self, token, identity):
+        response = self._http_client.patch(self.__URL, headers=self._token_headers(token), data=JSONify.dumps(identity))
+        self._check_response(response)
 
-    def __headers(self, token):
-        headers = {"Content-type": "application/x-www-form-urlencoded", "Accept": "text/json", "Token": token}
-        self.__logger.debug('headers: %s' % headers)
+        return CognitoDeviceIdentity.construct_from_jdict(response.json())
 
-        return headers
 
 
-    def __check_response(self, response):
-        self.__logger.debug('response: %s' % response.json())
+    def delete(self, token, device_tag):
+        payload = {"DeviceTag": device_tag}
 
-        status = HTTPStatus(response.status_code)
+        response = self._http_client.delete(self.__URL, headers=self._token_headers(token), data=JSONify.dumps(payload))
+        self._check_response(response)
 
-        if status != HTTPStatus.OK:
-            raise HTTPException.construct(status.value, response.reason, response.json())
+        # TODO: delete device from organisations?
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "CognitoDeviceFinder:{}"
+        return "CognitoDeviceManager:{}"
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/security/cognito_login_manager.py` & `scs-core-2.8.1/src/scs_core/aws/security/cognito_login_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,61 +3,59 @@
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 from collections import OrderedDict
 from enum import Enum
 
+from scs_core.aws.client.api_client import APIClient
 from scs_core.aws.data.http_response import HTTPResponse
 
 from scs_core.data.json import JSONable
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CognitoLoginManager(object):
+class CognitoLoginManager(APIClient):
     """
     classdocs
     """
 
-    __AUTHORIZATION = '@southcoastscience.com'
     __URL = 'https://lnh2y9ip75.execute-api.us-west-2.amazonaws.com/default/CognitoLogin'
+    __AUTH = '@southcoastscience.com'
+
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, http_client):
-        self.__http_client = http_client                # requests package
+        super().__init__(http_client)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def user_login(self, credentials):
         url = '/'.join((self.__URL, 'user'))
-        headers = {'Authorization': self.__AUTHORIZATION}
+        headers = self._auth_headers(self.__AUTH)
 
-        response = self.__http_client.post(url, headers=headers, json=credentials.as_json())
+        response = self._http_client.post(url, headers=headers, json=credentials.as_json())
+        self._check_response(response)
 
         return AuthenticationResult.construct_from_res(response)
 
 
     def device_login(self, credentials):
         url = '/'.join((self.__URL, 'device'))
-        headers = {'Authorization': self.__AUTHORIZATION}
+        headers = self._auth_headers(self.__AUTH)
 
-        response = self.__http_client.post(url, headers=headers, json=credentials.as_json())
+        response = self._http_client.post(url, headers=headers, json=credentials.as_json())
+        self._check_response(response)
 
         return AuthenticationResult.construct_from_res(response)
 
 
-    # ----------------------------------------------------------------------------------------------------------------
-
-    def __str__(self, *args, **kwargs):
-        return "CognitoLoginManager:{}"
-
-
 # --------------------------------------------------------------------------------------------------------------------
 
 class AuthenticationResult(HTTPResponse):
     """
     {"AccessToken": "...",
     "ExpiresIn": 3600,
     "TokenType": "Bearer",
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/security/cognito_membership.py` & `scs-core-2.8.1/src/scs_core/aws/security/cognito_membership.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     classdocs
     """
 
     @classmethod
     def merge(cls, cognito_accounts, org_memberships):
         org_dict = ArrayDict([(org_membership.username, org_membership) for org_membership in sorted(org_memberships)])
 
-        # Users...
+        # Accounts...
         return [cls(cognito_account, org_dict.get(cognito_account.username)) for cognito_account in cognito_accounts]
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, cognito_account, memberships):
         """
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/security/cognito_password_manager.py` & `scs-core-2.8.1/src/scs_core/aws/security/cognito_password_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,87 +11,52 @@
 
 https://docs.python.org/3/howto/enum.html#planet
 
 document example:
 "EmailSent"
 """
 
-from http import HTTPStatus
-
+from scs_core.aws.client.api_client import APIClient
 from scs_core.data.json import JSONify
-from scs_core.sys.http_exception import HTTPException
-from scs_core.sys.logging import Logging
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CognitoPasswordManager(object):
+class CognitoPasswordManager(APIClient):
     """
     classdocs
     """
 
     __URL = "https://df46l72wl7.execute-api.us-west-2.amazonaws.com/default/CognitoUserPassword"
-
-    __HEADERS = {'Content-type': 'application/x-www-form-urlencoded',
-                 'Accept': 'text/plain', 'Authorization': '@southcoastscience.com'}
+    __AUTH = "@southcoastscience.com"
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, http_client):
-        self.__http_client = http_client                # requests package
-        self.__logger = Logging.getLogger()
+        super().__init__(http_client)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def send_email(self, email):
         url = '/'.join((self.__URL, 'send-email'))
         payload = {'email': email}
 
-        response = self.__http_client.post(url, headers=self.__HEADERS, data=JSONify.dumps(payload))
-        status = HTTPStatus(response.status_code)
-
-        print("send_email - status_code: %s" % response.status_code)
-        print("send_email - text: %s" % response.text)
-        print("send_email - json: %s" % response.json())
-
-        if status != HTTPStatus.OK:
-            raise HTTPException.construct(status.value, response.reason, response.json())
+        response = self._http_client.post(url, headers=self._auth_headers(self.__AUTH), data=JSONify.dumps(payload))
+        self._check_response(response)
 
 
     def do_reset_password(self, email, code, new_password):
         url = '/'.join((self.__URL, 'reset'))
         payload = {'email': email, 'reset_code': code, 'new_password': new_password}
 
-        response = self.__http_client.post(url, headers=self.__HEADERS, data=JSONify.dumps(payload))
-        status = HTTPStatus(response.status_code)
-
-        print("do_reset_password - status_code: %s" % response.status_code)
-        print("do_reset_password - text: %s" % response.text)
-        print("do_reset_password - json: %s" % response.json())
-
-        if status != HTTPStatus.OK:
-            raise HTTPException.construct(status.value, response.reason, response.json())
+        response = self._http_client.post(url, headers=self._auth_headers(self.__AUTH), data=JSONify.dumps(payload))
+        self._check_response(response)
 
 
     def do_set_password(self, email, new_password, session):
         url = '/'.join((self.__URL, 'respond'))
         payload = {'email': email, 'new_password': new_password, 'session': session}
 
-        response = self.__http_client.post(url, headers=self.__HEADERS, data=JSONify.dumps(payload))
-        status = HTTPStatus(response.status_code)
-
-        print("do_set_password - status_code: %s" % response.status_code)
-        print("do_set_password - text: %s" % response.text)
-        print("do_set_password - json: %s" % response.json())
-
-        if status != HTTPStatus.OK:
-            ex = HTTPException.construct(status.value, response.reason, response.json())
-            print("raising: %s" % ex)
-            raise ex
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    def __str__(self, *args, **kwargs):
-        return "CognitoPasswordManager:{}"
+        response = self._http_client.post(url, headers=self._auth_headers(self.__AUTH), data=JSONify.dumps(payload))
+        self._check_response(response)
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/security/cognito_user.py` & `scs-core-2.8.1/src/scs_core/aws/security/cognito_user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,129 +1,49 @@
 """
 Created on 22 Nov 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 https://docs.aws.amazon.com/cognito/latest/developerguide/signing-up-users-in-your-app.html
 https://docs.aws.amazon.com/cognito/latest/developerguide/user-pool-settings-policies.html
-https://stackoverflow.com/questions/2520893/how-to-flush-the-input-stream-in-python
-
-example document (credentials):
-{"email": "production@southcoastscience.com", "password": "###", "retrieval-password": "###"}
 
 example document (identity):
 {"username": "8", "creation-date": "2021-11-24T12:51:12Z", "confirmation-status": "CONFIRMED", "enabled": true,
 "email": "bruno.beloff@southcoastscience.com", "given-name": "Bruno", "family-name": "Beloff", "is-super": true}
 
 example AWS response:
 {"username": 22, "email": "bruno.beloff@southcoastscience.com", "given-name": "Bruno", "family-name": "Beloff",
 "confirmation-status": "FORCE_CHANGE_PASSWORD", "enabled": true, "email-verified": false, "is-super": false,
 "is-tester": false, "created": "2023-03-07T15:32:17Z", "last-updated": "2023-03-08T14:12:00Z"}
 """
 
-import json
 import re
-import sys
-import termios
 
 from collections import OrderedDict
-from getpass import getpass
 
 from scs_core.data.datetime import LocalizedDatetime
 from scs_core.data.datum import Datum
-from scs_core.data.json import JSONable, MultiPersistentJSONable
+from scs_core.data.json import JSONable
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CognitoUserCredentials(MultiPersistentJSONable):
+class CognitoUserCredentials(object):
     """
     classdocs
     """
 
-    __FILENAME = "cognito_user_credentials.json"
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    @classmethod
-    def from_stdin(cls, name):
-        line = sys.stdin.readline()
-        jdict = json.loads(line)
-
-        return cls.construct_from_jdict(jdict, name=name)
-
-
-    @classmethod
-    def from_user(cls, name, existing_email=None):
-        try:
-            termios.tcflush(sys.stdin, termios.TCIOFLUSH)               # flush stdin
-        except termios.error:
-            pass
-
-        if existing_email:
-            email = existing_email
-
-        else:
-            print("Enter email address: ", end="", file=sys.stderr)
-            email = input().strip()
-
-        print("Enter password: ", end="", file=sys.stderr)
-        password = input().strip()
-
-        print("Enter retrieval password (RETURN for same): ", end="", file=sys.stderr)
-        retrieval_password = input().strip()
-
-        if not retrieval_password:
-            retrieval_password = password
-
-        return cls(name, email, password, retrieval_password)
-
-
-    @staticmethod
-    def password_from_user():
-        try:
-            termios.tcflush(sys.stdin, termios.TCIOFLUSH)               # flush stdin
-        except termios.error:
-            pass
-
-        return getpass().strip()
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    @classmethod
-    def persistence_location(cls, name):
-        filename = cls.__FILENAME if name is None else '_'.join((name, cls.__FILENAME))
-
-        return cls.aws_dir(), filename
-
-
-    @classmethod
-    def construct_from_jdict(cls, jdict, name=None, skeleton=False):
-        if not jdict:
-            return cls(None, None, None, None) if skeleton else None
-
-        email = jdict.get('email')
-        password = jdict.get('password')
-        retrieval_password = jdict.get('retrieval-password')
-
-        return cls(name, email, password, retrieval_password)
-
-
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, name, email, password, retrieval_password):
+    def __init__(self, email, password):
         """
         Constructor
         """
-        super().__init__(name)
-
         self.__email = email                                        # string (email)
         self.__password = password                                  # string (AWS password)
-        self.__retrieval_password = retrieval_password              # string
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def ok(self):
         if not self.email or not self.password:
             return False
@@ -135,26 +55,14 @@
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
-        jdict = OrderedDict()
-
-        jdict['email'] = self.email
-        jdict['password'] = self.password
-        jdict['retrieval-password'] = self.retrieval_password
-
-        return jdict
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
     @property
     def email(self):
         return self.__email
 
 
     @email.setter
     def email(self, email):
@@ -162,24 +70,18 @@
 
 
     @property
     def password(self):
         return self.__password
 
 
-    @property
-    def retrieval_password(self):
-        return self.__retrieval_password
-
-
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "CognitoUserCredentials:{name:%s, email:%s, password:%s, retrieval_password:%s}" %  \
-               (self.name, self.email, self.password, self.retrieval_password)
+        return "CognitoUserCredentials:{email:%s, password:%s}" %  (self.email, self.password)
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CognitoUserIdentity(JSONable):
     """
     classdocs
@@ -233,26 +135,36 @@
 
         if not re.findall(r'[\^$*.\[\]{}()?"!@#%&/\\,><\':;|_~`]', password):
             return False
 
         return True
 
 
+    @staticmethod
+    def ext_name(name):
+        return '-' if name is None or name.strip() == '' else name
+
+
+    @staticmethod
+    def int_name(name):
+        return None if name == '-' else name
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def construct_from_jdict(cls, jdict, skeleton=False):
         if not jdict:
             return cls(None, None, None, None, None, None, None, None, None, None, None, None) if skeleton else None
 
         username = jdict.get('username')
         email = jdict.get('email')
         password = jdict.get('password')
-        given_name = jdict.get('given-name')
-        family_name = jdict.get('family-name')
+        given_name = cls.int_name(jdict.get('given-name'))
+        family_name = cls.int_name(jdict.get('family-name'))
 
         confirmation_status = jdict.get('confirmation-status')
         enabled = jdict.get('enabled')
         email_verified = jdict.get('email-verified')
         is_super = jdict.get('is-super')
         is_tester = jdict.get('is-tester')
 
@@ -267,15 +179,15 @@
 
     def __init__(self, username, created, confirmation_status, enabled,
                  email_verified, email, given_name, family_name, password, is_super, is_tester, last_updated):
         """
         Constructor
         """
 
-        self._username = Datum.int(username, default=username)      # int, string or None
+        self._username = username                                   # string email address or hash
         self._created = created                                     # LocalisedDatetime
         self.__confirmation_status = confirmation_status            # string
         self.__enabled = Datum.bool(enabled)                        # bool or None
 
         self.__email_verified = bool(email_verified)                # bool
         self.__email = email                                        # string
         self.__given_name = given_name                              # string
@@ -296,34 +208,35 @@
                    and self.is_tester == other.is_tester
 
         except (TypeError, AttributeError):
             return False
 
 
     def __lt__(self, other):
-        if self.family_name is not None:
-            if other.family_name is None:
-                return False
+        # family_name...
+        self_name = self.ext_name(self.family_name)
+        other_name = self.ext_name(other.family_name)
 
-            if self.family_name.lower() < other.family_name.lower():
-                return True
+        if self_name.lower() < other_name.lower():
+            return True
 
-            if self.family_name.lower() > other.family_name.lower():
-                return False
+        if self_name.lower() > other_name.lower():
+            return False
 
-        if self.given_name is not None:
-            if other.given_name is None:
-                return False
+        # given_name...
+        self_name = self.ext_name(self.given_name)
+        other_name = self.ext_name(other.given_name)
 
-            if self.given_name.lower() < other.given_name.lower():
-                return True
+        if self_name.lower() < other_name.lower():
+            return True
 
-            if self.given_name.lower() > other.given_name.lower():
-                return False
+        if self_name.lower() > other_name.lower():
+            return False
 
+        # email...
         if self.email.lower() < other.email.lower():
             return True
 
         if self.email.lower() > other.email.lower():
             return False
 
         return False
@@ -364,16 +277,16 @@
             jdict['username'] = self.username
 
         jdict['email'] = self.email
 
         if self.password is not None:
             jdict['password'] = self.password
 
-        jdict['given-name'] = self.given_name
-        jdict['family-name'] = self.family_name
+        jdict['given-name'] = self.ext_name(self.given_name)
+        jdict['family-name'] = self.ext_name(self.family_name)
 
         if self.confirmation_status is not None:
             jdict['confirmation-status'] = self.confirmation_status
 
         if self.enabled is not None:
             jdict['enabled'] = self.enabled
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/security/organisation.py` & `scs-core-2.8.1/src/scs_core/aws/security/organisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, opr_id, org_id, path_root):
         """
         Constructor
         """
         self._opr_id = Datum.int(opr_id)                # AUTO PK: int
-        self.__org_id = int(org_id)                     # INDEX: int
+        self.__org_id = Datum.int(org_id)               # INDEX: int
         self.__path_root = path_root                    # UNIQUE: string
 
 
     def __eq__(self, other):
         try:
             return self.org_id == other.org_id and self.path_root == other.path_root
 
@@ -343,19 +343,19 @@
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, username, org_id, is_org_admin, is_device_admin, is_suspended):
         """
         Constructor
         """
-        self._username = int(username)                          # PK: int
-        self._org_id = int(org_id)                              # PK: int
-        self.__is_org_admin = bool(is_org_admin)                # INDEX: bool
-        self.__is_device_admin = bool(is_device_admin)          # INDEX: bool
-        self.__is_suspended = bool(is_suspended)                # INDEX: bool
+        self._username = username                                   # PK: string
+        self._org_id = Datum.int(org_id)                            # PK: int
+        self.__is_org_admin = bool(is_org_admin)                    # INDEX: bool
+        self.__is_device_admin = bool(is_device_admin)              # INDEX: bool
+        self.__is_suspended = bool(is_suspended)                    # INDEX: bool
 
 
     def __eq__(self, other):
         try:
             return self.username == other.username and self.org_id == other.org_id \
                    and self.is_org_admin == other.is_org_admin and self.is_device_admin == other.is_device_admin \
                    and self.is_suspended == other.is_suspended
@@ -480,17 +480,17 @@
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, username, opr_id, path_extension):
         """
         Constructor
         """
-        self._username = int(username)                  # PK: int
-        self._opr_id = int(opr_id)                      # PK: int
-        self._path_extension = path_extension           # PK: string
+        self._username = username                                   # PK: string
+        self._opr_id = Datum.int(opr_id)                            # PK: int
+        self._path_extension = path_extension                       # PK: string
 
 
     def __eq__(self, other):
         try:
             return self.username == other.username and self.opr_id == other.opr_id \
                    and self.path_extension == other.path_extension
 
@@ -639,15 +639,15 @@
 
     def __init__(self, device_tag, org_id, device_path, location_path, start_datetime, end_datetime,
                  deployment_label):
         """
         Constructor
         """
         self._device_tag = device_tag                   # PK: string
-        self._org_id = int(org_id)                      # PK: int
+        self._org_id = Datum.int(org_id)                # PK: int
         self.__device_path = device_path                # string
         self.__location_path = location_path            # string
 
         self._start_datetime = start_datetime           # PK: LocalizedDatetime
         self.__end_datetime = end_datetime              # LocalizedDatetime
         self.__deployment_label = deployment_label      # INDEX: string
 
@@ -700,23 +700,30 @@
 
         jdict[self.DEVICE_TAG] = self.device_tag
         jdict[self.ORG_ID] = self.org_id
         jdict[self.DEPLOYMENT_LABEL] = self.deployment_label
         jdict[self.DEVICE_PATH] = self.device_path
         jdict[self.LOCATION_PATH] = self.location_path
 
-        jdict[self.START_DATETIME] = self.start_datetime.as_iso8601()
+        jdict[self.START_DATETIME] = None if self.start_datetime is None else self.start_datetime.as_iso8601()
         jdict[self.END_DATETIME] = None if self.end_datetime is None else self.end_datetime.as_iso8601()
 
         return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
+    def control_path(self):
+        return self.device_path + 'control'
+
+
+    # ----------------------------------------------------------------------------------------------------------------
+
+    @property
     def username(self):
         return self.device_tag
 
 
     @property
     def device_tag(self):
         return self._device_tag
```

### Comparing `scs-core-2.4.6/src/scs_core/aws/security/organisation_manager.py` & `scs-core-2.8.1/src/scs_core/aws/security/organisation_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,282 +1,260 @@
 """
 Created on 17 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
-from http import HTTPStatus
-
+from scs_core.aws.client.api_client import APIClient
 from scs_core.aws.security.organisation import Organisation, OrganisationPathRoot, OrganisationUser, \
     OrganisationUserPath, OrganisationDevice
 
 from scs_core.data.json import JSONify
 
-from scs_core.sys.http_exception import HTTPException
-from scs_core.sys.logging import Logging
-
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class OrganisationManager(object):
+class OrganisationManager(APIClient):
     """
     classdocs
     """
 
     __MANAGER_URL = "https://04h65m94o8.execute-api.us-west-2.amazonaws.com/default/OrganisationManager"
     __EXECUTIVE_URL = "https://19tm2j6odj.execute-api.us-west-2.amazonaws.com/default/OrganisationExecutive"
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, http_client):
-        self.__http_client = http_client                # requests package
-        self.__logger = Logging.getLogger()
+        super().__init__(http_client)
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # Organisation...
 
     def find_organisations(self, token):
         url = '/'.join((self.__MANAGER_URL, 'organisation'))
 
-        response = self.__http_client.get(url, headers=self.__headers(token))
-        self.__check_response(response)
+        response = self._http_client.get(url, headers=self._token_headers(token))
+        self._check_response(response)
 
         return tuple(Organisation.construct_from_jdict(jdict) for jdict in response.json())
 
 
     def get_organisation_by_label(self, token, label):
         url = '/'.join((self.__MANAGER_URL, 'organisation'))
         payload = JSONify.dumps({"Label": label})
 
-        response = self.__http_client.get(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
+        response = self._http_client.get(url, headers=self._token_headers(token), data=payload)
+        self._check_response(response)
 
         return Organisation.construct_from_jdict(response.json())
 
 
     def insert_organisation(self, token, organisation):
         url = '/'.join((self.__EXECUTIVE_URL, 'organisation'))
         payload = JSONify.dumps(organisation)
 
-        response = self.__http_client.post(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
+        response = self._http_client.post(url, headers=self._token_headers(token), data=payload)
+        self._check_response(response)
 
         return Organisation.construct_from_jdict(response.json())
 
 
     def update_organisation(self, token, organisation):
         url = '/'.join((self.__MANAGER_URL, 'organisation'))
         payload = JSONify.dumps(organisation)
 
-        response = self.__http_client.patch(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
+        response = self._http_client.patch(url, headers=self._token_headers(token), data=payload)
+        self._check_response(response)
 
 
     def delete_organisation(self, token, org_id):
         url = '/'.join((self.__EXECUTIVE_URL, 'organisation'))
         payload = JSONify.dumps({"OrgID": org_id})
 
-        response = self.__http_client.delete(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
+        response = self._http_client.delete(url, headers=self._token_headers(token), data=payload)
+        self._check_response(response)
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # OrganisationPathRoot...
 
-    def find_oprs_by_organisation(self, token, org_id):
+    def find_oprs(self, token, org_id=None):
         url = '/'.join((self.__MANAGER_URL, 'opr'))
-        payload = JSONify.dumps({"OrgID": org_id})
+        payload = {}
 
-        response = self.__http_client.get(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
+        if org_id:
+            payload['OrgID'] = org_id
+
+        response = self._http_client.get(url, headers=self._token_headers(token), data=JSONify.dumps(payload))
+        self._check_response(response)
 
         return tuple(OrganisationPathRoot.construct_from_jdict(jdict) for jdict in response.json())
 
 
     def get_opr_by_path_root(self, token, path_root):
         url = '/'.join((self.__MANAGER_URL, 'opr'))
         payload = JSONify.dumps({"PathRoot": path_root})
 
-        response = self.__http_client.get(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
+        response = self._http_client.get(url, headers=self._token_headers(token), data=payload)
+        self._check_response(response)
 
         return OrganisationPathRoot.construct_from_jdict(response.json())
 
 
     def insert_opr(self, token, opr):
         url = '/'.join((self.__EXECUTIVE_URL, 'opr'))
         payload = JSONify.dumps(opr)
 
-        response = self.__http_client.post(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
+        response = self._http_client.post(url, headers=self._token_headers(token), data=payload)
+        self._check_response(response)
 
         return OrganisationPathRoot.construct_from_jdict(response.json())
 
 
     def delete_opr(self, token, opr_id):
         url = '/'.join((self.__EXECUTIVE_URL, 'opr'))
         payload = JSONify.dumps({"OPRID": opr_id})
 
-        response = self.__http_client.delete(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
+        response = self._http_client.delete(url, headers=self._token_headers(token), data=payload)
+        self._check_response(response)
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # OrganisationUser...
 
     def find_users(self, token):
         url = '/'.join((self.__MANAGER_URL, 'user'))
 
-        response = self.__http_client.get(url, headers=self.__headers(token))
-        self.__check_response(response)
+        response = self._http_client.get(url, headers=self._token_headers(token))
+        self._check_response(response)
 
         return tuple(OrganisationUser.construct_from_jdict(jdict) for jdict in response.json())
 
 
     def find_users_by_organisation(self, token, org_id):
         url = '/'.join((self.__MANAGER_URL, 'user'))
         payload = JSONify.dumps({"OrgID": org_id})
 
-        response = self.__http_client.get(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
+        response = self._http_client.get(url, headers=self._token_headers(token), data=payload)
+        self._check_response(response)
 
         return tuple(OrganisationUser.construct_from_jdict(jdict) for jdict in response.json())
 
 
     def find_users_by_username(self, token, username):
         url = '/'.join((self.__MANAGER_URL, 'user'))
         payload = JSONify.dumps({"Username": username})
 
-        response = self.__http_client.get(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
+        response = self._http_client.get(url, headers=self._token_headers(token), data=payload)
+        self._check_response(response)
 
         return tuple(OrganisationUser.construct_from_jdict(jdict) for jdict in response.json())
 
 
     def get_user(self, token, username, org_id):
         url = '/'.join((self.__MANAGER_URL, 'user'))
         payload = JSONify.dumps({"Username": username, "OrgID": org_id})
 
-        response = self.__http_client.get(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
+        response = self._http_client.get(url, headers=self._token_headers(token), data=payload)
+        self._check_response(response)
 
         return OrganisationUser.construct_from_jdict(response.json())
 
 
     def assert_user(self, token, user):
         url = '/'.join((self.__MANAGER_URL, 'user'))
         payload = JSONify.dumps(user)
 
-        response = self.__http_client.post(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
+        response = self._http_client.post(url, headers=self._token_headers(token), data=payload)
+        self._check_response(response)
 
 
     def delete_user(self, token, username, org_id):
         url = '/'.join((self.__EXECUTIVE_URL, 'user'))
         payload = JSONify.dumps({"Username": username, "OrgID": org_id})
 
-        response = self.__http_client.delete(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
+        response = self._http_client.delete(url, headers=self._token_headers(token), data=payload)
+        self._check_response(response)
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # OrganisationUserPath...
 
-    def find_oups(self, token, username, opr_id):
+    def find_oups(self, token, username=None, opr_id=None):
         url = '/'.join((self.__MANAGER_URL, 'oup'))
-        payload = JSONify.dumps({"Username": username, "OPRID": opr_id})
+        payload = {}
+
+        if username:
+            payload['Username'] = username
 
-        response = self.__http_client.get(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
+        if opr_id:
+            payload['OPRID'] = opr_id
 
-        print("response: %s" % response.json())
+        response = self._http_client.get(url, headers=self._token_headers(token), data=JSONify.dumps(payload))
+        self._check_response(response)
 
         return tuple(OrganisationUserPath.construct_from_jdict(jdict) for jdict in response.json())
 
 
     def assert_oup(self, token, oup):
         url = '/'.join((self.__MANAGER_URL, 'oup'))
         payload = JSONify.dumps(oup)
 
-        response = self.__http_client.post(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
+        response = self._http_client.post(url, headers=self._token_headers(token), data=payload)
+        self._check_response(response)
 
 
     def delete_oup(self, token, oup):
         url = '/'.join((self.__MANAGER_URL, 'oup'))
         payload = JSONify.dumps(oup)
 
-        response = self.__http_client.delete(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
+        response = self._http_client.delete(url, headers=self._token_headers(token), data=payload)
+        self._check_response(response)
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # OrganisationDevice...
 
     def find_devices(self, token):
         url = '/'.join((self.__MANAGER_URL, 'device'))
 
-        response = self.__http_client.get(url, headers=self.__headers(token))
-        self.__check_response(response)
+        response = self._http_client.get(url, headers=self._token_headers(token))
+        self._check_response(response)
 
         return tuple(OrganisationDevice.construct_from_jdict(jdict) for jdict in response.json())
 
 
     def find_devices_by_tag(self, token, device_tag):
         url = '/'.join((self.__MANAGER_URL, 'device'))
         payload = JSONify.dumps({"DeviceTag": device_tag})
 
-        response = self.__http_client.get(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
+        response = self._http_client.get(url, headers=self._token_headers(token), data=payload)
+        self._check_response(response)
 
         return tuple(OrganisationDevice.construct_from_jdict(jdict) for jdict in response.json())
 
 
     def find_devices_by_organisation(self, token, org_id):
         url = '/'.join((self.__MANAGER_URL, 'device'))
         payload = JSONify.dumps({"OrgID": org_id})
 
-        response = self.__http_client.get(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
+        response = self._http_client.get(url, headers=self._token_headers(token), data=payload)
+        self._check_response(response)
 
         return tuple(OrganisationDevice.construct_from_jdict(jdict) for jdict in response.json())
 
 
     def assert_device(self, token, device):
         url = '/'.join((self.__EXECUTIVE_URL, 'device'))
         payload = JSONify.dumps(device)
 
-        response = self.__http_client.post(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
+        response = self._http_client.post(url, headers=self._token_headers(token), data=payload)
+        self._check_response(response)
 
 
     def delete_device(self, token, device_tag):
         url = '/'.join((self.__EXECUTIVE_URL, 'device'))
         payload = JSONify.dumps({"DeviceTag": device_tag})
 
-        response = self.__http_client.delete(url, headers=self.__headers(token), data=payload)
-        self.__check_response(response)
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    def __headers(self, token):
-        headers = {"Content-type": "application/x-www-form-urlencoded", "Accept": "text/json", "Token": token}
-        self.__logger.debug('headers: %s' % headers)
-
-        return headers
-
-
-    def __check_response(self, response):
-        self.__logger.debug('response: %s' % response.json())
-
-        status = HTTPStatus(response.status_code)
-
-        if status != HTTPStatus.OK:
-            raise HTTPException.construct(status.value, response.reason, response.json())
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    def __str__(self, *args, **kwargs):
-        return "OrganisationManager:{}"
+        response = self._http_client.delete(url, headers=self._token_headers(token), data=payload)
+        self._check_response(response)
```

### Comparing `scs-core-2.4.6/src/scs_core/client/http_client.py` & `scs-core-2.8.1/src/scs_core/client/http_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 
 import http.client
 
 import urllib.parse
 
 from socket import gaierror, timeout as timeout_error
 
+from scs_core.client.http_exception import HTTPException
+from scs_core.client.http_status import HTTPStatus
 from scs_core.client.resource_unavailable_exception import ResourceUnavailableException
 
-from scs_core.sys.http_exception import HTTPException
-from scs_core.sys.http_status import HTTPStatus
-
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class HTTPClient(object):
     """
     classdocs
     """
@@ -37,14 +36,16 @@
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def connect(self, host, secure=True, verified=True, timeout=None):
         # print("connect: host: {}, timeout: {}".format(host, timeout), file=sys.stderr)
 
+        self.__host = host                                          # PersistenceManager
+
         if secure:
             # noinspection PyProtectedMember,PyUnresolvedReferences
             context = None if verified else ssl._create_unverified_context()
 
             if timeout is not None:
                 self.__conn = http.client.HTTPSConnection(host, context=context, timeout=timeout)
             else:
@@ -52,16 +53,14 @@
 
         else:
             if timeout is not None:
                 self.__conn = http.client.HTTPConnection(host, timeout=timeout)
             else:
                 self.__conn = http.client.HTTPConnection(host)
 
-        self.__host = host
-
 
     def close(self):
         if self.__conn:
             self.__conn.close()
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-core-2.4.6/src/scs_core/client/network.py` & `scs-core-2.8.1/src/scs_core/client/network.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,21 +68,25 @@
 
     def start(self):
         self.__proc = Process(target=self.run)
         self.__proc.start()
 
 
     def run(self):
-        Network.wait()
+        try:
+            Network.wait()
 
-        while True:
-            if not Network.is_available():
-                self.__network_unavailable_handler()
+            while True:
+                if not Network.is_available():
+                    self.__network_unavailable_handler()
 
-            time.sleep(self.__interval)
+                time.sleep(self.__interval)
+
+        except KeyboardInterrupt:
+            pass
 
 
     def join(self):
         self.__proc.join()
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-core-2.4.6/src/scs_core/client/resource_unavailable_exception.py` & `scs-core-2.8.1/src/scs_core/client/resource_unavailable_exception.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/client/sftp_client_conf.py` & `scs-core-2.8.1/src/scs_core/client/sftp_client_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/climate/absolute_humidity.py` & `scs-core-2.8.1/src/scs_core/climate/absolute_humidity.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/climate/icp10101_datum.py` & `scs-core-2.8.1/src/scs_core/climate/icp10101_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/climate/mpl115a2_calib.py` & `scs-core-2.8.1/src/scs_core/climate/mpl115a2_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/climate/mpl115a2_datum.py` & `scs-core-2.8.1/src/scs_core/climate/mpl115a2_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/climate/pressure_conf.py` & `scs-core-2.8.1/src/scs_core/climate/pressure_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/climate/pressure_datum.py` & `scs-core-2.8.1/src/scs_core/climate/pressure_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/climate/sht_conf.py` & `scs-core-2.8.1/src/scs_core/climate/sht_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/climate/sht_datum.py` & `scs-core-2.8.1/src/scs_core/climate/sht_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/comms/mqtt_conf.py` & `scs-core-2.8.1/src/scs_core/comms/mqtt_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/comms/uds_client.py` & `scs-core-2.8.1/src/scs_core/comms/uds_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/comms/uds_reader.py` & `scs-core-2.8.1/src/scs_core/comms/uds_reader.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/comms/uds_server.py` & `scs-core-2.8.1/src/scs_core/comms/uds_server.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/comms/uds_writer.py` & `scs-core-2.8.1/src/scs_core/comms/uds_writer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/control/command.py` & `scs-core-2.8.1/src/scs_core/control/command.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/control/control_datum.py` & `scs-core-2.8.1/src/scs_core/control/control_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/control/control_handler.py` & `scs-core-2.8.1/src/scs_core/control/control_handler.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/control/control_receipt.py` & `scs-core-2.8.1/src/scs_core/control/control_receipt.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/csv/csv_archive.py` & `scs-core-2.8.1/src/scs_core/csv/csv_archive.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/csv/csv_dict.py` & `scs-core-2.8.1/src/scs_core/csv/csv_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         return len(self.__cells)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_dict(self, row):
         if len(row) != len(self):
-            raise ValueError("unmatched lengths: header: %s row: %s" % (self, row))
+            raise ValueError("unmatched lengths: header: %s row: %s" % (list(self.paths()), row))
 
         dictionary = OrderedDict()
 
         for i in range(len(row)):
             try:
                 self.__cells[i].insert(dictionary, row[i])
             except TypeError:
```

### Comparing `scs-core-2.4.6/src/scs_core/csv/csv_log.py` & `scs-core-2.8.1/src/scs_core/csv/csv_log.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/csv/csv_log_cursor_queue.py` & `scs-core-2.8.1/src/scs_core/csv/csv_log_cursor_queue.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/csv/csv_log_reader.py` & `scs-core-2.8.1/src/scs_core/csv/csv_log_reader.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/csv/csv_logger.py` & `scs-core-2.8.1/src/scs_core/csv/csv_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, host, log, manager, write_interval):
         """
         Constructor
         """
-        self.__host = host                              # Host
+        self.__host = host                              # PersistenceManager
         self.__log = log                                # CSVLog
         self.__manager = manager                        # CSVSpaceManager
         self.__write_interval = write_interval          # int
 
         self.__paths = None                             # array of string
         self.__file = None                              # file handle
         self.__latest_write = None                      # timestamp
@@ -187,15 +187,15 @@
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, host, log, delete_oldest, min_free_space, check_interval):
         self.__logger = Logging.getLogger()
 
-        self.__host = host                                          # Host
+        self.__host = host                                          # PersistenceManager
         self.__log = log                                            # CSVLog
         self.__delete_oldest = delete_oldest                        # bool
         self.__min_free_space = min_free_space                      # int
         self.__check_interval = check_interval                      # int
 
         self.__check_count = check_interval
```

### Comparing `scs-core-2.4.6/src/scs_core/csv/csv_logger_conf.py` & `scs-core-2.8.1/src/scs_core/csv/csv_logger_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/csv/csv_reader.py` & `scs-core-2.8.1/src/scs_core/csv/csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/csv/csv_writer.py` & `scs-core-2.8.1/src/scs_core/csv/csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/aggregate.py` & `scs-core-2.8.1/src/scs_core/data/aggregate.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/array_dict.py` & `scs-core-2.8.1/src/scs_core/data/array_dict.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/average.py` & `scs-core-2.8.1/src/scs_core/data/average.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/categorical_regression.py` & `scs-core-2.8.1/src/scs_core/data/categorical_regression.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/checkpoint_generator.py` & `scs-core-2.8.1/src/scs_core/data/checkpoint_generator.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/crc.py` & `scs-core-2.8.1/src/scs_core/data/crc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/crypt.py` & `scs-core-2.8.1/src/scs_core/data/crypt.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/datetime.py` & `scs-core-2.8.1/src/scs_core/data/datetime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/datum.py` & `scs-core-2.8.1/src/scs_core/data/datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/duplicates.py` & `scs-core-2.8.1/src/scs_core/data/duplicates.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Created on 2 Mar 2019
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
+import json
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class Duplicates(object):
     """
     classdocs
     """
@@ -21,24 +23,26 @@
         self.__matches = {}
         self.__max_index = 0
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def test(self, index, key, value):
+        jstr = json.dumps(key)
+
         # test...
-        if key not in self.__matches:
-            self.__matches[key] = {}
-            is_duplicate = False
+        if jstr in self.__matches:
+            is_duplicate = True
 
         else:
-            is_duplicate = True
+            self.__matches[jstr] = {}
+            is_duplicate = False
 
         # store..
-        self.__matches[key][index] = value
+        self.__matches[jstr][index] = value
 
         if index > self.__max_index:
             self.__max_index = index
 
         # report...
         return is_duplicate
 
@@ -81,14 +85,25 @@
             if len(self.__matches[key]) > 1:
                 count += 1
 
         return count
 
 
     @property
+    def total_matches(self):
+        count = 0
+
+        for key in self.__matches:
+            if len(self.__matches[key]) > 1:
+                count += len(self.__matches[key])
+
+        return count
+
+
+    @property
     def max_index(self):
         return self.__max_index
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
```

### Comparing `scs-core-2.4.6/src/scs_core/data/histogram.py` & `scs-core-2.8.1/src/scs_core/data/histogram.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/interval.py` & `scs-core-2.8.1/src/scs_core/data/interval.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/join.py` & `scs-core-2.8.1/src/scs_core/data/join.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/json.py` & `scs-core-2.8.1/src/scs_core/data/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,14 @@
     """
 
     _SECURITY_DELAY =       3.0                                 # seconds
 
     __AWS_DIR =             "aws"                               # hard-coded rel path
     __CONF_DIR =            "conf"                              # hard-coded rel path
     __HUE_DIR =             "hue"                               # hard-coded rel path
-    __OSIO_DIR =            "osio"                              # hard-coded rel path
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def aws_dir(cls):
         return cls.__AWS_DIR
 
@@ -266,19 +265,14 @@
 
 
     @classmethod
     def hue_dir(cls):
         return cls.__HUE_DIR
 
 
-    @classmethod
-    def osio_dir(cls):
-        return cls.__OSIO_DIR
-
-
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, last_modified=None):
         self._last_modified = last_modified                     # LocalizedDatetime
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-core-2.4.6/src/scs_core/data/lin_regress.py` & `scs-core-2.8.1/src/scs_core/data/lin_regress.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/linear_regression.py` & `scs-core-2.8.1/src/scs_core/data/linear_regression.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/low_pass_filter.py` & `scs-core-2.8.1/src/scs_core/data/low_pass_filter.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/median_filter.py` & `scs-core-2.8.1/src/scs_core/data/median_filter.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/min_list.py` & `scs-core-2.8.1/src/scs_core/data/min_list.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/model_delta.py` & `scs-core-2.8.1/src/scs_core/data/model_delta.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/path_dict.py` & `scs-core-2.8.1/src/scs_core/data/path_dict.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/precision.py` & `scs-core-2.8.1/src/scs_core/data/precision.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/publication.py` & `scs-core-2.8.1/src/scs_core/data/publication.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/queue_report.py` & `scs-core-2.8.1/src/scs_core/data/queue_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/recurring_period.py` & `scs-core-2.8.1/src/scs_core/data/recurring_period.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
 class RecurringDay(RecurringPeriod):
     """
     classdocs
     """
 
     @classmethod
     def valid_intervals(cls):
-        return (1, )
+        return 1,
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, interval):
         """
         Constructor
```

### Comparing `scs-core-2.4.6/src/scs_core/data/regression.py` & `scs-core-2.8.1/src/scs_core/data/regression.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/rtc_datetime.py` & `scs-core-2.8.1/src/scs_core/data/rtc_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/sample_delta.py` & `scs-core-2.8.1/src/scs_core/data/sample_delta.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/stats.py` & `scs-core-2.8.1/src/scs_core/data/stats.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/str.py` & `scs-core-2.8.1/src/scs_core/data/str.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/timedelta.py` & `scs-core-2.8.1/src/scs_core/data/timedelta.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/tokens.py` & `scs-core-2.8.1/src/scs_core/data/tokens.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/data/topic_path.py` & `scs-core-2.8.1/src/scs_core/data/topic_path.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/display/display_conf.py` & `scs-core-2.8.1/src/scs_core/display/display_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/email/email_queue.py` & `scs-core-2.8.1/src/scs_core/email/email_queue.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/email/email_queue_manager.py` & `scs-core-2.8.1/src/scs_core/email/email_queue_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/estate/baseline_conf.py` & `scs-core-2.8.1/src/scs_core/estate/baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/estate/configuration.py` & `scs-core-2.8.1/src/scs_core/estate/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 Created on 27 Jan 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
+    VERSION = 1.3
+
 example document:
 {
     "rec": "2023-02-28T12:25:24Z",
     "tag": "scs-bgx-431",
-    "ver": 1.2,
+    "ver": 1.3,
     "val": {
         "hostname": "scs-bbe-431",
         "os": {
             "rel": "4.19.173-bone60",
             "vers": "#1buster PREEMPT Tue Feb 16 23:42:12 UTC 2021"
         },
         "packs": {
@@ -215,17 +217,14 @@
                 "tally": 1
             },
             "scs-status": {
                 "interval": 60.0,
                 "tally": 1
             }
         },
-        "shared-secret": {
-            "key": "jYPAFZoQDiSJJ1Rl"
-        },
         "sht-conf": {
             "int": "0x45",
             "ext": "0x45"
         },
         "networks": {
             "cdc-wdm0": {
                 "kind": "gsm",
@@ -235,19 +234,19 @@
             "eth0": {
                 "kind": "ethernet",
                 "state": "unavailable",
                 "connection": null
             }
         },
         "modem": {
-            "id": "e3f0ca1c313dcbcf4d586a9c47dc4fd6c1cb46e6",
+            "id": "e3f0ca1c3134d586a9c47dc4fd6c1cb46e6",
             "imei": "866758042325619",
             "mfr": "QUALCOMM INCORPORATED",
             "model": "QUECTEL Mobile Broadband Module",
-            "rev": "EC25EFAR06A03M4G"
+            "rev": "EC2506A03M4G"
         },
         "sim": {
             "imsi": "234301951432536",
             "iccid": "8944303382697124815",
             "operator-code": "23430",
             "operator-name": "EE"
         },
@@ -316,26 +315,25 @@
 
 from scs_core.sync.schedule import Schedule
 
 from scs_core.sys.filesystem import FilesystemReport
 from scs_core.sys.modem import Modem, SIM
 from scs_core.sys.network import Networks
 from scs_core.sys.platform import PlatformSummary
-from scs_core.sys.shared_secret import SharedSecret
 from scs_core.sys.system_id import SystemID
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class Configuration(JSONable):
     """
     classdocs
     """
 
-    VERSION = 1.2
+    VERSION = 1.3
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def construct_from_jstr(cls, jstr):
         try:
             return cls.construct_from_jdict(json.loads(jstr))
@@ -349,15 +347,15 @@
             if skeleton:
                 return cls(None, None, None, None, None,
                            None, None, None, None, None,
                            None, None, None, None, None,
                            None, None, None, None, None,
                            None, None, None, None, None,
                            None, None, None, None, None,
-                           None, None, None, None)
+                           None, None, None)
             else:
                 return None
 
         hostname = jdict.get('hostname')
         platform = PlatformSummary.construct_from_jdict(jdict.get('os'))
         packs = PackageVersions.construct_from_jdict(jdict.get('packs'))
 
@@ -381,33 +379,32 @@
         pressure_conf = PressureConf.construct_from_jdict(jdict.get('pressure-conf'))
         psu_conf = PSUConf.construct_from_jdict(jdict.get('psu-conf'))
         psu_version = PSUVersion.construct_from_jdict(jdict.get('psu-version'))
         pt1000_calib = Pt1000Calib.construct_from_jdict(jdict.get('pt1000-calib'))
         scd30_baseline = SCD30Baseline.construct_from_jdict(jdict.get('scd30-baseline'))
         scd30_conf = SCD30Conf.construct_from_jdict(jdict.get('scd30-conf'))
         schedule = Schedule.construct_from_jdict(jdict.get('schedule'))
-        shared_secret = SharedSecret.construct_from_jdict(jdict.get('shared-secret'))
         sht_conf = SHTConf.construct_from_jdict(jdict.get('sht-conf'))
         networks = Networks.construct_from_jdict(jdict.get('networks'))
         modem = Modem.construct_from_jdict(jdict.get('modem'))
         sim = SIM.construct_from_jdict(jdict.get('sim'))
         system_id = SystemID.construct_from_jdict(jdict.get('system-id'))
         timezone_conf = TimezoneConf.construct_from_jdict(jdict.get('timezone-conf'))
 
         return cls(hostname, platform, packs, afe_baseline, afe_id, aws_group_config,
                    aws_project, data_log, display_conf, vcal_baseline, gas_baseline,
                    gas_model_conf, gps_conf, interface_conf, mpl115a2_calib,
                    mqtt_conf, ndir_conf, opc_conf, opc_version, pmx_model_conf,
                    pressure_conf, psu_conf, psu_version, pt1000_calib, scd30_baseline,
-                   scd30_conf, schedule, shared_secret, sht_conf, networks,
-                   modem, sim, system_id, timezone_conf)
+                   scd30_conf, schedule, sht_conf, networks, modem,
+                   sim, system_id, timezone_conf)
 
 
     @classmethod
-    def load(cls, manager, psu_version=None):
+    def load(cls, manager, psu_version=None, exclude_sim=False):
         csv_logger_conf = CSVLoggerConf.load(manager)
 
         hostname = socket.gethostname()
         platform = PlatformSummary.construct()
         packs = PackageVersions.construct_from_installation(manager.scs_path(), manager)
 
         afe_baseline = AFEBaseline.load(manager)
@@ -430,40 +427,39 @@
         pressure_conf = PressureConf.load(manager)
         psu_conf = PSUConf.load(manager)
         psu_version = psu_version
         pt1000_calib = Pt1000Calib.load(manager)
         scd30_baseline = SCD30Baseline.load(manager)
         scd30_conf = SCD30Conf.load(manager)
         schedule = Schedule.load(manager)
-        shared_secret = SharedSecret.load(manager)
         sht_conf = SHTConf.load(manager)
         networks = manager.networks()
         modem = manager.modem()
-        sim = manager.sim()
+        sim = None if exclude_sim else manager.sim()
         system_id = SystemID.load(manager)
         timezone_conf = TimezoneConf.load(manager)
 
         return cls(hostname, platform, packs, afe_baseline, afe_id, aws_group_config,
                    aws_project, data_log, display_conf, vcal_baseline, gas_baseline,
                    gas_model_conf, gps_conf, interface_conf, mpl115a2_calib,
                    mqtt_conf, ndir_conf, opc_conf, opc_version, pmx_model_conf,
                    pressure_conf, psu_conf, psu_version, pt1000_calib, scd30_baseline,
-                   scd30_conf, schedule, shared_secret, sht_conf, networks,
-                   modem, sim, system_id, timezone_conf)
+                   scd30_conf, schedule, sht_conf, networks, modem,
+                   sim, system_id, timezone_conf)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, hostname, platform, packs, afe_baseline, afe_id, aws_group_config,
                  aws_project, data_log, display_conf, vcal_baseline, gas_baseline,
                  gas_model_conf, gps_conf, interface_conf, mpl115a2_calib,
                  mqtt_conf, ndir_conf, opc_conf, opc_version, pmx_model_conf,
                  pressure_conf, psu_conf, psu_version, pt1000_calib, scd30_baseline,
-                 scd30_conf, schedule, shared_secret, sht_conf, networks,
-                 modem, sim, system_id, timezone_conf):
+                 scd30_conf, schedule, sht_conf, networks, modem,
+                 sim, system_id, timezone_conf):
         """
         Constructor
         """
 
         self.__hostname = hostname                                  # string
         self.__platform = platform                                  # PlatformSummary
         self.__packs = packs                                        # PackageVersions
@@ -488,15 +484,14 @@
         self.__pressure_conf = pressure_conf                        # PressureConf
         self.__psu_conf = psu_conf                                  # PSUConf
         self.__psu_version = psu_version                            # PSUVersion
         self.__pt1000_calib = pt1000_calib                          # Pt1000Calib
         self.__scd30_baseline = scd30_baseline                      # SCD30Baseline
         self.__scd30_conf = scd30_conf                              # SCD30Conf
         self.__schedule = schedule                                  # Schedule
-        self.__shared_secret = shared_secret                        # SharedSecret
         self.__sht_conf = sht_conf                                  # SHTConf
         self.__networks = networks                                  # Networks
         self.__modem = modem                                        # Modem
         self.__sim = sim                                            # SIM
         self.__system_id = system_id                                # SystemID
         self.__timezone_conf = timezone_conf                        # TimezoneConf
 
@@ -512,31 +507,30 @@
                    self.interface_conf == other.interface_conf and self.mpl115a2_calib == other.mpl115a2_calib and \
                    self.mqtt_conf == other.mqtt_conf and self.ndir_conf == other.ndir_conf and \
                    self.opc_conf == other.opc_conf and self.pmx_model_conf == other.pmx_model_conf and \
                    self.pmx_model_conf == other.pmx_model_conf and self.pressure_conf == other.pressure_conf and \
                    self.psu_conf == other.psu_conf and self.psu_version == other.psu_version and \
                    self.pt1000_calib == other.pt1000_calib and self.scd30_baseline == other.scd30_baseline and \
                    self.scd30_conf == other.scd30_conf and self.schedule == other.schedule and \
-                   self.shared_secret == other.shared_secret and self.sht_conf == other.sht_conf and \
-                   self.networks == other.networks and self.modem == other.modem and \
-                   self.sim == other.sim and self.system_id == other.system_id and \
-                   self.timezone_conf == other.timezone_conf
+                   self.sht_conf == other.sht_conf and self.networks == other.networks and \
+                   self.modem == other.modem and self.sim == other.sim and \
+                   self.system_id == other.system_id and self.timezone_conf == other.timezone_conf
 
         except (TypeError, AttributeError):
             return False
 
 
     def diff(self, other):
         diff = Configuration(None, None, None, None, None,
                              None, None, None, None, None,
                              None, None, None, None, None,
                              None, None, None, None, None,
                              None, None, None, None, None,
                              None, None, None, None, None,
-                             None, None, None, None)
+                             None, None, None)
 
         if self.hostname != other.hostname:
             diff.__hostname = self.hostname
 
         if self.platform != other.platform:
             diff.__platform = self.platform
 
@@ -608,17 +602,14 @@
 
         if self.scd30_conf != other.scd30_conf:
             diff.__scd30_conf = self.scd30_conf
 
         if self.schedule != other.schedule:
             diff.__schedule = self.schedule
 
-        if self.shared_secret != other.shared_secret:
-            diff.__shared_secret = self.shared_secret
-
         if self.sht_conf != other.sht_conf:
             diff.__sht_conf = self.sht_conf
 
         if self.networks != other.networks:
             diff.__networks = self.networks
 
         if self.modem != other.modem:
@@ -716,17 +707,14 @@
 
         if self.scd30_conf:
             self.scd30_conf.save(manager)
 
         if self.schedule:
             self.schedule.save(manager)
 
-        if self.shared_secret:
-            self.shared_secret.save(manager)
-
         if self.sht_conf:
             self.sht_conf.save(manager)
 
         if self.networks:
             raise ValueError('networks may not be set')
 
         if self.modem:
@@ -771,16 +759,14 @@
         jdict['pressure-conf'] = self.pressure_conf
         jdict['psu-conf'] = self.psu_conf
         jdict['psu-version'] = self.psu_version
         jdict['pt1000-calib'] = self.pt1000_calib
         jdict['scd30-baseline'] = self.scd30_baseline
         jdict['scd30-conf'] = self.scd30_conf
         jdict['schedule'] = self.schedule
-        jdict['shared-secret'] = self.shared_secret
-        jdict['sht-conf'] = self.sht_conf
         jdict['sht-conf'] = self.sht_conf
         jdict['networks'] = self.networks
         jdict['modem'] = self.modem
         jdict['sim'] = self.sim
         jdict['system-id'] = self.system_id
         jdict['timezone-conf'] = self.timezone_conf
 
@@ -921,19 +907,14 @@
 
     @property
     def schedule(self):
         return self.__schedule
 
 
     @property
-    def shared_secret(self):
-        return self.__shared_secret
-
-
-    @property
     def sht_conf(self):
         return self.__sht_conf
 
 
     @property
     def networks(self):
         return self.__networks
@@ -963,16 +944,16 @@
 
     def __str__(self, *args, **kwargs):
         return "Configuration:{hostname:%s, platform:%s, packs:%s, afe_baseline:%s, afe_id:%s, aws_group_config:%s, " \
                "aws_project:%s, data_log:%s, display_conf:%s, vcal_baseline:%s, gas_baseline:%s, " \
                "gas_model_conf:%s, gps_conf:%s, interface_conf:%s, mpl115a2_calib:%s, " \
                "mqtt_conf:%s, ndir_conf:%s, opc_conf:%s, opc_version:%s, pmx_model_conf:%s, " \
                "pressure_conf:%s, psu_conf:%s, psu_version:%s, pt1000_calib:%s, scd30_baseline:%s, " \
-               "scd30_conf:%s, schedule:%s, shared_secret:%s, sht_conf:%s, networks:%s,  " \
-               "modem:%s, sim:%s, system_id:%s, timezone_conf:%s}" % \
+               "scd30_conf:%s, schedule:%s, sht_conf:%s, networks:%s, modem:%s, " \
+               "sim:%s, system_id:%s, timezone_conf:%s}" % \
                (self.hostname, self.platform, self.packs, self.afe_baseline, self.afe_id, self.aws_group_config,
                 self.aws_project, self.data_log, self.display_conf, self.vcal_baseline, self.gas_baseline,
                 self.gas_model_conf, self.gps_conf, self.interface_conf, self.mpl115a2_calib,
                 self.mqtt_conf, self.ndir_conf, self.opc_conf, self.opc_version, self.pmx_model_conf,
                 self.pressure_conf, self.psu_conf, self.psu_version, self.pt1000_calib, self.scd30_baseline,
-                self.scd30_conf, self.schedule, self.shared_secret, self.sht_conf, self.networks,
-                self.modem, self.sim, self.system_id, self.timezone_conf)
+                self.scd30_conf, self.schedule, self.sht_conf, self.networks, self.modem,
+                self.sim, self.system_id, self.timezone_conf)
```

### Comparing `scs-core-2.4.6/src/scs_core/estate/configuration_check.py` & `scs-core-2.8.1/src/scs_core/estate/configuration_check.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/estate/git_pull.py` & `scs-core-2.8.1/src/scs_core/estate/git_pull.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/estate/git_pull_check.py` & `scs-core-2.8.1/src/scs_core/estate/git_pull_check.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/estate/mqtt_device_poller.py` & `scs-core-2.8.1/src/scs_core/estate/mqtt_device_poller.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, host, s3_manager, dynamo_client=None, dynamo_resource=None):
         """
         Constructor
         """
-        self.__host = host
+        self.__host = host                                          # PersistenceManager
         self.__s3_manager = s3_manager
         self.__dynamo_manager = DynamoManager(dynamo_client, dynamo_resource) if dynamo_client and dynamo_resource \
             else None
 
         self.__logger = logging.getLogger()
```

### Comparing `scs-core-2.4.6/src/scs_core/estate/mqtt_peer.py` & `scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,233 +1,184 @@
 """
-Created on 8 Mar 2019
+Created on 9 Dec 2020
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-example:
-{"peers": {"scs-bbe-002": {"hostname": "scs-bbe-002", "tag": "scs-be2-2", "shared-secret": "secret1",
-"topic": "south-coast-science-dev/production-test/device/alpha-bb-eng-000002/control"}}
+The A4CalibratedDatum is a normalised electrochem output voltage. Its vCal field represents the calibrated weV
+minus the calibrated aeV.
+
+(Obsolete: The vXCal field should only be computed when the NO2 concentration is known precisely, so this should be
+done in the preprocessing phase for the O3 model.)
+
+example document:
+{"weV": 0.39519, "aeV": 0.39963, "weC": 0.00627, "cnc": 61.9, "vCal": -9.801, "xCal": -12.601}
 """
 
 from collections import OrderedDict
 
-from scs_core.data.json import JSONable, PersistentJSONable
-from scs_core.data.str import Str
+from scs_core.data.datum import Datum
+
+from scs_core.gas.a4.a4_calib import A4Calib
+from scs_core.gas.a4.a4_datum import A4Datum
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class MQTTPeer(JSONable):
+class A4Calibrator(object):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    @classmethod
-    def construct_from_jdict(cls, jdict):
-        if not jdict:
-            return None
+    def __init__(self, calib: A4Calib):
+        """
+        Constructor
+        """
+        self.__we_elc_v = round(calib.we_elc_mv / 1000.0, 3)                        # we_electronic_zero_mv
+        self.__ae_elc_v = round(calib.ae_elc_mv / 1000.0, 3)                        # ae_electronic_zero_mv
 
-        hostname = jdict.get('hostname')
-        tag = jdict.get('tag')
-        shared_secret = jdict.get('shared-secret')
-        topic = jdict.get('topic')
+        self.__we_sens_v = round(calib.we_sens_mv / 1000.0, 6)                      # we_sensitivity_mv_ppb
 
-        return MQTTPeer(hostname, tag, shared_secret, topic)
+        if calib.is_ox_sensor():
+            self.__we_no2_x_sens_v = round(calib.we_no2_x_sens_mv / 1000.0, 6)      # we_cross_sensitivity_no2_mv_ppb
+        else:
+            self.__we_no2_x_sens_v = None
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, hostname, tag, shared_secret, topic):
-        """
-        Constructor
-        """
-        self.__hostname = hostname                              # string
-        self.__tag = tag                                        # string
-        self.__shared_secret = shared_secret                    # string
-        self.__topic = topic                                    # string
-
+    def calibrate(self, datum):
+        v_cal = self.__calibrate(datum, self.we_sens_v)
+        x_cal = self.__calibrate(datum, self.we_no2_x_sens_v)
 
-    # ----------------------------------------------------------------------------------------------------------------
+        return A4CalibratedDatum(datum.we_v, datum.ae_v, datum.we_c, datum.cnc, v_cal, x_cal=x_cal)
 
-    def as_json(self):
-        jdict = OrderedDict()
 
-        jdict['hostname'] = self.hostname
-        jdict['tag'] = self.tag
-        jdict['shared-secret'] = self.shared_secret
-        jdict['topic'] = self.topic
+    def __calibrate(self, datum, we_sens_v):
+        if we_sens_v is None:
+            return None
 
-        return jdict
+        # zero offset...
+        we_v_zero_cal = datum.we_v - self.we_elc_v
+        ae_v_zero_cal = datum.ae_v - self.ae_elc_v
 
+        # remove noise...
+        v_zero_cal = we_v_zero_cal - ae_v_zero_cal
 
-    # ----------------------------------------------------------------------------------------------------------------
+        # gain...
+        return v_zero_cal / we_sens_v
 
-    @property
-    def hostname(self):
-        return self.__hostname
 
+    def set_we_v_zero_x_cal(self, datum, no2_cnc):
+        # we_v_x = no2_cnc * self.we_no2_x_sens_v
+        # datum.we_v_zero_x_cal = we_v_x - self.we_elc_v
+        pass
 
-    @property
-    def tag(self):
-        return self.__tag
 
+    # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def shared_secret(self):
-        return self.__shared_secret
+    def we_elc_v(self):
+        return self.__we_elc_v
 
 
-    @shared_secret.setter
-    def shared_secret(self, shared_secret):
-        self.__shared_secret = shared_secret
+    @property
+    def ae_elc_v(self):
+        return self.__ae_elc_v
 
 
     @property
-    def topic(self):
-        return self.__topic
+    def we_sens_v(self):
+        return self.__we_sens_v
 
 
-    @topic.setter
-    def topic(self, topic):
-        self.__topic = topic
+    @property
+    def we_no2_x_sens_v(self):
+        return self.__we_no2_x_sens_v
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "MQTTPeer:{hostname:%s, tag:%s, shared_secret:%s, topic:%s}" % \
-               (self.hostname, self.tag, self.shared_secret, self.topic)
+        return "A4Calibrator:{we_elc_v:%s, ae_elc_v:%s, we_sens_v:%s, we_no2_x_sens_v:%s}" % \
+               (self.we_elc_v, self.ae_elc_v, self.we_sens_v, self.we_no2_x_sens_v)
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class MQTTPeerSet(PersistentJSONable):
+class A4CalibratedDatum(A4Datum):
     """
     classdocs
     """
 
-    __FILENAME =    "mqtt_peers.json"
-
-    @classmethod
-    def persistence_location(cls):
-        return cls.conf_dir(), cls.__FILENAME
-
-
-    @classmethod
-    def load(cls, manager, encryption_key=None, skeleton=False):
-        instance = super().load(manager, encryption_key=encryption_key, skeleton=skeleton)
-
-        if instance is None:
-            instance = cls(OrderedDict())
-
-        return instance
-
-
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
-    def construct_from_jdict(cls, jdict, skeleton=False):
+    def construct_from_jdict(cls, jdict):
         if not jdict:
             return None
 
-        peers = OrderedDict()
-
-        for hostname, item in jdict.get('peers').items():
-            peer = MQTTPeer.construct_from_jdict(item)
+        we_v = jdict.get('weV')
+        ae_v = jdict.get('aeV')
+        we_c = jdict.get('weC')
+        cnc = jdict.get('cnc')
 
-            peers[hostname] = peer
+        v_cal = jdict.get('vCal')
+        x_cal = jdict.get('xCal')
 
-        return cls(peers)
+        return cls(we_v, ae_v, we_c, cnc, v_cal, x_cal)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, peers):
+    def __init__(self, we_v, ae_v, we_c, cnc, v_cal, x_cal=None):
         """
         Constructor
         """
-        super().__init__()
-
-        self.__peers = peers                                # OrderedDict of string: MQTTPeer
-
+        super().__init__(we_v, ae_v, we_c, cnc)
 
-    def __len__(self):
-        return len(self.__peers)
+        self.__v_cal = Datum.float(v_cal, 3)                        # calibrated ppb
+        self.__x_cal = Datum.float(x_cal, 3)                        # calibrated ppb according to cross-sensitivity
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         jdict = OrderedDict()
 
-        jdict['peers'] = self.__peers
-
-        return jdict
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    def insert(self, peer: MQTTPeer):
-        # add...
-        self.__peers[peer.hostname] = peer
-
-        # sort...
-        peers = OrderedDict()
+        jdict['weV'] = self.we_v
+        jdict['aeV'] = self.ae_v
+        jdict['weC'] = self.we_c                                # may be None
+        jdict['cnc'] = self.cnc                                 # may be None
 
-        for hostname in sorted(self.__peers.keys()):
-            peers[hostname] = self.__peers[hostname]
+        if self.v_cal is not None:
+            jdict['vCal'] = self.v_cal
 
-        self.__peers = peers
+        if self.x_cal is not None:
+            jdict['xCal'] = self.x_cal
 
-
-    def remove(self, hostname):
-        try:
-            del(self.__peers[hostname])
-            return True
-
-        except KeyError:
-            return False
+        return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def subset(self, hostname_substring=None, topic_substring=None):
-        subset = OrderedDict()
-
-        for hostname, peer in self.__peers.items():
-            if hostname_substring is not None and hostname_substring not in hostname:
-                continue
-
-            if topic_substring is not None and topic_substring not in peer.topic:
-                continue
-
-            subset[peer.hostname] = peer
-
-        return MQTTPeerSet(subset)
-
-
-    def peer(self, hostname):
-        try:
-            return self.__peers[hostname]
-        except KeyError:
-            return None
-
+    @property
+    def v_cal(self):
+        return self.__v_cal
 
-    def peer_by_tag(self, tag):
-        for peer in self.__peers.values():
-            if peer.tag == tag:
-                return peer
 
-        return None
+    @property
+    def x_cal(self):
+        return self.__x_cal
 
 
-    @property
-    def peers(self):
-        return tuple(self.__peers.values())
+    # @x_cal.setter
+    # def x_cal(self, x_cal):
+    #     self.__x_cal = round(x_cal, 9)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "MQTTPeerSet:{peers:%s}" % Str.collection(self.__peers)
+        return "A4CalibratedDatum:{we_v:%s, ae_v:%s, we_c:%s, cnc:%s, v_cal:%s, x_cal:%s}" % \
+               (self.we_v, self.ae_v, self.we_c, self.cnc, self.v_cal, self.x_cal)
```

### Comparing `scs-core-2.4.6/src/scs_core/estate/package_version.py` & `scs-core-2.8.1/src/scs_core/estate/package_version.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/exegesis/gas/exegete_catalogue.py` & `scs-core-2.8.1/src/scs_core/exegesis/gas/exegete_catalogue.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/exegesis/gas/exegete_collection.py` & `scs-core-2.8.1/src/scs_core/exegesis/gas/exegete_collection.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/exegesis/particulate/exegete_catalogue.py` & `scs-core-2.8.1/src/scs_core/exegesis/particulate/exegete_catalogue.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/exegesis/particulate/exegete_collection.py` & `scs-core-2.8.1/src/scs_core/exegesis/particulate/exegete_collection.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/exegesis/particulate/text.py` & `scs-core-2.8.1/src/scs_core/exegesis/particulate/text.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/a4/a4.py` & `scs-core-2.8.1/src/scs_core/gas/a4/a4.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     @classmethod
     def init(cls):
         cls.SENSORS[cls.CODE_CO] =      A4(cls.CODE_CO,     'CO A4',    'CO',   3)
         cls.SENSORS[cls.CODE_H2S] =     A4(cls.CODE_H2S,    'H2SA4',    'H2S',  3)
         cls.SENSORS[cls.CODE_NO] =      A4(cls.CODE_NO,     'NO A4',    'NO',   3)
         cls.SENSORS[cls.CODE_NO2] =     A4(cls.CODE_NO2,    'NO2A43F',  'NO2',  3)      # was NOGA4
-        cls.SENSORS[cls.CODE_OX] =      A4(cls.CODE_OX,     'OXA431',   'Ox',   3)      # was OXGA4
+        cls.SENSORS[cls.CODE_OX] =      A4(cls.CODE_OX,     'OXA431',   'Ox',   3)      # was OXGA4, ref in A4Calib
         cls.SENSORS[cls.CODE_SO2] =     A4(cls.CODE_SO2,    'SO2A4',    'SO2',  3)
 
         cls.SENSORS[cls.CODE_VOCe] =    A4(cls.CODE_VOCe,   'VOCA4',    'VOCe', 3)
 
         cls.SENSORS[cls.CODE_TEST_1] =  A4(cls.CODE_TEST_1, 'TEST',     'SN1',  3)
         cls.SENSORS[cls.CODE_TEST_2] =  A4(cls.CODE_TEST_2, 'TEST',     'SN2',  3)
         cls.SENSORS[cls.CODE_TEST_3] =  A4(cls.CODE_TEST_3, 'TEST',     'SN3',  3)
```

### Comparing `scs-core-2.4.6/src/scs_core/gas/a4/a4_calib.py` & `scs-core-2.8.1/src/scs_core/gas/a4/a4_calib.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 """
 Created on 24 Sep 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
+
+document example:
+{"serial_number": "212810464", "sensor_type": "NOGA4", "we_electronic_zero_mv": 300, "we_sensor_zero_mv": 0,
+"we_total_zero_mv": 300, "ae_electronic_zero_mv": 300, "ae_sensor_zero_mv": 0, "ae_total_zero_mv": 300,
+"we_sensitivity_na_ppb": -0.445, "we_cross_sensitivity_no2_na_ppb": "n/a", "pcb_gain": -0.7,
+"we_sensitivity_mv_ppb": 0.325, "we_cross_sensitivity_no2_mv_ppb": 0.324}
 """
 
 from collections import OrderedDict
 
 from scs_core.data.datum import Datum
+
 from scs_core.gas.sensor_calib import SensorCalib
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class A4Calib(SensorCalib):
     """
     classdocs
     """
+    __NO2_CROSS_SENSITIVITY_TYPES = ['OXA431']
 
     __OX_SENSOR_PREFIX = 'OX'
 
     __CALIBRATED_GASES = ('CO', 'H2S', 'NO', 'NO2', 'Ox', 'SO2', 'VOCe')
 
     @classmethod
     def calibrated_gases(cls):
@@ -89,14 +97,16 @@
         self.__we_x_sens_na = Datum.float(we_x_sens_na, 3)          # WE cross-sensitivity                  nA
 
         self.__pcb_gain = Datum.float(pcb_gain, 3)                  # PCB gain                              mv / nA
 
         self.__we_sens_mv = Datum.float(we_sens_mv, 3)              # WE sensitivity                        mV / ppb
         self.__we_no2_x_sens_mv = Datum.float(we_no2_x_sens_mv, 3)  # WE cross-sensitivity                  mV / ppb
 
+        self.validate()
+
 
     def __eq__(self, other):
         try:
             return self.serial_number == other.serial_number and self.sensor_type == other.sensor_type and \
                    self.we_elc_mv == other.we_elc_mv and self.we_cal_mv == other.we_cal_mv and \
                    self.we_tot_mv == other.we_tot_mv and \
                    self.ae_elc_mv == other.ae_elc_mv and self.ae_cal_mv == other.ae_cal_mv and \
@@ -107,14 +117,36 @@
 
         except (TypeError, AttributeError):
             return False
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
+    def validate(self):
+        # sensitivity...
+        if self.we_sens_na == 0.0:
+            raise ValueError('%s - we_sensitivity_na_ppb: zero sensitivity' % self.sensor_type)
+
+        if self.pcb_gain == 0.0:
+            raise ValueError('%s - pcb_gain: zero sensitivity' % self.sensor_type)
+
+        if self.we_sens_mv == 0.0:
+            raise ValueError('%s - we_sensitivity_mv_ppb: zero sensitivity' % self.sensor_type)
+
+        # cross-sensitivity...
+        if self.has_no2_cross_sensitivity():
+            if self.we_x_sens_na is None or self.we_x_sens_na == 0.0:
+                raise ValueError('%s - we_cross_sensitivity_no2_na_ppb: zero sensitivity' % self.sensor_type)
+
+            if self.we_no2_x_sens_mv is None or self.we_no2_x_sens_mv == 0.0:
+                raise ValueError('%s - we_cross_sensitivity_no2_mv_ppb: zero sensitivity' % self.sensor_type)
+
+
+    # ----------------------------------------------------------------------------------------------------------------
+
     def set_defaults(self):
         if self.__we_elc_mv is None:
             self.__we_elc_mv = self.DEFAULT_WE_ELECTRONIC_ZERO_MV
 
         if self.__we_cal_mv is None:
             self.__we_cal_mv = self.DEFAULT_WE_SENSOR_ZERO_MV
 
@@ -138,16 +170,16 @@
         if self.__we_sens_na is None:
             return
 
         we_sens_mv = -0.7313 * self.__we_sens_na + -0.0006          # coefficients found from Alphasense calibrations
         self.__we_sens_mv = round(we_sens_mv, 3)
 
 
-    def reports_no2_cross_sensitivity(self):
-        return self.__we_no2_x_sens_mv is not None
+    def has_no2_cross_sensitivity(self):
+        return self.sensor_type in self.__NO2_CROSS_SENSITIVITY_TYPES
 
 
     def is_ox_sensor(self):
         return self.sensor_type.upper().startswith(self.__OX_SENSOR_PREFIX)
 
 
     # ----------------------------------------------------------------------------------------------------------------
@@ -163,20 +195,20 @@
         jdict['we_total_zero_mv'] = self.we_tot_mv
 
         jdict['ae_electronic_zero_mv'] = self.ae_elc_mv
         jdict['ae_sensor_zero_mv'] = self.ae_cal_mv
         jdict['ae_total_zero_mv'] = self.ae_tot_mv
 
         jdict['we_sensitivity_na_ppb'] = self.we_sens_na
-        jdict['we_cross_sensitivity_no2_na_ppb'] = self.we_x_sens_na if self.we_x_sens_na else "n/a"
+        jdict['we_cross_sensitivity_no2_na_ppb'] = "n/a" if self.we_x_sens_na is None else self.we_x_sens_na
 
         jdict['pcb_gain'] = self.pcb_gain
 
         jdict['we_sensitivity_mv_ppb'] = self.we_sens_mv
-        jdict['we_cross_sensitivity_no2_mv_ppb'] = self.we_no2_x_sens_mv if self.we_no2_x_sens_mv else "n/a"
+        jdict['we_cross_sensitivity_no2_mv_ppb'] = "n/a" if self.we_no2_x_sens_mv is None else self.we_no2_x_sens_mv
 
         return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
```

### Comparing `scs-core-2.4.6/src/scs_core/gas/a4/a4_calibrated_datum.py` & `scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum_vA.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 """
 Created on 9 Dec 2020
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-The A4CalibratedDatum is a normalised electrochem output voltage. Its vCal field represents the calibrated weV
-minus the calibrated aeV.
-
-(Obsolete: The vXCal field should only be computed when the NO2 concentration is known precisely, so this should be
-done in the preprocessing phase for the O3 model.)
-
-example document:
-{"weV": 0.39519, "aeV": 0.39963, "weC": 0.00627, "cnc": 61.9, "vCal": -9.801, "xCal": -12.601}
+The A4CalibratedDatum is designed to provide a model training data set that encapsulates the calibration of the
+electrochemical sensor - the fields we_v_cal, ae_v_zero_cal and cal_x_v have no meaning beyond this.
+cal_x_v is only relevant to sensors with NO2 cross-sensitivity.
 """
 
 from collections import OrderedDict
 
 from scs_core.data.datum import Datum
 
 from scs_core.gas.a4.a4_calib import A4Calib
@@ -30,155 +25,97 @@
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, calib: A4Calib):
         """
         Constructor
         """
-        self.__we_elc_v = round(calib.we_elc_mv / 1000.0, 3)                        # we_electronic_zero_mv
-        self.__ae_elc_v = round(calib.ae_elc_mv / 1000.0, 3)                        # ae_electronic_zero_mv
-
-        self.__we_sens_v = round(calib.we_sens_mv / 1000.0, 6)                      # we_sensitivity_mv_ppb
-
-        if calib.is_ox_sensor():
-            self.__we_no2_x_sens_v = round(calib.we_no2_x_sens_mv / 1000.0, 6)      # we_cross_sensitivity_no2_mv_ppb
-        else:
-            self.__we_no2_x_sens_v = None
+        self.__calib = calib                                                # A4Calib
 
+        self.__we_elc_v = calib.we_elc_mv / 1000.0
+        self.__ae_elc_v = calib.ae_elc_mv / 1000.0
 
-    # ----------------------------------------------------------------------------------------------------------------
-
-    def calibrate(self, datum):
-        v_cal = self.__calibrate(datum, self.we_sens_v)
-        x_cal = self.__calibrate(datum, self.we_no2_x_sens_v)
+        self.__we_sens_v = calib.we_sens_mv / 1000.0
 
-        return A4CalibratedDatum(datum.we_v, datum.ae_v, datum.we_c, datum.cnc, v_cal, x_cal=x_cal)
+        self.__we_no2_x_sens_v = None if calib.we_no2_x_sens_mv is None else calib.we_no2_x_sens_mv / 1000.0
 
 
-    def __calibrate(self, datum, we_sens_v):
-        if we_sens_v is None:
-            return None
+    # ----------------------------------------------------------------------------------------------------------------
 
+    def calibrate(self, datum, no2_cnc=None):
         # zero offset...
-        we_v_zero_cal = datum.we_v - self.we_elc_v
-        ae_v_zero_cal = datum.ae_v - self.ae_elc_v
+        we_v_zero_cal = datum.we_v - self.__we_elc_v
+        ae_v_zero_cal = datum.ae_v - self.__ae_elc_v
 
         # remove noise...
         v_zero_cal = we_v_zero_cal - ae_v_zero_cal
 
         # gain...
-        return v_zero_cal / we_sens_v
+        v_cal = v_zero_cal / self.__we_sens_v
 
+        # cross sensitivity...
+        v_x_cal = None if no2_cnc is None else no2_cnc * self.__we_no2_x_sens_v
 
-    def set_we_v_zero_x_cal(self, datum, no2_cnc):
-        # we_v_x = no2_cnc * self.we_no2_x_sens_v
-        # datum.we_v_zero_x_cal = we_v_x - self.we_elc_v
-        pass
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    @property
-    def we_elc_v(self):
-        return self.__we_elc_v
-
-
-    @property
-    def ae_elc_v(self):
-        return self.__ae_elc_v
-
-
-    @property
-    def we_sens_v(self):
-        return self.__we_sens_v
-
-
-    @property
-    def we_no2_x_sens_v(self):
-        return self.__we_no2_x_sens_v
+        return A4CalibratedDatum(datum.we_v, datum.ae_v, datum.we_c, datum.cnc, v_cal, v_x_cal)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "A4Calibrator:{we_elc_v:%s, ae_elc_v:%s, we_sens_v:%s, we_no2_x_sens_v:%s}" % \
-               (self.we_elc_v, self.ae_elc_v, self.we_sens_v, self.we_no2_x_sens_v)
+        return "A4Calibrator:{calib:%s}" % self.__calib
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class A4CalibratedDatum(A4Datum):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    @classmethod
-    def construct_from_jdict(cls, jdict):
-        if not jdict:
-            return None
-
-        we_v = jdict.get('weV')
-        ae_v = jdict.get('aeV')
-        we_c = jdict.get('weC')
-        cnc = jdict.get('cnc')
-
-        v_cal = jdict.get('vCal')
-        x_cal = jdict.get('xCal')
-
-        return cls(we_v, ae_v, we_c, cnc, v_cal, x_cal)
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    def __init__(self, we_v, ae_v, we_c, cnc, v_cal, x_cal=None):
+    def __init__(self, we_v, ae_v, we_c, cnc, v_cal, v_x_cal):
         """
         Constructor
         """
         super().__init__(we_v, ae_v, we_c, cnc)
 
-        self.__v_cal = Datum.float(v_cal, 3)                        # calibrated ppb
-        self.__x_cal = Datum.float(x_cal, 3)                        # calibrated ppb according to cross-sensitivity
+        self.__v_cal = Datum.float(v_cal, 6)                    # calibrated voltage
+        self.__v_x_cal = Datum.float(v_x_cal, 9)                # calibrated cross-sensitivity voltage
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         jdict = OrderedDict()
 
         jdict['weV'] = self.we_v
         jdict['aeV'] = self.ae_v
+
         jdict['weC'] = self.we_c                                # may be None
         jdict['cnc'] = self.cnc                                 # may be None
 
-        if self.v_cal is not None:
-            jdict['vCal'] = self.v_cal
+        jdict['vCal'] = self.v_cal
 
-        if self.x_cal is not None:
-            jdict['xCal'] = self.x_cal
+        if self.v_x_cal is not None:
+            jdict['vXCal'] = self.v_x_cal
 
         return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def v_cal(self):
         return self.__v_cal
 
 
     @property
-    def x_cal(self):
-        return self.__x_cal
-
-
-    # @x_cal.setter
-    # def x_cal(self, x_cal):
-    #     self.__x_cal = round(x_cal, 9)
+    def v_x_cal(self):
+        return self.__v_x_cal
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "A4CalibratedDatum:{we_v:%s, ae_v:%s, we_c:%s, cnc:%s, v_cal:%s, x_cal:%s}" % \
-               (self.we_v, self.ae_v, self.we_c, self.cnc, self.v_cal, self.x_cal)
+        return "A4CalibratedDatum(vA):{we_v:%s, ae_v:%s, we_c:%s, cnc:%s, v_cal:%s, v_x_cal:%s}" % \
+               (self.we_v, self.ae_v, self.we_c, self.cnc, self.v_cal, self.v_x_cal)
```

### Comparing `scs-core-2.4.6/src/scs_core/gas/a4/a4_calibrated_datum_v1.py` & `scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum_v1.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/a4/a4_calibrated_datum_vB.py` & `scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum_vB.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/a4/a4_calibrated_datum_vC.py` & `scs-core-2.8.1/src/scs_core/gas/a4/a4_calibrated_datum_vC.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/a4/a4_datum.py` & `scs-core-2.8.1/src/scs_core/gas/a4/a4_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/a4/a4_temp_comp.py` & `scs-core-2.8.1/src/scs_core/gas/a4/a4_temp_comp.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/afe/afe_datum.py` & `scs-core-2.8.1/src/scs_core/gas/afe/afe_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/afe/pt1000_calib.py` & `scs-core-2.8.1/src/scs_core/gas/afe/pt1000_calib.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/afe/pt1000_datum.py` & `scs-core-2.8.1/src/scs_core/gas/afe/pt1000_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/afe_baseline.py` & `scs-core-2.8.1/src/scs_core/gas/afe_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/afe_calib.py` & `scs-core-2.8.1/src/scs_core/gas/afe_calib.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 from scs_core.client.http_client import HTTPClient
 
 from scs_core.gas.afe.pt1000_calib import Pt1000Calib
 
 from scs_core.gas.sensor import Sensor
 from scs_core.gas.sensor_calib import SensorCalib
 
+from scs_core.sys.logging import Logging
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class CalibCurrency(object):
     """
     classdocs
     """
@@ -96,23 +98,28 @@
     def persistence_location(cls):
         return cls.conf_dir(), cls.__FILENAME
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
-    def download(cls, serial_number):
+    def download(cls, serial_number, parse=True):
         http_client = HTTPClient()
         http_client.connect(AFECalib.ALPHASENSE_HOST)
 
         try:
             path = AFECalib.ALPHASENSE_PATH + serial_number
-            jdict = json.loads(http_client.get(path, None, AFECalib.ALPHASENSE_HEADER))
+            response = http_client.get(path, None, AFECalib.ALPHASENSE_HEADER)
+
+            logger = Logging.getLogger()
+            logger.debug("afe response: %s" % response)
+
+            jdict = json.loads(response)
 
-            return cls.construct_from_jdict(jdict)
+            return cls.construct_from_jdict(jdict) if parse else jdict
 
         finally:
             http_client.close()
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-core-2.4.6/src/scs_core/gas/afe_id.py` & `scs-core-2.8.1/src/scs_core/gas/afe_id.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/d4/d4_datum.py` & `scs-core-2.8.1/src/scs_core/gas/d4/d4_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/dsi_calib.py` & `scs-core-2.8.1/src/scs_core/gas/dsi_calib.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 import json
 
 from scs_core.client.http_client import HTTPClient
 
 from scs_core.gas.afe_calib import AFECalib
 from scs_core.gas.sensor_calib import SensorCalib
 
+from scs_core.sys.logging import Logging
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class DSICalib(AFECalib):
     """
     classdocs
     """
@@ -37,23 +39,28 @@
                 "we_cross_sensitivity_no2_na_ppb": -0.3, "pcb_gain": -0.7, "we_sensitivity_mv_ppb": 0.2, 
                 "we_cross_sensitivity_no2_mv_ppb": "n/a"}}
                 '''
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
-    def download(cls, serial_number):
+    def download(cls, serial_number, parse=True):
         http_client = HTTPClient()
         http_client.connect(AFECalib.ALPHASENSE_HOST)
 
         try:
             path = SensorCalib.ALPHASENSE_PATH + serial_number
-            jstr = http_client.get(path, None, SensorCalib.ALPHASENSE_HEADER)
+            response = http_client.get(path, None, SensorCalib.ALPHASENSE_HEADER)
+
+            logger = Logging.getLogger()
+            logger.debug("dsi response: %s" % response)
+
+            jdict = json.loads(response)
 
-            return cls.construct_from_jdict(json.loads(jstr))
+            return cls.construct_from_jdict(jdict) if parse else jdict
 
         finally:
             http_client.close()
 
 
     # ----------------------------------------------------------------------------------------------------------------
```

### Comparing `scs-core-2.4.6/src/scs_core/gas/gas.py` & `scs-core-2.8.1/src/scs_core/gas/gas.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/isi/isi_datum.py` & `scs-core-2.8.1/src/scs_core/gas/isi/isi_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/minimum.py` & `scs-core-2.8.1/src/scs_core/gas/minimum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/ndir/ndir.py` & `scs-core-2.8.1/src/scs_core/gas/ndir/ndir.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/ndir/ndir_conf.py` & `scs-core-2.8.1/src/scs_core/gas/ndir/ndir_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/ndir/ndir_datum.py` & `scs-core-2.8.1/src/scs_core/gas/ndir/ndir_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/ndir/ndir_version.py` & `scs-core-2.8.1/src/scs_core/gas/ndir/ndir_version.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/ndir/ndir_voltages.py` & `scs-core-2.8.1/src/scs_core/gas/ndir/ndir_voltages.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/pid/pid.py` & `scs-core-2.8.1/src/scs_core/gas/pid/pid.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/pid/pid_calib.py` & `scs-core-2.8.1/src/scs_core/gas/pid/pid_calib.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class PIDCalib(SensorCalib):
     """
     classdocs
-
     """
 
     @classmethod
     def construct_from_jdict(cls, jdict, skeleton=False):
         if not jdict:
             return None
 
@@ -52,26 +51,35 @@
         Constructor
         """
         SensorCalib.__init__(self, serial_number, sensor_type)
 
         self.__pid_elc_mv = Datum.float(pid_elc_mv, 3)                  # PID electronic zero           mV
         self.__pid_sens_mv_ppm = Datum.float(pid_sens_mv_ppm, 6)        # PID sensitivity               mV / ppm
 
+        self.validate()
+
 
     def __eq__(self, other):
         try:
             return self.serial_number == other.serial_number and self.sensor_type == other.sensor_type and \
                    self.pid_elc_mv == other.pid_elc_mv and self.pid_sens_mv_ppm == other.pid_sens_mv_ppm
 
         except (TypeError, AttributeError):
             return False
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
+    def validate(self):
+        if self.pid_sens_mv_ppm == 0.0:
+            raise ValueError('%s - pid_sensitivity_mv_ppm: zero sensitivity' % self.sensor_type)
+
+
+    # ----------------------------------------------------------------------------------------------------------------
+
     def set_defaults(self):
         pass                                # PID may have null values
 
 
     def set_sens_mv_from_sens_na(self):
         pass                                # sensitivity nA data is not available
```

### Comparing `scs-core-2.4.6/src/scs_core/gas/pid/pid_calibrated_datum.py` & `scs-core-2.8.1/src/scs_core/gas/pid/pid_calibrated_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/pid/pid_datum.py` & `scs-core-2.8.1/src/scs_core/gas/pid/pid_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/pid/pid_temp_comp.py` & `scs-core-2.8.1/src/scs_core/gas/pid/pid_temp_comp.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/scd30/scd30_baseline.py` & `scs-core-2.8.1/src/scs_core/gas/scd30/scd30_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/scd30/scd30_conf.py` & `scs-core-2.8.1/src/scs_core/gas/scd30/scd30_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/scd30/scd30_datum.py` & `scs-core-2.8.1/src/scs_core/gas/scd30/scd30_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/sensor.py` & `scs-core-2.8.1/src/scs_core/gas/sensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     CODE_TEST_1 =       '01'            # test load
     CODE_TEST_2 =       '02'            # test load
     CODE_TEST_3 =       '03'            # test load
     CODE_TEST_4 =       '04'            # test load
 
     SENSORS =       {}
 
-
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def find(cls, serial_number):
         if serial_number is None:
             return None
 
@@ -73,15 +72,15 @@
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def has_no2_cross_sensitivity(self):
         if self.calib is None:
             return False
 
-        return self.calib.reports_no2_cross_sensitivity() and self.gas_name != 'NO2'
+        return self.calib.has_no2_cross_sensitivity()
 
 
     @abstractmethod
     def sample(self, afe, temp, index, no2_sample=None):
         pass
```

### Comparing `scs-core-2.4.6/src/scs_core/gas/sensor_baseline.py` & `scs-core-2.8.1/src/scs_core/gas/sensor_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/gas/sensor_calib.py` & `scs-core-2.8.1/src/scs_core/gas/sensor_calib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Created on 30 Sep 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
-from abc import ABC
+from abc import ABC, abstractmethod
 
 from scs_core.data.json import JSONable
 from scs_core.gas.sensor import Sensor
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
@@ -39,15 +39,15 @@
 
         raise ValueError(sensor_type)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
-    def reports_no2_cross_sensitivity(cls):                     # the default - override as necessary
+    def has_no2_cross_sensitivity(cls):                     # the default - override as necessary
         return False
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, serial_number, sensor_type):
         """
@@ -63,14 +63,21 @@
 
         except (TypeError, AttributeError):
             return False
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
+    @abstractmethod
+    def validate(self):
+        pass
+
+
+    # ----------------------------------------------------------------------------------------------------------------
+
     def sensor(self, baseline):
         sensor = Sensor.find(self.__serial_number)
 
         sensor.calib = self
         sensor.baseline = baseline
 
         return sensor
```

### Comparing `scs-core-2.4.6/src/scs_core/gps/gps_conf.py` & `scs-core-2.8.1/src/scs_core/gps/gps_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/interface/interface_conf.py` & `scs-core-2.8.1/src/scs_core/interface/interface_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/led/led.py` & `scs-core-2.8.1/src/scs_core/led/led.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/led/led_state.py` & `scs-core-2.8.1/src/scs_core/led/led_state.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/location/timezone.py` & `scs-core-2.8.1/src/scs_core/location/timezone.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/location/timezone_conf.py` & `scs-core-2.8.1/src/scs_core/location/timezone_conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Created on 11 Aug 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-The TimezoneConf subsystem enables the device user to set the reported timezone independently from the
+The TimezoneConf subsystem enables the device user to set the reported timezone independently of the
 system timezone. If no timezone_conf.json document is found, then the system "localzone" is used.
 
 https://stackoverflow.com/questions/13866926/python-pytz-list-of-timezones
 
 example JSON:
 {"set-on": "2017-08-12T11:20:28.740+00:00", "name": "Europe/London"}
 """
```

### Comparing `scs-core-2.4.6/src/scs_core/location/timezone_offset.py` & `scs-core-2.8.1/src/scs_core/location/timezone_offset.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/catalogue/model_compendium.py` & `scs-core-2.8.1/src/scs_core/model/catalogue/model_compendium.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/catalogue/model_compendium_group.py` & `scs-core-2.8.1/src/scs_core/model/catalogue/model_compendium_group.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/catalogue/term.py` & `scs-core-2.8.1/src/scs_core/model/catalogue/term.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/catalogue/training_period.py` & `scs-core-2.8.1/src/scs_core/model/catalogue/training_period.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/gas/baseline.py` & `scs-core-2.8.1/src/scs_core/model/gas/baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/gas/gas_baseline.py` & `scs-core-2.8.1/src/scs_core/model/gas/gas_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/gas/gas_inference_client.py` & `scs-core-2.8.1/src/scs_core/model/gas/gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/gas/gas_model_conf.py` & `scs-core-2.8.1/src/scs_core/model/gas/gas_model_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/gas/s1/gas_request.py` & `scs-core-2.8.1/src/scs_core/model/gas/s1/gas_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/gas/s1/s1_gas_inference_client.py` & `scs-core-2.8.1/src/scs_core/model/gas/s1/s1_gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/gas/vB/gas_request.py` & `scs-core-2.8.1/src/scs_core/model/gas/vB/gas_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/gas/vB/vb_gas_inference_client.py` & `scs-core-2.8.1/src/scs_core/model/gas/vB/vb_gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/gas/vE/gas_request.py` & `scs-core-2.8.1/src/scs_core/model/gas/vE/gas_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/gas/vE/ve_gas_inference_client.py` & `scs-core-2.8.1/src/scs_core/model/gas/vE/ve_gas_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/gas/vcal_baseline.py` & `scs-core-2.8.1/src/scs_core/model/gas/vcal_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/model_conf.py` & `scs-core-2.8.1/src/scs_core/model/model_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/pmx/pmx_inference_client.py` & `scs-core-2.8.1/src/scs_core/model/pmx/pmx_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/pmx/pmx_model_conf.py` & `scs-core-2.8.1/src/scs_core/model/pmx/pmx_model_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/pmx/s1/pmx_request.py` & `scs-core-2.8.1/src/scs_core/model/pmx/s1/pmx_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py` & `scs-core-2.8.1/src/scs_core/model/pmx/s1/s1_pmx_inference_client.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/monitor/monitor_error.py` & `scs-core-2.8.1/src/scs_core/monitor/monitor_error.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/monitor/monitor_request.py` & `scs-core-2.8.1/src/scs_core/monitor/monitor_request.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/monitor/monitor_response.py` & `scs-core-2.8.1/src/scs_core/monitor/monitor_response.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/osio/client/api_auth.py` & `scs-core-2.8.1/src/scs_core/sys/exception_report.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,100 @@
 """
-Created on 17 Nov 2016
+Created on 9 Jan 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-example document:
-{"org-id": "south-coast-science-test-user", "api-key": "9fdfb841-3433-45b8-b223-3f5a283ceb8e"}
+http://softwareengineering.stackexchange.com/questions/298364/exception-handling-in-python-am-i-doing-this-wrong-and-why
 """
 
+import sys
+import traceback
+
 from collections import OrderedDict
 
-from scs_core.data.json import PersistentJSONable
+from scs_core.data.json import JSONable
+from scs_core.data.str import Str
+
+from scs_core.sys.trace_entry import TraceEntry
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class APIAuth(PersistentJSONable):
+class ExceptionReport(JSONable):
     """
     classdocs
     """
 
-    __FILENAME = "osio_api_auth.json"
+    # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
-    def persistence_location(cls):
-        return cls.osio_dir(), cls.__FILENAME
+    def construct(cls, ex):
+        excls = ex.__class__
+        args = ex.args
 
+        info = sys.exc_info()
 
-    # ----------------------------------------------------------------------------------------------------------------
+        if len(info) < 3:
+            return ExceptionReport(excls, args, None, None)
 
-    @classmethod
-    def construct_from_jdict(cls, jdict, skeleton=False):
-        if not jdict:
-            return None
+        tb = info[2]
+        fe = traceback.format_exception(excls, ex, tb)
+        entries = [entry.strip() for entry in fe]
 
-        org_id = jdict.get('org-id')
-        api_key = jdict.get('api-key')
+        trace = [TraceEntry.construct(line) for line in entries[1:-1]]
+        summary = entries[-1]
 
-        return APIAuth(org_id, api_key)
+        return ExceptionReport(excls, args, trace, summary)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, org_id, api_key):
+    def __init__(self, cls, args, trace, summary):
         """
         Constructor
         """
-        super().__init__()
-
-        self.__org_id = org_id                  # String
-        self.__api_key = api_key                # String
+        self.__cls = cls
+        self.__args = args
+        self.__trace = trace
+        self.__summary = summary
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         jdict = OrderedDict()
 
-        jdict['org-id'] = self.org_id
-        jdict['api-key'] = self.api_key
+        jdict['cls'] = self.__class__.__name__
+        jdict['args'] = self.args
+        jdict['trace'] = self.trace
+        jdict['sum'] = self.summary
 
         return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def org_id(self):
-        return self.__org_id
+    def cls(self):
+        return self.__cls
+
+
+    @property
+    def trace(self):
+        return self.__trace
+
+
+    @property
+    def summary(self):
+        return self.__summary
 
 
     @property
-    def api_key(self):
-        return self.__api_key
+    def args(self):
+        return self.__args
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "APIAuth:{org_id:%s, api_key:%s}" % (self.org_id, self.api_key)
+        return "ExceptionReport:{cls:%s, args:%s, trace:%s, summary:%s}" % \
+               (self.__class__.__name__, Str.collection(self.args), Str.collection(self.trace), self.summary)
```

### Comparing `scs-core-2.4.6/src/scs_core/osio/client/client_auth.py` & `scs-core-2.8.1/src/scs_core/sys/platform.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,99 +1,91 @@
 """
-Created on 17 Nov 2016
+Created on 28 Feb 2023
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-example document:
-{"user_id": "southcoastscience-dev", "client-id": "5401", "client-password": "wtxSrs2e"}
+JSON example:
+{"rel": "4.19.103-bone47", "vers": "#1buster PREEMPT Thu Feb 20 17:40:41 UTC 2020"}
+
+https://docs.python.org/3/library/platform.html
 """
 
+import platform
+
 from collections import OrderedDict
 
-from scs_core.data.json import PersistentJSONable
+from scs_core.data.json import JSONable
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class ClientAuth(PersistentJSONable):
+class PlatformSummary(JSONable):
     """
     classdocs
     """
 
-    MQTT_HOST =        "mqtt.opensensors.io"          # hard-coded URL
-
-    MQTT_TIMEOUT =     20.0         # seconds
-
-
     # ----------------------------------------------------------------------------------------------------------------
 
-    __FILENAME = "osio_client_auth.json"
-
     @classmethod
-    def persistence_location(cls):
-        return cls.osio_dir(), cls.__FILENAME
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    @classmethod
-    def construct_from_jdict(cls, jdict, skeleton=False):
+    def construct_from_jdict(cls, jdict):
         if not jdict:
             return None
 
-        user_id = jdict.get('user-id')
+        release = jdict.get('rel')
+        version = jdict.get('vers')
+
+        return cls(release, version)
 
-        client_id = jdict.get('client-id')
-        client_password = jdict.get('client-password')
 
-        return ClientAuth(user_id, client_id, client_password)
+    @classmethod
+    def construct(cls):
+        uname = platform.uname()
+
+        return cls(uname.release, uname.version)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, user_id, client_id, client_password):
+    def __init__(self, release, version):
         """
         Constructor
         """
-        super().__init__()
+        self.__release = release                          # string
+        self.__version = version                          # string
+
 
-        self.__user_id = user_id                        # string
+    def __eq__(self, other):
+        try:
+            return self.release == other.release and self.version == other.version
 
-        self.__client_id = client_id                    # string
-        self.__client_password = client_password        # string
+        except (TypeError, AttributeError):
+            return False
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         jdict = OrderedDict()
 
-        jdict['user-id'] = self.user_id
-
-        jdict['client-id'] = self.client_id
-        jdict['client-password'] = self.client_password
+        jdict['rel'] = self.release
+        jdict['vers'] = self.version
 
         return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def user_id(self):
-        return self.__user_id
-
-
-    @property
-    def client_id(self):
-        return self.__client_id
+    def release(self):
+        return self.__release
 
 
     @property
-    def client_password(self):
-        return self.__client_password
+    def version(self):
+        return self.__version
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "ClientAuth:{user_id:%s, client_id:%s, client_password:%s}" % \
-                    (self.user_id, self.client_id, self.client_password)
+        return "PlatformSummary:{release:%s, version:%s}" %  \
+               (self.release, self.version)
```

### Comparing `scs-core-2.4.6/src/scs_core/osio/client/client_exception.py` & `scs-core-2.8.1/src/scs_core/aws/manager/device_monitor_specification_manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,68 @@
 """
-Created on 30 Mar 2017
+Created on 17 Jun 2023
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
-import json
+from scs_core.aws.client.api_client import APIClient
 
-from collections import OrderedDict
-
-from scs_core.data.json import JSONable
-from scs_core.osio.data.error import Error
+from scs_core.aws.data.device_monitor_email_list import DeviceMonitorEmailList
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class ClientException(RuntimeError, JSONable):
+class DeviceMonitorSpecificationManager(APIClient):
     """
     classdocs
     """
 
-    # ----------------------------------------------------------------------------------------------------------------
+    # TODO: update URL
+    __URL = "https://n0ctatmvjl.execute-api.us-west-2.amazonaws.com/default/DeviceMonitorSpecification"
 
-    @classmethod
-    def construct(cls, http_exception):
-        try:
-            jdict = json.loads(http_exception.data)
-        except ValueError:
-            return ClientException(None)
-
-        try:
-            error = Error.construct_from_jdict(jdict['error'])
-        except KeyError:
-            return ClientException(None)
+    # ----------------------------------------------------------------------------------------------------------------
 
-        return ClientException(error)
+    def __init__(self, http_client):
+        super().__init__(http_client)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, error, *args):
-        super().__init__(*args)
+    def find(self, token, email_address=None, device_tag_filter=None, exact=False):
+        payload = {
+            'email_address': email_address,
+            'device_tag': device_tag_filter,
+            'exact': exact
+        }
 
-        self.__error = error
+        response = self._http_client.get(self.__URL, headers=self._token_headers(token), json=payload)
+        self._check_response(response)
 
+        return DeviceMonitorEmailList(response.json())
 
-    # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
-        jdict = OrderedDict()
+    def add(self, token, email_address, device_tag):
+        payload = {
+            'email_address': email_address,
+            'device_tag': device_tag
+        }
 
-        jdict['error'] = self.error
+        response = self._http_client.post(self.__URL, headers=self._token_headers(token), json=payload)
+        self._check_response(response)
 
-        return jdict
+        return DeviceMonitorEmailList(response.json())      # only the updated entry is returned
 
 
-    # ----------------------------------------------------------------------------------------------------------------
+    def remove(self, token, email_address, device_tag=None):
+        payload = {
+            'email_address': email_address,
+            'device_tag': device_tag
+        }
 
-    @property
-    def error(self):
-        return self.__error
+        response = self._http_client.delete(self.__URL, headers=self._token_headers(token), json=payload)
+        self._check_response(response)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "ClientException:{error:%s}" % self.error
+        return "DeviceMonitorSpecificationManager:{}"
```

### Comparing `scs-core-2.4.6/src/scs_core/osio/data/derived_data.py` & `scs-core-2.8.1/src/scs_core/psu/psu_uptime.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,70 @@
 """
-Created on 2 Apr 2017
+Created on 8 Aug 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 example:
-"derived-data": {
-    "interval": 3600
-}
+{"secs": 57}
 """
 
 from collections import OrderedDict
 
+from scs_core.data.datum import Datum
 from scs_core.data.json import JSONable
+from scs_core.data.timedelta import Timedelta
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class DerivedData(JSONable):
+class PSUUptime(JSONable):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def construct_from_jdict(cls, jdict):
         if not jdict:
             return None
 
-        interval = int(jdict.get('interval'))
+        seconds = jdict.get('secs')
 
-        return DerivedData(interval)
+        return PSUUptime(seconds)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, interval):
+    def __init__(self, seconds):
         """
         Constructor
         """
-        self.__interval = interval                          # int
+        self.__seconds = Datum.int(seconds)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         jdict = OrderedDict()
 
-        jdict['interval'] = self.interval
+        jdict['period'] = self.timedelta
 
         return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def interval(self):
-        return self.__interval
+    def seconds(self):
+        return self.__seconds
+
+
+    @property
+    def timedelta(self):
+        return Timedelta(seconds=self.seconds)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "DerivedData:{interval:%s}" % self.interval
+        return "PSUUptime:{seconds:%s}" % self.seconds
```

### Comparing `scs-core-2.4.6/src/scs_core/osio/data/location.py` & `scs-core-2.8.1/src/scs_core/sys/system_temp.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,109 +1,78 @@
 """
-Created on 9 Nov 2016
+Created on 10 Jan 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
-
-example:
-"location": {
-    "lat": 50.819456,
-    "lon": -0.128336,
-    "postcode": "bn2 1af"
-}
 """
 
 from collections import OrderedDict
 
 from scs_core.data.json import JSONable
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class Location(JSONable):
+class SystemTemp(JSONable):
     """
     classdocs
-   """
+    """
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def construct_from_jdict(cls, jdict):
         if not jdict:
             return None
 
-        lat = jdict.get('lat')
-        lng = jdict.get('lon')
+        board = jdict.get('brd')
+        host = jdict.get('hst')
 
-        elevation = jdict.get('elevation')
+        return cls(board, host)
 
-        zipcode = jdict.get('zip')
-        postcode = jdict.get('postcode')
 
-        return Location(lat, lng, elevation, zipcode, postcode)
+    @classmethod
+    def construct(cls, board_datum, host_datum):
+        board = None if board_datum is None else board_datum.temp
+        host = None if host_datum is None else host_datum.temp
+
+        return cls(board, host)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, lat, lng, elevation, zipcode, postcode):
+    def __init__(self, board, host):
         """
         Constructor
         """
-        self.__lat = lat                    # float
-        self.__lng = lng                    # float
-
-        self.__elevation = elevation        # int
-
-        self.__zip = zipcode                # string
-        self.__postcode = postcode          # string
+        self.__board = board
+        self.__host = host                                          # PersistenceManager
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         jdict = OrderedDict()
 
-        jdict['lat'] = self.lat
-        jdict['lon'] = self.lng
-
-        if self.elevation is not None:
-            jdict['elevation'] = self.elevation
+        jdict['brd'] = self.board
 
-        if self.zip:
-            jdict['zip'] = self.zip
-
-        jdict['postcode'] = self.postcode
+        if self.host is not None:
+            jdict['hst'] = self.host
 
         return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def lat(self):
-        return self.__lat
-
-
-    @property
-    def lng(self):
-        return self.__lng
-
-
-    @property
-    def elevation(self):
-        return self.__elevation
-
-
-    @property
-    def zip(self):
-        return self.__zip
+    def board(self):
+        return self.__board
 
 
     @property
-    def postcode(self):
-        return None if self.__postcode is None else self.__postcode.upper()
+    def host(self):
+        return self.__host
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "Location:{lat:%s, lng:%s, elevation:%s, zip:%s, postcode:%s}" % \
-                        (self.lat, self.lng, self.elevation, self.zip, self.postcode)
+        return "SystemTemp:{board:%s, host:%s}" % (self.board, self.host)
```

### Comparing `scs-core-2.4.6/src/scs_core/osio/data/message_body.py` & `scs-core-2.8.1/src/scs_core/position/nmea/gptime.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 """
-Created on 7 Nov 2016
+Created on 1 Jan 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-example:
-25 June 2016 17:44:28 BST: {"datum":{"conc":92,"dens":184},"measured-at":"2016-06-25T17:41:01+01:00"}
+https://www.nmea.org
+https://en.wikipedia.org/wiki/NMEA_0183
 """
 
-from collections import OrderedDict
-
-from scs_core.data.json import JSONable
-
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class MessageBody(JSONable):
+class GPTime(object):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, data):
+    def __init__(self, time):
         """
         Constructor
         """
-        self.__data = data                  # string
+        self.__time = time                # string - hhmmss.ss
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
-        jdict = OrderedDict()
-
-        jdict['data'] = self.data
+    def as_iso8601(self):
+        """
+        example: 00:38:05.210Z
+        """
+        if self.__time is None:
+            return None
 
-        return jdict
+        return "%s:%s:%s0Z" % (self.__time[:2], self.__time[2:4], self.__time[4:])
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def data(self):
-        return self.__data
+    def time(self):
+        return self.__time
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "MessageBody:{data:%s}" % self.data
+        return "GPTime:{time:%s}" % self.time
```

### Comparing `scs-core-2.4.6/src/scs_core/osio/data/message_tag.py` & `scs-core-2.8.1/src/scs_core/particulate/opc_version.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,90 +1,93 @@
 """
-Created on 6 Mar 2017
+Created on 3 Sep 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-co-ordinated with scs_core.sys.DeviceID message_tag() method
+found from the OPC firmware
 
-example:
-scs-pfa-3
+example JSON:
+{"serial": "177336702", "firmware": "OPC-N3 Iss1.1 FirmwareVer=1.17a...........................BS"}
 """
 
-from scs_core.data.json import JSONable
+from collections import OrderedDict
+
+from scs_core.data.json import MultiPersistentJSONable
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class MessageTag(JSONable):
+class OPCVersion(MultiPersistentJSONable):
     """
     classdocs
     """
 
+    __FILENAME = "opc_version.json"
+
+    @classmethod
+    def persistence_location(cls, name):
+        filename = cls.__FILENAME if name is None else '_'.join((name, cls.__FILENAME))
+
+        return cls.conf_dir(), filename
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
-    def construct_from_jdict(cls, jdict):
+    def construct_from_jdict(cls, jdict, name=None, skeleton=False):
         if not jdict:
             return None
 
-        fields = jdict.split('-')
-
-        vendor_id = fields[0]
-        model_id = fields[1]
-        serial_number = int(fields[2])
-        signature = None                    # fields[3]
+        serial_no = jdict.get('serial')
+        firmware = jdict.get('firmware')
 
-        return MessageTag(vendor_id, model_id, serial_number, signature)
+        return cls(serial_no, firmware, name=name)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, vendor_id, model_id, serial_number, signature):
+    def __init__(self, serial_no, firmware, name=None):
         """
         Constructor
         """
-        self.__vendor_id = vendor_id                # string (3 chars)
-        self.__model_id = model_id                  # string (3 chars)
-        self.__serial_number = serial_number        # int
-        self.__signature = signature                # string
+        super().__init__(name)
 
+        self.__serial_no = serial_no                        # string
+        self.__firmware = firmware                          # string
 
-    # ----------------------------------------------------------------------------------------------------------------
 
-    def is_valid(self, message):
-        print("sig: %s msg: %s" % (self.signature, message))
-        return True
+    def __eq__(self, other):                                # ignore name
+        try:
+            return self.serial_no == other.serial_no and self.firmware == other.firmware
 
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    def as_json(self):
-        return self.vendor_id + '-' + self.model_id + '-' + self.serial_number + '-' + self.signature
+        except (TypeError, AttributeError):
+            return False
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def vendor_id(self):
-        return self.__vendor_id
+    def serial_no(self):
+        return self.__serial_no
 
 
     @property
-    def model_id(self):
-        return self.__model_id
+    def firmware(self):
+        return self.__firmware
 
 
-    @property
-    def serial_number(self):
-        return self.__serial_number
+    # ----------------------------------------------------------------------------------------------------------------
+
+    def as_json(self):
+        jdict = OrderedDict()
 
+        jdict['serial'] = self.serial_no
+        jdict['firmware'] = self.firmware
 
-    @property
-    def signature(self):
-        return self.__signature
+        return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "MessageTag:{vendor_id:%s, model_id:%s, serial_number:%s, signature:%s}" % \
-               (self.vendor_id, self.model_id, self.serial_number, self.signature)
+        return "OPCVersion:{name:%s, serial_no:%s, firmware:%s}" %  \
+               (self.name, self.serial_no, self.firmware)
```

### Comparing `scs-core-2.4.6/src/scs_core/osio/data/organisation.py` & `scs-core-2.8.1/src/scs_core/sys/shared_secret.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,104 +1,96 @@
 """
-Created on 8 Mar 2017
+Created on 2 Apr 2018
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-example:
-{
-  "id": "south-coast-science-dev",
-  "name": "South Coast Science  (dev)",
-  "website": "https://www.southcoastscience.com/",
-  "description": "Development operations for South Coast Science air quality monitoring instruments.",
-  "email": "bruno.beloff@southcoastscience.com"
-}
+https://stackoverflow.com/questions/2257441/
+random-string-generation-with-upper-case-letters-and-digits-in-python/23728630#23728630
+
+example document:
+{"key": "sxBhncFybpbMwZUa"}
 """
 
+import random
+import string
+
 from collections import OrderedDict
 
-from scs_core.data.json import JSONable
+from scs_core.data.json import PersistentJSONable
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class Organisation(JSONable):
+class SharedSecret(PersistentJSONable):
     """
     classdocs
-   """
+    """
+
+    __FILENAME = "shared_secret.json"
+
+    @classmethod
+    def persistence_location(cls):
+        return cls.conf_dir(), cls.__FILENAME
+
 
     # ----------------------------------------------------------------------------------------------------------------
 
+    __KEY_LENGTH = 16
+
     @classmethod
-    def construct_from_jdict(cls, jdict):
+    def generate(cls):
+        return ''.join(random.SystemRandom().choice(string.ascii_letters + string.digits)
+                       for _ in range(cls.__KEY_LENGTH))
+
+
+    # ----------------------------------------------------------------------------------------------------------------
+
+    @classmethod
+    def construct_from_jdict(cls, jdict, skeleton=False):
         if not jdict:
             return None
 
-        id = jdict.get('id')
-        name = jdict.get('name')
-        website = jdict.get('website')
-        description = jdict.get('description')
-        email = jdict.get('email')
+        key = jdict.get('key')
 
-        return Organisation(id, name, website, description, email)
+        return SharedSecret(key)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, id, name, website, description, email):
+    def __init__(self, key):
         """
         Constructor
         """
-        self.__id = id                          # string
-        self.__name = name                      # string
-        self.__website = website                # string
-        self.__description = description        # string
-        self.__email = email                    # string
-
-
-    # ----------------------------------------------------------------------------------------------------------------
+        super().__init__()
 
-    def as_json(self):
-        jdict = OrderedDict()
+        self.__key = key            # String
 
-        if self.id is not None:
-            jdict['id'] = self.id
 
-        jdict['name'] = self.name
-        jdict['website'] = self.website
-        jdict['description'] = self.description
-        jdict['email'] = self.email
+    def __eq__(self, other):
+        try:
+            return self.key == other.key
 
-        return jdict
+        except (TypeError, AttributeError):
+            return False
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    @property
-    def id(self):
-        return self.__id
-
-
-    @property
-    def name(self):
-        return self.__name
-
+    def as_json(self):
+        jdict = OrderedDict()
 
-    @property
-    def website(self):
-        return self.__website
+        jdict['key'] = self.key
 
+        return jdict
 
-    @property
-    def description(self):
-        return self.__description
 
+    # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def email(self):
-        return self.__email
+    def key(self):
+        return self.__key
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "Organisation:{id:%s, name:%s, website:%s, description:%s, email:%s}" % \
-               (self.id, self.name, self.website, self.description, self.email)
+        return "SharedSecret:{key:%s}" % self.key
```

### Comparing `scs-core-2.4.6/src/scs_core/osio/data/schema.py` & `scs-core-2.8.1/src/scs_core/sys/ipv4_address.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,72 @@
 """
-Created on 14 Feb 2017
+Created on 2 Mar 2020
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
-
-example:
-{
-    "id": 28,
-    "name": "south-coast-science-gases-Ox-NO2-NO-CO",
-    "description": "South Coast Science Air Quality Sensor; concentration of gases"
-}
 """
 
-from collections import OrderedDict
-
-from scs_core.data.json import JSONable
-
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class Schema(JSONable):
+class IPv4Address(object):
     """
     classdocs
-   """
+    """
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
-    def construct_from_jdict(cls, jdict):
-        if not jdict:
-            return None
+    def is_valid(cls, dot_decimal):
+        try:
+            octets = [int(octet) for octet in dot_decimal.split('.') if 0 <= int(octet) <= 255]
+        except (TypeError, ValueError):
+            return False
 
-        id = jdict.get('id')
-        name = jdict.get('name')
-        description = jdict.get('description')
+        if len(octets) != 4:
+            return False
 
-        return Schema(id, name, description)
+        return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, id, name, description):
-        """
-        Constructor
-        """
-        self.__id = id                          # int
-        self.__name = name                      # string
-        self.__description = description        # string
-
+    @classmethod
+    def construct(cls, dot_decimal):
+        if dot_decimal is None:
+            return None
 
-    # ----------------------------------------------------------------------------------------------------------------
+        octets = [int(octet) for octet in dot_decimal.split('.')]
 
-    def as_json(self):
-        jdict = OrderedDict()
+        return cls(octets)
 
-        jdict['id'] = self.id
-        jdict['name'] = self.name
 
-        if self.description is not None:
-            jdict['description'] = self.description
+    # ----------------------------------------------------------------------------------------------------------------
 
-        return jdict
+    def __init__(self, octets):
+        """
+        Constructor
+        """
+        self.__octets = octets                          # array of int
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    @property
-    def id(self):
-        return self.__id
+    def lso_range(self, start, end):
+        if not 0 < start < 255:
+            raise ValueError(start)
 
+        if not 0 < end < 255:
+            raise ValueError(end)
 
-    @property
-    def name(self):
-        return self.__name
+        for i in range(start, end + 1, 1):
+            yield IPv4Address(self.__octets[:-1] + [i])
 
 
-    @property
-    def description(self):
-        return self.__description
+    # ----------------------------------------------------------------------------------------------------------------
 
+    def dot_decimal(self):
+        return '.'.join([str(octet) for octet in self.__octets])
 
-    # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "Schema:{id:%s, name:%s, description:%s}" % (self.id, self.name, self.description)
+        return "IPv4Address:{%s}" %  self.dot_decimal()
+
```

### Comparing `scs-core-2.4.6/src/scs_core/osio/data/topic_contributor.py` & `scs-core-2.8.1/src/scs_core/position/nmea/nmea_report.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,83 +1,95 @@
 """
-Created on 10 Nov 2016
+Created on 31 Dec 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-example:
-{
-    "name": "South Coast Science - Dev",
-    "id": "southcoastscience-dev",
-    "gravatar-hash": "07f512e9fe64863039df0c0f1834cc25"
-}
-"""
-
-from collections import OrderedDict
+A helper class for validating and preparing GPS module output strings.
 
-from scs_core.data.json import JSONable
+https://www.nmea.org
+https://en.wikipedia.org/wiki/NMEA_0183
+"""
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class TopicContributor(JSONable):
+class NMEAReport(object):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
-    def construct_from_jdict(cls, jdict):
-        if not jdict:
-            return None
+    def checksum(cls, text):
+        cs = 0
+        for c in text[1:]:
+            cs ^= ord(c)
+
+        return cs
+
+
+    # ----------------------------------------------------------------------------------------------------------------
+
+    @classmethod
+    def construct(cls, line):
+        main = line.strip().split("*")
+
+        if len(main) != 2:
+            raise ValueError("malformed line:%s" % (line.strip()))
 
-        name = jdict.get('name')
-        id = jdict.get('id')
-        gravatar_hash = jdict.get('gravatar-hash')
+        fields = [item.strip() for item in main[0].split(",")]
+        cs = int(main[1], 16)
 
-        return TopicContributor(name, id, gravatar_hash)
+        if cs != cls.checksum(main[0]):
+            raise ValueError("invalid checksum:%s" % (line.strip()))
+
+        return NMEAReport(fields)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, name, id, gravatar_hash):
+    def __init__(self, fields):
         """
         Constructor
         """
-        self.__name = name                      # string
-        self.__id = id                          # string
-        self.__gravatar_hash = gravatar_hash    # string
+        self.__fields = fields
 
 
-    # ----------------------------------------------------------------------------------------------------------------
+    def __len__(self):
+        return len(self.__fields)
 
-    def as_json(self):
-        jdict = OrderedDict()
 
-        jdict['name'] = self.name
-        jdict['id'] = self.id
-        jdict['gravatar-hash'] = self.gravatar_hash
+    # ----------------------------------------------------------------------------------------------------------------
 
-        return jdict
+    @property
+    def message_id(self):
+        return self.str(0) if len(self) > 0 else None
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    @property
-    def name(self):
-        return self.__name
+    def int(self, index):
+        number_str = self.str(index)
+        number = None if number_str is None else int(number_str)
 
+        return number
 
-    @property
-    def id(self):
-        return self.__id
 
+    def float(self, index, precision):
+        index_str = self.str(index)
+        number = None if index_str is None else float(index_str)
 
-    @property
-    def gravatar_hash(self):
-        return self.__gravatar_hash
+        if number is None:
+            return None
+
+        return round(number, precision)
+
+
+    def str(self, index):
+        return self.__fields[index] if len(self.__fields[index]) > 0 else None
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "TopicContributor:{name:%s, id:%s, gravatar_hash:%s}" % (self.name, self.id, self.gravatar_hash)
+        return "NMEAReport:{fields:%s}" % self.__fields
```

### Comparing `scs-core-2.4.6/src/scs_core/osio/data/topic_info.py` & `scs-core-2.8.1/src/scs_core/aws/security/opr_membership.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,112 +1,72 @@
 """
-Created on 10 Nov 2016
+Created on 3 Apr 2023
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-example:
-{
-    "format": "application/json"
-}
+example document:
 """
 
 from collections import OrderedDict
 
+from scs_core.data.array_dict import ArrayDict
 from scs_core.data.json import JSONable
+from scs_core.data.str import Str
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class TopicInfo(JSONable):
+class OPRMembership(JSONable):
     """
     classdocs
-   """
-
-    FORMAT_JSON = "application/json"
-    FORMAT_TEXT = "text"
-
-
-    # ----------------------------------------------------------------------------------------------------------------
+    """
 
     @classmethod
-    def construct_from_jdict(cls, jdict):
-        if not jdict:
-            return None
-
-        topic_format = jdict.get('format')
-        topic_type = jdict.get('type')
-        schema = jdict.get('schema')
-        graph_path = jdict.get('graph-path')
+    def merge(cls, oprs, oups):
+        org_dict = ArrayDict([(oup.opr_id, oup) for oup in sorted(oups)])
 
-        return TopicInfo(topic_format, topic_type, schema, graph_path)
+        # OrganisationPathRoots...
+        return [cls(opr, org_dict.get(opr.opr_id)) for opr in oprs]
 
 
     # ----------------------------------------------------------------------------------------------------------------
-    # for the v2 API, schema_id goes in Topic...
 
-    def __init__(self, topic_format, topic_type=None, schema=None, graph_path=None):
+    def __init__(self, opr, memberships):
         """
         Constructor
         """
-        self.__format = topic_format        # string
-        self.__type = topic_type            # string
-        self.__schema = schema              # string
-        self.__graph_path = graph_path      # string
+        self.__opr = opr                                    # OrganisationPathRoot
+        self.__memberships = memberships                    # array of OrganisationUserPath
+
+
+    def __lt__(self, other):
+        return self.opr < other.opr
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         jdict = OrderedDict()
 
-        if self.format:
-            jdict['format'] = self.format
-
-        if self.type:
-            jdict['type'] = self.type
-
-        if self.schema:
-            jdict['schema'] = self.schema
-
-        if self.graph_path:
-            jdict['graph-path'] = self.graph_path
+        jdict['opr'] = self.opr
+        jdict['memberships'] = self.memberships
 
         return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def schema_id(self):
-        if self.__schema is None:
-            return None
-
-        return self.__schema.id
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    @property
-    def format(self):
-        return self.__format
-
-
-    @property
-    def type(self):
-        return self.__type
-
-
-    @property
-    def schema(self):
-        return self.__schema
+    def opr(self):
+        return self.__opr
 
 
     @property
-    def graph_path(self):
-        return self.__graph_path
+    def memberships(self):
+        return self.__memberships
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "TopicInfo:{format:%s, type:%s, schema:%s, graph_path:%s}" % \
-                    (self.format, self.type, self.schema, self.graph_path)
+        return "OPRMembership:{opr:%s, memberships:%s}" % \
+               (self.opr, Str.collection(self.memberships))
```

### Comparing `scs-core-2.4.6/src/scs_core/osio/data/user.py` & `scs-core-2.8.1/src/scs_core/sys/eeprom_image.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,131 +1,98 @@
 """
-Created on 21 Mar 2017
+Created on 25 Sep 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
-
-{
-  "id": "southcoastscience-dev",
-  "name": "South Coast Science - Dev",
-  "email": "opensensors-dev@southcoastscience.com",
-  "month": "2016-11"
-}
 """
 
-from collections import OrderedDict
-
-from scs_core.data.json import JSONable
+import struct
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class User(JSONable):
+class EEPROMImage(object):
     """
-    classdocs
-   """
+    Load a .eep file
+    """
+    @classmethod
+    def construct_from_file(cls, filename, min_size=0):
+        content = []
 
-    # ----------------------------------------------------------------------------------------------------------------
+        # file content...
+        f = open(filename, "rb")
 
-    @classmethod
-    def construct_from_jdict(cls, jdict, skeleton=False):
-        if not jdict:
+        try:
+            while True:
+                byte = f.read(1)
+
+                if not byte:
+                    break
+
+                content.append(struct.unpack('B', byte)[0])
+
+        except RuntimeError:
             return None
 
-        id = jdict.get('id')
-        name = jdict.get('name')
-        email = jdict.get('email')
-        
-        start = jdict.get('month')
+        finally:
+            f.close()
+
+        # padding...
+        if min_size and len(content) < min_size:
+            content += [0] * (min_size - len(content))
 
-        return User(id, name, email, None, start)
+        return EEPROMImage(content)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, id, name, email, password, start):
+    def __init__(self, content):
         """
         Constructor
         """
-        self.__id = id                  # string
-        self.__name = name              # string
-        self.__email = email            # string
-
-        self.__password = password      # string
-
-        self.__start = start            # string (year-month)
-
-
-    # ----------------------------------------------------------------------------------------------------------------
+        self.__content = content
 
-    def as_json(self):
-        jdict = OrderedDict()
 
-        if self.id is not None:
-            jdict['id'] = self.id
+    def __len__(self):
+        return len(self.__content)
 
-        if self.name is not None:
-            jdict['name'] = self.name
 
-        if self.email is not None:
-            jdict['email'] = self.email
+    def __eq__(self, other):
+        try:
+            return self.content == other.content
 
-        if self.password is not None:
-            jdict['password'] = self.password
+        except AttributeError:
+            return False
 
-        if self.start is not None:
-            jdict['month'] = self.start
 
-        return jdict
+    def __ne__(self, other):
+        return not self.__eq__(other)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def start_year(self):
-        if self.start is None:
-            return None
-
-        year = self.start.split('-')[0]
+    def formatted(self, width):
+        addr = 0
 
-        return int(year)
+        while addr < len(self.__content):
+            values = self.__content[addr: addr + width]
 
+            hexs = ' '.join("%02x" % value for value in values)
+            hexs = hexs.ljust(width * 3)
 
-    def start_month(self):
-        if self.start is None:
-            return None
+            chrs = ''.join(chr(value) if 31 < value < 128 else '.' for value in values)    # non-printable chars are '.'
 
-        month = self.start.split('-')[1]
+            print("0x%04x: %s        %s" % (addr, hexs, chrs))
 
-        return int(month)
+            addr += width
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def id(self):
-        return self.__id
-
-
-    @property
-    def name(self):
-        return self.__name
-
-
-    @property
-    def email(self):
-        return self.__email
-
-
-    @property
-    def password(self):
-        return self.__password
-
-
-    @property
-    def start(self):
-        return self.__start
+    def content(self):
+        return self.__content
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "User:{id:%s, name:%s, email:%s, password:%s, start:%s}" % \
-               (self.id, self.name, self.email, self.password, self.start)
+        return "EEPROMImage:{content:%s}" % self.content
```

### Comparing `scs-core-2.4.6/src/scs_core/osio/manager/message_manager.py` & `scs-core-2.8.1/src/scs_core/position/nmea/gpgga.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,158 +1,146 @@
 """
-Created on 13 Nov 2016
+Created on 30 Dec 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
-"""
 
-import sys
-import time
+Global positioning system fix data
+$xxGGA,time,lat,NS,long,EW,quality,numSV,HDOP,alt,M,sep,M,diffAge,diffStation*cs
+
+example sentence:
+$GPGGA,092725.00,4717.11399,N,00833.91590,E,1,08,1.01,499.6,M,48.0,M,,*5B
 
-import urllib.parse
+example values:
+GPGGA:{time:GPTime:{time:141058.00}, loc:GPLoc:{lat:5049.38432, ns:N, lng:00007.37801, ew:W}, quality:2, num_sv:06,
+hdop:3.10, alt:37.5, sep:45.4, diff_age:None, diff_station:0000}
 
-from scs_core.data.datetime import LocalizedDatetime
+GPGGA:{time:GPTime:{time:140047.00}, loc:GPLoc:{lat:None, ns:None, lng:None, ew:None}, quality:0, num_sv:00,
+hdop:99.99, alt:None, sep:None, diff_age:None, diff_station:None}
 
-from scs_core.osio.client.rest_client import RESTClient
-from scs_core.osio.data.message import Message
+https://www.nmea.org
+https://en.wikipedia.org/wiki/NMEA_0183
+"""
+
+from scs_core.position.nmea.gploc import GPLoc
+from scs_core.position.nmea.gptime import GPTime
+from scs_core.position.nmea.nmea_sentence import NMEASentence
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class MessageManager(object):
+class GPGGA(NMEASentence):
     """
     classdocs
     """
 
-    # ----------------------------------------------------------------------------------------------------------------
+    MESSAGE_IDS = ("$GNGGA", "$GPGGA")
 
-    def __init__(self, api_key, verbose=False):
-        """
-        Constructor
-        """
-        self.__rest_client = RESTClient(api_key)
-        self.__verbose = verbose
+    QUALITY_NO_FIX =                0
+    QUALITY_AUTONOMOUS_GNSS =       1
+    QUALITY_DIFFERENTIAL_GNSS =     2
+    QUALITY_ESTIMATED_FIX =         6
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def find_for_topic(self, topic, start_date, end_date, batch_pause=0.0):
-        request_path = '/v1/messages/topic/' + topic
-
-        total = 0
-        collection = []
+    @classmethod
+    def construct(cls, r):
+        if r.message_id not in cls.MESSAGE_IDS:
+            raise TypeError("invalid sentence:%s" % r)
 
-        # request...
-        self.__rest_client.connect()
+        time = GPTime(r.str(1))
 
-        try:
-            for batch in self.__find(request_path, start_date, end_date):
-                collection.extend(batch)
+        lat = r.str(2)
+        ns = r.str(3)
 
-                if self.__verbose:
-                    now = LocalizedDatetime.now().utc()
-                    batch_count = len(batch)
-                    total += batch_count
+        lng = r.str(4)
+        ew = r.str(5)
 
-                    print("%s: batch: %d total: %d" % (now.as_iso8601(), batch_count, total), file=sys.stderr)
-                    sys.stderr.flush()
+        loc = GPLoc(lat, ns, lng, ew)
 
-                time.sleep(batch_pause)     # prevent "Rate limit exceeded" error
+        quality = r.int(6)
+        num_sv = r.int(7)
+        hdop = r.float(8, 3)
+        alt = r.float(9, 2)
+        sep = r.float(11, 2)
 
-        finally:
-            self.__rest_client.close()
+        diff_age = r.float(13, 3)
+        diff_station = r.str(14)
 
-        return collection
+        return GPGGA(r.message_id, time, loc, quality, num_sv, hdop, alt, sep, diff_age, diff_station)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __find(self, request_path, start_date, end_date):
-        params = {'start-date': start_date.as_iso8601(), 'end-date': end_date.as_iso8601()}
-
-        while True:
-            # request...
-            jdict = self.__rest_client.get(request_path, params=params)
-
-            # messages...
-            msgs_jdict = jdict.get('messages')
-            messages = [Message.construct_from_jdict(msg_jdict) for msg_jdict in msgs_jdict] if msgs_jdict else []
-
-            yield messages
+    def __init__(self, message_id, time, loc, quality, num_sv, hdop, alt, sep, diff_age, diff_station):
+        """
+        Constructor
+        """
+        super().__init__(message_id)
 
-            # next...
-            next_jdict = jdict.get('next')
-            next_query = NextMessageQuery.construct_from_uri(next_jdict)
+        self.__time = time                          # GPTime
+        self.__loc = loc                            # GPLoc
 
-            if next_query is None:
-                return
+        self.__quality = quality                    # int
+        self.__num_sv = num_sv                      # int
+        self.__hdop = hdop                          # float(2)
+        self.__alt = alt                            # float(1) - altitude (metres)
+        self.__sep = sep                            # float(1) - geoid separation (metres)
 
-            params['start-date'] = next_query.start_date.as_iso8601()
-            params['end-date'] = next_query.end_date.as_iso8601()
+        self.__diff_age = diff_age                  # float(3) - age of differential corrections (seconds)
+        self.__diff_station = diff_station          # string - ID of station providing differential corrections
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __str__(self, *args, **kwargs):
-        return "MessageManager:{rest_client:%s, verbose:%s}" % (self.__rest_client, self.__verbose)
-
-
-# --------------------------------------------------------------------------------------------------------------------
-
-class NextMessageQuery(object):
-    """
-    classdocs
+    @property
+    def time(self):
+        return self.__time
 
-    example query:
-    /v1/messages/topic//users/southcoastscience-dev/test/json?
-    start-date=2016-11-13T07:11:14.779Z&end-date=2016-11-13T08:48:08.901+00:00
-    """
 
-    # ----------------------------------------------------------------------------------------------------------------
+    @property
+    def loc(self):
+        return self.__loc
 
-    @classmethod
-    def construct_from_uri(cls, uri):
-        if not uri:
-            return None
 
-        # parse...
-        parse = urllib.parse.urlparse(urllib.parse.unquote(uri))
-        params = urllib.parse.parse_qs(parse[4])
+    @property
+    def quality(self):
+        return self.__quality
 
-        if 'start-date' not in params or 'end-date' not in params:
-            return None
 
-        # construct...
-        start_date = LocalizedDatetime.construct_from_iso8601(params['start-date'][0])
-        end_date = LocalizedDatetime.construct_from_iso8601(params['end-date'][0])
+    @property
+    def num_sv(self):
+        return self.__num_sv
 
-        if not start_date or not end_date:
-            return None
 
-        return NextMessageQuery(start_date, end_date)
+    @property
+    def hdop(self):
+        return self.__hdop
 
 
-    # ----------------------------------------------------------------------------------------------------------------
+    @property
+    def alt(self):
+        return self.__alt
 
-    def __init__(self, start_date, end_date):
-        """
-        Constructor
-        """
-        self.__start_date = start_date          # LocalizedDatetime
-        self.__end_date = end_date              # LocalizedDatetime
 
+    @property
+    def sep(self):
+        return self.__sep
 
-    # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def start_date(self):
-        return self.__start_date
+    def diff_age(self):
+        return self.__diff_age
 
 
     @property
-    def end_date(self):
-        return self.__end_date
+    def diff_station(self):
+        return self.__diff_station
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "NextMessageQuery:{start_date:%s, end_date:%s}" % (self.start_date, self.end_date)
+        return "GPGGA:{source:%s, time:%s, loc:%s, quality:%s, num_sv:%s, hdop:%s, alt:%s, sep:%s, " \
+               "diff_age:%s, diff_station:%s}" % \
+                    (self.source, self.time, self.loc, self.quality, self.num_sv, self.hdop, self.alt, self.sep,
+                     self.diff_age, self.diff_station)
```

### Comparing `scs-core-2.4.6/src/scs_core/osio/manager/organisation_manager.py` & `scs-core-2.8.1/src/scs_core/sys/serial.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,123 +1,120 @@
 """
-Created on 8 Mar 2017
+Created on 19 Mar 2019
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
+
+https://stackoverflow.com/questions/7266558/pyserial-buffer-wont-flush
 """
 
-import urllib.parse
+import time
 
-from scs_core.osio.client.rest_client import RESTClient
-from scs_core.osio.data.organisation import Organisation
+from abc import ABC, abstractmethod
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class OrganisationManager(object):
+class Serial(ABC):
     """
     classdocs
     """
-    __FINDER_BATCH_SIZE = 100
+
+    _DEFAULT_EOL = "\n"
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, api_key):
+    def __init__(self, device_identifier, baud_rate, hard_handshake=False):
         """
         Constructor
         """
-        self.__rest_client = RESTClient(api_key)
+        self._device_identifier = device_identifier             # string device path or int port number
+        self._baud_rate = baud_rate                             # int
+        self._hard_handshake = hard_handshake                   # bool
 
+        self._ser = None
 
-    # ----------------------------------------------------------------------------------------------------------------
-
-    def find(self, org_id):
-        request_path = '/v1/orgs/' + urllib.parse.quote(org_id, '')
 
-        # request...
-        self.__rest_client.connect()
+    # ----------------------------------------------------------------------------------------------------------------
 
-        try:
-            response_jdict = self.__rest_client.get(request_path)
-        except RuntimeError:
-            response_jdict = None
+    @abstractmethod
+    def open(self, lock_timeout, comms_timeout):
+        pass
 
-        self.__rest_client.close()
 
-        topic = Organisation.construct_from_jdict(response_jdict)
+    @abstractmethod
+    def close(self):
+        pass
 
-        return topic
 
+    # ----------------------------------------------------------------------------------------------------------------
 
-    def find_owned_by_user(self, org_id):
-        orgs = []
+    def read_lines(self, eol=None, timeout=None):
+        while True:
+            try:
+                yield self.read_line(eol, timeout)
 
-        # request...
-        self.__rest_client.connect()
+            except TimeoutError:
+                return
 
-        try:
-            for batch in self.__get(org_id):
-                orgs.extend(batch)
 
-        finally:
-            self.__rest_client.close()
+    def read_line(self, eol=None, timeout=None):
+        terminator = self._DEFAULT_EOL if eol is None else eol
+        end_time = None if timeout is None else time.time() + timeout
 
-        return orgs
+        line = ""
+        while True:
+            if timeout is not None and time.time() > end_time:
+                raise TimeoutError(timeout)
 
+            char = self._ser.read().decode(errors='ignore')
+            line += char
 
-    # ----------------------------------------------------------------------------------------------------------------
+            if line.endswith(terminator):
+                break
 
-    def create(self, org):
-        request_path = '/v1/orgs'
+        return line.strip()
 
-        # request...
-        self.__rest_client.connect()
 
-        try:
-            response = self.__rest_client.post(request_path, org.as_json())
+    def write_line(self, text, eol=None):
+        terminator = self._DEFAULT_EOL if eol is None else eol
 
-        finally:
-            self.__rest_client.close()
+        text_ln = text.strip() + terminator
+        packet = text_ln.encode()
 
-        print("create response: %s" % response)
+        return self._ser.write(packet)
 
-        return response
 
+    # ----------------------------------------------------------------------------------------------------------------
 
-    def update(self, org_id, org):
-        request_path = '/v1/orgs/' + org_id
+    def read(self, count):
+        chars = self._ser.read(count)
 
-        # request...
-        self.__rest_client.connect()
+        return chars
 
-        try:
-            self.__rest_client.put(request_path, org.as_json())
-        finally:
-            self.__rest_client.close()
 
+    def write(self, *chars):
+        self._ser.write(bytearray(chars))
 
-    # ----------------------------------------------------------------------------------------------------------------
 
-    def __get(self, user_id):
-        request_path = '/v12/users/' + user_id + '/owned-orgs'
-        params = {'offset': 0, 'count': self.__FINDER_BATCH_SIZE}
+    def flush_input(self):
+        self._ser.flushInput()
 
-        while True:
-            # request...
-            response_jdict = self.__rest_client.get(request_path, params=params)
 
-            # organisations...
-            orgs = [Organisation.construct_from_jdict(org_jdict) for org_jdict in response_jdict] \
-                if response_jdict else []
+    def flush_output(self):
+        self._ser.flushOutput()
 
-            yield orgs
 
-            if len(orgs) == 0:
-                break
+    # ----------------------------------------------------------------------------------------------------------------
 
-            # next...
-            params['offset'] += len(orgs)
+    @property
+    @abstractmethod
+    def device_identifier(self):
+        return None
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "OrganisationManager:{rest_client:%s}" % self.__rest_client
+        is_open = False if self._ser is None else self._ser.is_open
+
+        return self.__class__.__name__ + ":{device_identifier:%s, baud_rate=%d, hard_handshake=%s, serial_open:%s}" % \
+            (self._device_identifier, self._baud_rate, self._hard_handshake, is_open)
```

### Comparing `scs-core-2.4.6/src/scs_core/osio/manager/schema_manager.py` & `scs-core-2.8.1/src/scs_core/sys/timeout.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 """
-Created on 14 Feb 2017
+Created on 16 Sep 2019
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
+
+Timeout context manager. Usage:
+
+timeout = Timeout(10)
+
+try:
+    with timeout:
+        my_func()
+
+except TimeoutError:
+    print("function timed out!")
+
+https://www.jujens.eu/posts/en/2018/Jun/02/python-timeout-function/
 """
 
-from scs_core.osio.client.rest_client import RESTClient
-from scs_core.osio.data.schema import Schema
+import signal
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class SchemaManager(object):
+class Timeout(object):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, api_key):
+    def __init__(self, seconds):
         """
         Constructor
         """
-        self.__rest_client = RESTClient(api_key)
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    def find_all(self):
-        request_path = '/v2/schemas'
+        self.__seconds = seconds                                    # number
 
-        # request...
-        self.__rest_client.connect()
 
-        try:
-            response_jdict = self.__rest_client.get(request_path)
+    def __enter__(self):
+        # handler...
+        def raise_timeout(_signum, _frame):
+            signal.signal(signal.SIGALRM, signal.SIG_IGN)
+            raise TimeoutError
 
-        finally:
-            self.__rest_client.close()
+        # signal...
+        signal.signal(signal.SIGALRM, raise_timeout)
+        signal.alarm(int(round(self.__seconds)))
 
-        schemas = [Schema.construct_from_jdict(schema_jdict) for schema_jdict in response_jdict]
 
-        return schemas
+    def __exit__(self, _exc_type, _exc_val, _exc_tb):
+        signal.signal(signal.SIGALRM, signal.SIG_IGN)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "SchemaManager:{rest_client:%s}" % self.__rest_client
+        return "Timeout:{seconds:%s}" % self.__seconds
```

### Comparing `scs-core-2.4.6/src/scs_core/osio/manager/user_manager.py` & `scs-core-2.8.1/src/scs_core/position/nmea/gpdatetime.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,87 +1,56 @@
 """
-Created on 21 Mar 2017
+Created on 1 Jan 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
-"""
 
-from scs_core.osio.client.rest_client import RESTClient
-from scs_core.osio.data.user import User
-from scs_core.osio.data.user_metadata import UserMetadata
+https://www.nmea.org
+https://en.wikipedia.org/wiki/NMEA_0183
+"""
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class UserManager(object):
+class GPDateTime(object):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, api_key):
+    def __init__(self, date, time):
         """
         Constructor
         """
-        self.__rest_client = RESTClient(api_key)
+        self.__date = date                # ddmmyy
+        self.__time = time                # hhmmss.ss
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def find(self, user_id):
-        request_path = '/v1/users/' + user_id
-
-        # request...
-        self.__rest_client.connect()
-
-        try:
-            response_jdict = self.__rest_client.get(request_path)
-        except RuntimeError:
-            response_jdict = None
-
-        self.__rest_client.close()
-
-        user = User.construct_from_jdict(response_jdict)
-
-        return user
-
-
-    def find_public(self, user_id):
-        request_path = '/v1/public/users/' + user_id
-
-        # request...
-        self.__rest_client.connect()
-
-        try:
-            response_jdict = self.__rest_client.get(request_path)
-        except RuntimeError:
-            response_jdict = None
-
-        self.__rest_client.close()
-
-        user = UserMetadata.construct_from_jdict(response_jdict)
-
-        return user
-
+    def as_iso8601(self):
+        """
+        example: 2016-08-13T00:38:05.210+00:00
+        """
+        if self.__date is None or self.__time is None:
+            return None
 
-    def find_members_of_org(self, org_id):
-        pass
+        return "20%s-%s-%sT%s:%s:%s0Z" % \
+               (self.__date[4:], self.__date[2:4], self.__date[:2], self.__time[:2], self.__time[2:4], self.__time[4:])
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def update(self, user_id, user):
-        request_path = '/v1/users/' + user_id
+    @property
+    def date(self):
+        return self.__date
 
-        # request...
-        self.__rest_client.connect()
 
-        try:
-            self.__rest_client.put(request_path, user.as_json())
-        finally:
-            self.__rest_client.close()
+    @property
+    def time(self):
+        return self.__time
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "UserManager:{rest_client:%s}" % self.__rest_client
+        return "GPDateTime:{date:%s, time:%s}" % (self.date, self.time)
```

### Comparing `scs-core-2.4.6/src/scs_core/particulate/opc_conf.py` & `scs-core-2.8.1/src/scs_core/particulate/opc_conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,92 +26,84 @@
     @classmethod
     def persistence_location(cls, name):
         filename = cls.__FILENAME if name is None else '_'.join((name, cls.__FILENAME))
 
         return cls.conf_dir(), filename
 
 
+    @classmethod
+    def load(cls, manager, name=None, encryption_key=None, skeleton=False):
+        conf = super().load(manager, name=name, encryption_key=encryption_key, skeleton=skeleton)
+
+        if conf:
+            conf.__dev_path = manager.opc_spi_dev_path()
+
+        return conf
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def construct_from_jdict(cls, jdict, name=None, skeleton=False):
         if not jdict:
             return None
 
         model = jdict.get('model')
         sample_period = jdict.get('sample-period')
         restart_on_zeroes = jdict.get('restart-on-zeroes', True)
         power_saving = jdict.get('power-saving')
 
-        bus = jdict.get('bus')
-        address = jdict.get('address')
+        dev_path = jdict.get('dev_path')
 
-        return cls(model, sample_period, restart_on_zeroes, power_saving, bus, address, name=name)
+        return cls(model, sample_period, restart_on_zeroes, power_saving, dev_path, name=name)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, model, sample_period, restart_on_zeroes, power_saving, bus, address, name=None):
+    def __init__(self, model, sample_period, restart_on_zeroes, power_saving, dev_path, name=None):
         """
         Constructor
         """
         super().__init__(name)
 
         self.__model = model                                        # string
         self.__sample_period = int(sample_period)                   # int
         self.__restart_on_zeroes = bool(restart_on_zeroes)          # bool
         self.__power_saving = bool(power_saving)                    # bool
 
-        self.__bus = bus                                            # int
-        self.__address = address                                    # int
+        self.__dev_path = dev_path                                  # string
 
 
     def __eq__(self, other):                            # ignore name
         try:
             return self.model == other.model and self.sample_period == other.sample_period and \
                    self.restart_on_zeroes == other.restart_on_zeroes and self.power_saving == other.power_saving and \
-                   self.bus == other.bus and self.address == other.address
+                   self.dev_path == other.dev_path
 
         except (TypeError, AttributeError):
             return False
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     # noinspection PyMethodMayBeStatic,PyUnusedLocal
-    def opc_monitor(self, interface, host):
+    def opc_monitor(self, interface):
         return None
 
 
     # noinspection PyMethodMayBeStatic,PyUnusedLocal
-    def opc(self, interface, host):
+    def opc(self, interface):
         return None
 
 
     # noinspection PyMethodMayBeStatic
     def uses_spi(self):
         return True
 
 
-    def opc_bus(self, host):
-        try:
-            return int(self.__bus)
-
-        except TypeError:
-            return host.opc_spi_bus()
-
-
-    def opc_address(self, host):
-        try:
-            return int(self.__address)
-
-        except TypeError:
-            return host.opc_spi_device()
-
-
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def model(self):
         return self.__model
 
 
@@ -127,42 +119,34 @@
 
     @property
     def restart_on_zeroes(self):
         return self.__restart_on_zeroes
 
 
     @property
-    def bus(self):
-        return self.__bus
-
-
-    @property
-    def address(self):
-        return self.__address
+    def dev_path(self):
+        return self.__dev_path
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         jdict = OrderedDict()
 
         jdict['model'] = self.model
         jdict['sample-period'] = self.sample_period
         jdict['restart-on-zeroes'] = self.restart_on_zeroes
         jdict['power-saving'] = self.power_saving
 
-        if self.__bus is not None:
-            jdict['bus'] = self.bus
-
-        if self.__address is not None:
-            jdict['address'] = self.address
+        if self.__dev_path is not None:
+            jdict['dev_path'] = self.dev_path
 
         return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
         return "OPCConf(core):{name:%s, model:%s, sample_period:%s, restart_on_zeroes:%s, power_saving:%s, " \
-               "bus:%s, address:%s}" %  \
+               "dev_path:%s}" %  \
                (self.name, self.model, self.sample_period, self.restart_on_zeroes, self.power_saving,
-                self.bus, self.address)
+                self.dev_path)
```

### Comparing `scs-core-2.4.6/src/scs_core/particulate/opc_datum.py` & `scs-core-2.8.1/src/scs_core/particulate/opc_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/particulate/pmx_datum.py` & `scs-core-2.8.1/src/scs_core/particulate/pmx_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/particulate/sps_datum.py` & `scs-core-2.8.1/src/scs_core/particulate/sps_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/position/gps_datum.py` & `scs-core-2.8.1/src/scs_core/position/gps_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/position/nmea/gpdatetime.py` & `scs-core-2.8.1/src/scs_core/sys/memory.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,48 @@
 """
-Created on 1 Jan 2017
+Created on 14 Jan 2023
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-https://www.nmea.org
-https://en.wikipedia.org/wiki/NMEA_0183
+https://stackoverflow.com/questions/938733/total-memory-used-by-python-process
 """
 
+import os
+
+from psutil import Process
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class GPDateTime(object):
+class Memory(object):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, date, time):
+    def __init__(self):
         """
         Constructor
         """
-        self.__date = date                # ddmmyy
-        self.__time = time                # hhmmss.ss
+        self.__process = Process(os.getpid())
+        self.__base_usage = self.__process.memory_info().rss
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_iso8601(self):
-        """
-        example: 2016-08-13T00:38:05.210+00:00
-        """
-        if self.__date is None or self.__time is None:
-            return None
+    def total(self):
+        usage = self.__process.memory_info().rss
 
-        return "20%s-%s-%sT%s:%s:%s0Z" % \
-               (self.__date[4:], self.__date[2:4], self.__date[:2], self.__time[:2], self.__time[2:4], self.__time[4:])
-
-
-    # ----------------------------------------------------------------------------------------------------------------
+        return int(round(usage / 1024))
 
-    @property
-    def date(self):
-        return self.__date
 
+    def heap(self):
+        usage = self.__process.memory_info().rss - self.__base_usage
 
-    @property
-    def time(self):
-        return self.__time
+        return int(round(usage / 1024))
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "GPDateTime:{date:%s, time:%s}" % (self.date, self.time)
+        return "Memory:{process:%s, base_usage:%s}" % (self.__process, self.__base_usage)
```

### Comparing `scs-core-2.4.6/src/scs_core/position/nmea/gpgga.py` & `scs-core-2.8.1/src/scs_core/sys/ps_datum.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,146 +1,177 @@
 """
-Created on 30 Dec 2016
+Created on 13 Jun 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-Global positioning system fix data
-$xxGGA,time,lat,NS,long,EW,quality,numSV,HDOP,alt,M,sep,M,diffAge,diffStation*cs
+command example:
+ps -Ao ppid,pid,uid,tty,pmem,pcpu,cputime,etime,args -w -w
 
-example sentence:
-$GPGGA,092725.00,4717.11399,N,00833.91590,E,1,08,1.01,499.6,M,48.0,M,,*5B
-
-example values:
-GPGGA:{time:GPTime:{time:141058.00}, loc:GPLoc:{lat:5049.38432, ns:N, lng:00007.37801, ew:W}, quality:2, num_sv:06,
-hdop:3.10, alt:37.5, sep:45.4, diff_age:None, diff_station:0000}
+report examples:
+  154 26605   502 ??        0.0   0.0   0:00.37 01-00:43:12 /usr/bin/ssh-agent -l
+  154 39364   502 ??        6.3  31.5  22:58.40    02:26:25 /Applications/PyCharm.app/Contents/MacOS/pycharm
+
+JSON example:
+{"ppid": 154, "pid": 26605, "uid": 502, "tty": "??", "pcpu": 0.0, "pmem": 0.0,
+"cpu": {"days": 0, "hours": 0, "minutes": 0, "seconds": 0, "millis": 370},
+"elapsed": {"days": 1, "hours": 0, "minutes": 43, "seconds": 12, "millis": 0},
+"cmd": "/usr/bin/ssh-agent -l"}
+"""
 
-GPGGA:{time:GPTime:{time:140047.00}, loc:GPLoc:{lat:None, ns:None, lng:None, ew:None}, quality:0, num_sv:00,
-hdop:99.99, alt:None, sep:None, diff_age:None, diff_station:None}
+import re
 
-https://www.nmea.org
-https://en.wikipedia.org/wiki/NMEA_0183
-"""
+from collections import OrderedDict
 
-from scs_core.position.nmea.gploc import GPLoc
-from scs_core.position.nmea.gptime import GPTime
-from scs_core.position.nmea.nmea_sentence import NMEASentence
+from scs_core.data.json import JSONable
+from scs_core.data.timedelta import Timedelta
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class GPGGA(NMEASentence):
+class PsDatum(JSONable):
     """
     classdocs
     """
 
-    MESSAGE_IDS = ("$GNGGA", "$GPGGA")
+    # ----------------------------------------------------------------------------------------------------------------
+
+    @classmethod
+    def construct_from_report(cls, report):
+        mat = re.match(r'^\s*(\d+)\s+(\d+)\s+(\d+)\s+(\S+)\s+(\d+\.\d+)\s+(\d+\.\d+)\s+(\S+)\s+(\S+)\s+(.+)$',
+                       report)
 
-    QUALITY_NO_FIX =                0
-    QUALITY_AUTONOMOUS_GNSS =       1
-    QUALITY_DIFFERENTIAL_GNSS =     2
-    QUALITY_ESTIMATED_FIX =         6
+        if mat is None:
+            return None
 
+        fields = mat.groups()
 
-    # ----------------------------------------------------------------------------------------------------------------
+        ppid = int(fields[0])
+        pid = int(fields[1])
+        uid = int(fields[2])
+        tty = fields[3]
 
-    @classmethod
-    def construct(cls, r):
-        if r.message_id not in cls.MESSAGE_IDS:
-            raise TypeError("invalid sentence:%s" % r)
+        pcpu = float(fields[4])
+        pmem = float(fields[5])
+
+        cpu_time = Timedelta.construct_from_ps_time_report(fields[6])
+        elapsed_time = Timedelta.construct_from_ps_elapsed_report(fields[7])
+        cmd = fields[8]
+
+        return PsDatum(ppid, pid, uid, tty, pcpu, pmem, cpu_time, elapsed_time, cmd)
 
-        time = GPTime(r.str(1))
 
-        lat = r.str(2)
-        ns = r.str(3)
+    @classmethod
+    def construct_from_jdict(cls, jdict):
+        if not jdict:
+            return None
 
-        lng = r.str(4)
-        ew = r.str(5)
+        ppid = int(jdict.get('ppid'))
+        pid = int(jdict.get('pid'))
+        uid = int(jdict.get('uid'))
+        tty = jdict.get('tty')
 
-        loc = GPLoc(lat, ns, lng, ew)
+        pcpu = float(jdict.get('pcpu'))
+        pmem = float(jdict.get('pmem'))
 
-        quality = r.int(6)
-        num_sv = r.int(7)
-        hdop = r.float(8, 3)
-        alt = r.float(9, 2)
-        sep = r.float(11, 2)
+        cpu_time = Timedelta.construct_from_jdict(jdict.get('cpu'))
+        elapsed_time = Timedelta.construct_from_jdict(jdict.get('elapsed'))
 
-        diff_age = r.float(13, 3)
-        diff_station = r.str(14)
+        cmd = jdict.get('cmd')
 
-        return GPGGA(r.message_id, time, loc, quality, num_sv, hdop, alt, sep, diff_age, diff_station)
+        return PsDatum(ppid, pid, uid, tty, pcpu, pmem, cpu_time, elapsed_time, cmd)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, message_id, time, loc, quality, num_sv, hdop, alt, sep, diff_age, diff_station):
+    def __init__(self, ppid, pid, uid, tty, pcpu, pmem, cpu_time, elapsed_time, cmd):
         """
         Constructor
         """
-        super().__init__(message_id)
+        self.__ppid = ppid                  # int               parent process ID
+        self.__pid = pid                    # int               process ID
+        self.__uid = uid                    # int               user ID
+        self.__tty = tty                    # string            TTY
+
+        self.__pcpu = pcpu                  # float             % CPU
+        self.__pmem = pmem                  # float             % memory
+
+        self.__cpu_time = cpu_time          # Timedelta
+        self.__elapsed_time = elapsed_time  # Timedelta
+
+        self.__cmd = cmd                    # string
+
+
+    # ----------------------------------------------------------------------------------------------------------------
+
+    def as_json(self):
+        jdict = OrderedDict()
+
+        jdict['ppid'] = self.ppid
+        jdict['pid'] = self.pid
+        jdict['uid'] = self.uid
+        jdict['tty'] = self.tty
+
+        jdict['pcpu'] = self.pcpu
+        jdict['pmem'] = self.pmem
 
-        self.__time = time                          # GPTime
-        self.__loc = loc                            # GPLoc
+        jdict['cpu'] = self.cpu_time
+        jdict['elapsed'] = self.elapsed_time
 
-        self.__quality = quality                    # int
-        self.__num_sv = num_sv                      # int
-        self.__hdop = hdop                          # float(2)
-        self.__alt = alt                            # float(1) - altitude (metres)
-        self.__sep = sep                            # float(1) - geoid separation (metres)
+        jdict['cmd'] = self.cmd
 
-        self.__diff_age = diff_age                  # float(3) - age of differential corrections (seconds)
-        self.__diff_station = diff_station          # string - ID of station providing differential corrections
+        return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def time(self):
-        return self.__time
+    def ppid(self):
+        return self.__ppid
 
 
     @property
-    def loc(self):
-        return self.__loc
+    def pid(self):
+        return self.__pid
 
 
     @property
-    def quality(self):
-        return self.__quality
+    def uid(self):
+        return self.__uid
 
 
     @property
-    def num_sv(self):
-        return self.__num_sv
+    def tty(self):
+        return self.__tty
 
 
     @property
-    def hdop(self):
-        return self.__hdop
+    def pcpu(self):
+        return self.__pcpu
 
 
     @property
-    def alt(self):
-        return self.__alt
+    def pmem(self):
+        return self.__pmem
 
 
     @property
-    def sep(self):
-        return self.__sep
+    def cpu_time(self):
+        return self.__cpu_time
 
 
     @property
-    def diff_age(self):
-        return self.__diff_age
+    def elapsed_time(self):
+        return self.__elapsed_time
 
 
     @property
-    def diff_station(self):
-        return self.__diff_station
+    def cmd(self):
+        return self.__cmd
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "GPGGA:{source:%s, time:%s, loc:%s, quality:%s, num_sv:%s, hdop:%s, alt:%s, sep:%s, " \
-               "diff_age:%s, diff_station:%s}" % \
-                    (self.source, self.time, self.loc, self.quality, self.num_sv, self.hdop, self.alt, self.sep,
-                     self.diff_age, self.diff_station)
+        return "PsDatum:{ppid:%s, pid:%s, uid:%s, tty:%s, pcpu:%s, pmem:%s, " \
+               "cpu_time:%s, elapsed_time:%s, cmd:%s}" %  \
+               (self.ppid, self.pid, self.uid, self.tty, self.pcpu, self.pmem,
+                self.cpu_time, self.elapsed_time, self.cmd)
```

### Comparing `scs-core-2.4.6/src/scs_core/position/nmea/gpgll.py` & `scs-core-2.8.1/src/scs_core/position/nmea/gpgll.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/position/nmea/gpgsa.py` & `scs-core-2.8.1/src/scs_core/position/nmea/gpgsa.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/position/nmea/gpgsv.py` & `scs-core-2.8.1/src/scs_core/position/nmea/gpgsv.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/position/nmea/gploc.py` & `scs-core-2.8.1/src/scs_core/position/nmea/gploc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/position/nmea/gprmc.py` & `scs-core-2.8.1/src/scs_core/position/nmea/gprmc.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/position/nmea/gpvtg.py` & `scs-core-2.8.1/src/scs_core/position/nmea/gpvtg.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/position/nmea/nmea_sentence.py` & `scs-core-2.8.1/src/scs_core/position/nmea/nmea_sentence.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/position/position.py` & `scs-core-2.8.1/src/scs_core/position/position.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/psu/psu.py` & `scs-core-2.8.1/src/scs_core/psu/psu.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/psu/psu_conf.py` & `scs-core-2.8.1/src/scs_core/psu/psu_conf.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/psu/psu_report.py` & `scs-core-2.8.1/src/scs_core/psu/psu_report.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/psu/psu_version.py` & `scs-core-2.8.1/src/scs_core/psu/psu_version.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sample/climate_sample.py` & `scs-core-2.8.1/src/scs_core/sample/climate_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sample/configuration_sample.py` & `scs-core-2.8.1/src/scs_core/sample/configuration_sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 example document:
 {"rec": "2021-10-06T11:27:48Z", "tag": "scs-be2-3", "ver": 1.00, "val": {"hostname": "scs-bbe-003",
 "packs": {"scs_comms": {"repo": "scs_comms_ge910", "version": null}, "scs_core": {"repo": "scs_core",
 "version": "1.0.32"}, "scs_dev": {"repo": "scs_dev", "version": "1.0.11"}, "scs_dfe": {"repo": "scs_dfe_eng",
 "version": "1.0.10"}, "scs_exegesis": {"repo": "scs_exegesis", "version": null},
 "scs_greengrass": {"repo": "scs_greengrass", "version": "1.0.3"}, "scs_host": {"repo": "scs_host_bbe_southern",
 "version": "1.0.6"}, "scs_inference": {"repo": "scs_inference", "version": null}, "scs_mfr": {"repo": "scs_mfr",
-"version": "1.0.14"}, "scs_ndir": {"repo": "scs_ndir", "version": null}, "scs_osio": {"repo": "scs_osio",
-"version": null}, "scs_psu": {"repo": "scs_psu", "version": "1.0.10"}},
+"version": "1.0.14"}, "scs_ndir": {"repo": "scs_ndir", "version": null},
+"scs_psu": {"repo": "scs_psu", "version": "1.0.10"}},
 "afe-baseline": {"sn1": {"calibrated-on": "2021-08-22T12:46:44Z", "offset": 13, "env": {"hmd": 62.6, "tmp": 24.5,
 "pA": 102.1}}, "sn2": {"calibrated-on": "2021-08-22T12:46:38Z", "offset": -7, "env": {"hmd": 62.7, "tmp": 24.5,
 "pA": 102.1}}, "sn3": {"calibrated-on": "2021-08-22T12:46:46Z", "offset": 24, "env": {"hmd": 62.6, "tmp": 24.5,
 "pA": 102.1}}, "sn4": {"calibrated-on": "2021-08-22T12:46:41Z", "offset": 9, "env": {"hmd": 62.6, "tmp": 24.5,
 "pA": 102.1}}}, "afe-id": {"serial_number": "27-000001", "type": "810-0023-02", "calibrated_on": "2016-11-01",
 "sn1": {"serial_number": "212060308", "sensor_type": "NO2A43F"}, "sn2": {"serial_number": "132950202",
 "sensor_type": "CO A4"}, "sn3": {"serial_number": "134060009", "sensor_type": "SO2A4"},
@@ -207,15 +207,15 @@
         if not self.__items[sample.tag] or not self.__latest_only:
             if sample not in self.__items[sample.tag]:            # we might not be reading all the fields in the DB!
                 self.__items[sample.tag].append(sample)
             return
 
         for item in self.__items[sample.tag]:
             if sample.rec > item.rec:
-                self.__items[sample.tag] = (sample, )
+                self.__items[sample.tag] = [sample]
                 return
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def diffs(self):
         diff_history = ConfigurationSampleHistory()
```

### Comparing `scs-core-2.4.6/src/scs_core/sample/gases_sample.py` & `scs-core-2.8.1/src/scs_core/sample/gases_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sample/particulates_sample.py` & `scs-core-2.8.1/src/scs_core/sample/particulates_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sample/pressure_sample.py` & `scs-core-2.8.1/src/scs_core/sample/pressure_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sample/sample.py` & `scs-core-2.8.1/src/scs_core/sample/sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sample/status_sample.py` & `scs-core-2.8.1/src/scs_core/sample/status_sample.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sampler/sampler.py` & `scs-core-2.8.1/src/scs_core/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sync/interval_timer.py` & `scs-core-2.8.1/src/scs_core/sync/interval_timer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sync/line_reader.py` & `scs-core-2.8.1/src/scs_core/sync/line_reader.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sync/runner.py` & `scs-core-2.8.1/src/scs_core/sync/runner.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sync/schedule.py` & `scs-core-2.8.1/src/scs_core/sync/schedule.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sync/synchronised_process.py` & `scs-core-2.8.1/src/scs_core/sync/synchronised_process.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sync/timed_runner.py` & `scs-core-2.8.1/src/scs_core/sync/timed_runner.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sys/command.py` & `scs-core-2.8.1/src/scs_core/sys/command.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sys/disk_usage.py` & `scs-core-2.8.1/src/scs_core/sys/disk_volume.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,81 @@
 """
-Created on 16 Apr 2018
+Created on 14 Oct 2020
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 JSON example:
-{"path": "/srv/removable_data_storage", "free": 15423610880, "used": 329793536, "total": 15753404416,
-"is-available": true}
+{"filesystem": "/dev/mmcblk0p1", "total": 15384184, "used": 319296, "free": 14892092,
+"mounted-on": "/srv/SCS_logging", "is-available": false}
 
-https://www.geeksforgeeks.org/python-os-statvfs-method/
+https://stackoverflow.com/questions/35469685/in-python-how-do-i-get-a-list-of-all-partitions-in-mac-os-x
 """
 
 import os
+import re
 
 from collections import OrderedDict
 
 from scs_core.data.json import JSONable
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class DiskUsage(JSONable):
+class DiskVolume(JSONable):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
-    def construct_from_statvfs(cls, path, statvfs):
-        free = statvfs.f_bfree * statvfs.f_bsize
-        total = statvfs.f_blocks * statvfs.f_bsize
-        used = total - free
+    def construct_from_df_row(cls, row):
+        match = re.search(r'([^ ]+)\s+([0-9]+)\s+([0-9]+)\s+([0-9]+)\s+([0-9]+)%\s+([^ ]+)', row)
 
-        return cls(path, free, used, total)
+        if match is None:
+            return None
+
+        groups = match.groups()
+
+        filesystem = groups[0]
+        total = groups[1]
+        used = groups[2]
+        free = groups[3]
+        mounted_on = groups[5]
+
+        return cls(filesystem, free, used, total, mounted_on)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, path, free, used, total):
+    def __init__(self, filesystem, free, used, total, mounted_on):
         """
         Constructor
         """
-        self.__path = path                          # string
+        self.__filesystem = filesystem                      # string
+        self.__total = int(total)                           # int blocks
+        self.__used = int(used)                             # int blocks
+        self.__free = int(free)                             # int blocks
+        self.__mounted_on = mounted_on                      # string
+
+
+    # ----------------------------------------------------------------------------------------------------------------
+
+    def as_json(self):
+        jdict = OrderedDict()
 
-        self.__free = int(free)                     # int bytes
-        self.__used = int(used)                     # int bytes
-        self.__total = int(total)                   # int bytes
+        jdict['filesystem'] = self.filesystem
+        jdict['free'] = self.free
+        jdict['used'] = self.used
+        jdict['total'] = self.total
+        jdict['mounted-on'] = self.mounted_on
+
+        jdict['is-available'] = self.is_available
+
+        return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def percent_used(self):
         if not self.is_available:
             return None
@@ -58,42 +84,26 @@
 
         return round(percent, 1)
 
 
     @property
     def is_available(self):
         try:
-            os.listdir(self.path)
+            os.listdir(self.mounted_on)
             return True
 
         except OSError:
             return False
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def as_json(self):
-        jdict = OrderedDict()
-
-        jdict['path'] = self.path
-
-        jdict['free'] = self.free
-        jdict['used'] = self.used
-        jdict['total'] = self.total
-
-        jdict['is-available'] = self.is_available
-
-        return jdict
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
     @property
-    def path(self):
-        return self.__path
+    def filesystem(self):
+        return self.__filesystem
 
 
     @property
     def free(self):
         return self.__free
 
 
@@ -103,62 +113,67 @@
 
 
     @property
     def total(self):
         return self.__total
 
 
+    @property
+    def mounted_on(self):
+        return self.__mounted_on
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "DiskUsage:{path:%s, free:%s, used:%s, total:%s}" %  \
-               (self.path, self.free, self.used, self.total)
+        return "DiskVolume:{filesystem:%s, free:%s, used:%s, total:%s, mounted_on:%s}" %  \
+               (self.filesystem, self.free, self.used, self.total, self.mounted_on)
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class ReportedDiskUsage(DiskUsage):
+class ReportedDiskVolume(DiskVolume):
     """
     classdocs
     """
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
     def construct_from_jdict(cls, jdict):
         if not jdict:
             return None
 
-        path = jdict.get('path')
-
+        filesystem = jdict.get('filesystem')
         free = jdict.get('free')
         used = jdict.get('used')
         total = jdict.get('total')
+        mounted_on = jdict.get('mounted-on')
 
         is_available = jdict.get('is-available')
 
-        return cls(path, free, used, total, is_available)
+        return cls(filesystem, free, used, total, mounted_on, is_available)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, path, free, used, total, is_available):
+    def __init__(self, filesystem, free, used, total, mounted_on, is_available):
         """
         Constructor
         """
-        super().__init__(path, free, used, total)
+        super().__init__(filesystem, free, used, total, mounted_on)
 
-        self.__is_available = is_available                      # bool
+        self.__is_available = is_available                  # bool
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def is_available(self):
         return self.__is_available
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "ReportedDiskUsage:{path:%s, free:%s, used:%s, total:%s, is_available:%s}" %  \
-               (self.path, self.free, self.used, self.total, self.is_available)
+        return "ReportedDiskVolume:{filesystem:%s, free:%s, used:%s, total:%s, mounted_on:%s, is_available:%s}" %  \
+               (self.filesystem, self.free, self.used, self.total, self.mounted_on, self.is_available)
```

### Comparing `scs-core-2.4.6/src/scs_core/sys/filesystem.py` & `scs-core-2.8.1/src/scs_core/sys/filesystem.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sys/http_exception.py` & `scs-core-2.8.1/src/scs_core/client/http_exception.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Created on 30 Mar 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
+
+https://en.wikipedia.org/wiki/List_of_HTTP_status_codes
 """
 
 from collections import OrderedDict
 
+from scs_core.data.datetime import LocalizedDatetime
 from scs_core.data.json import JSONable
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 class HTTPException(RuntimeError, JSONable):
     """
@@ -40,14 +43,23 @@
 
         if status == HTTPNotAllowedException.STATUS:
             return HTTPNotAllowedException(status, reason, data)
 
         if status == HTTPConflictException.STATUS:
             return HTTPConflictException(status, reason, data)
 
+        if status == HTTPBadGatewayException.STATUS:
+            return HTTPBadGatewayException(status, reason, data)
+
+        if status == HTTPServiceUnavailableException.STATUS:
+            return HTTPServiceUnavailableException(status, reason, data)
+
+        if status == HTTPGatewayTimeoutException.STATUS:
+            return HTTPGatewayTimeoutException(status, reason, data)
+
         return cls(status, reason, data)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, status, reason, data):
         """
@@ -85,21 +97,28 @@
     @property
     def data(self):
         return self.__data
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
+    @property
+    def error_report(self):
+        now = LocalizedDatetime.now().utc().as_iso8601()
+        return "%s: HTTP response: %s (%s) %s" % (now, self.status, self.reason, self.data)
+
+
     def __str__(self, *args, **kwargs):
         name = self.__class__.__name__
 
         return name + ":{status:%s, reason:%s, data:%s}" % (self.status, self.reason, self.data)
 
 
 # --------------------------------------------------------------------------------------------------------------------
+# 400 client errors...
 
 class HTTPBadRequestException(HTTPException):
     """
     classdocs
     """
     STATUS = 400
 
@@ -159,7 +178,50 @@
     """
     STATUS = 409
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self, status, reason, data):
         super().__init__(status, reason, data)
+
+
+# --------------------------------------------------------------------------------------------------------------------
+# 500 server errors...
+
+class HTTPBadGatewayException(HTTPException):
+    """
+    classdocs
+    """
+    STATUS = 502
+
+    # ----------------------------------------------------------------------------------------------------------------
+
+    def __init__(self, status, reason, data):
+        super().__init__(status, reason, data)
+
+
+# --------------------------------------------------------------------------------------------------------------------
+
+class HTTPServiceUnavailableException(HTTPException):
+    """
+    classdocs
+    """
+    STATUS = 503
+
+    # ----------------------------------------------------------------------------------------------------------------
+
+    def __init__(self, status, reason, data):
+        super().__init__(status, reason, data)
+
+
+# --------------------------------------------------------------------------------------------------------------------
+
+class HTTPGatewayTimeoutException(HTTPException):
+    """
+    classdocs
+    """
+    STATUS = 504
+
+    # ----------------------------------------------------------------------------------------------------------------
+
+    def __init__(self, status, reason, data):
+        super().__init__(status, reason, data)
```

### Comparing `scs-core-2.4.6/src/scs_core/sys/logging.py` & `scs-core-2.8.1/src/scs_core/sys/logging.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sys/modem.py` & `scs-core-2.8.1/src/scs_core/sys/modem.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sys/network.py` & `scs-core-2.8.1/src/scs_core/sys/network.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sys/node.py` & `scs-core-2.8.1/src/scs_core/sys/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,30 +191,20 @@
         pass
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # SPI...
 
     @abstractmethod
-    def ndir_spi_bus(self):
+    def ndir_spi_dev_path(self):
         pass
 
 
     @abstractmethod
-    def ndir_spi_device(self):
-        pass
-
-
-    @abstractmethod
-    def opc_spi_bus(self):
-        pass
-
-
-    @abstractmethod
-    def opc_spi_device(self):
+    def opc_spi_dev_path(self):
         pass
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # time...
 
     @abstractmethod
```

### Comparing `scs-core-2.4.6/src/scs_core/sys/persistence_manager.py` & `scs-core-2.8.1/src/scs_core/sys/persistence_manager.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sys/process_comms.py` & `scs-core-2.8.1/src/scs_core/sys/process_comms.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sys/shared_secret.py` & `scs-core-2.8.1/src/scs_core/sys/trace_entry.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,96 +1,67 @@
 """
-Created on 2 Apr 2018
+Created on 9 Jan 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
-
-https://stackoverflow.com/questions/2257441/
-random-string-generation-with-upper-case-letters-and-digits-in-python/23728630#23728630
-
-example document:
-{"key": "sxBhncFybpbMwZUa"}
 """
 
-import random
-import string
-
 from collections import OrderedDict
 
-from scs_core.data.json import PersistentJSONable
+from scs_core.data.json import JSONable
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class SharedSecret(PersistentJSONable):
+class TraceEntry(JSONable):
     """
     classdocs
     """
 
-    __FILENAME = "shared_secret.json"
-
-    @classmethod
-    def persistence_location(cls):
-        return cls.conf_dir(), cls.__FILENAME
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    __KEY_LENGTH = 16
-
-    @classmethod
-    def generate(cls):
-        return ''.join(random.SystemRandom().choice(string.ascii_letters + string.digits)
-                       for _ in range(cls.__KEY_LENGTH))
-
-
     # ----------------------------------------------------------------------------------------------------------------
 
     @classmethod
-    def construct_from_jdict(cls, jdict, skeleton=False):
-        if not jdict:
-            return None
+    def construct(cls, text):
+        lines = [line.strip() for line in text.splitlines()]
 
-        key = jdict.get('key')
+        location = lines[0]
+        statement = lines[1] if len(lines) > 1 else None
 
-        return SharedSecret(key)
+        return TraceEntry(location, statement)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self, key):
+    def __init__(self, location, statement):
         """
         Constructor
         """
-        super().__init__()
-
-        self.__key = key            # String
-
-
-    def __eq__(self, other):
-        try:
-            return self.key == other.key
-
-        except (TypeError, AttributeError):
-            return False
+        self.__location = location
+        self.__statement = statement
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def as_json(self):
         jdict = OrderedDict()
 
-        jdict['key'] = self.key
+        jdict['loc'] = self.location
+        jdict['stat'] = self.statement
 
         return jdict
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def key(self):
-        return self.__key
+    def location(self):
+        return self.__location
+
+
+    @property
+    def statement(self):
+        return self.__statement
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "SharedSecret:{key:%s}" % self.key
+        return "TraceEntry:{location:%s, statement:%s}" % (self.location, self.statement)
```

### Comparing `scs-core-2.4.6/src/scs_core/sys/signalled_exit.py` & `scs-core-2.8.1/src/scs_core/sys/signalled_exit.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sys/subprocess.py` & `scs-core-2.8.1/src/scs_core/sys/subprocess.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sys/system_id.py` & `scs-core-2.8.1/src/scs_core/sys/system_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Created on 17 Feb 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 Note: The system_serial_number is independent of both dfe serial number and host serial number. It is typically
 associated with the hostname. The combination vendor-id + model-id + system-sn must be universally unique.
 
-example:
+examples:
 {"vendor-id": "scs", "model-id": "ap1", "model": "Alpha Pi Eng", "config": "V1", "system-sn": 6}
 {"vendor-id": "SCS", "model-id": "BGB", "model": "Praxis", "config": "BGB", "system-sn": 406}
 """
 
 from collections import OrderedDict
 
 from scs_core.data.datetime import LocalizedDatetime
@@ -57,21 +57,21 @@
     def __init__(self, vendor_id, model_id, model_name, configuration, system_serial_number,
                  last_modified=None):
         """
         Constructor
         """
         super().__init__(last_modified=last_modified)
 
-        self.__vendor_id = vendor_id                # string (3 chars)
-        self.__model_id = model_id                  # string (3 chars)
+        self.__vendor_id = vendor_id                                # string (3 chars)
+        self.__model_id = model_id                                  # string (3 chars)
 
-        self.__model_name = model_name              # string
-        self.__configuration = configuration        # string
+        self.__model_name = model_name                              # string
+        self.__configuration = configuration                        # string
 
-        self.__system_serial_number = system_serial_number        # string (by convention, int)
+        self.__system_serial_number = system_serial_number          # string (by convention, int)
 
 
     def __eq__(self, other):
         try:
             return bool(self.last_modified) == bool(other.last_modified) and \
                    self.vendor_id == other.vendor_id and self.model_id == other.model_id and \
                    self.model_name == other.model_name and self.configuration == other.configuration and \
```

### Comparing `scs-core-2.4.6/src/scs_core/sys/tail.py` & `scs-core-2.8.1/src/scs_core/sys/tail.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sys/timer.py` & `scs-core-2.8.1/src/scs_core/sys/timer.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core/sys/uptime_datum.py` & `scs-core-2.8.1/src/scs_core/sys/uptime_datum.py`

 * *Files identical despite different names*

### Comparing `scs-core-2.4.6/src/scs_core.egg-info/SOURCES.txt` & `scs-core-2.8.1/src/scs_core.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,29 +33,33 @@
 src/scs_core/aqcsv/specification/qc.py
 src/scs_core/aqcsv/specification/qualifier.py
 src/scs_core/aqcsv/specification/unit.py
 src/scs_core/aws/__init__.py
 src/scs_core/aws/client/__init__.py
 src/scs_core/aws/client/access_key.py
 src/scs_core/aws/client/api_auth.py
+src/scs_core/aws/client/api_client.py
 src/scs_core/aws/client/client.py
 src/scs_core/aws/client/client_auth.py
+src/scs_core/aws/client/device_control_client.py
 src/scs_core/aws/client/email_client.py
 src/scs_core/aws/client/monitor_auth.py
 src/scs_core/aws/client/mqtt_client.py
 src/scs_core/aws/client/rest_client.py
 src/scs_core/aws/config/__init__.py
 src/scs_core/aws/config/aws.py
 src/scs_core/aws/config/project.py
 src/scs_core/aws/data/__init__.py
 src/scs_core/aws/data/alert.py
 src/scs_core/aws/data/byline.py
 src/scs_core/aws/data/byline_list.py
 src/scs_core/aws/data/dataset.py
 src/scs_core/aws/data/deployment.py
+src/scs_core/aws/data/device_monitor_email_list.py
+src/scs_core/aws/data/device_monitor_report.py
 src/scs_core/aws/data/device_report.py
 src/scs_core/aws/data/email_list.py
 src/scs_core/aws/data/http_response.py
 src/scs_core/aws/data/message.py
 src/scs_core/aws/data/power_list.py
 src/scs_core/aws/data/runtime_record.py
 src/scs_core/aws/data/status_list.py
@@ -66,41 +70,50 @@
 src/scs_core/aws/greengrass/aws_deployment_reporter.py
 src/scs_core/aws/greengrass/aws_group.py
 src/scs_core/aws/greengrass/aws_group_configuration.py
 src/scs_core/aws/greengrass/aws_identity.py
 src/scs_core/aws/greengrass/gg_errors.py
 src/scs_core/aws/manager/__init__.py
 src/scs_core/aws/manager/alert_specification_manager.py
-src/scs_core/aws/manager/alert_status_finder.py
+src/scs_core/aws/manager/alert_status_manager.py
 src/scs_core/aws/manager/byline_manager.py
 src/scs_core/aws/manager/configuration_check_finder.py
 src/scs_core/aws/manager/configuration_check_requester.py
 src/scs_core/aws/manager/configuration_finder.py
+src/scs_core/aws/manager/device_monitor_specification_manager.py
+src/scs_core/aws/manager/device_monitor_status_manager.py
 src/scs_core/aws/manager/dynamo_manager.py
 src/scs_core/aws/manager/ec2_message_manager.py
 src/scs_core/aws/manager/lambda_bylines.py
 src/scs_core/aws/manager/lambda_message_manager.py
 src/scs_core/aws/manager/s3_manager.py
 src/scs_core/aws/manager/sagemaker_model_manager.py
 src/scs_core/aws/manager/sagemaker_trial_manager.py
 src/scs_core/aws/security/__init__.py
-src/scs_core/aws/security/byline_filter.py
+src/scs_core/aws/security/access_key_manager.py
+src/scs_core/aws/security/cognito_client_credentials.py
 src/scs_core/aws/security/cognito_device.py
+src/scs_core/aws/security/cognito_device_creator.py
 src/scs_core/aws/security/cognito_device_finder.py
 src/scs_core/aws/security/cognito_device_manager.py
 src/scs_core/aws/security/cognito_login_manager.py
 src/scs_core/aws/security/cognito_membership.py
 src/scs_core/aws/security/cognito_password_manager.py
 src/scs_core/aws/security/cognito_user.py
 src/scs_core/aws/security/cognito_user_finder.py
 src/scs_core/aws/security/cognito_user_manager.py
+src/scs_core/aws/security/device_whitelist_manager.py
+src/scs_core/aws/security/opr_membership.py
 src/scs_core/aws/security/organisation.py
 src/scs_core/aws/security/organisation_manager.py
+src/scs_core/aws/security/path_filter.py
 src/scs_core/client/__init__.py
 src/scs_core/client/http_client.py
+src/scs_core/client/http_exception.py
+src/scs_core/client/http_status.py
 src/scs_core/client/network.py
 src/scs_core/client/resource_unavailable_exception.py
 src/scs_core/client/sftp_client_conf.py
 src/scs_core/climate/__init__.py
 src/scs_core/climate/absolute_humidity.py
 src/scs_core/climate/icp10101_datum.py
 src/scs_core/climate/mpl115a2_calib.py
@@ -269,60 +282,14 @@
 src/scs_core/model/pmx/s1/__init__.py
 src/scs_core/model/pmx/s1/pmx_request.py
 src/scs_core/model/pmx/s1/s1_pmx_inference_client.py
 src/scs_core/monitor/__init__.py
 src/scs_core/monitor/monitor_error.py
 src/scs_core/monitor/monitor_request.py
 src/scs_core/monitor/monitor_response.py
-src/scs_core/osio/__init__.py
-src/scs_core/osio/client/__init__.py
-src/scs_core/osio/client/api_auth.py
-src/scs_core/osio/client/client_auth.py
-src/scs_core/osio/client/client_exception.py
-src/scs_core/osio/client/realtime_client.py
-src/scs_core/osio/client/rest_client.py
-src/scs_core/osio/config/__init__.py
-src/scs_core/osio/config/project.py
-src/scs_core/osio/config/project_client.py
-src/scs_core/osio/config/project_source.py
-src/scs_core/osio/config/project_topic.py
-src/scs_core/osio/data/__init__.py
-src/scs_core/osio/data/abstract_topic.py
-src/scs_core/osio/data/derived_data.py
-src/scs_core/osio/data/derived_topic.py
-src/scs_core/osio/data/device.py
-src/scs_core/osio/data/device_summary.py
-src/scs_core/osio/data/device_topic.py
-src/scs_core/osio/data/error.py
-src/scs_core/osio/data/location.py
-src/scs_core/osio/data/message.py
-src/scs_core/osio/data/message_body.py
-src/scs_core/osio/data/message_event.py
-src/scs_core/osio/data/message_payload.py
-src/scs_core/osio/data/message_response.py
-src/scs_core/osio/data/message_tag.py
-src/scs_core/osio/data/organisation.py
-src/scs_core/osio/data/schema.py
-src/scs_core/osio/data/topic.py
-src/scs_core/osio/data/topic_contributor.py
-src/scs_core/osio/data/topic_info.py
-src/scs_core/osio/data/topic_metadata.py
-src/scs_core/osio/data/topic_stats.py
-src/scs_core/osio/data/topic_summary.py
-src/scs_core/osio/data/user.py
-src/scs_core/osio/data/user_metadata.py
-src/scs_core/osio/data/user_topic.py
-src/scs_core/osio/manager/__init__.py
-src/scs_core/osio/manager/device_manager.py
-src/scs_core/osio/manager/message_event_subscriber.py
-src/scs_core/osio/manager/message_manager.py
-src/scs_core/osio/manager/organisation_manager.py
-src/scs_core/osio/manager/schema_manager.py
-src/scs_core/osio/manager/topic_manager.py
-src/scs_core/osio/manager/user_manager.py
 src/scs_core/particulate/__init__.py
 src/scs_core/particulate/opc_conf.py
 src/scs_core/particulate/opc_datum.py
 src/scs_core/particulate/opc_version.py
 src/scs_core/particulate/pmx_datum.py
 src/scs_core/particulate/sps_datum.py
 src/scs_core/position/__init__.py
@@ -366,16 +333,14 @@
 src/scs_core/sys/__init__.py
 src/scs_core/sys/command.py
 src/scs_core/sys/disk_usage.py
 src/scs_core/sys/disk_volume.py
 src/scs_core/sys/eeprom_image.py
 src/scs_core/sys/exception_report.py
 src/scs_core/sys/filesystem.py
-src/scs_core/sys/http_exception.py
-src/scs_core/sys/http_status.py
 src/scs_core/sys/ipv4_address.py
 src/scs_core/sys/logging.py
 src/scs_core/sys/memory.py
 src/scs_core/sys/modem.py
 src/scs_core/sys/network.py
 src/scs_core/sys/node.py
 src/scs_core/sys/persistence_manager.py
```

