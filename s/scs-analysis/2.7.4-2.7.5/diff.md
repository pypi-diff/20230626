# Comparing `tmp/scs-analysis-2.7.4.tar.gz` & `tmp/scs-analysis-2.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs-analysis-2.7.4.tar", last modified: Mon Jun 26 10:36:59 2023, max compression
+gzip compressed data, was "scs-analysis-2.7.5.tar", last modified: Mon Jun 26 10:46:13 2023, max compression
```

## Comparing `scs-analysis-2.7.4.tar` & `scs-analysis-2.7.5.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:36:59.055981 scs-analysis-2.7.4/
--rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/LICENSE
--rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/MANIFEST.in
--rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-06-26 10:36:59.055981 scs-analysis-2.7.4/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)      766 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/README.md
--rw-rw-r--   0 jade      (1002) jade      (1002)       41 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/README.rst
--rw-rw-r--   0 jade      (1002) jade      (1002)      217 2023-06-26 10:36:47.000000 scs-analysis-2.7.4/requirements.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-06-26 10:36:59.055981 scs-analysis-2.7.4/setup.cfg
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5100 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/setup.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:36:59.043981 scs-analysis-2.7.4/src/
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:36:59.047981 scs-analysis-2.7.4/src/scs_analysis/
--rwxrwxr-x   0 jade      (1002) jade      (1002)      183 2023-06-26 10:36:47.000000 scs-analysis-2.7.4/src/scs_analysis/__init__.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2467 2023-04-17 09:22:53.000000 scs-analysis-2.7.4/src/scs_analysis/access_key.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)    10112 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/alert.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4014 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/alert_status.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2235 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/aws_api_auth.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4611 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/aws_byline.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2655 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/aws_client_auth.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7224 2023-02-06 14:01:57.000000 scs-analysis-2.7.4/src/scs_analysis/aws_mqtt_client.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7079 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/aws_topic_history.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2139 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/aws_topic_publisher.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2918 2023-02-06 14:01:57.000000 scs-analysis-2.7.4/src/scs_analysis/aws_upload_interval.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)    14469 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/baseline.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5964 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/baseline_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:36:59.047981 scs-analysis-2.7.4/src/scs_analysis/chart/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/chart/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1630 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/chart/chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4546 2023-04-17 09:22:53.000000 scs-analysis-2.7.4/src/scs_analysis/chart/histo_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4249 2023-04-17 09:22:53.000000 scs-analysis-2.7.4/src/scs_analysis/chart/multi_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4317 2023-04-17 09:22:53.000000 scs-analysis-2.7.4/src/scs_analysis/chart/single_chart.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:36:59.055981 scs-analysis-2.7.4/src/scs_analysis/cmd/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1966 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_access_key.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     9948 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_alert.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5170 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_alert_status.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2713 2022-11-09 12:09:25.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_aws_api_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3826 2022-11-09 12:09:25.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_aws_byline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3092 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_aws_client_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7868 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_aws_topic_history.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1522 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7348 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6605 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_baseline_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4572 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_cognito_devices.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2943 2023-03-20 10:12:25.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_cognito_password.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3570 2023-03-20 10:12:25.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3183 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_cognito_user_identity.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7027 2023-03-20 10:12:25.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_cognito_users.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5419 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_configuration_csv.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4706 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_configuration_monitor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4426 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3321 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_csv_collation_summary.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2867 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_csv_collator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3410 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_csv_join.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2774 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_csv_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2761 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_csv_segmentor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3372 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_csv_writer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3657 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_device_controller.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4066 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_histo_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3039 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_localised_datetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2011 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_monitor_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5603 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_mqtt_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3378 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_multi_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3490 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_node.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5404 2023-03-20 10:12:25.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_organisation_devices.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4524 2023-04-17 09:22:53.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_organisation_path_roots.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4630 2023-04-17 09:22:53.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_organisation_user_paths.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6422 2023-03-20 10:12:25.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_organisation_users.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4992 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_organisations.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3560 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_aggregate.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3536 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_collator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2628 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_concentration.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2813 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_distance.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2189 2023-04-17 09:22:53.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_duplicates.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3020 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_error.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1677 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_filter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1688 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_interval.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4763 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_iso_8601.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2566 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_low_pass.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2312 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_median.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2782 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_nullify.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1224 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_paths.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1579 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_record.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3899 2023-04-17 09:22:53.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_slope.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1577 2022-09-20 10:07:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_sort.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3100 2022-09-20 10:07:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_stats.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5204 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_subset.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2264 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_tally.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2566 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_time_shift.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2325 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_timezone.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3701 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_single_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1441 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_socket_receiver.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1540 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_uds.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5093 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/cognito_devices.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5753 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/cognito_password.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5483 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/cognito_user_credentials.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7801 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/cognito_user_identity.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7743 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/cognito_users.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7418 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/configuration_csv.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3494 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/configuration_monitor.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3854 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/configuration_monitor_check.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6401 2023-02-06 14:01:57.000000 scs-analysis-2.7.4/src/scs_analysis/csv_collation_summary.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3967 2023-02-06 14:01:57.000000 scs-analysis-2.7.4/src/scs_analysis/csv_collator.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6835 2023-02-06 14:01:57.000000 scs-analysis-2.7.4/src/scs_analysis/csv_join.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5065 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/csv_reader.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4697 2023-02-06 14:01:57.000000 scs-analysis-2.7.4/src/scs_analysis/csv_segmentor.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3800 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/csv_writer.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6115 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/device_controller.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:36:59.055981 scs-analysis-2.7.4/src/scs_analysis/handler/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/handler/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4051 2023-03-20 10:12:25.000000 scs-analysis-2.7.4/src/scs_analysis/handler/aws_mqtt_publisher.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2329 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/handler/batch_download_reporter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1436 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/handler/configuration_csv_generator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5557 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/handler/csv_collator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5893 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/handler/csv_segmentor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1184 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/handler/mqtt_reporter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2007 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/handler/sample_midpoint.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/handler/sample_regression.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4308 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/histo_chart.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2127 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/localised_datetime.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2544 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/monitor_auth.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4367 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/multi_chart.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5982 2023-02-06 14:01:57.000000 scs-analysis-2.7.4/src/scs_analysis/node.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5896 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/organisation_devices.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4713 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/organisation_path_roots.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4925 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/organisation_user_paths.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5783 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/organisation_users.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5300 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/organisations.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7233 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/sample_aggregate.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4821 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/sample_average.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5162 2023-02-06 14:01:57.000000 scs-analysis-2.7.4/src/scs_analysis/sample_collator.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5566 2023-02-06 14:01:57.000000 scs-analysis-2.7.4/src/scs_analysis/sample_concentration.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3970 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/sample_distance.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3765 2023-04-17 09:22:53.000000 scs-analysis-2.7.4/src/scs_analysis/sample_duplicates.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4685 2023-02-06 14:01:57.000000 scs-analysis-2.7.4/src/scs_analysis/sample_error.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3102 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/sample_interval.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7990 2023-02-06 14:01:57.000000 scs-analysis-2.7.4/src/scs_analysis/sample_iso_8601.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3802 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/sample_low_pass.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3571 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/sample_max.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3776 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/sample_median.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3529 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/sample_midpoint.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3570 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/sample_min.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5072 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/sample_noise.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4017 2023-02-06 14:01:57.000000 scs-analysis-2.7.4/src/scs_analysis/sample_nullify.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1667 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/sample_paths.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3320 2023-06-26 09:33:48.000000 scs-analysis-2.7.4/src/scs_analysis/sample_regression.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5707 2023-04-17 09:22:53.000000 scs-analysis-2.7.4/src/scs_analysis/sample_slope.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2502 2023-02-06 14:01:57.000000 scs-analysis-2.7.4/src/scs_analysis/sample_sort.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5928 2022-09-20 10:07:36.000000 scs-analysis-2.7.4/src/scs_analysis/sample_stats.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6001 2023-02-06 14:01:57.000000 scs-analysis-2.7.4/src/scs_analysis/sample_subset.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2897 2023-02-06 14:01:57.000000 scs-analysis-2.7.4/src/scs_analysis/sample_time_shift.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4732 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/sample_timezone.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4463 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/single_chart.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2451 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/socket_receiver.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1891 2023-02-06 14:01:57.000000 scs-analysis-2.7.4/src/scs_analysis/timer.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1849 2022-08-17 09:53:36.000000 scs-analysis-2.7.4/src/scs_analysis/uds_receiver.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:36:59.047981 scs-analysis-2.7.4/src/scs_analysis.egg-info/
--rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-06-26 10:36:59.000000 scs-analysis-2.7.4/src/scs_analysis.egg-info/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)     5870 2023-06-26 10:36:59.000000 scs-analysis-2.7.4/src/scs_analysis.egg-info/SOURCES.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-06-26 10:36:59.000000 scs-analysis-2.7.4/src/scs_analysis.egg-info/dependency_links.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)      232 2023-06-26 10:36:59.000000 scs-analysis-2.7.4/src/scs_analysis.egg-info/requires.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)       13 2023-06-26 10:36:59.000000 scs-analysis-2.7.4/src/scs_analysis.egg-info/top_level.txt
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:46:13.763654 scs-analysis-2.7.5/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/LICENSE
+-rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/MANIFEST.in
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-06-26 10:46:13.763654 scs-analysis-2.7.5/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)      766 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/README.md
+-rw-rw-r--   0 jade      (1002) jade      (1002)       41 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/README.rst
+-rw-rw-r--   0 jade      (1002) jade      (1002)      232 2023-06-26 10:45:57.000000 scs-analysis-2.7.5/requirements.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-06-26 10:46:13.763654 scs-analysis-2.7.5/setup.cfg
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5100 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/setup.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:46:13.751654 scs-analysis-2.7.5/src/
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:46:13.755654 scs-analysis-2.7.5/src/scs_analysis/
+-rwxrwxr-x   0 jade      (1002) jade      (1002)      183 2023-06-26 10:45:57.000000 scs-analysis-2.7.5/src/scs_analysis/__init__.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2467 2023-04-17 09:22:53.000000 scs-analysis-2.7.5/src/scs_analysis/access_key.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)    10112 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/alert.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4014 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/alert_status.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2235 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/aws_api_auth.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4611 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/aws_byline.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2655 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/aws_client_auth.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7224 2023-02-06 14:01:57.000000 scs-analysis-2.7.5/src/scs_analysis/aws_mqtt_client.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7079 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/aws_topic_history.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2139 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/aws_topic_publisher.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2918 2023-02-06 14:01:57.000000 scs-analysis-2.7.5/src/scs_analysis/aws_upload_interval.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)    14469 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/baseline.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5964 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/baseline_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:46:13.755654 scs-analysis-2.7.5/src/scs_analysis/chart/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/chart/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1630 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/chart/chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4546 2023-04-17 09:22:53.000000 scs-analysis-2.7.5/src/scs_analysis/chart/histo_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4249 2023-04-17 09:22:53.000000 scs-analysis-2.7.5/src/scs_analysis/chart/multi_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4317 2023-04-17 09:22:53.000000 scs-analysis-2.7.5/src/scs_analysis/chart/single_chart.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:46:13.759654 scs-analysis-2.7.5/src/scs_analysis/cmd/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1966 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_access_key.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9948 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_alert.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5170 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_alert_status.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2713 2022-11-09 12:09:25.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_aws_api_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3826 2022-11-09 12:09:25.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_aws_byline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3092 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_aws_client_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7868 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_aws_topic_history.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1522 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7348 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6605 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_baseline_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4572 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_cognito_devices.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2943 2023-03-20 10:12:25.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_cognito_password.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3570 2023-03-20 10:12:25.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3183 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_cognito_user_identity.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7027 2023-03-20 10:12:25.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_cognito_users.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5419 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_configuration_csv.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4706 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_configuration_monitor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4426 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3321 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_csv_collation_summary.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2867 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_csv_collator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3410 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_csv_join.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2774 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_csv_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2761 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_csv_segmentor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3372 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_csv_writer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3657 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_device_controller.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4066 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_histo_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3039 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_localised_datetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2011 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_monitor_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5603 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_mqtt_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3378 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_multi_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3490 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_node.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5404 2023-03-20 10:12:25.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_organisation_devices.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4524 2023-04-17 09:22:53.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_organisation_path_roots.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4630 2023-04-17 09:22:53.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_organisation_user_paths.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6422 2023-03-20 10:12:25.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_organisation_users.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4992 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_organisations.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3560 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_aggregate.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3536 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_collator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2628 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_concentration.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2813 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_distance.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2189 2023-04-17 09:22:53.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_duplicates.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3020 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_error.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1677 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_filter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1688 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_interval.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4763 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_iso_8601.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2566 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_low_pass.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2312 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_median.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2782 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_nullify.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1224 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_paths.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1579 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_record.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3899 2023-04-17 09:22:53.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_slope.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1577 2022-09-20 10:07:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_sort.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3100 2022-09-20 10:07:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_stats.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5204 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_subset.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2264 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_tally.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2566 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_time_shift.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2325 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_timezone.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3701 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_single_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1441 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_socket_receiver.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1540 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_uds.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5093 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/cognito_devices.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5753 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/cognito_password.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5483 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/cognito_user_credentials.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7801 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/cognito_user_identity.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7743 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/cognito_users.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7418 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/configuration_csv.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3494 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/configuration_monitor.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3854 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/configuration_monitor_check.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6401 2023-02-06 14:01:57.000000 scs-analysis-2.7.5/src/scs_analysis/csv_collation_summary.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3967 2023-02-06 14:01:57.000000 scs-analysis-2.7.5/src/scs_analysis/csv_collator.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6835 2023-02-06 14:01:57.000000 scs-analysis-2.7.5/src/scs_analysis/csv_join.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5065 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/csv_reader.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4697 2023-02-06 14:01:57.000000 scs-analysis-2.7.5/src/scs_analysis/csv_segmentor.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3800 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/csv_writer.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6115 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/device_controller.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:46:13.763654 scs-analysis-2.7.5/src/scs_analysis/handler/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/handler/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4051 2023-03-20 10:12:25.000000 scs-analysis-2.7.5/src/scs_analysis/handler/aws_mqtt_publisher.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2329 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/handler/batch_download_reporter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1436 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/handler/configuration_csv_generator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5557 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/handler/csv_collator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5893 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/handler/csv_segmentor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1184 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/handler/mqtt_reporter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2007 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/handler/sample_midpoint.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/handler/sample_regression.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4308 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/histo_chart.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2127 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/localised_datetime.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2544 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/monitor_auth.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4367 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/multi_chart.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5982 2023-02-06 14:01:57.000000 scs-analysis-2.7.5/src/scs_analysis/node.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5896 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/organisation_devices.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4713 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/organisation_path_roots.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4925 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/organisation_user_paths.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5783 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/organisation_users.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5300 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/organisations.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7233 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/sample_aggregate.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4821 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/sample_average.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5162 2023-02-06 14:01:57.000000 scs-analysis-2.7.5/src/scs_analysis/sample_collator.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5566 2023-02-06 14:01:57.000000 scs-analysis-2.7.5/src/scs_analysis/sample_concentration.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3970 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/sample_distance.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3765 2023-04-17 09:22:53.000000 scs-analysis-2.7.5/src/scs_analysis/sample_duplicates.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4685 2023-02-06 14:01:57.000000 scs-analysis-2.7.5/src/scs_analysis/sample_error.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3102 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/sample_interval.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7990 2023-02-06 14:01:57.000000 scs-analysis-2.7.5/src/scs_analysis/sample_iso_8601.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3802 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/sample_low_pass.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3571 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/sample_max.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3776 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/sample_median.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3529 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/sample_midpoint.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3570 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/sample_min.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5072 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/sample_noise.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4017 2023-02-06 14:01:57.000000 scs-analysis-2.7.5/src/scs_analysis/sample_nullify.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1667 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/sample_paths.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3320 2023-06-26 09:33:48.000000 scs-analysis-2.7.5/src/scs_analysis/sample_regression.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5707 2023-04-17 09:22:53.000000 scs-analysis-2.7.5/src/scs_analysis/sample_slope.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2502 2023-02-06 14:01:57.000000 scs-analysis-2.7.5/src/scs_analysis/sample_sort.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5928 2022-09-20 10:07:36.000000 scs-analysis-2.7.5/src/scs_analysis/sample_stats.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6001 2023-02-06 14:01:57.000000 scs-analysis-2.7.5/src/scs_analysis/sample_subset.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2897 2023-02-06 14:01:57.000000 scs-analysis-2.7.5/src/scs_analysis/sample_time_shift.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4732 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/sample_timezone.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4463 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/single_chart.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2451 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/socket_receiver.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1891 2023-02-06 14:01:57.000000 scs-analysis-2.7.5/src/scs_analysis/timer.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1849 2022-08-17 09:53:36.000000 scs-analysis-2.7.5/src/scs_analysis/uds_receiver.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 10:46:13.755654 scs-analysis-2.7.5/src/scs_analysis.egg-info/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-06-26 10:46:13.000000 scs-analysis-2.7.5/src/scs_analysis.egg-info/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5870 2023-06-26 10:46:13.000000 scs-analysis-2.7.5/src/scs_analysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-06-26 10:46:13.000000 scs-analysis-2.7.5/src/scs_analysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)      247 2023-06-26 10:46:13.000000 scs-analysis-2.7.5/src/scs_analysis.egg-info/requires.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)       13 2023-06-26 10:46:13.000000 scs-analysis-2.7.5/src/scs_analysis.egg-info/top_level.txt
```

### Comparing `scs-analysis-2.7.4/LICENSE` & `scs-analysis-2.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/PKG-INFO` & `scs-analysis-2.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 2.7.4
+Version: 2.7.5
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `scs-analysis-2.7.4/README.md` & `scs-analysis-2.7.5/README.md`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/setup.py` & `scs-analysis-2.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/access_key.py` & `scs-analysis-2.7.5/src/scs_analysis/access_key.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/alert.py` & `scs-analysis-2.7.5/src/scs_analysis/alert.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/alert_status.py` & `scs-analysis-2.7.5/src/scs_analysis/alert_status.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/aws_api_auth.py` & `scs-analysis-2.7.5/src/scs_analysis/aws_api_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/aws_byline.py` & `scs-analysis-2.7.5/src/scs_analysis/aws_byline.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/aws_client_auth.py` & `scs-analysis-2.7.5/src/scs_analysis/aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/aws_mqtt_client.py` & `scs-analysis-2.7.5/src/scs_analysis/aws_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/aws_topic_history.py` & `scs-analysis-2.7.5/src/scs_analysis/aws_topic_history.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/aws_topic_publisher.py` & `scs-analysis-2.7.5/src/scs_analysis/aws_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/aws_upload_interval.py` & `scs-analysis-2.7.5/src/scs_analysis/aws_upload_interval.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/baseline.py` & `scs-analysis-2.7.5/src/scs_analysis/baseline.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/baseline_conf.py` & `scs-analysis-2.7.5/src/scs_analysis/baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/chart/chart.py` & `scs-analysis-2.7.5/src/scs_analysis/chart/chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/chart/histo_chart.py` & `scs-analysis-2.7.5/src/scs_analysis/chart/histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/chart/multi_chart.py` & `scs-analysis-2.7.5/src/scs_analysis/chart/multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/chart/single_chart.py` & `scs-analysis-2.7.5/src/scs_analysis/chart/single_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_access_key.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_access_key.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_alert.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_alert.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_alert_status.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_alert_status.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_aws_api_auth.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_aws_api_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_aws_byline.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_aws_byline.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_aws_client_auth.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_aws_topic_history.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_aws_topic_history.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_aws_topic_publisher.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_aws_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_baseline.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_baseline.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_baseline_conf.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_cognito_devices.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_cognito_devices.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_cognito_password.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_cognito_password.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_cognito_user_credentials.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_cognito_user_credentials.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_cognito_user_identity.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_cognito_user_identity.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_cognito_users.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_cognito_users.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_configuration_csv.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_configuration_csv.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_configuration_monitor.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_configuration_monitor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_configuration_monitor_check.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_configuration_monitor_check.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_csv_collation_summary.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_csv_collation_summary.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_csv_collator.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_csv_join.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_csv_join.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_csv_reader.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_csv_segmentor.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_csv_writer.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_device_controller.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_device_controller.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_histo_chart.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_localised_datetime.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_localised_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_monitor_auth.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_mqtt_client.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_multi_chart.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_node.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_node.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_organisation_devices.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_organisation_devices.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_organisation_path_roots.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_organisation_path_roots.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_organisation_user_paths.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_organisation_user_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_organisation_users.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_organisation_users.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_organisations.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_organisations.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_aggregate.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_aggregate.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_collator.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_concentration.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_concentration.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_distance.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_distance.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_duplicates.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_duplicates.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_error.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_error.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_filter.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_filter.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_interval.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_interval.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_iso_8601.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_iso_8601.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_low_pass.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_low_pass.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_median.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_median.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_nullify.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_nullify.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_paths.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_record.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_record.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_slope.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_slope.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_sort.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_sort.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_stats.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_stats.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_subset.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_subset.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_tally.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_tally.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_time_shift.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_time_shift.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_sample_timezone.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_sample_timezone.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_single_chart.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_single_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_socket_receiver.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_socket_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cmd/cmd_uds.py` & `scs-analysis-2.7.5/src/scs_analysis/cmd/cmd_uds.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cognito_devices.py` & `scs-analysis-2.7.5/src/scs_analysis/cognito_devices.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cognito_password.py` & `scs-analysis-2.7.5/src/scs_analysis/cognito_password.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cognito_user_credentials.py` & `scs-analysis-2.7.5/src/scs_analysis/cognito_user_credentials.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cognito_user_identity.py` & `scs-analysis-2.7.5/src/scs_analysis/cognito_user_identity.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/cognito_users.py` & `scs-analysis-2.7.5/src/scs_analysis/cognito_users.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/configuration_csv.py` & `scs-analysis-2.7.5/src/scs_analysis/configuration_csv.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/configuration_monitor.py` & `scs-analysis-2.7.5/src/scs_analysis/configuration_monitor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/configuration_monitor_check.py` & `scs-analysis-2.7.5/src/scs_analysis/configuration_monitor_check.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/csv_collation_summary.py` & `scs-analysis-2.7.5/src/scs_analysis/csv_collation_summary.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/csv_collator.py` & `scs-analysis-2.7.5/src/scs_analysis/csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/csv_join.py` & `scs-analysis-2.7.5/src/scs_analysis/csv_join.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/csv_reader.py` & `scs-analysis-2.7.5/src/scs_analysis/csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/csv_segmentor.py` & `scs-analysis-2.7.5/src/scs_analysis/csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/csv_writer.py` & `scs-analysis-2.7.5/src/scs_analysis/csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/device_controller.py` & `scs-analysis-2.7.5/src/scs_analysis/device_controller.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/handler/aws_mqtt_publisher.py` & `scs-analysis-2.7.5/src/scs_analysis/handler/aws_mqtt_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/handler/aws_mqtt_subscription_handler.py` & `scs-analysis-2.7.5/src/scs_analysis/handler/aws_mqtt_subscription_handler.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/handler/batch_download_reporter.py` & `scs-analysis-2.7.5/src/scs_analysis/handler/batch_download_reporter.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/handler/configuration_csv_generator.py` & `scs-analysis-2.7.5/src/scs_analysis/handler/configuration_csv_generator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/handler/csv_collator.py` & `scs-analysis-2.7.5/src/scs_analysis/handler/csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/handler/csv_segmentor.py` & `scs-analysis-2.7.5/src/scs_analysis/handler/csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/handler/mqtt_reporter.py` & `scs-analysis-2.7.5/src/scs_analysis/handler/mqtt_reporter.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/handler/sample_midpoint.py` & `scs-analysis-2.7.5/src/scs_analysis/handler/sample_midpoint.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/handler/sample_regression.py` & `scs-analysis-2.7.5/src/scs_analysis/handler/sample_regression.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/histo_chart.py` & `scs-analysis-2.7.5/src/scs_analysis/histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/localised_datetime.py` & `scs-analysis-2.7.5/src/scs_analysis/localised_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/monitor_auth.py` & `scs-analysis-2.7.5/src/scs_analysis/monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/multi_chart.py` & `scs-analysis-2.7.5/src/scs_analysis/multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/node.py` & `scs-analysis-2.7.5/src/scs_analysis/node.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/organisation_devices.py` & `scs-analysis-2.7.5/src/scs_analysis/organisation_devices.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/organisation_path_roots.py` & `scs-analysis-2.7.5/src/scs_analysis/organisation_path_roots.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/organisation_user_paths.py` & `scs-analysis-2.7.5/src/scs_analysis/organisation_user_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/organisation_users.py` & `scs-analysis-2.7.5/src/scs_analysis/organisation_users.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/organisations.py` & `scs-analysis-2.7.5/src/scs_analysis/organisations.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_aggregate.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_aggregate.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_average.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_average.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_collator.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_concentration.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_concentration.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_distance.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_distance.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_duplicates.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_duplicates.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_error.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_error.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_interval.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_interval.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_iso_8601.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_iso_8601.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_low_pass.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_low_pass.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_max.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_max.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_median.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_median.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_midpoint.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_midpoint.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_min.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_min.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_noise.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_noise.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_nullify.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_nullify.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_paths.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_regression.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_regression.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_slope.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_slope.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_sort.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_sort.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_stats.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_stats.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_subset.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_subset.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_time_shift.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_time_shift.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/sample_timezone.py` & `scs-analysis-2.7.5/src/scs_analysis/sample_timezone.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/single_chart.py` & `scs-analysis-2.7.5/src/scs_analysis/single_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/socket_receiver.py` & `scs-analysis-2.7.5/src/scs_analysis/socket_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/timer.py` & `scs-analysis-2.7.5/src/scs_analysis/timer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis/uds_receiver.py` & `scs-analysis-2.7.5/src/scs_analysis/uds_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.7.4/src/scs_analysis.egg-info/PKG-INFO` & `scs-analysis-2.7.5/src/scs_analysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 2.7.4
+Version: 2.7.5
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `scs-analysis-2.7.4/src/scs_analysis.egg-info/SOURCES.txt` & `scs-analysis-2.7.5/src/scs_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

