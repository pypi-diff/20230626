# Comparing `tmp/scs-analysis-2.0.0.tar.gz` & `tmp/scs-analysis-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs-analysis-2.0.0.tar", last modified: Mon Apr 17 09:23:19 2023, max compression
+gzip compressed data, was "scs-analysis-2.7.2.tar", last modified: Mon Jun 26 09:35:20 2023, max compression
```

## Comparing `scs-analysis-2.0.0.tar` & `scs-analysis-2.7.2.tar`

### file list

```diff
@@ -1,177 +1,162 @@
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-04-17 09:23:19.674593 scs-analysis-2.0.0/
--rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/LICENSE
--rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/MANIFEST.in
--rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-04-17 09:23:19.674593 scs-analysis-2.0.0/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)      766 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/README.md
--rw-rw-r--   0 jade      (1002) jade      (1002)       41 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/README.rst
--rw-rw-r--   0 jade      (1002) jade      (1002)      235 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/requirements.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-04-17 09:23:19.674593 scs-analysis-2.0.0/setup.cfg
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5453 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/setup.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-04-17 09:23:19.642593 scs-analysis-2.0.0/src/
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-04-17 09:23:19.658594 scs-analysis-2.0.0/src/scs_analysis/
--rwxrwxr-x   0 jade      (1002) jade      (1002)      183 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/__init__.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2467 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/access_key.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     8568 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/alert.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3559 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/alert_status.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2235 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/aws_api_auth.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4536 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/aws_byline.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2655 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/aws_client_auth.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7224 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/aws_mqtt_client.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7386 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/aws_mqtt_control.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6971 2023-03-20 10:12:25.000000 scs-analysis-2.0.0/src/scs_analysis/aws_topic_history.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2139 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/aws_topic_publisher.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2918 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/aws_upload_interval.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)    15290 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/baseline.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5964 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/baseline_conf.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-04-17 09:23:19.658594 scs-analysis-2.0.0/src/scs_analysis/chart/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/chart/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1630 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/chart/chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4546 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/chart/histo_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4249 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/chart/multi_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4317 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/chart/single_chart.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-04-17 09:23:19.670593 scs-analysis-2.0.0/src/scs_analysis/cmd/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1966 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_access_key.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7915 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_alert.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3474 2022-09-20 10:07:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_alert_status.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2713 2022-11-09 12:09:25.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_api_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3826 2022-11-09 12:09:25.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_byline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3092 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_client_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7868 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_topic_history.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1522 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7223 2022-09-20 10:07:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_baseline.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6605 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_baseline_conf.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4498 2023-03-20 10:12:25.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_devices.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2943 2023-03-20 10:12:25.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_password.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3570 2023-03-20 10:12:25.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3183 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_user_identity.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     7027 2023-03-20 10:12:25.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_users.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5051 2022-09-20 10:07:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_configuration_csv.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4330 2022-09-20 10:07:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_configuration_monitor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4076 2022-09-20 10:07:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3321 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_collation_summary.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2867 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_collator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3410 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_join.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2774 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_reader.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2761 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_segmentor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3372 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_writer.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4066 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_histo_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3039 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_localised_datetime.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2011 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_monitor_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5603 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_mqtt_client.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4622 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_mqtt_control.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6780 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_mqtt_peers.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3378 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_multi_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3490 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_node.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5404 2023-03-20 10:12:25.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisation_devices.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4524 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisation_path_roots.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4630 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisation_user_paths.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     6422 2023-03-20 10:12:25.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisation_users.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4992 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisations.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1931 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_osio_api_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2265 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_osio_client_auth.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1571 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_osio_topic.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3892 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_osio_topic_history.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2678 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_osio_topic_publisher.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3560 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_aggregate.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3536 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_collator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2628 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_concentration.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2813 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_distance.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2189 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_duplicates.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3020 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_error.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1677 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_filter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1688 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_interval.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4763 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_iso_8601.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2566 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_low_pass.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2312 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_median.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2782 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_nullify.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1224 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_paths.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1579 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_record.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3899 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_slope.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1577 2022-09-20 10:07:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_sort.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3100 2022-09-20 10:07:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_stats.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5204 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_subset.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2264 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_tally.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2566 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_time_shift.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2325 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_timezone.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     3701 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_single_chart.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1441 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_socket_receiver.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1540 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_uds.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5870 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/cognito_devices.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5742 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/cognito_password.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5459 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/cognito_user_credentials.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     8074 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/cognito_user_identity.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     8110 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/cognito_users.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7280 2022-09-20 10:07:36.000000 scs-analysis-2.0.0/src/scs_analysis/configuration_csv.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3362 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/configuration_monitor.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3697 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/configuration_monitor_check.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6401 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/csv_collation_summary.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3967 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/csv_collator.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6835 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/csv_join.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5065 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/csv_reader.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4697 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/csv_segmentor.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3800 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/csv_writer.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-04-17 09:23:19.674593 scs-analysis-2.0.0/src/scs_analysis/handler/
--rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/__init__.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     4051 2023-03-20 10:12:25.000000 scs-analysis-2.0.0/src/scs_analysis/handler/aws_mqtt_publisher.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2329 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/batch_download_reporter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1436 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/configuration_csv_generator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5557 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/csv_collator.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     5893 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/csv_segmentor.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1184 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/mqtt_reporter.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1552 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/osio_mqtt_client_handler.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     1622 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/osio_mqtt_control_handler.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2007 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/sample_midpoint.py
--rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/handler/sample_regression.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4308 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/histo_chart.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2127 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/localised_datetime.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2544 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/monitor_auth.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6301 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/mqtt_peers.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4367 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/multi_chart.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5982 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/node.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6237 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/organisation_devices.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5053 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/organisation_path_roots.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5266 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/organisation_user_paths.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6124 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/organisation_users.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5640 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/organisations.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1637 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/osio_api_auth.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4951 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/osio_client_auth.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5808 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/osio_mqtt_client.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6563 2023-03-20 10:12:25.000000 scs-analysis-2.0.0/src/scs_analysis/osio_mqtt_control.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3912 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/osio_topic_history.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3738 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/osio_topic_publisher.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7233 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/sample_aggregate.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4822 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_average.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5162 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_collator.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5566 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_concentration.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3970 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/sample_distance.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3765 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/sample_duplicates.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4685 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_error.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3103 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_interval.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     7990 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_iso_8601.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3803 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_low_pass.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3572 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_max.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3777 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_median.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3530 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_midpoint.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3571 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_min.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5072 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/sample_noise.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4017 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_nullify.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1667 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/sample_paths.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     3321 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/sample_regression.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5707 2023-04-17 09:22:53.000000 scs-analysis-2.0.0/src/scs_analysis/sample_slope.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2502 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_sort.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     5928 2022-09-20 10:07:36.000000 scs-analysis-2.0.0/src/scs_analysis/sample_stats.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     6001 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_subset.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2897 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/sample_time_shift.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4732 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/sample_timezone.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     4463 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/single_chart.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     2451 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/socket_receiver.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1891 2023-02-06 14:01:57.000000 scs-analysis-2.0.0/src/scs_analysis/timer.py
--rwxrwxr-x   0 jade      (1002) jade      (1002)     1849 2022-08-17 09:53:36.000000 scs-analysis-2.0.0/src/scs_analysis/uds_receiver.py
-drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-04-17 09:23:19.658594 scs-analysis-2.0.0/src/scs_analysis.egg-info/
--rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-04-17 09:23:19.000000 scs-analysis-2.0.0/src/scs_analysis.egg-info/PKG-INFO
--rw-rw-r--   0 jade      (1002) jade      (1002)     6489 2023-04-17 09:23:19.000000 scs-analysis-2.0.0/src/scs_analysis.egg-info/SOURCES.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-04-17 09:23:19.000000 scs-analysis-2.0.0/src/scs_analysis.egg-info/dependency_links.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)      250 2023-04-17 09:23:19.000000 scs-analysis-2.0.0/src/scs_analysis.egg-info/requires.txt
--rw-rw-r--   0 jade      (1002) jade      (1002)       13 2023-04-17 09:23:19.000000 scs-analysis-2.0.0/src/scs_analysis.egg-info/top_level.txt
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:35:20.542601 scs-analysis-2.7.2/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1076 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/LICENSE
+-rw-rw-r--   0 jade      (1002) jade      (1002)       32 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/MANIFEST.in
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-06-26 09:35:20.542601 scs-analysis-2.7.2/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)      766 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/README.md
+-rw-rw-r--   0 jade      (1002) jade      (1002)       41 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/README.rst
+-rw-rw-r--   0 jade      (1002) jade      (1002)      232 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/requirements.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)       38 2023-06-26 09:35:20.542601 scs-analysis-2.7.2/setup.cfg
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5100 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/setup.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:35:20.530601 scs-analysis-2.7.2/src/
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:35:20.534601 scs-analysis-2.7.2/src/scs_analysis/
+-rwxrwxr-x   0 jade      (1002) jade      (1002)      183 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/__init__.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2467 2023-04-17 09:22:53.000000 scs-analysis-2.7.2/src/scs_analysis/access_key.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)    10112 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/alert.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4014 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/alert_status.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2235 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/aws_api_auth.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4611 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/aws_byline.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2655 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/aws_client_auth.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7224 2023-02-06 14:01:57.000000 scs-analysis-2.7.2/src/scs_analysis/aws_mqtt_client.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7079 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/aws_topic_history.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2139 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/aws_topic_publisher.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2918 2023-02-06 14:01:57.000000 scs-analysis-2.7.2/src/scs_analysis/aws_upload_interval.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)    14469 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/baseline.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5964 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/baseline_conf.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:35:20.538601 scs-analysis-2.7.2/src/scs_analysis/chart/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/chart/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1630 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/chart/chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4546 2023-04-17 09:22:53.000000 scs-analysis-2.7.2/src/scs_analysis/chart/histo_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4249 2023-04-17 09:22:53.000000 scs-analysis-2.7.2/src/scs_analysis/chart/multi_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4317 2023-04-17 09:22:53.000000 scs-analysis-2.7.2/src/scs_analysis/chart/single_chart.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:35:20.542601 scs-analysis-2.7.2/src/scs_analysis/cmd/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1966 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_access_key.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     9948 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_alert.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5170 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_alert_status.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2713 2022-11-09 12:09:25.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_aws_api_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3826 2022-11-09 12:09:25.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_aws_byline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3092 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_aws_client_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7868 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_aws_topic_history.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1522 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_aws_topic_publisher.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7348 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_baseline.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6605 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_baseline_conf.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4572 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_cognito_devices.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2943 2023-03-20 10:12:25.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_cognito_password.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3570 2023-03-20 10:12:25.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_cognito_user_credentials.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3183 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_cognito_user_identity.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     7027 2023-03-20 10:12:25.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_cognito_users.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5419 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_configuration_csv.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4706 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_configuration_monitor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4426 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_configuration_monitor_check.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3321 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_csv_collation_summary.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2867 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_csv_collator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3410 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_csv_join.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2774 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_csv_reader.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2761 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_csv_segmentor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3372 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_csv_writer.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3657 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_device_controller.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4066 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_histo_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3039 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_localised_datetime.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2011 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_monitor_auth.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5603 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_mqtt_client.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3378 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_multi_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3490 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_node.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5404 2023-03-20 10:12:25.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_organisation_devices.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4524 2023-04-17 09:22:53.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_organisation_path_roots.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4630 2023-04-17 09:22:53.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_organisation_user_paths.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     6422 2023-03-20 10:12:25.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_organisation_users.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4992 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_organisations.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3560 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_aggregate.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3536 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_collator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2628 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_concentration.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2813 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_distance.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2189 2023-04-17 09:22:53.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_duplicates.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3020 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_error.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1677 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_filter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1688 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_interval.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4763 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_iso_8601.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2566 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_low_pass.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2312 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_median.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2782 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_nullify.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1224 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_paths.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1579 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_record.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3899 2023-04-17 09:22:53.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_slope.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1577 2022-09-20 10:07:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_sort.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3100 2022-09-20 10:07:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_stats.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5204 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_subset.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2264 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_tally.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2566 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_time_shift.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2325 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_timezone.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     3701 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_single_chart.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1441 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_socket_receiver.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1540 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_uds.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5093 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/cognito_devices.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5753 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/cognito_password.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5483 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/cognito_user_credentials.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7801 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/cognito_user_identity.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7743 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/cognito_users.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7418 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/configuration_csv.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3494 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/configuration_monitor.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3854 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/configuration_monitor_check.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6401 2023-02-06 14:01:57.000000 scs-analysis-2.7.2/src/scs_analysis/csv_collation_summary.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3967 2023-02-06 14:01:57.000000 scs-analysis-2.7.2/src/scs_analysis/csv_collator.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6835 2023-02-06 14:01:57.000000 scs-analysis-2.7.2/src/scs_analysis/csv_join.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5065 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/csv_reader.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4697 2023-02-06 14:01:57.000000 scs-analysis-2.7.2/src/scs_analysis/csv_segmentor.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3800 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/csv_writer.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6115 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/device_controller.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:35:20.542601 scs-analysis-2.7.2/src/scs_analysis/handler/
+-rw-rw-r--   0 jade      (1002) jade      (1002)        0 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/handler/__init__.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     4051 2023-03-20 10:12:25.000000 scs-analysis-2.7.2/src/scs_analysis/handler/aws_mqtt_publisher.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2329 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/handler/aws_mqtt_subscription_handler.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/handler/batch_download_reporter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1436 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/handler/configuration_csv_generator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5557 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/handler/csv_collator.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5893 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/handler/csv_segmentor.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1184 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/handler/mqtt_reporter.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2007 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/handler/sample_midpoint.py
+-rw-rw-r--   0 jade      (1002) jade      (1002)     2151 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/handler/sample_regression.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4308 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/histo_chart.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2127 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/localised_datetime.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2544 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/monitor_auth.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4367 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/multi_chart.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5982 2023-02-06 14:01:57.000000 scs-analysis-2.7.2/src/scs_analysis/node.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5896 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/organisation_devices.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4713 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/organisation_path_roots.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4925 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/organisation_user_paths.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5783 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/organisation_users.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5300 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/organisations.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7233 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/sample_aggregate.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4821 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/sample_average.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5162 2023-02-06 14:01:57.000000 scs-analysis-2.7.2/src/scs_analysis/sample_collator.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5566 2023-02-06 14:01:57.000000 scs-analysis-2.7.2/src/scs_analysis/sample_concentration.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3970 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/sample_distance.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3765 2023-04-17 09:22:53.000000 scs-analysis-2.7.2/src/scs_analysis/sample_duplicates.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4685 2023-02-06 14:01:57.000000 scs-analysis-2.7.2/src/scs_analysis/sample_error.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3102 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/sample_interval.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     7990 2023-02-06 14:01:57.000000 scs-analysis-2.7.2/src/scs_analysis/sample_iso_8601.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3802 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/sample_low_pass.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3571 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/sample_max.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3776 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/sample_median.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3529 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/sample_midpoint.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3570 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/sample_min.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5072 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/sample_noise.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4017 2023-02-06 14:01:57.000000 scs-analysis-2.7.2/src/scs_analysis/sample_nullify.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1667 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/sample_paths.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     3320 2023-06-26 09:33:48.000000 scs-analysis-2.7.2/src/scs_analysis/sample_regression.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5707 2023-04-17 09:22:53.000000 scs-analysis-2.7.2/src/scs_analysis/sample_slope.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2502 2023-02-06 14:01:57.000000 scs-analysis-2.7.2/src/scs_analysis/sample_sort.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     5928 2022-09-20 10:07:36.000000 scs-analysis-2.7.2/src/scs_analysis/sample_stats.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     6001 2023-02-06 14:01:57.000000 scs-analysis-2.7.2/src/scs_analysis/sample_subset.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2897 2023-02-06 14:01:57.000000 scs-analysis-2.7.2/src/scs_analysis/sample_time_shift.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4732 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/sample_timezone.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     4463 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/single_chart.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     2451 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/socket_receiver.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1891 2023-02-06 14:01:57.000000 scs-analysis-2.7.2/src/scs_analysis/timer.py
+-rwxrwxr-x   0 jade      (1002) jade      (1002)     1849 2022-08-17 09:53:36.000000 scs-analysis-2.7.2/src/scs_analysis/uds_receiver.py
+drwxrwxr-x   0 jade      (1002) jade      (1002)        0 2023-06-26 09:35:20.534601 scs-analysis-2.7.2/src/scs_analysis.egg-info/
+-rw-rw-r--   0 jade      (1002) jade      (1002)     1474 2023-06-26 09:35:20.000000 scs-analysis-2.7.2/src/scs_analysis.egg-info/PKG-INFO
+-rw-rw-r--   0 jade      (1002) jade      (1002)     5870 2023-06-26 09:35:20.000000 scs-analysis-2.7.2/src/scs_analysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)        1 2023-06-26 09:35:20.000000 scs-analysis-2.7.2/src/scs_analysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)      247 2023-06-26 09:35:20.000000 scs-analysis-2.7.2/src/scs_analysis.egg-info/requires.txt
+-rw-rw-r--   0 jade      (1002) jade      (1002)       13 2023-06-26 09:35:20.000000 scs-analysis-2.7.2/src/scs_analysis.egg-info/top_level.txt
```

### Comparing `scs-analysis-2.0.0/LICENSE` & `scs-analysis-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/PKG-INFO` & `scs-analysis-2.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 2.0.0
+Version: 2.7.2
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `scs-analysis-2.0.0/README.md` & `scs-analysis-2.7.2/README.md`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/setup.py` & `scs-analysis-2.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """
 Created on 4 Sep 2020
-Updated 23 Mar 2021
 
 @author: Jade Page (jade.page@southcoastscience.com)
 
 https://packaging.python.org/tutorials/packaging-projects/
 https://packaging.python.org/guides/single-sourcing-package-version/
 """
 
@@ -61,15 +60,14 @@
         'src/scs_analysis/access_key.py',
         'src/scs_analysis/alert.py',
         'src/scs_analysis/alert_status.py',
         'src/scs_analysis/aws_api_auth.py',
         'src/scs_analysis/aws_byline.py',
         'src/scs_analysis/aws_client_auth.py',
         'src/scs_analysis/aws_mqtt_client.py',
-        'src/scs_analysis/aws_mqtt_control.py',
         'src/scs_analysis/aws_topic_history.py',
         'src/scs_analysis/aws_topic_publisher.py',
         'src/scs_analysis/aws_upload_interval.py',
         'src/scs_analysis/baseline.py',
         'src/scs_analysis/baseline_conf.py',
         'src/scs_analysis/cognito_devices.py',
         'src/scs_analysis/cognito_password.py',
@@ -81,31 +79,25 @@
         'src/scs_analysis/configuration_monitor_check.py',
         'src/scs_analysis/csv_collation_summary.py',
         'src/scs_analysis/csv_collator.py',
         'src/scs_analysis/csv_join.py',
         'src/scs_analysis/csv_reader.py',
         'src/scs_analysis/csv_segmentor.py',
         'src/scs_analysis/csv_writer.py',
+        'src/scs_analysis/device_controller.py',
         'src/scs_analysis/histo_chart.py',
         'src/scs_analysis/localised_datetime.py',
         'src/scs_analysis/monitor_auth.py',
-        'src/scs_analysis/mqtt_peers.py',
         'src/scs_analysis/multi_chart.py',
         'src/scs_analysis/node.py',
         'src/scs_analysis/organisation_devices.py',
         'src/scs_analysis/organisation_path_roots.py',
         'src/scs_analysis/organisation_user_paths.py',
         'src/scs_analysis/organisation_users.py',
         'src/scs_analysis/organisations.py',
-        'src/scs_analysis/osio_api_auth.py',
-        'src/scs_analysis/osio_client_auth.py',
-        'src/scs_analysis/osio_mqtt_client.py',
-        'src/scs_analysis/osio_mqtt_control.py',
-        'src/scs_analysis/osio_topic_history.py',
-        'src/scs_analysis/osio_topic_publisher.py',
         'src/scs_analysis/sample_aggregate.py',
         'src/scs_analysis/sample_average.py',
         'src/scs_analysis/sample_collator.py',
         'src/scs_analysis/sample_concentration.py',
         'src/scs_analysis/sample_distance.py',
         'src/scs_analysis/sample_duplicates.py',
         'src/scs_analysis/sample_error.py',
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/access_key.py` & `scs-analysis-2.7.2/src/scs_analysis/access_key.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/alert.py` & `scs-analysis-2.7.2/src/scs_analysis/cognito_users.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,234 +1,215 @@
 #!/usr/bin/env python3
 
 """
-Created on 29 Jun 2021
+Created on 24 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
-DESCRIPTION
-The alert utility is used to create, update, delete and find alert specifications.
+source repo: scs_analysis
 
-Alerts take the form of emails, sent when a parameter falls below or above specified bounds, or when the value is null
-(a null value is being reported, or no reports are available). The alert specification sets these bounds, together with
-the aggregation period (usually in minutes). The minimum period is one minute.
+DESCRIPTION
+The cognito_users utility is used to create, update and retrieve AWS Cognito identities. This utility can only be used
+by organisation administrators and superusers.
 
-In --find mode, results can be filtered by topic, field or creator email address.
+If the --Create function is used, an email is sent to the new user. The verification link in the email must be
+excercised in order for the account to gain a CONFIRMED status.
 
 SYNOPSIS
-alert.py  { -F | -R ID | -C | -U ID | -D ID } [-p TOPIC] [-f FIELD] [-l LOWER] [-u UPPER] [-n { 1 | 0 }]
-[-a INTERVAL UNITS] [-t INTERVAL] [-s { 1 | 0 }] [-c EMAIL_ADDR] [-e EMAIL_ADDR] [-i INDENT] [-v]
+cognito_users.py  [-c CREDENTIALS] { -F [{ -e EMAIL_ADDR | -l ORG_LABEL | -c CONFIRMATION | -s { 1 | 0 } } }] | \
+-C | -U -e EMAIL_ADDR | -D -e EMAIL_ADDR } [-i INDENT] [-v]
 
 EXAMPLES
-alert.py -v -C -p south-coast-science-dev/development/loc/1/gases -f val.NO2.cnc -u 1000.0 -a 1 M \
--e someone@me.com -i4
+cognito_users.py -Fe bruno.beloff@southcoastscience.com
 
 DOCUMENT EXAMPLE
-{"id": 77, "topic": "south-coast-science-dev/development/loc/1/gases", "field": "val.CO.cnc", "lower-threshold": null,
-"upper-threshold": 1000.0, "alert-on-none": true, "aggregation-period": {"interval": 1, "units": "M"},
-"test-interval": null, "creator-email-address": "authorization@southcoastscience.com",
-"to": "someone@me.com", "cc-list": [], "suspended": false}
+{"username": "8", "creation-date": "2021-11-24T12:51:12Z", "confirmation-status": "CONFIRMED", "enabled": true,
+"email": "bruno.beloff@southcoastscience.com", "given-name": "Bruno", "family-name": "Beloff", "is-super": true}
 
 SEE ALSO
-scs_analysis/alert_status
-scs_analysis/monitor_auth
-
-BUGS
-* The --test-interval flag is not currently in use, and is ignored.
-* Email CC addresses cannot be added or removed.
+scs_analysis/cognito_credentials
+scs_analysis/cognito_devices
+scs_analysis/organisation_users
+
+RESOURCES
+https://docs.aws.amazon.com/cognito/latest/developerguide/signing-up-users-in-your-app.html
+https://docs.aws.amazon.com/cognito/latest/developerguide/user-pool-settings-policies.html
 """
 
-import json
-
 import requests
 import sys
 
-from scs_analysis.cmd.cmd_alert import CmdAlert
+from scs_analysis.cmd.cmd_cognito_users import CmdCognitoUsers
 
-from scs_core.aws.client.api_auth import APIAuth
-from scs_core.aws.client.monitor_auth import MonitorAuth
+from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
+from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
+from scs_core.aws.security.cognito_membership import CognitoMembership
+from scs_core.aws.security.cognito_user import CognitoUserIdentity
+from scs_core.aws.security.cognito_user_finder import CognitoUserFinder
+from scs_core.aws.security.cognito_user_manager import CognitoUserCreator, CognitoUserEditor, CognitoUserDeleter
 
-from scs_core.aws.data.alert import AlertSpecification
+from scs_core.aws.security.organisation_manager import OrganisationManager
 
-from scs_core.aws.manager.alert_specification_manager import AlertSpecificationManager
-from scs_core.aws.manager.byline_manager import BylineManager
+from scs_core.client.http_exception import HTTPException, HTTPConflictException
 
-from scs_core.data.datetime import LocalizedDatetime
+from scs_core.data.datum import Datum
 from scs_core.data.json import JSONify
-from scs_core.data.path_dict import PathDict
-from scs_core.data.str import Str
 
-from scs_core.sys.http_exception import HTTPException
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
+    cmd = None
     logger = None
+    gatekeeper = None
+    credentials = None
     auth = None
-    response = None
+    finder = None
+    manager = None
+    org = None
     report = None
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # cmd...
 
-        cmd = CmdAlert()
+        cmd = CmdCognitoUsers()
 
         if not cmd.is_valid():
             cmd.print_help(sys.stderr)
             exit(2)
 
-        Logging.config('alert', verbose=cmd.verbose)
+        Logging.config('cognito_users', verbose=cmd.verbose)
         logger = Logging.getLogger()
 
         logger.info(cmd)
 
 
         # ------------------------------------------------------------------------------------------------------------
+        # authentication...
+
+        if not cmd.create:
+            credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
+
+            if not credentials:
+                exit(1)
+
+            gatekeeper = CognitoLoginManager(requests)
+            auth = gatekeeper.user_login(credentials)
+
+            if not auth.is_ok():
+                logger.error("login: %s" % auth.authentication_status.description)
+                exit(1)
+
+
+        # ------------------------------------------------------------------------------------------------------------
         # resources...
 
-        # MonitorAuth...
-        if not MonitorAuth.exists(Host):
-            logger.error('MonitorAuth not available.')
-            exit(1)
-
-        try:
-            auth = MonitorAuth.load(Host, encryption_key=MonitorAuth.password_from_user())
-        except (KeyError, ValueError):
-            logger.error('incorrect password.')
-            exit(1)
-
-        alert_manager = AlertSpecificationManager(requests, auth)
-        logger.info(alert_manager)
-
-        # APIAuth...
-        api_auth = APIAuth.load(Host)
-
-        if api_auth is None:
-            logger.error("APIAuth not available.")
-            exit(1)
-
-        # byline manager...
-        byline_manager = BylineManager(api_auth)
-        logger.info(byline_manager)
+        if not cmd.create:
+            finder = CognitoUserFinder(requests)
+
+        manager = OrganisationManager(requests)
+
+        if cmd.org_label:
+            org = manager.get_organisation_by_label(auth.id_token, cmd.org_label)
+
+            if org is None:
+                logger.error("no organisation found for label: '%s'." % cmd.org_label)
+                exit(1)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
         if cmd.find:
-            creator_filter = auth.email_address if cmd.creator is None else cmd.creator
-            response = alert_manager.find(cmd.topic, cmd.field, creator_filter)
-            report = sorted(response.alerts)
+            if cmd.email is not None:
+                report = sorted(finder.find_by_email(auth.id_token, cmd.email))
 
-        if cmd.retrieve:
-            report = alert_manager.retrieve(cmd.retrieve_id)
+            elif cmd.org_label is not None:
+                org_users = manager.find_users_by_organisation(auth.id_token, org.org_id)
+                usernames = [org_user.username for org_user in org_users]
 
-        if cmd.create:
-            # validate...
-            if not cmd.is_complete():
-                logger.error("minimum parameters are topic, path, a threshold, and an aggregation period.")
-                exit(2)
-
-            byline = byline_manager.find_latest_byline_for_topic(cmd.topic)
-
-            if byline is None or cmd.topic != byline.topic:
-                logger.error("the topic '%s' is not available." % cmd.topic)
-                exit(2)
-
-            message = PathDict(json.loads(byline.message))
-
-            if not message.has_path(cmd.field):
-                paths = Str.collection(message.paths())
-                logger.error("the field '%s' is not available. Available fields are: %s" % (cmd.field, paths))
-                exit(2)
+                report = sorted(finder.find_by_usernames(auth.id_token, usernames))
 
-            # create...
-            to = auth.email_address if cmd.to is None else cmd.to
+            elif cmd.confirmation_status is not None:
+                report = sorted(finder.find_by_status(auth.id_token,
+                                                      CognitoUserIdentity.status(cmd.confirmation_status)))
 
-            alert = AlertSpecification(None, cmd.topic, cmd.field, cmd.lower_threshold, cmd.upper_threshold,
-                                       cmd.alert_on_none, cmd.aggregation_period, cmd.test_interval, auth.email_address,
-                                       to, [], cmd.suspended)
+            elif cmd.enabled is not None:
+                report = sorted(finder.find_by_enabled(auth.id_token, cmd.enabled))
 
-            if not alert.has_valid_thresholds():
-                logger.error("threshold values are invalid.")
-                exit(2)
+            else:
+                report = sorted(finder.find_all(auth.id_token))
 
-            if not alert.has_valid_aggregation_period():
-                logger.error("the aggregation period is invalid.")
-                exit(2)
+            if cmd.memberships:
+                org_users = manager.find_users(auth.id_token)
+                report = CognitoMembership.merge(report, org_users)
 
-            report = alert_manager.create(alert)
+        if cmd.create:
+            # create...
+            if not Datum.is_email_address(cmd.email):
+                logger.error("The email address '%s' is not valid." % cmd.email)
+                exit(1)
+
+            identity = CognitoUserIdentity(None, None, None, True,
+                                           False, cmd.email, cmd.given_name, cmd.family_name, None,
+                                           False, False, None)
+
+            manager = CognitoUserCreator(requests)
+            report = manager.create(identity)
 
         if cmd.update:
-            # validate...
-            if cmd.topic is not None or cmd.field is not None:
-                logger.error("topic and field may not be changed.")
-                exit(2)
-
-            alert = alert_manager.retrieve(cmd.update_id)
-
-            if alert is None:
-                logger.error("no alert found with ID %s." % cmd.update_id)
-                exit(2)
-
-            if auth.email_address != alert.creator_email_address:
-                logger.error("you do not have permission to update this alert.")
-                exit(2)
+            # find...
+            identity = finder.get_by_email(auth.id_token, cmd.update)
 
-            # update...
-            lower_threshold = alert.lower_threshold if cmd.lower_threshold is None else cmd.lower_threshold
-            upper_threshold = alert.upper_threshold if cmd.upper_threshold is None else cmd.upper_threshold
-            alert_on_none = alert.alert_on_none if cmd.alert_on_none is None else bool(cmd.alert_on_none)
-            aggregation_period = alert.aggregation_period if cmd.aggregation_period is None else cmd.aggregation_period
-            test_interval = alert.test_interval if cmd.test_interval is None else cmd.test_interval
-            suspended = alert.suspended if cmd.suspended is None else bool(cmd.suspended)
-            to = alert.to if cmd.to is None else cmd.to
-
-            updated = AlertSpecification(alert.id, alert.topic, alert.field, lower_threshold, upper_threshold,
-                                         alert_on_none, aggregation_period, test_interval, alert.creator_email_address,
-                                         to, alert.cc_list, suspended)
-
-            if not updated.has_valid_thresholds():
-                logger.error("threshold values are invalid.")
-                exit(2)
-
-            if not updated.has_valid_aggregation_period():
-                logger.error("the aggregation period is invalid.")
-                exit(2)
+            if identity is None:
+                logger.error("no identity found for email: '%s'." % cmd.update)
+                exit(1)
 
-            report = alert_manager.update(updated)
+            # update...
+            enabled = identity.enabled if cmd.enabled is None else cmd.enabled
+            email = identity.email if cmd.email is None else cmd.email
+            given_name = identity.given_name if cmd.given_name is None else cmd.given_name
+            family_name = identity.family_name if cmd.family_name is None else cmd.family_name
+
+            if not Datum.is_email_address(email):
+                logger.error("The email address '%s' is not valid." % email)
+                exit(1)
+
+            new_identity = CognitoUserIdentity(identity.username, None, None, enabled,
+                                               identity.email_verified, email, given_name, family_name, None,
+                                               identity.is_super, identity.is_tester, None)
+
+            auth = gatekeeper.user_login(credentials)                          # renew credentials
+            manager = CognitoUserEditor(requests, auth.id_token)
+            report = manager.update(new_identity)
 
         if cmd.delete:
-            alert = alert_manager.retrieve(cmd.delete_id)
+            # TODO: delete user from organisations?
+            manager = CognitoUserDeleter(requests, auth.id_token)
+            manager.delete(cmd.delete)
 
-            if alert is None:
-                logger.error("no alert found with ID %s." % cmd.delete_id)
-                exit(2)
-
-            alert_manager.delete(cmd.delete_id)
 
         # ------------------------------------------------------------------------------------------------------------
         # end...
 
-        # report...
         if report is not None:
             print(JSONify.dumps(report, indent=cmd.indent))
 
         if cmd.find:
-            logger.info('retrieved: %s' % len(response.alerts))
-
-        # ------------------------------------------------------------------------------------------------------------
-        # end...
+            logger.info("found: %s" % len(report))
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
+    except HTTPConflictException as ex:
+        logger.error("the email address '%s' is already in use." % cmd.email)
+        exit(1)
+
     except HTTPException as ex:
-        now = LocalizedDatetime.now().utc().as_iso8601()
-        logger.error("%s: HTTP response: %s (%s) %s" % (now, ex.status, ex.reason, ex.data))
+        logger.error(ex.error_report)
         exit(1)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/alert_status.py` & `scs-analysis-2.7.2/src/scs_analysis/alert_status.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,112 +2,124 @@
 
 """
 Created on 29 Jun 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 DESCRIPTION
-The alert_status utility is used to report on the alerts generated by a specific alert specification. Alert causes are:
+The alert_status utility is used to report on the history of alerts generated by a specific alert specification.
+Alert causes are:
 
 * L - Below lower threshold
 * U - Above upper threshold
 * N - Null value
+* OK - data has returned within bounds
 
 SYNOPSIS
-alert_status.py { -l | -d [-c CAUSE] } [-i INDENT] [-v] ID
+alert_status.py [-c CREDENTIALS] { -F { -l | -d [-a CAUSE] } | -D } [-i INDENT] [-v] ID
 
 EXAMPLES
-alert_status.py -d -cL 123
+alert_status.py -vi4 -c bruno -Fl 87
 
 DOCUMENT EXAMPLE
 {"id": 77, "rec": "2021-09-07T11:40:00Z", "cause": null, "val": 589.6}
 
 SEE ALSO
 scs_analysis/alert
-scs_analysis/monitor_auth
+scs_analysis/cognito_user_credentials
 """
 
 import requests
 import sys
 
 from scs_analysis.cmd.cmd_alert_status import CmdAlertStatus
 
-from scs_core.aws.client.monitor_auth import MonitorAuth
-from scs_core.aws.manager.alert_status_finder import AlertStatusFinder
+from scs_core.aws.manager.alert_status_manager import AlertStatusManager
+
+from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
+from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
+
+from scs_core.client.http_exception import HTTPException, HTTPNotFoundException
 
 from scs_core.data.json import JSONify
-from scs_core.data.datetime import LocalizedDatetime
 
-from scs_core.sys.http_exception import HTTPException
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
-    logger = None
-    auth = None
     response = None
     report = None
 
-    try:
-        # ------------------------------------------------------------------------------------------------------------
-        # cmd...
+    # ------------------------------------------------------------------------------------------------------------
+    # cmd...
 
-        cmd = CmdAlertStatus()
+    cmd = CmdAlertStatus()
 
-        if not cmd.is_valid():
-            cmd.print_help(sys.stderr)
-            exit(2)
+    if not cmd.is_valid():
+        cmd.print_help(sys.stderr)
+        exit(2)
 
-        Logging.config('alert_status', verbose=cmd.verbose)
-        logger = Logging.getLogger()
+    Logging.config('alert_status', verbose=cmd.verbose)
+    logger = Logging.getLogger()
 
-        logger.info(cmd)
+    logger.info(cmd)
 
+    try:
         # ------------------------------------------------------------------------------------------------------------
-        # validation...
+        # authentication...
 
-        try:
-            int(cmd.id)
-        except (TypeError, ValueError):
-            logger.error('the ID must be an integer.')
+        credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
+
+        if not credentials:
+            exit(1)
+
+        gatekeeper = CognitoLoginManager(requests)
+        auth = gatekeeper.user_login(credentials)
+
+        if not auth.is_ok():
+            logger.error("login: %s" % auth.authentication_status.description)
             exit(1)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # resources...
 
-        if not MonitorAuth.exists(Host):
-            logger.error('MonitorAuth not available.')
-            exit(1)
+        status_manager = AlertStatusManager(requests)
 
-        try:
-            auth = MonitorAuth.load(Host, encryption_key=MonitorAuth.password_from_user())
-        except (KeyError, ValueError):
-            logger.error('incorrect password.')
-            exit(1)
 
-        finder = AlertStatusFinder(requests, auth)
-        logger.info(finder)
+        # ------------------------------------------------------------------------------------------------------------
+        # validation...
+
+        try:
+            int(cmd.id)
+        except (TypeError, ValueError):
+            logger.error('the ID must be an integer.')
+            exit(2)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
-        if cmd.latest:
-            response = finder.find(cmd.id, None, cmd.response_mode())
-            report = response.alert_statuses[0] if response.alert_statuses else None
+        if cmd.find:
+            if cmd.latest:
+                response = status_manager.find(auth.id_token, cmd.id, None, cmd.response_mode())
+                report = response.alert_statuses[0] if response.alert_statuses else None
+
+            if cmd.history:
+                response = status_manager.find(auth.id_token, cmd.id, cmd.cause, cmd.response_mode())
+                report = sorted(response.alert_statuses)
+
+        if cmd.delete:
+            status_manager.delete(auth.id_token, cmd.id)
 
-        if cmd.history:
-            response = finder.find(cmd.id, cmd.cause, cmd.response_mode())
-            report = sorted(response.alert_statuses)
 
         # ------------------------------------------------------------------------------------------------------------
         # end...
 
         # report...
         if report is not None:
             print(JSONify.dumps(report, indent=cmd.indent))
@@ -115,11 +127,14 @@
         if cmd.history:
             logger.info('retrieved: %s' % len(response.alert_statuses))
 
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
+    except HTTPNotFoundException:
+        logger.error("no alert found with ID %s." % cmd.id)
+        exit(2)
+
     except HTTPException as ex:
-        now = LocalizedDatetime.now().utc().as_iso8601()
-        logger.error("%s: HTTP response: %s (%s) %s" % (now, ex.status, ex.reason, ex.data))
+        logger.error(ex.error_report)
         exit(1)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/aws_api_auth.py` & `scs-analysis-2.7.2/src/scs_analysis/aws_api_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/aws_byline.py` & `scs-analysis-2.7.2/src/scs_analysis/aws_byline.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,20 +35,20 @@
 import sys
 
 from scs_analysis.cmd.cmd_aws_byline import CmdAWSByline
 from scs_analysis.handler.batch_download_reporter import BatchDownloadReporter
 
 from scs_core.aws.manager.byline_manager import BylineManager
 
+from scs_core.client.http_exception import HTTPException
 from scs_core.client.network import Network
 from scs_core.client.resource_unavailable_exception import ResourceUnavailableException
 
 from scs_core.data.json import JSONify
 
-from scs_core.sys.http_exception import HTTPException
 from scs_core.sys.logging import Logging
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
@@ -128,15 +128,19 @@
 
     # ----------------------------------------------------------------------------------------------------------------
     # end...
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
-    except (ConnectionError, HTTPException, ResourceUnavailableException) as ex:
+    except HTTPException as ex:
+        logger.error(ex.error_report)
+        exit(1)
+
+    except (ConnectionError, ResourceUnavailableException) as ex:
         logger.error(repr(ex))
         exit(1)
 
     finally:
         if cmd.verbose and group is not None and len(group):
             latest_pub = group.latest_pub()
             latest_iso = None if latest_pub is None else latest_pub.as_iso8601()
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/aws_client_auth.py` & `scs-analysis-2.7.2/src/scs_analysis/aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/aws_mqtt_client.py` & `scs-analysis-2.7.2/src/scs_analysis/aws_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/aws_topic_history.py` & `scs-analysis-2.7.2/src/scs_analysis/aws_topic_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,27 +59,28 @@
 from scs_analysis.cmd.cmd_aws_topic_history import CmdAWSTopicHistory
 from scs_analysis.handler.batch_download_reporter import BatchDownloadReporter
 
 from scs_core.aws.client.api_auth import APIAuth
 from scs_core.aws.manager.byline_manager import BylineManager
 from scs_core.aws.manager.lambda_message_manager import MessageManager
 
+from scs_core.client.http_exception import HTTPException
 from scs_core.client.network import Network
 from scs_core.client.resource_unavailable_exception import ResourceUnavailableException
 
 from scs_core.data.checkpoint_generator import CheckpointGenerator
 from scs_core.data.datetime import LocalizedDatetime
 from scs_core.data.json import JSONify
 
-from scs_core.sys.http_exception import HTTPException
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
+# TODO: remove APIAuth requirement
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     agent = None
     reporter = None
     start_time = None
@@ -195,15 +196,19 @@
 
     # ----------------------------------------------------------------------------------------------------------------
     # end...
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
-    except (HTTPException, ResourceUnavailableException) as ex:
+    except HTTPException as ex:
+        logger.error(ex.error_report)
+        exit(1)
+
+    except ResourceUnavailableException as ex:
         logger.error(repr(ex))
         exit(1)
 
     finally:
         if reporter:
             logger.info("blocks: %s" % reporter.block_count)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/aws_topic_publisher.py` & `scs-analysis-2.7.2/src/scs_analysis/aws_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/aws_upload_interval.py` & `scs-analysis-2.7.2/src/scs_analysis/aws_upload_interval.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/baseline.py` & `scs-analysis-2.7.2/src/scs_analysis/baseline.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,33 +54,30 @@
 import requests
 import sys
 
 from scs_analysis.cmd.cmd_baseline import CmdBaseline
 
 from scs_analysis.handler.batch_download_reporter import BatchDownloadReporter
 
-from scs_core.aws.client.access_key import AccessKey
 from scs_core.aws.client.api_auth import APIAuth
-from scs_core.aws.client.client import Client
-from scs_core.aws.client.client_auth import ClientAuth
-from scs_core.aws.client.mqtt_client import MQTTClient, MQTTSubscriber
-
+from scs_core.aws.client.device_control_client import DeviceControlClient
 from scs_core.aws.manager.byline_manager import BylineManager
 from scs_core.aws.manager.lambda_message_manager import MessageManager
-from scs_core.aws.manager.s3_manager import S3PersistenceManager
 
-from scs_core.control.control_handler import ControlHandler
+from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
+from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
+
+from scs_core.client.http_exception import HTTPGatewayTimeoutException
 
 from scs_core.data.datetime import LocalizedDatetime
 from scs_core.data.json import JSONify
 from scs_core.data.timedelta import Timedelta
 
 from scs_core.estate.baseline_conf import BaselineConf
 from scs_core.estate.configuration import Configuration
-from scs_core.estate.mqtt_peer import MQTTPeerSet
 
 from scs_core.gas.afe_baseline import AFEBaseline
 from scs_core.gas.afe_calib import AFECalib
 from scs_core.gas.minimum import Minimum
 
 from scs_core.sample.gases_sample import GasesSample
 
@@ -114,71 +111,64 @@
     Logging.config('baseline', verbose=cmd.verbose)
     logger = Logging.getLogger()
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # authentication...
 
-        # AccessKey (for S3PersistenceManager)...
-        if not AccessKey.exists(Host):
-            logger.error("AccessKey not available.")
+        credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
+
+        if not credentials:
             exit(1)
 
-        try:
-            key = AccessKey.load(Host, encryption_key=AccessKey.password_from_user())
-        except (KeyError, ValueError):
-            logger.error("incorrect password.")
+        gatekeeper = CognitoLoginManager(requests)
+        auth = gatekeeper.user_login(credentials)
+
+        if not auth.is_ok():
+            logger.error("login: %s" % auth.authentication_status.description)
             exit(1)
 
         # APIAuth (for MessageManager)...
         api_auth = APIAuth.load(Host)
 
         if api_auth is None:
             logger.error("APIAuth is not available")
             exit(1)
 
-        # ClientAuth (for MQTTClient)...
-        client_auth = ClientAuth.load(Host)
-
-        if client_auth is None:
-            logger.error("ClientAuth not available.")
-            exit(1)
-
 
         # ------------------------------------------------------------------------------------------------------------
         # resources...
 
-        # S3PersistenceManager...
-        s3_client = Client.construct('s3', key)
-        s3_resource_client = Client.resource('s3', key)
-
-        s3_manager = S3PersistenceManager(s3_client, s3_resource_client)
-
         # reporter...
         reporter = BatchDownloadReporter()
 
         # BylineManager...
         byline_manager = BylineManager(requests, reporter=reporter)
 
         # MessageManager...
         message_manager = MessageManager(api_auth, reporter=reporter)
 
-        # PersistenceManager...
-        persistence_manager = s3_manager if cmd.aws else Host
+        # DeviceControlClient...
+        client = DeviceControlClient(requests)
+
 
+        # ------------------------------------------------------------------------------------------------------------
+        # run...
 
         for device_tag in cmd.device_tags:
             try:
+                device_updates = 0
+
                 # ----------------------------------------------------------------------------------------------------
                 # configuration...
 
                 logger.error("configuration...")
 
                 # BaselineConf...
-                baseline_conf = BaselineConf.load(persistence_manager, name=cmd.conf_name)
+                baseline_conf = BaselineConf.load(Host, name=cmd.conf_name)
 
                 if baseline_conf is None:
                     logger.error("the BaselineConf '%s' is not available." % cmd.conf_name)
                     continue
 
                 try:
                     baseline_conf = cmd.override(baseline_conf)
@@ -192,71 +182,55 @@
                 # topics...
                 group = byline_manager.find_bylines_for_device(device_tag)
 
                 if group is None:
                     logger.error("no bylines found for %s." % device_tag)
                     continue
 
-                gases_topic = group.latest_topic('/gases')
-                control_topic = group.latest_topic('/control')
+                gases_topic = group.latest_topic(suffix='/gases')
+                control_topic = group.latest_topic(suffix='/control')
 
                 if gases_topic is None:
                     logger.error("no gases topic found for %s." % device_tag)
                     continue
 
                 if control_topic is None:
                     logger.error("no control topic found for %s." % device_tag)
                     continue
 
                 logger.error("gases_topic: %s" % gases_topic)
                 logger.error("control_topic: %s" % control_topic)
 
-                # MQTT peer...
-                peer_group = MQTTPeerSet.load(s3_manager)
-                peer = peer_group.peer_by_tag(device_tag)
-
-                if peer is None:
-                    logger.error("no MQTT peer found for tag '%s'." % device_tag)
-                    continue
-
-                logger.error("hostname: %s" % peer.hostname)
-
-                # MQTTClient...
-                handler = ControlHandler(host_tag, device_tag)
-                subscriber = MQTTSubscriber(control_topic, handler.handle)
-
-                mqtt_client = MQTTClient(subscriber)
-                mqtt_client.connect(client_auth)
-
-                # Configuration...
-                stdout, stderr, return_code = handler.publish(mqtt_client, control_topic, ['configuration'],
-                                                              MQTT_TIMEOUT, peer.shared_secret)
+                # configuration...
+                response = client.interact(auth.id_token, device_tag, ['configuration'])
+                command = response.command
 
-                if return_code != 0:
-                    logger.error("Configuration cannot be retrieved: %s" % stderr[0])
+                if command.return_code != 0:
+                    logger.error("configuration cannot be retrieved: %s" % command.stderr[0])
                     continue
 
-                jdict = json.loads(stdout[0])
+                jdict = json.loads(command.stdout[0])
                 device_conf = Configuration.construct_from_jdict(jdict.get('val'))
 
                 # noinspection PyUnresolvedReferences
                 ox_index = None if device_conf.afe_id is None else device_conf.afe_id.sensor_index('Ox')
 
                 # AFECalib...
                 if ox_index is None:
                     ox_sensor = None
 
                 else:
-                    stdout, stderr, return_code = handler.publish(mqtt_client, control_topic, ['afe_calib'],
-                                                                  MQTT_TIMEOUT, peer.shared_secret)
-                    if return_code != 0:
-                        logger.error("AFECAlib cannot be retrieved: %s" % stderr[0])
+                    response = client.interact(auth.id_token, device_tag, ['afe_calib'])
+                    command = response.command
+
+                    if command.return_code != 0:
+                        logger.error("AFECAlib cannot be retrieved: %s" % command.stderr[0])
                         continue
 
-                    jdict = json.loads(stdout[0])
+                    jdict = json.loads(command.stdout[0])
                     afe_calib = AFECalib.construct_from_jdict(jdict)
 
                     afe_baseline = AFEBaseline.null_datum() if device_conf.afe_baseline is None else \
                         device_conf.afe_baseline
 
                     ox_baseline = afe_baseline.sensor_baseline(ox_index)
                     ox_calib = afe_calib.sensor_calib(ox_index)
@@ -264,15 +238,15 @@
                     ox_sensor = ox_calib.sensor(ox_baseline)
                     # logger.error(ox_sensor)
 
                 logger.error("-")
 
 
                 # ----------------------------------------------------------------------------------------------------
-                # run...
+                # analysis...
 
                 # data...
                 logger.error("data...")
 
                 now = LocalizedDatetime.now()
 
                 start = baseline_conf.start_datetime(now)
@@ -363,49 +337,56 @@
 
                     if minimum.index == 0:
                         logger.error("WARNING: the first datum for %s is the minimum value" % minimum.path)
 
                     elif minimum.index == len(data) - 1:
                         logger.error("WARNING: the last datum for %s is the minimum value" % minimum.path)
 
-                    # command...
+
+                    # ------------------------------------------------------------------------------------------------
+                    # update...
+
                     cmd_tokens = minimum.cmd_tokens(conf_minimums)
                     logger.error(' '.join([str(token) for token in cmd_tokens]))
 
                     if cmd.rehearse:
                         continue
 
-                    stdout, stderr, return_code = handler.publish(mqtt_client, control_topic, cmd_tokens, MQTT_TIMEOUT,
-                                                                  peer.shared_secret)
-                    if stderr:
-                        print(*stderr, sep='\n', file=sys.stderr)
-                    if stdout:
-                        print(*stdout, sep='\n', file=sys.stdout)
+                    response = client.interact(auth.id_token, device_tag, cmd_tokens)
+                    command = response.command
 
-                if return_code != 0:
+                    if command.stderr:
+                        print(*command.stderr, sep='\n', file=sys.stderr)
+                    if command.stdout:
+                        print(*command.stdout, sep='\n', file=sys.stdout)
+
+                    if command.return_code != 0:
+                        logger.error("update could not be performed: %s" % command.stderr[0])
+                        continue
+
+                    device_updates += 1
+
+                if not device_updates:
                     continue
 
+                # reboot...
                 logger.error("-")
 
-                # reboot...
                 logger.error(cmd.uptake)
 
-                handler.publish(mqtt_client, control_topic, [cmd.uptake], MQTT_TIMEOUT, peer.shared_secret)
+                client.interact(auth.id_token, device_tag, [cmd.uptake])
 
-            except TimeoutError:
-                logger.error("device is not available.")
+            except HTTPGatewayTimeoutException:
+                logger.error("device '%s' is not available." % device_tag)
                 continue
 
             processed_count += 1
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # end...
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
     finally:
-        if mqtt_client:
-            mqtt_client.disconnect()
-
         logger.info("devices: %d processed: %d" % (len(cmd.device_tags), processed_count))
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/baseline_conf.py` & `scs-analysis-2.7.2/src/scs_analysis/baseline_conf.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/chart/chart.py` & `scs-analysis-2.7.2/src/scs_analysis/chart/chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/chart/histo_chart.py` & `scs-analysis-2.7.2/src/scs_analysis/chart/histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/chart/multi_chart.py` & `scs-analysis-2.7.2/src/scs_analysis/chart/multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/chart/single_chart.py` & `scs-analysis-2.7.2/src/scs_analysis/chart/single_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_access_key.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_access_key.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_alert.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_aws_topic_history.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,251 +1,256 @@
 """
-Created on 29 Jun 2021
+Created on 20 Feb 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
+
+source repo: scs_analysis
 """
 
+import logging
 import optparse
 
-from scs_core.data.recurring_period import RecurringPeriod
+from scs_core.data.datetime import LocalizedDatetime
+from scs_core.data.timedelta import Timedelta
 
 
+# TODO: add backoff limit flag
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdAlert(object):
+class CmdAWSTopicHistory(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog  { -F | -R ID | -C | -U ID | -D ID } "
-                                                    "[-p TOPIC] [-f FIELD] [-l LOWER] [-u UPPER] "
-                                                    "[-n { 1 | 0 }] [-a INTERVAL UNITS] [-t INTERVAL] [-s { 1 | 0 }] "
-                                                    "[-c EMAIL_ADDR] [-e EMAIL_ADDR] [-i INDENT] [-v]",
+        self.__parser = optparse.OptionParser(usage="%prog { -l | -a LATEST_AT [-b BACK-OFF] | "
+                                                    "-t { [[DD-]HH:]MM[:SS] | :SS } | -s START [-e END] } "
+                                                    "{ -c HH:MM:SS [-m] [-x] | [-w] [-f] } [-r] [{ -v | -d }] TOPIC",
                                               version="%prog 1.0")
 
-        # operations...
-        self.__parser.add_option("--find", "-F", action="store_true", dest="find", default=False,
-                                 help="find alerts for given TOPIC (and FIELD) or creator email")
-
-        self.__parser.add_option("--retrieve", "-R", type="int", action="store", dest="retrieve_id",
-                                 help="retrieve alert with given ID")
-
-        self.__parser.add_option("--create", "-C", action="store_true", dest="create", default=False,
-                                 help="create alert")
+        # functions...
+        self.__parser.add_option("--latest", "-l", action="store_true", dest="latest", default=False,
+                                 help="the most recent document")
 
-        self.__parser.add_option("--update", "-U", type="int", action="store", dest="update_id",
-                                 help="update alert with given ID")
+        self.__parser.add_option("--latest-at", "-a", type="string", nargs=1, action="store", dest="latest_at",
+                                 help="the most recent document before ISO 8601 datetime")
 
-        self.__parser.add_option("--delete", "-D", type="int", action="store", dest="delete_id",
-                                 help="delete alert with given ID")
+        self.__parser.add_option("--back-off", "-b", type="int", nargs=1, action="store", dest="back_off",
+                                 help="maximum look-back period (seconds)")
 
-        # fields...
-        self.__parser.add_option("--topic-path", "-p", type="string", action="store", dest="topic",
-                                 help="topic path")
+        self.__parser.add_option("--timedelta", "-t", type="string", nargs=1, action="store", dest="timedelta",
+                                 help="starting days / hours / minutes / seconds ago, and ending now")
 
-        self.__parser.add_option("--field", "-f", type="string", action="store", dest="field",
-                                 help="field")
+        self.__parser.add_option("--start", "-s", type="string", nargs=1, action="store", dest="start",
+                                 help="ISO 8601 datetime START")
 
-        self.__parser.add_option("--lower-threshold", "-l", type="float", action="store", dest="lower_threshold",
-                                 help="lower threshold")
+        self.__parser.add_option("--end", "-e", type="string", nargs=1, action="store", dest="end",
+                                 help="ISO 8601 datetime END")
 
-        self.__parser.add_option("--upper-threshold", "-u", type="float", action="store", dest="upper_threshold",
-                                 help="upper threshold")
+        # aggregation...
+        self.__parser.add_option("--checkpoint", "-c", type="string", nargs=1, action="store", dest="checkpoint",
+                                 help="a time specification as **:/05:00")
 
-        self.__parser.add_option("--alert-on-none", "-n", type="int", action="store", dest="alert_on_none",
-                                 default=False, help="alert on none (default false)")
+        self.__parser.add_option("--min-max", "-m", action="store_true", dest="min_max", default=False,
+                                 help="include min and max in addition to midpoint")
 
-        self.__parser.add_option("--aggregation-period", "-a", type="string", nargs=2, action="store",
-                                 dest="aggregation_period", help="aggregation interval and units { D | H | M }")
+        self.__parser.add_option("--exclude-remainder", "-x", action="store_true", dest="exclude_remainder",
+                                 help="ignore documents after the last complete period")
 
-        self.__parser.add_option("--test-interval", "-t", type="string", action="store", dest="test_interval",
-                                 help="test interval")
-
-        self.__parser.add_option("--suspended", "-s", type="int", action="store", dest="suspended",
-                                 default=False, help="suspended (default false)")
+        # output...
+        self.__parser.add_option("--wrapper", "-w", action="store_true", dest="include_wrapper", default=False,
+                                 help="include storage wrapper")
 
-        # email...
-        self.__parser.add_option("--creator", "-c", type="string", action="store", dest="creator",
-                                 help="email address of alert creator (admin use only)")
+        self.__parser.add_option("--fetch-last", "-f", action="store_true", dest="fetch_last", default=False,
+                                 help="fetch the last available hour of data if the requested data is unavailable")
 
-        self.__parser.add_option("--email-to", "-e", type="string", action="store", dest="to",
-                                 help="email To address")
-
-        # output...
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
-                                 help="pretty-print the output with INDENT")
+        self.__parser.add_option("--rec-only", "-r", action="store_true", dest="rec_only", default=False,
+                                 help="retrieve only the rec field")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
+        self.__parser.add_option("--debug", "-d", action="store_true", dest="debug", default=False,
+                                 help="report narrative and request / response to stderr")
+
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        count = 0
+        if self.topic is None:
+            return False
 
-        if self.find:
-            count += 1
+        if self.__opts.start is None and self.__opts.end is not None:
+            return False
+
+        count = 0
 
-        if self.retrieve:
+        if self.latest:
             count += 1
 
-        if self.create:
+        if self.__opts.latest_at is not None:
             count += 1
 
-        if self.update:
+        if self.__opts.timedelta is not None:
             count += 1
 
-        if self.delete:
+        if self.__opts.start is not None:
             count += 1
 
         if count != 1:
             return False
 
-        if self.__opts.aggregation_period is not None:
-            try:
-                int(self.__opts.aggregation_period[0])
-            except ValueError:
-                return False
-
-        if self.alert_on_none is not None and self.alert_on_none != 0 and self.alert_on_none != 1:
+        if self.back_off is not None and not self.latest_at:
             return False
 
-        if self.suspended is not None and self.suspended != 0 and self.suspended != 1:
+        if self.include_wrapper and self.checkpoint:
             return False
 
-        return True
+        if self.rec_only and self.fetch_last:
+            return False
 
+        if self.rec_only and self.min_max:
+            return False
 
-    def is_complete(self):
-        if not self.create:
-            return True
+        if self.min_max and not self.checkpoint:
+            return False
 
-        if self.topic is None or self.field is None or self.aggregation_period is None:
+        if self.exclude_remainder and not self.checkpoint:
             return False
 
-        if self.lower_threshold is None and self.upper_threshold is None and not self.alert_on_none:
+        if self.verbose and self.debug:
             return False
 
         return True
 
 
-    # ----------------------------------------------------------------------------------------------------------------
+    def is_valid_latest_at(self):
+        if self.__opts.latest_at is None:
+            return True
 
-    @property
-    def find(self):
-        return self.__opts.find
+        return self.latest_at is not None
 
 
-    @property
-    def retrieve_id(self):
-        return self.__opts.retrieve_id
+    def is_valid_timedelta(self):
+        if self.__opts.timedelta is None:
+            return True
 
+        return self.timedelta is not None
 
-    @property
-    def retrieve(self):
-        return self.__opts.retrieve_id is not None
 
+    def is_valid_start(self):
+        if self.__opts.start is None:
+            return True
 
-    @property
-    def create(self):
-        return self.__opts.create
+        return self.start is not None
 
 
-    @property
-    def update_id(self):
-        return self.__opts.update_id
+    def is_valid_end(self):
+        if self.__opts.end is None:
+            return True
 
+        return self.end is not None
 
-    @property
-    def update(self):
-        return self.__opts.update_id is not None
 
+    def log_level(self):
+        if self.debug:
+            return logging.DEBUG
 
-    @property
-    def delete_id(self):
-        return self.__opts.delete_id
+        if self.verbose:
+            return logging.INFO
+
+        return logging.ERROR
 
 
+    # ----------------------------------------------------------------------------------------------------------------
+
     @property
-    def delete(self):
-        return self.__opts.delete_id is not None
+    def latest(self):
+        return self.__opts.latest
 
 
     @property
-    def topic(self):
-        return self.__opts.topic
+    def latest_at(self):
+        return LocalizedDatetime.construct_from_iso8601(self.__opts.latest_at)
 
 
     @property
-    def field(self):
-        return self.__opts.field
+    def back_off(self):
+        return self.__opts.back_off
 
 
     @property
-    def lower_threshold(self):
-        return self.__opts.lower_threshold
+    def timedelta(self):
+        return Timedelta.construct_from_flag(self.__opts.timedelta)
 
 
     @property
-    def upper_threshold(self):
-        return self.__opts.upper_threshold
+    def start(self):
+        return LocalizedDatetime.construct_from_iso8601(self.__opts.start)
 
 
     @property
-    def alert_on_none(self):
-        return self.__opts.alert_on_none
+    def end(self):
+        return LocalizedDatetime.construct_from_iso8601(self.__opts.end)
 
 
     @property
-    def aggregation_period(self):
-        period = self.__opts.aggregation_period
-        return None if period is None else RecurringPeriod.construct(period[0], period[1])
+    def fetch_last(self):
+        return self.__opts.fetch_last
 
 
     @property
-    def test_interval(self):
-        return self.__opts.test_interval
+    def checkpoint(self):
+        return self.__opts.checkpoint
 
 
     @property
-    def suspended(self):
-        return self.__opts.suspended
+    def include_wrapper(self):
+        return self.__opts.include_wrapper
 
 
     @property
-    def creator(self):
-        return self.__opts.creator
+    def rec_only(self):
+        return self.__opts.rec_only
 
 
     @property
-    def to(self):
-        return self.__opts.to
+    def min_max(self):
+        return self.__opts.min_max
 
 
     @property
-    def indent(self):
-        return self.__opts.indent
+    def exclude_remainder(self):
+        return self.__opts.exclude_remainder
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
+    @property
+    def debug(self):
+        return self.__opts.debug
+
+
+    @property
+    def topic(self):
+        return self.__args[0] if len(self.__args) > 0 else None
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdAlert:{find:%s, retrieve:%s, create:%s, update:%s, delete:%s, topic:%s, field:%s, " \
-               "lower_threshold:%s, upper_threshold:%s, alert_on_none:%s, aggregation_period:%s, " \
-               "test_interval:%s, suspended:%s, creator:%s, to:%s, indent:%s, verbose:%s}" % \
-               (self.find, self.retrieve_id, self.create, self.update_id, self.delete_id, self.topic, self.field,
-                self.lower_threshold, self.upper_threshold, self.alert_on_none, self.aggregation_period,
-                self.test_interval, self.suspended, self.creator, self.to, self.indent, self.verbose)
+        return "CmdAWSTopicHistory:{latest:%s, latest_at:%s, latest_at:%s, timedelta:%s, start:%s, end:%s, " \
+               "fetch_last:%s, checkpoint:%s, include_wrapper:%s, rec_only:%s, min_max:%s, " \
+               "exclude_remainder:%s, verbose:%s, debug:%s, topic:%s}" % \
+                    (self.latest, self.__opts.latest_at, self.back_off, self.__opts.timedelta, self.start, self.end,
+                     self.fetch_last, self.checkpoint, self.include_wrapper, self.rec_only, self.min_max,
+                     self.exclude_remainder, self.verbose, self.debug, self.topic)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_alert_status.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_csv_segmentor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,111 +1,89 @@
 """
-Created on 29 Jun 2021
+Created on 10 Mar 2020
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
+
+source repo: scs_analysis
 """
 
 import optparse
 
-from scs_core.aws.manager.alert_status_finder import AlertStatusFinderRequest
+from scs_core.data.timedelta import Timedelta
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdAlertStatus(object):
+class CmdCSVSegmentor(object):
     """unix command line handler"""
 
-    __CAUSES = {'L': '<L', 'U': '>U', 'N': 'NV'}
-
-    # --------------------------------------------------------------------------------------------------------------------
-
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog { -l | -d [-c CAUSE] } [-i INDENT] [-v] ID",
-                                              version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog -m { [DD-]HH:MM[:SS] | :SS } [-i ISO] [-f FILE_PREFIX] "
+                                                    "[-v]", version="%prog 1.0")
 
-        # operations...
-        self.__parser.add_option("--latest", "-l", action="store_true", dest="latest", default=False,
-                                 help="return latest status report only")
-
-        self.__parser.add_option("--history", "-d", action="store_true", dest="history", default=False,
-                                 help="return history of status reports")
-
-        # filters...
-        self.__parser.add_option("--cause", "-c", type="string", action="store", dest="cause",
-                                 help="filter by cause { L | U | N }")
-
-        # output...
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
-                                 help="pretty-print the output with INDENT")
+        # compulsory...
+        self.__parser.add_option("--max-interval", "-m", type="string", nargs=1, action="store", dest="max_interval",
+                                 help="maximum permitted interval")
+
+        # optional...
+        self.__parser.add_option("--iso-path", "-i", type="string", nargs=1, action="store", default="rec", dest="iso",
+                                 help="path for ISO 8601 datetime field (default 'rec')")
+
+        self.__parser.add_option("--file-prefix", "-f", type="string", nargs=1, action="store", dest="file_prefix",
+                                 help="file prefix for contiguous CSVs")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.id is None:
-            return False
-
-        if self.latest == self.history:
-            return False
-
-        if self.latest and self.__opts.cause is not None:
-            return False
-
-        if self.__opts.cause is not None and self.__opts.cause not in self.__CAUSES:
+        if self.__opts.max_interval is None:
             return False
 
         return True
 
 
-    def response_mode(self):
-        return AlertStatusFinderRequest.Mode.LATEST if self.latest else AlertStatusFinderRequest.Mode.HISTORY
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    @property
-    def id(self):
-        return self.__args[0] if self.__args else None
+    def is_valid_interval(self):
+        if self.__opts.max_interval is None:
+            return True
 
+        return self.max_interval is not None
 
-    @property
-    def latest(self):
-        return self.__opts.latest
 
+    # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def history(self):
-        return self.__opts.history
+    def max_interval(self):
+        return Timedelta.construct_from_flag(self.__opts.max_interval)
 
 
     @property
-    def cause(self):
-        return None if self.__opts.cause is None else self.__CAUSES[self.__opts.cause]
+    def iso(self):
+        return self.__opts.iso
 
 
     @property
-    def indent(self):
-        return self.__opts.indent
+    def file_prefix(self):
+        return self.__opts.file_prefix
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdAlertStatus:{id:%s, latest:%s, history:%s, cause:%s, indent:%s, verbose:%s}" % \
-               (self.id, self.latest, self.history, self.__opts.cause, self.indent, self.verbose)
+        return "CmdCSVSegmentor:{max_interval:%s, iso:%s, file_prefix:%s, verbose:%s}" % \
+               (self.__opts.max_interval, self.iso, self.file_prefix, self.verbose)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_api_auth.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_aws_api_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_byline.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_aws_byline.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_client_auth.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_aws_client_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_topic_history.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_baseline_conf.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,256 +1,203 @@
 """
-Created on 20 Feb 2017
+Created on 31 Jul 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
-
-source repo: scs_analysis
 """
 
-import logging
 import optparse
 
-from scs_core.data.datetime import LocalizedDatetime
-from scs_core.data.timedelta import Timedelta
-
 
-# TODO: add backoff limit flag
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdAWSTopicHistory(object):
-    """unix command line handler"""
+class CmdBaselineConf(object):
+    """
+    unix command line handler
+    """
+
+    # ----------------------------------------------------------------------------------------------------------------
 
     def __init__(self):
-        """
-        Constructor
-        """
-        self.__parser = optparse.OptionParser(usage="%prog { -l | -a LATEST_AT [-b BACK-OFF] | "
-                                                    "-t { [[DD-]HH:]MM[:SS] | :SS } | -s START [-e END] } "
-                                                    "{ -c HH:MM:SS [-m] [-x] | [-w] [-f] } [-r] [{ -v | -d }] TOPIC",
-                                              version="%prog 1.0")
-
-        # functions...
-        self.__parser.add_option("--latest", "-l", action="store_true", dest="latest", default=False,
-                                 help="the most recent document")
-
-        self.__parser.add_option("--latest-at", "-a", type="string", nargs=1, action="store", dest="latest_at",
-                                 help="the most recent document before ISO 8601 datetime")
-
-        self.__parser.add_option("--back-off", "-b", type="int", nargs=1, action="store", dest="back_off",
-                                 help="maximum look-back period (seconds)")
-
-        self.__parser.add_option("--timedelta", "-t", type="string", nargs=1, action="store", dest="timedelta",
-                                 help="starting days / hours / minutes / seconds ago, and ending now")
-
-        self.__parser.add_option("--start", "-s", type="string", nargs=1, action="store", dest="start",
-                                 help="ISO 8601 datetime START")
-
-        self.__parser.add_option("--end", "-e", type="string", nargs=1, action="store", dest="end",
-                                 help="ISO 8601 datetime END")
-
-        # aggregation...
-        self.__parser.add_option("--checkpoint", "-c", type="string", nargs=1, action="store", dest="checkpoint",
-                                 help="a time specification as **:/05:00")
+        self.__parser = optparse.OptionParser(usage="%prog [-a] { -z | -l | -n FROM TO | -c NAME [-t TIMEZONE_NAME] "
+                                                    "[-s START] [-e END] [-p AGGREGATION] [-g GAS MINIMUM] [-r GAS] } "
+                                                    "[-i INDENT] [-v]", version="%prog 1.0")
 
-        self.__parser.add_option("--min-max", "-m", action="store_true", dest="min_max", default=False,
-                                 help="include min and max in addition to midpoint")
+        # source...
+        self.__parser.add_option("--aws", "-a", action="store_true", dest="aws", default=False,
+                                 help="Use AWS S3 instead of local storage for configuration")
 
-        self.__parser.add_option("--exclude-remainder", "-x", action="store_true", dest="exclude_remainder",
-                                 help="ignore documents after the last complete period")
+        # helpers...
+        self.__parser.add_option("--zones", "-z", action="store_true", dest="zones", default=False,
+                                 help="list the available timezone names to stderr")
 
-        # output...
-        self.__parser.add_option("--wrapper", "-w", action="store_true", dest="include_wrapper", default=False,
-                                 help="include storage wrapper")
+        self.__parser.add_option("--list", "-l", action="store_true", dest="list", default=False,
+                                 help="list the available baseline configurations")
+
+        # identity...
+        self.__parser.add_option("--duplicate", "-n", type="string", nargs=2, action="store", dest="duplicate",
+                                 help="create a new configuration based on FROM")
+
+        self.__parser.add_option("--conf-name", "-c", type="string", nargs=1, action="store", dest="conf_name",
+                                 help="the name of the baseline configuration")
+
+        # fields...
+        self.__parser.add_option("--timezone", "-t", type="string", nargs=1, action="store", dest="timezone",
+                                 help="set the timezone for the tests")
+
+        self.__parser.add_option("--start-hour", "-s", type="int", nargs=1, action="store", dest="start_hour",
+                                 help="test starts at the beginning of start hour")
+
+        self.__parser.add_option("--end-hour", "-e", type="int", nargs=1, action="store", dest="end_hour",
+                                 help="test ends at the beginning of end hour")
+
+        self.__parser.add_option("--aggregation-period", "-p", type="int", nargs=1, action="store",
+                                 dest="aggregation_period", help="aggregation in minutes")
 
-        self.__parser.add_option("--fetch-last", "-f", action="store_true", dest="fetch_last", default=False,
-                                 help="fetch the last available hour of data if the requested data is unavailable")
+        self.__parser.add_option("--set-gas", "-g", type="string", nargs=2, action="store", dest="set_gas",
+                                 help="set minimum for GAS")
 
-        self.__parser.add_option("--rec-only", "-r", action="store_true", dest="rec_only", default=False,
-                                 help="retrieve only the rec field")
+        self.__parser.add_option("--remove-gas", "-r", type="string", nargs=1, action="store", dest="remove_gas",
+                                 help="remove GAS from minimums")
+
+        # output...
+        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+                                 help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
-        self.__parser.add_option("--debug", "-d", action="store_true", dest="debug", default=False,
-                                 help="report narrative and request / response to stderr")
-
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.topic is None:
-            return False
-
-        if self.__opts.start is None and self.__opts.end is not None:
-            return False
-
         count = 0
 
-        if self.latest:
+        if self.zones:
             count += 1
 
-        if self.__opts.latest_at is not None:
+        if self.list:
             count += 1
 
-        if self.__opts.timedelta is not None:
+        if self.duplicate_from is not None:
             count += 1
 
-        if self.__opts.start is not None:
+        if self.conf_name is not None:
             count += 1
 
         if count != 1:
             return False
 
-        if self.back_off is not None and not self.latest_at:
-            return False
-
-        if self.include_wrapper and self.checkpoint:
-            return False
-
-        if self.rec_only and self.fetch_last:
+        try:
+            _ = self.set_gas_minimum
+        except ValueError:
             return False
 
-        if self.rec_only and self.min_max:
-            return False
-
-        if self.min_max and not self.checkpoint:
-            return False
+        return True
 
-        if self.exclude_remainder and not self.checkpoint:
-            return False
 
-        if self.verbose and self.debug:
+    def is_complete(self):
+        if self.timezone is None or self.start_hour is None or self.end_hour is None or \
+                self.aggregation_period is None:
             return False
 
         return True
 
 
-    def is_valid_latest_at(self):
-        if self.__opts.latest_at is None:
-            return True
-
-        return self.latest_at is not None
-
-
-    def is_valid_timedelta(self):
-        if self.__opts.timedelta is None:
-            return True
-
-        return self.timedelta is not None
-
-
-    def is_valid_start(self):
-        if self.__opts.start is None:
-            return True
+    def duplicate(self):
+        return self.__opts.duplicate is not None
 
-        return self.start is not None
 
-
-    def is_valid_end(self):
-        if self.__opts.end is None:
-            return True
-
-        return self.end is not None
-
-
-    def log_level(self):
-        if self.debug:
-            return logging.DEBUG
-
-        if self.verbose:
-            return logging.INFO
-
-        return logging.ERROR
+    def set(self):
+        return self.timezone is not None or self.start_hour is not None or self.end_hour is not None or \
+               self.aggregation_period is not None or self.__opts.set_gas is not None or self.remove_gas is not None
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def latest(self):
-        return self.__opts.latest
+    def aws(self):
+        return self.__opts.aws
 
 
     @property
-    def latest_at(self):
-        return LocalizedDatetime.construct_from_iso8601(self.__opts.latest_at)
+    def zones(self):
+        return self.__opts.zones
 
 
     @property
-    def back_off(self):
-        return self.__opts.back_off
+    def list(self):
+        return self.__opts.list
 
 
     @property
-    def timedelta(self):
-        return Timedelta.construct_from_flag(self.__opts.timedelta)
+    def duplicate_from(self):
+        return self.__opts.duplicate[0] if self.__opts.duplicate else None
 
 
     @property
-    def start(self):
-        return LocalizedDatetime.construct_from_iso8601(self.__opts.start)
+    def duplicate_to(self):
+        return self.__opts.duplicate[1] if self.__opts.duplicate else None
 
 
     @property
-    def end(self):
-        return LocalizedDatetime.construct_from_iso8601(self.__opts.end)
+    def conf_name(self):
+        return self.__opts.conf_name
 
 
     @property
-    def fetch_last(self):
-        return self.__opts.fetch_last
+    def timezone(self):
+        return self.__opts.timezone
 
 
     @property
-    def checkpoint(self):
-        return self.__opts.checkpoint
+    def start_hour(self):
+        return self.__opts.start_hour
 
 
     @property
-    def include_wrapper(self):
-        return self.__opts.include_wrapper
+    def end_hour(self):
+        return self.__opts.end_hour
 
 
     @property
-    def rec_only(self):
-        return self.__opts.rec_only
+    def aggregation_period(self):
+        return self.__opts.aggregation_period
 
 
     @property
-    def min_max(self):
-        return self.__opts.min_max
+    def set_gas_name(self):
+        return None if self.__opts.set_gas is None else self.__opts.set_gas[0]
 
 
     @property
-    def exclude_remainder(self):
-        return self.__opts.exclude_remainder
+    def set_gas_minimum(self):
+        return None if self.__opts.set_gas is None else int(self.__opts.set_gas[1])
 
 
     @property
-    def verbose(self):
-        return self.__opts.verbose
+    def remove_gas(self):
+        return self.__opts.remove_gas
 
 
     @property
-    def debug(self):
-        return self.__opts.debug
+    def indent(self):
+        return self.__opts.indent
 
 
     @property
-    def topic(self):
-        return self.__args[0] if len(self.__args) > 0 else None
+    def verbose(self):
+        return self.__opts.verbose
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdAWSTopicHistory:{latest:%s, latest_at:%s, latest_at:%s, timedelta:%s, start:%s, end:%s, " \
-               "fetch_last:%s, checkpoint:%s, include_wrapper:%s, rec_only:%s, min_max:%s, " \
-               "exclude_remainder:%s, verbose:%s, debug:%s, topic:%s}" % \
-                    (self.latest, self.__opts.latest_at, self.back_off, self.__opts.timedelta, self.start, self.end,
-                     self.fetch_last, self.checkpoint, self.include_wrapper, self.rec_only, self.min_max,
-                     self.exclude_remainder, self.verbose, self.debug, self.topic)
+        return "CmdBaselineConf:{aws:%s, zones:%s, list:%s, list:%s, conf_name:%s, timezone:%s, start_hour:%s, " \
+               "end_hour:%s, aggregation_period:%s, set_gas:%s, remove_gas:%s, indent:%s, verbose:%s}" % \
+               (self.aws, self.zones, self.list, self.__opts.duplicate, self.conf_name, self.timezone, self.start_hour,
+                self.end_hour, self.aggregation_period, self.__opts.set_gas, self.remove_gas, self.indent, self.verbose)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_aws_topic_publisher.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_aws_topic_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_baseline.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_baseline.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,25 +23,26 @@
 
     def __init__(self):
         """
         Constructor
         """
         cmds = ' | '.join(self.__UPTAKE_CMDS)
 
-        self.__parser = optparse.OptionParser(usage="%prog [-a] -c NAME -f { V | E } [{ -r | -u COMMAND }] "
+        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] -n CONF_NAME -f { V | E } "
+                                                    "[{ -r | -u COMMAND }] "
                                                     "[-s START] [-e END] [-p AGGREGATION] [-m GAS MINIMUM] "
                                                     "[{ -o GAS | -x GAS }] [-v] DEVICE_TAG_1 .. DEVICE_TAG_N",
                                               version="%prog 1.0")
 
-        # source...
-        self.__parser.add_option("--aws", "-a", action="store_true", dest="aws", default=False,
-                                 help="Use AWS S3 instead of local storage for configuration")
-
         # identity...
-        self.__parser.add_option("--conf-name", "-c", type="string", nargs=1, action="store", dest="conf_name",
+        self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
+                                 help="the stored credentials to be presented")
+
+        # target...
+        self.__parser.add_option("--conf-name", "-n", type="string", nargs=1, action="store", dest="conf_name",
                                  help="the name of the baseline configuration")
 
         # function...
         self.__parser.add_option("--fields", "-f", type="string", nargs=1, action="store", dest="fields",
                                  help="baseline Val or Exg fields")
 
         self.__parser.add_option("--rehearse", "-r", action="store_true", dest="rehearse", default=False,
@@ -123,16 +124,16 @@
     def excludes_gas(self, gas):
         return self.only_gas is not None and gas != self.only_gas
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def aws(self):
-        return self.__opts.aws
+    def credentials_name(self):
+        return self.__opts.credentials_name
 
 
     @property
     def conf_name(self):
         return self.__opts.conf_name
 
 
@@ -199,13 +200,13 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdBaseline:{aws:%s, conf_name:%s, fields:%s, rehearse:%s, uptake:%s, start_hour:%s, " \
+        return "CmdBaseline:{credentials_name:%s, conf_name:%s, fields:%s, rehearse:%s, uptake:%s, start_hour:%s, " \
                "end_hour:%s, aggregation_period:%s, minimum:%s, only_gas:%s, exclude_gas:%s, " \
                "verbose:%s, device_tags:%s}" % \
-               (self.aws, self.conf_name, self.fields, self.rehearse, self.uptake, self.start_hour,
+               (self.credentials_name, self.conf_name, self.fields, self.rehearse, self.uptake, self.start_hour,
                 self.end_hour, self.aggregation_period, self.__opts.minimum, self.only_gas, self.exclude_gas,
                 self.verbose, self.device_tags)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_baseline_conf.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_organisation_devices.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,57 @@
 """
-Created on 31 Jul 2021
+Created on 19 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdBaselineConf(object):
-    """
-    unix command line handler
-    """
-
-    # ----------------------------------------------------------------------------------------------------------------
+class CmdOrganisationDevices(object):
+    """unix command line handler"""
 
     def __init__(self):
-        self.__parser = optparse.OptionParser(usage="%prog [-a] { -z | -l | -n FROM TO | -c NAME [-t TIMEZONE_NAME] "
-                                                    "[-s START] [-e END] [-p AGGREGATION] [-g GAS MINIMUM] [-r GAS] } "
+        """
+        Constructor
+        """
+        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] { -F { -l ORG_LABEL | -t DEVICE_TAG } | "
+                                                    "-C -l ORG_LABEL -t DEVICE_TAG -p PATH_ROOT GROUP LOCATION"
+                                                    " -d DEPLOYMENT_LABEL | "
+                                                    "-D -t DEVICE_TAG } "
                                                     "[-i INDENT] [-v]", version="%prog 1.0")
 
-        # source...
-        self.__parser.add_option("--aws", "-a", action="store_true", dest="aws", default=False,
-                                 help="Use AWS S3 instead of local storage for configuration")
-
-        # helpers...
-        self.__parser.add_option("--zones", "-z", action="store_true", dest="zones", default=False,
-                                 help="list the available timezone names to stderr")
-
-        self.__parser.add_option("--list", "-l", action="store_true", dest="list", default=False,
-                                 help="list the available baseline configurations")
-
         # identity...
-        self.__parser.add_option("--duplicate", "-n", type="string", nargs=2, action="store", dest="duplicate",
-                                 help="create a new configuration based on FROM")
+        self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
+                                 help="the stored credentials to be presented")
 
-        self.__parser.add_option("--conf-name", "-c", type="string", nargs=1, action="store", dest="conf_name",
-                                 help="the name of the baseline configuration")
+        # operations...
+        self.__parser.add_option("--Find", "-F", action="store_true", dest="find", default=False,
+                                 help="find devices for the given organisation or device tag")
 
-        # fields...
-        self.__parser.add_option("--timezone", "-t", type="string", nargs=1, action="store", dest="timezone",
-                                 help="set the timezone for the tests")
+        self.__parser.add_option("--Create", "-C", action="store_true", dest="create", default=False,
+                                 help="create a device")
 
-        self.__parser.add_option("--start-hour", "-s", type="int", nargs=1, action="store", dest="start_hour",
-                                 help="test starts at the beginning of start hour")
+        self.__parser.add_option("--Delete", "-D", action="store_true", dest="delete", default=False,
+                                 help="delete the device")
 
-        self.__parser.add_option("--end-hour", "-e", type="int", nargs=1, action="store", dest="end_hour",
-                                 help="test ends at the beginning of end hour")
+        # fields...
+        self.__parser.add_option("--org-label", "-l", type="string", action="store", dest="org_label",
+                                 help="the organisation label")
 
-        self.__parser.add_option("--aggregation-period", "-p", type="int", nargs=1, action="store",
-                                 dest="aggregation_period", help="aggregation in minutes")
+        self.__parser.add_option("--device-tag", "-t", type="string", action="store", dest="device_tag",
+                                 help="the device tag")
 
-        self.__parser.add_option("--set-gas", "-g", type="string", nargs=2, action="store", dest="set_gas",
-                                 help="set minimum for GAS")
+        self.__parser.add_option("--project", "-p", type="string", nargs=3, action="store", dest="project",
+                                 help="path root, group and location number")
 
-        self.__parser.add_option("--remove-gas", "-r", type="string", nargs=1, action="store", dest="remove_gas",
-                                 help="remove GAS from minimums")
+        self.__parser.add_option("--deployment-label", "-d", type="string", action="store", dest="deployment_label",
+                                 help="the device's deployment label")
 
         # output...
         self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
@@ -69,119 +60,91 @@
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
         count = 0
 
-        if self.zones:
+        if self.find:
             count += 1
 
-        if self.list:
+        if self.create:
             count += 1
 
-        if self.duplicate_from is not None:
-            count += 1
-
-        if self.conf_name is not None:
+        if self.delete:
             count += 1
 
         if count != 1:
             return False
 
-        try:
-            _ = self.set_gas_minimum
-        except ValueError:
+        if self.find and self.org_label is None and self.device_tag is None:
             return False
 
-        return True
+        if (self.create or self.delete) and (self.org_label is None or self.device_tag is None):
+            return False
 
+        if self.delete and (self.__opts.project is None):
+            return False
 
-    def is_complete(self):
-        if self.timezone is None or self.start_hour is None or self.end_hour is None or \
-                self.aggregation_period is None:
+        if self.create and (self.__opts.project is None or self.deployment_label is None):
             return False
 
         return True
 
 
-    def duplicate(self):
-        return self.__opts.duplicate is not None
-
-
-    def set(self):
-        return self.timezone is not None or self.start_hour is not None or self.end_hour is not None or \
-               self.aggregation_period is not None or self.__opts.set_gas is not None or self.remove_gas is not None
-
-
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def aws(self):
-        return self.__opts.aws
-
-
-    @property
-    def zones(self):
-        return self.__opts.zones
-
-
-    @property
-    def list(self):
-        return self.__opts.list
-
-
-    @property
-    def duplicate_from(self):
-        return self.__opts.duplicate[0] if self.__opts.duplicate else None
+    def credentials_name(self):
+        return self.__opts.credentials_name
 
 
     @property
-    def duplicate_to(self):
-        return self.__opts.duplicate[1] if self.__opts.duplicate else None
+    def find(self):
+        return self.__opts.find
 
 
     @property
-    def conf_name(self):
-        return self.__opts.conf_name
+    def create(self):
+        return self.__opts.create
 
 
     @property
-    def timezone(self):
-        return self.__opts.timezone
+    def delete(self):
+        return self.__opts.delete
 
 
     @property
-    def start_hour(self):
-        return self.__opts.start_hour
+    def org_label(self):
+        return self.__opts.org_label
 
 
     @property
-    def end_hour(self):
-        return self.__opts.end_hour
+    def device_tag(self):
+        return self.__opts.device_tag
 
 
     @property
-    def aggregation_period(self):
-        return self.__opts.aggregation_period
+    def project_organisation(self):
+        return None if self.__opts.project is None else self.__opts.project[0]
 
 
     @property
-    def set_gas_name(self):
-        return None if self.__opts.set_gas is None else self.__opts.set_gas[0]
+    def project_group(self):
+        return None if self.__opts.project is None else self.__opts.project[1]
 
 
     @property
-    def set_gas_minimum(self):
-        return None if self.__opts.set_gas is None else int(self.__opts.set_gas[1])
+    def project_location(self):
+        return None if self.__opts.project is None else self.__opts.project[2]
 
 
     @property
-    def remove_gas(self):
-        return self.__opts.remove_gas
+    def deployment_label(self):
+        return self.__opts.deployment_label
 
 
     @property
     def indent(self):
         return self.__opts.indent
 
 
@@ -193,11 +156,11 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdBaselineConf:{aws:%s, zones:%s, list:%s, list:%s, conf_name:%s, timezone:%s, start_hour:%s, " \
-               "end_hour:%s, aggregation_period:%s, set_gas:%s, remove_gas:%s, indent:%s, verbose:%s}" % \
-               (self.aws, self.zones, self.list, self.__opts.duplicate, self.conf_name, self.timezone, self.start_hour,
-                self.end_hour, self.aggregation_period, self.__opts.set_gas, self.remove_gas, self.indent, self.verbose)
+        return "CmdOrganisationDevices:{credentials_name:%s, find:%s, create:%s, delete:%s, " \
+               "org_label:%s, device_tag:%s, project:%s, deployment_label:%s, indent:%s, verbose:%s}" % \
+               (self.credentials_name, self.find, self.create, self.delete,
+                self.org_label, self.device_tag, self.__opts.project, self.deployment_label, self.indent, self.verbose)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_devices.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_cognito_devices.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,42 +13,41 @@
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
         self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] "
-                                                    "{ -F [-t TAG] [-m] "
-                                                    "| -C TAG SHARED_SECRET "
-                                                    "| -U TAG SHARED_SECRET "
+                                                    "{ -F [-t TAG] [-n INVOICE] [-m] "
+                                                    "| -U TAG INVOICE "
                                                     "| -D TAG } "
                                                     "[-i INDENT] [-v]",
                                               version="%prog 1.0")
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--Find", "-F", action="store_true", dest="find", default=False,
                                  help="list the devices visible to me")
 
-        self.__parser.add_option("--Create", "-C", type="string", action="store", nargs=2, dest="create",
-                                 help="create a device")
-
         self.__parser.add_option("--Update", "-U", type="string", action="store", nargs=2, dest="update",
                                  help="update the device")
 
         self.__parser.add_option("--Delete", "-D", type="string", action="store", nargs=1, dest="delete",
                                  help="delete the device (superuser only)")
 
         # filters...
         self.__parser.add_option("--tag", "-t", type="string", action="store", dest="tag",
                                  help="filter by device tag")
 
+        self.__parser.add_option("--invoice", "-n", type="string", action="store", dest="invoice",
+                                 help="filter by invoice")
+
         # output...
         self.__parser.add_option("--memberships", "-m", action="store_true", dest="memberships", default=False,
                                  help="show device's organisation memberships")
 
         self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
@@ -62,18 +61,15 @@
 
     def is_valid(self):
         count = 0
 
         if self.find:
             count += 1
 
-        if self.create is not None:
-            count += 1
-
-        if self.update is not None:
+        if self.update:
             count += 1
 
         if self.delete is not None:
             count += 1
 
         if count != 1:
             return False
@@ -93,34 +89,44 @@
 
     @property
     def find(self):
         return self.__opts.find
 
 
     @property
-    def create(self):
-        return self.__opts.create
+    def update(self):
+        return bool(self.__opts.update)
 
 
     @property
-    def update(self):
-        return self.__opts.update
+    def update_tag(self):
+        return self.__opts.update[0] if self.update else None
+
+
+    @property
+    def update_invoice(self):
+        return self.__opts.update[1] if self.update else None
 
 
     @property
     def delete(self):
         return self.__opts.delete
 
 
     @property
     def tag(self):
         return self.__opts.tag
 
 
     @property
+    def invoice(self):
+        return self.__opts.invoice
+
+
+    @property
     def memberships(self):
         return self.__opts.memberships
 
 
     @property
     def indent(self):
         return self.__opts.indent
@@ -134,11 +140,11 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdCognitoDevices:{credentials_name:%s, find:%s, create:%s, update:%s, delete:%s, " \
-               "tag:%s, memberships:%s, indent:%s, verbose:%s}" % \
-               (self.credentials_name, self.find, self.create, self.update, self.delete,
-                self.tag, self.memberships, self.indent, self.verbose)
+        return "CmdCognitoDevices:{credentials_name:%s, find:%s, update:%s, delete:%s, " \
+               "tag:%s, invoice:%s, memberships:%s, indent:%s, verbose:%s}" % \
+               (self.credentials_name, self.find, self.update, self.delete,
+                self.tag, self.invoice, self.memberships, self.indent, self.verbose)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_password.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_cognito_password.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_user_credentials.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_cognito_user_credentials.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_user_identity.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_cognito_user_identity.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_cognito_users.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_cognito_users.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_configuration_csv.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_configuration_monitor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,164 +1,156 @@
 """
-Created on 7 Jul 2021
+Created on 20 Apr 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
 from scs_core.aws.manager.configuration_finder import ConfigurationRequest
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdConfigurationCSV(object):
+class CmdConfigurationMonitor(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog { -n | -s | -l OUTPUT_CSV | "
-                                                    "{ -d | -f } [-o OUTPUT_CSV_DIR] } [-t DEVICE_TAG [-e]] "
-                                                    "[-v] [NODE_1..NODE_N]", version="%prog 1.0")
-
-        # help...
-        self.__parser.add_option("--node-names", "-n", action="store_true", dest="node_names", default=False,
-                                 help="list the available nodes")
+        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] [-t TAG [-e]] { -l | -f | -d | -o } "
+                                                    "[-i INDENT] [-v]", version="%prog 1.0")
 
-        # mode...
-        self.__parser.add_option("--separate", "-s", action="store_true", dest="separate", default=False,
-                                 help="retrieve latest configurations to separate CSVs (ignores NODEs)")
+        # identity...
+        self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
+                                 help="the stored credentials to be presented")
+
+        # filters...
+        self.__parser.add_option("--tag-filter", "-t", type="string", action="store", dest="tag_filter",
+                                 help="the (partial) tag of the device(s)")
 
-        self.__parser.add_option("--latest", "-l", type="string", action="store", dest="latest",
-                                 help="retrieve latest configurations to single CSV")
+        self.__parser.add_option("--exactly", "-e", action="store_true", dest="exact_match", default=False,
+                                 help="exact match for tag")
 
-        self.__parser.add_option("--diff-histories", "-d", action="store_true", dest="diff_histories", default=False,
-                                 help="retrieve configuration history differences")
+        # mode...
+        self.__parser.add_option("--latest", "-l", action="store_true", dest="latest", default=False,
+                                 help="report latest configuration for each device")
 
-        self.__parser.add_option("--full-histories", "-f", action="store_true", dest="full_histories", default=False,
-                                 help="retrieve full configuration histories")
+        self.__parser.add_option("--full-history", "-f", action="store_true", dest="history", default=False,
+                                 help="report full configuration history")
 
-        # filter...
-        self.__parser.add_option("--device-tag", "-t", type="string", action="store", dest="device_tag",
-                                 help="the device for the history report")
+        self.__parser.add_option("--diff-history", "-d", action="store_true", dest="diff", default=False,
+                                 help="report configuration differences")
 
-        self.__parser.add_option("--exactly", "-e", action="store_true", dest="exact_match", default=False,
-                                 help="exact match for tag")
+        self.__parser.add_option("--tags-only", "-o", action="store_true", dest="tags_only", default=False,
+                                 help="report device tags only")
 
         # output...
-        self.__parser.add_option("--output-csv-dir", "-o", type="string", action="store", dest="output_csv_dir",
-                                 help="the directory in which to write histories")
+        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+                                 help="pretty-print the output with INDENT")
 
-        # narrative...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
         count = 0
 
-        if self.node_names:
-            count += 1
-
-        if self.separate:
+        if self.latest:
             count += 1
 
-        if self.latest:
+        if self.history:
             count += 1
 
-        if self.diff_histories:
+        if self.diff:
             count += 1
 
-        if self.full_histories:
+        if self.tags_only:
             count += 1
 
         if count != 1:
             return False
 
-        if self.device_tag is None and self.exact_match:
+        if self.exact_match and self.tag_filter is None:
             return False
 
         return True
 
 
-    def request_mode(self):
-        if self.separate or self.latest:
+    def response_mode(self):
+        if self.latest:
             return ConfigurationRequest.Mode.LATEST
 
-        if self.diff_histories:
+        if self.history:
+            return ConfigurationRequest.Mode.HISTORY
+
+        if self.diff:
             return ConfigurationRequest.Mode.DIFF
 
-        if self.full_histories:
-            return ConfigurationRequest.Mode.HISTORY
+        if self.tags_only:
+            return ConfigurationRequest.Mode.TAGS_ONLY
 
         return None
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def node_names(self):
-        return self.__opts.node_names
-
+    def credentials_name(self):
+        return self.__opts.credentials_name
 
     @property
-    def separate(self):
-        return self.__opts.separate
+    def tag_filter(self):
+        return self.__opts.tag_filter
 
 
     @property
-    def latest(self):
-        return self.__opts.latest
+    def exact_match(self):
+        return self.__opts.exact_match
 
 
     @property
-    def diff_histories(self):
-        return self.__opts.diff_histories
+    def latest(self):
+        return self.__opts.latest
 
 
     @property
-    def full_histories(self):
-        return self.__opts.full_histories
+    def history(self):
+        return self.__opts.history
 
 
     @property
-    def device_tag(self):
-        return self.__opts.device_tag
+    def diff(self):
+        return self.__opts.diff
 
 
     @property
-    def exact_match(self):
-        return self.__opts.exact_match
+    def tags_only(self):
+        return self.__opts.tags_only
 
 
     @property
-    def output_csv_dir(self):
-        return self.__opts.output_csv_dir
+    def indent(self):
+        return self.__opts.indent
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
-    @property
-    def nodes(self):
-        return self.__args
-
-
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdConfigurationCSV:{node_names:%s, separate:%s, latest:%s, diff_histories:%s, full_histories:%s, " \
-               "device_tag:%s, exact_match:%s, output_csv_dir:%s, verbose:%s, nodes:%s}" %  \
-               (self.node_names, self.separate, self.latest, self.diff_histories, self.full_histories,
-                self.device_tag, self.exact_match, self.output_csv_dir, self.verbose, self.nodes)
+        return "CmdConfigurationMonitor:{credentials_name:%s, tag_filter:%s, exact_match:%s, latest:%s, history:%s, " \
+               "diff:%s, tags_only:%s, indent:%s, verbose:%s}" % \
+               (self.credentials_name, self.tag_filter, self.exact_match, self.latest, self.history,
+                self.diff, self.tags_only, self.indent, self.verbose)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_configuration_monitor.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_configuration_monitor_check.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,126 +2,112 @@
 Created on 20 Apr 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
-from scs_core.aws.manager.configuration_finder import ConfigurationRequest
+from scs_core.aws.manager.configuration_check_finder import ConfigurationCheckRequest
+
+from scs_core.estate.configuration_check import ConfigurationCheck
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdConfigurationMonitor(object):
+class CmdConfigurationMonitorCheck(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-t TAG [-e]] { -l | -f | -d | -o } [-i INDENT] [-v]",
-                                              version="%prog 1.0")
+        codes = ' | '.join(ConfigurationCheck.result_codes())
+
+        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] { -f TAG | [-t TAG [-e]] [-o] } "
+                                                    "[-i INDENT] [-v]", version="%prog 1.0")
+
+        # identity...
+        self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
+                                 help="the stored credentials to be presented")
+
+        # operations...
+        self.__parser.add_option("--force", "-f", type="string", action="store", dest="force",
+                                 help="force check the device with TAG now")
 
         # filters...
         self.__parser.add_option("--tag-filter", "-t", type="string", action="store", dest="tag_filter",
                                  help="the (partial) tag of the device(s)")
 
         self.__parser.add_option("--exactly", "-e", action="store_true", dest="exact_match", default=False,
                                  help="exact match for tag")
 
-        # mode...
-        self.__parser.add_option("--latest", "-l", action="store_true", dest="latest", default=False,
-                                 help="report latest configuration for each device")
-
-        self.__parser.add_option("--full-history", "-f", action="store_true", dest="history", default=False,
-                                 help="report full configuration history")
-
-        self.__parser.add_option("--diff-history", "-d", action="store_true", dest="diff", default=False,
-                                 help="report configuration differences")
+        self.__parser.add_option("--result", "-r", type="string", nargs=1, action="store", dest="result_code",
+                                 help="match the result { %s }" % codes)
 
+        # output...
         self.__parser.add_option("--tags-only", "-o", action="store_true", dest="tags_only", default=False,
                                  help="report device tags only")
 
-        # output...
         self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        count = 0
-
-        if self.latest:
-            count += 1
-
-        if self.history:
-            count += 1
-
-        if self.diff:
-            count += 1
-
-        if self.tags_only:
-            count += 1
-
-        if count != 1:
+        if self.force and (self.tag_filter or self.result_code or self.tags_only):
             return False
 
         if self.exact_match and self.tag_filter is None:
             return False
 
-        return True
-
+        if self.result_code and self.result_code not in ConfigurationCheck.result_codes():
+            return False
 
-    def response_mode(self):
-        if self.latest:
-            return ConfigurationRequest.Mode.LATEST
+        return True
 
-        if self.history:
-            return ConfigurationRequest.Mode.HISTORY
 
-        if self.diff:
-            return ConfigurationRequest.Mode.DIFF
+    def result(self):
+        return ConfigurationCheck.result_string(self.result_code)
 
-        if self.tags_only:
-            return ConfigurationRequest.Mode.TAGS_ONLY
 
-        return None
+    def response_mode(self):
+        return ConfigurationCheckRequest.Mode.TAGS_ONLY if self.tags_only else ConfigurationCheckRequest.Mode.FULL
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def tag_filter(self):
-        return self.__opts.tag_filter
+    def credentials_name(self):
+        return self.__opts.credentials_name
 
 
     @property
-    def exact_match(self):
-        return self.__opts.exact_match
+    def force(self):
+        return self.__opts.force
 
 
     @property
-    def latest(self):
-        return self.__opts.latest
+    def tag_filter(self):
+        return self.__opts.tag_filter
 
 
     @property
-    def history(self):
-        return self.__opts.history
+    def exact_match(self):
+        return self.__opts.exact_match
 
 
     @property
-    def diff(self):
-        return self.__opts.diff
+    def result_code(self):
+        return self.__opts.result_code
 
 
     @property
     def tags_only(self):
         return self.__opts.tags_only
 
 
@@ -138,11 +124,11 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdConfigurationMonitor:{tag_filter:%s, exact_match:%s, latest:%s, history:%s, diff:%s, " \
-               "tags_only:%s, indent:%s, verbose:%s}" % \
-               (self.tag_filter, self.exact_match, self.latest, self.history, self.diff,
-                self.tags_only, self.indent, self.verbose)
+        return "CmdConfigurationMonitorCheck:{credentials_name:%s, force:%s, tag_filter:%s, exact_match:%s, " \
+               "result_code:%s, tags_only:%s, indent:%s, verbose:%s}" % \
+               (self.credentials_name, self.force, self.tag_filter, self.exact_match,
+                self.result_code, self.tags_only, self.indent, self.verbose)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_configuration_monitor_check.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_histo_chart.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,125 +1,128 @@
 """
-Created on 20 Apr 2021
+Created on 4 Aug 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
+
+source repo: scs_analysis
 """
 
 import optparse
 
-from scs_core.aws.manager.configuration_check_finder import ConfigurationCheckRequest
-
-from scs_core.estate.configuration_check import ConfigurationCheck
-
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdConfigurationMonitorCheck(object):
-    """unix command line handler"""
+class CmdHistoChart(object):
+    """
+    unix command line handler
+    """
 
     def __init__(self):
         """
         Constructor
         """
-        codes = ' | '.join(ConfigurationCheck.result_codes())
+        self.__parser = optparse.OptionParser(usage="%prog [-b] [-x MIN MAX] [-c BIN_COUNT] [-p PRECISION] "
+                                                    "[-o FILENAME] [-e] [-t TITLE] [-v] PATH", version="%prog 1.0")
+
+        # optional...
+        self.__parser.add_option("--batch", "-b", action="store_true", dest="batch_mode", default=False,
+                                 help="wait for all data before displaying chart")
 
-        self.__parser = optparse.OptionParser(usage="%prog { -c TAG | [-t TAG [-e]] [-r RESULT] [-o] } [-i INDENT] "
-                                                    "[-v]", version="%prog 1.0")
+        self.__parser.add_option("--x", "-x", type="float", nargs=2, action="store", default=(-1.0, 1.0), dest="x",
+                                 help="set x-axis to min / max (default -1, 1)")
 
-        # operations...
-        self.__parser.add_option("--check", "-c", type="string", action="store", dest="check",
-                                 help="check the device with TAG now")
+        self.__parser.add_option("--bincount", "-c", type="int", nargs=1, action="store", default=200, dest="bin_count",
+                                 help="number of bins (default 200)")
 
-        # filters...
-        self.__parser.add_option("--tag-filter", "-t", type="string", action="store", dest="tag_filter",
-                                 help="the (partial) tag of the device(s)")
+        self.__parser.add_option("--precision", "-p", type="int", nargs=1, action="store", default=3, dest="precision",
+                                 help="precision of reported deltas (default 3)")
 
-        self.__parser.add_option("--exactly", "-e", action="store_true", dest="exact_match", default=False,
-                                 help="exact match for tag")
+        self.__parser.add_option("--skip-malformed", "-s", action="store_true", dest="skip_malformed", default=False,
+                                 help="ignore rows with missing path values")
 
-        self.__parser.add_option("--result", "-r", type="string", nargs=1, action="store", dest="result_code",
-                                 help="match the result { %s }" % codes)
+        self.__parser.add_option("--output", "-o", type="string", nargs=1, action="store", dest="outfile",
+                                 help="output histogram to CSV file")
 
-        # output...
-        self.__parser.add_option("--tags-only", "-o", action="store_true", dest="tags_only", default=False,
-                                 help="report device tags only")
+        self.__parser.add_option("--echo", "-e", action="store_true", dest="echo", default=False,
+                                 help="echo stdin to stdout")
 
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
-                                 help="pretty-print the output with INDENT")
+        self.__parser.add_option("--title", "-t", type="string", nargs=1, action="store", dest="title",
+                                 help="chart title")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.check_tag and (self.tag_filter or self.result_code or self.tags_only):
-            return False
-
-        if self.exact_match and self.tag_filter is None:
-            return False
-
-        if self.result_code and self.result_code not in ConfigurationCheck.result_codes():
+        if self.path is None:
             return False
 
         return True
 
 
-    def result(self):
-        return ConfigurationCheck.result_string(self.result_code)
+    # ----------------------------------------------------------------------------------------------------------------
 
+    @property
+    def batch_mode(self):
+        return self.__opts.batch_mode
 
-    def response_mode(self):
-        return ConfigurationCheckRequest.Mode.TAGS_ONLY if self.tags_only else ConfigurationCheckRequest.Mode.FULL
 
+    @property
+    def x(self):
+        return self.__opts.x
 
-    # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def check_tag(self):
-        return self.__opts.check
+    def bin_count(self):
+        return self.__opts.bin_count
 
 
     @property
-    def tag_filter(self):
-        return self.__opts.tag_filter
+    def precision(self):
+        return self.__opts.precision
 
 
     @property
-    def exact_match(self):
-        return self.__opts.exact_match
+    def outfile(self):
+        return self.__opts.outfile
 
 
     @property
-    def result_code(self):
-        return self.__opts.result_code
+    def echo(self):
+        return self.__opts.echo
 
 
     @property
-    def tags_only(self):
-        return self.__opts.tags_only
+    def skip_malformed(self):
+        return self.__opts.skip_malformed
 
 
     @property
-    def indent(self):
-        return self.__opts.indent
+    def title(self):
+        return self.__opts.title
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
+    @property
+    def path(self):
+        return self.__args[0] if len(self.__args) > 0 else None
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdConfigurationMonitorCheck:{check:%s, tag_filter:%s, exact_match:%s, result_code:%s, tags_only:%s, " \
-               "indent:%s, verbose:%s}" % \
-               (self.check_tag, self.tag_filter, self.exact_match, self.result_code, self.tags_only,
-                self.indent, self.verbose)
+        return "CmdHistoChart:{batch_mode:%s, x:%s, bin_count:%d, precision:%d, outfile:%s, echo:%s, " \
+               "skip_malformed:%s, title:%s, verbose:%s, path:%s}" % \
+                    (self.batch_mode, self.x, self.bin_count, self.precision, self.outfile, self.echo,
+                     self.skip_malformed, self.title, self.verbose, self.path)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_collation_summary.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_csv_collation_summary.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_collator.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_join.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_csv_join.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_reader.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_segmentor.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_distance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,95 @@
 """
-Created on 10 Mar 2020
+Created on 11 Jul 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
-from scs_core.data.timedelta import Timedelta
-
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdCSVSegmentor(object):
+class CmdSampleDistance(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog -m { [DD-]HH:MM[:SS] | :SS } [-i ISO] [-f FILE_PREFIX] "
-                                                    "[-v]", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog -p LAT LNG [-i ISO] [-q QUALITY] [-v] GPS_PATH",
+                                              version="%prog 1.0")
 
         # compulsory...
-        self.__parser.add_option("--max-interval", "-m", type="string", nargs=1, action="store", dest="max_interval",
-                                 help="maximum permitted interval")
+        self.__parser.add_option("--position", "-p", type="float", nargs=2, action="store", dest="position",
+                                 help="position (in degrees)")
 
         # optional...
         self.__parser.add_option("--iso-path", "-i", type="string", nargs=1, action="store", default="rec", dest="iso",
-                                 help="path for ISO 8601 datetime field (default 'rec')")
+                                 help="path for ISO 8601 datetime output (default 'rec')")
 
-        self.__parser.add_option("--file-prefix", "-f", type="string", nargs=1, action="store", dest="file_prefix",
-                                 help="file prefix for contiguous CSVs")
+        self.__parser.add_option("--quality", "-q", type="int", nargs=1, action="store", dest="quality",
+                                 help="minimum acceptable GPS quality")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.__opts.max_interval is None:
+        if self.position is None or self.path is None:
             return False
 
         return True
 
 
-    def is_valid_interval(self):
-        if self.__opts.max_interval is None:
-            return True
+    # ----------------------------------------------------------------------------------------------------------------
 
-        return self.max_interval is not None
+    @property
+    def position(self):
+        return self.__opts.position
 
 
-    # ----------------------------------------------------------------------------------------------------------------
+    @property
+    def lat(self):
+        return None if self.__opts.position is None else self.__opts.position[0]
+
 
     @property
-    def max_interval(self):
-        return Timedelta.construct_from_flag(self.__opts.max_interval)
+    def lng(self):
+        return None if self.__opts.position is None else self.__opts.position[1]
 
 
     @property
     def iso(self):
         return self.__opts.iso
 
 
     @property
-    def file_prefix(self):
-        return self.__opts.file_prefix
+    def quality(self):
+        return self.__opts.quality
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
+    @property
+    def path(self):
+        return self.__args[0] if len(self.__args) > 0 else None
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdCSVSegmentor:{max_interval:%s, iso:%s, file_prefix:%s, verbose:%s}" % \
-               (self.__opts.max_interval, self.iso, self.file_prefix, self.verbose)
+        return "CmdSampleDistance:{position:%s, iso:%s, quality:%s, verbose:%s, path:%s}" % \
+               (self.position, self.iso, self.quality, self.verbose, self.path)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_csv_writer.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_histo_chart.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_single_chart.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,49 @@
 """
-Created on 4 Aug 2016
+Created on 11 Jul 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdHistoChart(object):
-    """
-    unix command line handler
-    """
+class CmdSingleChart(object):
+    """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-b] [-x MIN MAX] [-c BIN_COUNT] [-p PRECISION] "
-                                                    "[-o FILENAME] [-e] [-t TITLE] [-v] PATH", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [-b] [-r] [-x POINTS] [-y MIN MAX] [-e] [-t TITLE] [-v] "
+                                                    "[PATH]", version="%prog 1.0")
 
         # optional...
         self.__parser.add_option("--batch", "-b", action="store_true", dest="batch_mode", default=False,
                                  help="wait for all data before displaying chart")
 
-        self.__parser.add_option("--x", "-x", type="float", nargs=2, action="store", default=(-1.0, 1.0), dest="x",
-                                 help="set x-axis to min / max (default -1, 1)")
+        self.__parser.add_option("--relative", "-r", action="store_true", dest="relative", default=False,
+                                 help="display relative values (first value is 0)")
 
-        self.__parser.add_option("--bincount", "-c", type="int", nargs=1, action="store", default=200, dest="bin_count",
-                                 help="number of bins (default 200)")
+        self.__parser.add_option("--x", "-x", type="int", nargs=1, action="store", default=600, dest="x",
+                                 help="number of x points (default 600)")
 
-        self.__parser.add_option("--precision", "-p", type="int", nargs=1, action="store", default=3, dest="precision",
-                                 help="precision of reported deltas (default 3)")
-
-        self.__parser.add_option("--skip-malformed", "-s", action="store_true", dest="skip_malformed", default=False,
-                                 help="ignore rows with missing path values")
-
-        self.__parser.add_option("--output", "-o", type="string", nargs=1, action="store", dest="outfile",
-                                 help="output histogram to CSV file")
+        self.__parser.add_option("--y", "-y", type="float", nargs=2, action="store", default=(-10.0, 10.0), dest="y",
+                                 help="set y-axis to min / max (default -10, 10)")
 
         self.__parser.add_option("--echo", "-e", action="store_true", dest="echo", default=False,
                                  help="echo stdin to stdout")
 
+        self.__parser.add_option("--skip-malformed", "-s", action="store_true", dest="skip_malformed", default=False,
+                                 help="ignore rows with missing path values")
+
         self.__parser.add_option("--title", "-t", type="string", nargs=1, action="store", dest="title",
                                  help="chart title")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
@@ -67,31 +62,26 @@
 
     @property
     def batch_mode(self):
         return self.__opts.batch_mode
 
 
     @property
-    def x(self):
-        return self.__opts.x
+    def relative(self):
+        return self.__opts.relative
 
 
     @property
-    def bin_count(self):
-        return self.__opts.bin_count
-
-
-    @property
-    def precision(self):
-        return self.__opts.precision
+    def x(self):
+        return self.__opts.x
 
 
     @property
-    def outfile(self):
-        return self.__opts.outfile
+    def y(self):
+        return self.__opts.y
 
 
     @property
     def echo(self):
         return self.__opts.echo
 
 
@@ -118,11 +108,11 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdHistoChart:{batch_mode:%s, x:%s, bin_count:%d, precision:%d, outfile:%s, echo:%s, " \
-               "skip_malformed:%s, title:%s, verbose:%s, path:%s}" % \
-                    (self.batch_mode, self.x, self.bin_count, self.precision, self.outfile, self.echo,
-                     self.skip_malformed, self.title, self.verbose, self.path)
+        return "CmdSingleChart:{batch_mode:%s, relative:%s, x:%d, y:%s, echo:%s, skip_malformed:%s, title:%s, " \
+               "verbose:%s, path:%s}" % \
+                    (self.batch_mode, self.relative, self.x, self.y, self.echo, self.skip_malformed, self.title,
+                     self.verbose, self.path)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_localised_datetime.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_localised_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_monitor_auth.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_mqtt_client.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_mqtt_control.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_slope.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,146 +1,126 @@
 """
-Created on 9 May 2017
+Created on 23 Oct 2020
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_core.data.timedelta import Timedelta
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdMQTTControl(object):
+class CmdSampleSlope(object):
     """unix command line handler"""
 
-    DEFAULT_TIMEOUT = 30                # seconds
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog { -p HOSTNAME [-a] | -d TAG SHARED_SECRET TOPIC } "
-                                                    "{ -i | -r [CMD_TOKENS] } [-t TIMEOUT] [-v]", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog -n NAME [-i ISO] [-t TALLY] [-m [DD-]HH:MM[:SS]] [-x] "
+                                                    "[-p PRECISION] [-v] PATH", version="%prog 1.0")
 
         # compulsory...
-        self.__parser.add_option("--peer", "-p", type="string", nargs=1, action="store", dest="peer",
-                                 help="use the stored MQTT peer")
-
-        self.__parser.add_option("--device", "-d", type="string", nargs=3, action="store", dest="device",
-                                 help="specify a tag, shared secret and topic for the peer")
+        self.__parser.add_option("--name", "-n", type="string", nargs=1, action="store", dest="name",
+                                 help="slope field name (i.e. '1min')")
 
         # optional...
-        self.__parser.add_option("--aws", "-a", action="store_true", dest="aws", default=False,
-                                 help="Use AWS S3 instead of local storage for peer")
+        self.__parser.add_option("--iso-path", "-i", type="string", nargs=1, action="store", default="rec", dest="iso",
+                                 help="path for ISO 8601 datetime field (default 'rec')")
 
-        self.__parser.add_option("--receipt", "-r", action="store_true", dest="receipt", default=False,
-                                 help="wait for receipt from target peer")
+        self.__parser.add_option("--tally", "-t", type="int", nargs=1, action="store", default=2, dest="tally",
+                                 help="compute for rolling TALLY number of data points (default 2)")
 
-        self.__parser.add_option("--interactive", "-i", action="store_true", dest="interactive", default=False,
-                                 help="interactive mode (always waits for receipt)")
+        self.__parser.add_option("--max-interval", "-m", type="string", nargs=1, action="store", dest="max_interval",
+                                 help="restart regression on long intervals")
 
-        self.__parser.add_option("--timeout", "-t", type="int", nargs=1, action="store", dest="timeout",
-                                 default=self.DEFAULT_TIMEOUT,
-                                 help="receipt timeout in seconds (default %d)" % self.DEFAULT_TIMEOUT)
+        self.__parser.add_option("--exclude-incomplete", "-x", action="store_true", dest="exclude_incomplete",
+                                 default=False, help="exclude incomplete tallies")
+
+        self.__parser.add_option("--prec", "-p", type="int", nargs=1, action="store", default=6, dest="precision",
+                                 help="precision (default 6 decimal places)")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.is_stored_peer() == self.is_device():
-            return False
-
-        if self.interactive == self.receipt:
+        if self.name is None:
             return False
 
-        if self.interactive and self.cmd_tokens is not None:
+        if self.tally < 1:
             return False
 
-        if self.aws and not self.is_stored_peer():
+        if self.path is None:
             return False
 
         return True
 
 
-    # ----------------------------------------------------------------------------------------------------------------
-
-    def is_stored_peer(self):
-        return self.__opts.peer is not None
-
+    def is_valid_interval(self):
+        if self.__opts.max_interval is None:
+            return True
 
-    def is_device(self):
-        return self.__opts.device is not None
+        return self.max_interval is not None
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def peer_hostname(self):
-        return self.__opts.peer
-
-
-    @property
-    def aws(self):
-        return self.__opts.aws
+    def name(self):
+        return self.__opts.name
 
 
     @property
-    def device_tag(self):
-        return None if self.__opts.device is None else self.__opts.device[0]
+    def iso(self):
+        return self.__opts.iso
 
 
     @property
-    def device_shared_secret(self):
-        return None if self.__opts.device is None else self.__opts.device[1]
+    def tally(self):
+        return self.__opts.tally
 
 
     @property
-    def device_topic(self):
-        return None if self.__opts.device is None else self.__opts.device[2]
+    def max_interval(self):
+        return Timedelta.construct_from_flag(self.__opts.max_interval)
 
 
     @property
-    def cmd_tokens(self):
-        return self.__args[0].split() if len(self.__args) > 0 else None
+    def exclude_incomplete(self):
+        return self.__opts.exclude_incomplete
 
 
     @property
-    def receipt(self):
-        return self.__opts.receipt
+    def precision(self):
+        return self.__opts.precision
 
 
     @property
-    def interactive(self):
-        return self.__opts.interactive
-
-
-    @property
-    def timeout(self):
-        return self.__opts.timeout
+    def verbose(self):
+        return self.__opts.verbose
 
 
     @property
-    def verbose(self):
-        return self.__opts.verbose
+    def path(self):
+        return self.__args[0] if len(self.__args) > 0 else None
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdMQTTControl:{peer:%s, device:%s, aws:%s, cmd_tokens:%s, receipt:%s, interactive:%s, " \
-               "timeout:%s, verbose:%s}" % \
-               (self.__opts.peer, self.__opts.device, self.aws, self.cmd_tokens, self.receipt, self.interactive,
-                self.timeout, self.verbose)
+        return "CmdSampleSlope:{name:%s, iso:%s, tally:%s, exclude_incomplete:%s, precision:%s, verbose:%s, " \
+               "path:%s}" % \
+               (self.name, self.iso, self.tally, self.exclude_incomplete, self.precision, self.verbose,
+                self.path)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_mqtt_peers.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_organisation_users.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,203 +1,176 @@
 """
-Created on 9 Mar 2019
+Created on 18 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdMQTTPeers(object):
+class CmdOrganisationUsers(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-a] { -p [-e] | -l [-n HOSTNAME] [-t TOPIC] | -m | "
-                                                    "-c HOSTNAME TAG SHARED_SECRET TOPIC | "
-                                                    "-u HOSTNAME { -s SHARED_SECRET | -t TOPIC } | "
-                                                    "-r HOSTNAME } [-i INDENT] [-v]", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] { -F [{ -e EMAIL | -l ORG_LABEL }] | "
+                                                    "-R -e EMAIL -l ORG_LABEL | "
+                                                    "-C -e EMAIL -l ORG_LABEL -o { 1 | 0 } -d { 1 | 0 } | "
+                                                    "-U -e EMAIL -l ORG_LABEL [-o { 1 | 0 }] [-d { 1 | 0 }] "
+                                                    "[-s { 1 | 0 }] | "
+                                                    "-D -e EMAIL -l ORG_LABEL } "
+                                                    "[-i INDENT] [-v]", version="%prog 1.0")
 
-        # source...
-        self.__parser.add_option("--aws", "-a", action="store_true", dest="aws", default=False,
-                                 help="Use AWS S3 instead of local storage")
+        # identity...
+        self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
+                                 help="the stored credentials to be presented")
 
-        # functions...
-        self.__parser.add_option("--import", "-p", action="store_true", dest="import_peers", default=False,
-                                 help="import MQTT peers from stdin")
+        # operations...
+        self.__parser.add_option("--Find", "-F", action="store_true", dest="find", default=False,
+                                 help="find users for the given username or organisation")
 
-        self.__parser.add_option("--list", "-l", action="store_true", dest="list", default=False,
-                                 help="list the stored MQTT peers to stdout")
+        self.__parser.add_option("--Retrieve", "-R", action="store_true", dest="retrieve", default=False,
+                                 help="retrieve the user for the given username and organisation")
 
-        self.__parser.add_option("--missing", "-m", action="store_true", dest="missing", default=False,
-                                 help="list known devices missing from S3 MQTT peers")
+        self.__parser.add_option("--Create", "-C", action="store_true", dest="create", default=False,
+                                 help="create a user")
 
-        self.__parser.add_option("--create", "-c", type="string", nargs=4, action="store", dest="create",
-                                 help="create an MQTT peer")
+        self.__parser.add_option("--Update", "-U", action="store_true", dest="update", default=False,
+                                 help="Update the user")
 
-        self.__parser.add_option("--update", "-u", type="string", nargs=1, action="store", dest="update",
-                                 help="update an MQTT peer")
+        self.__parser.add_option("--Delete", "-D", action="store_true", dest="delete", default=False,
+                                 help="delete the user for the given username and organisation")
 
-        self.__parser.add_option("--remove", "-r", type="string", nargs=1, action="store", dest="remove",
-                                 help="delete an MQTT peer")
+        # fields...
+        self.__parser.add_option("--email", "-e", type="string", action="store", dest="email",
+                                 help="the user's email address (exact match)")
 
-        # filters...
-        self.__parser.add_option("--hostname", "-n", type="string", nargs=1, action="store", dest="hostname",
-                                 help="filter peers with the given hostname substring")
+        self.__parser.add_option("--org-label", "-l", type="string", action="store", dest="org_label",
+                                 help="the organisation label")
 
-        self.__parser.add_option("--shared-secret", "-s", type="string", nargs=1, action="store", dest="shared_secret",
-                                 help="specify shared secret")
+        self.__parser.add_option("--org-admin", "-o", type="int", action="store", dest="org_admin",
+                                 help="the organisation administrator status")
 
-        self.__parser.add_option("--topic", "-t", type="string", nargs=1, action="store", dest="topic",
-                                 help="specify topic")
+        self.__parser.add_option("--device-admin", "-d", type="int", action="store", dest="device_admin",
+                                 help="the device administrator status")
 
-        # output...
-        self.__parser.add_option("--echo", "-e", action="store_true", dest="echo", default=False,
-                                 help="echo stdin to stdout (import only)")
+        self.__parser.add_option("--suspended", "-s", type="int", action="store", dest="suspended",
+                                 help="the suspended status")
 
+        # output...
         self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
-                                 help="pretty-print the output with INDENT (not with echo)")
+                                 help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
         count = 0
 
-        if self.is_import():
-            count += 1
-
-        if self.missing:
+        if self.find:
             count += 1
 
-        if self.list:
+        if self.retrieve:
             count += 1
 
-        if self.is_create():
+        if self.create:
             count += 1
 
-        if self.is_update():
+        if self.update:
             count += 1
 
-        if self.is_remove():
+        if self.delete:
             count += 1
 
         if count != 1:
             return False
 
-        if not self.is_import() and self.echo:
+        if self.org_admin is not None and self.org_admin != 0 and self.org_admin != 1:
             return False
 
-        if self.__opts.list is None and (self.__opts.hostname is not None or self.__opts.for_topic is not None):
+        if self.device_admin is not None and self.device_admin != 0 and self.device_admin != 1:
             return False
 
-        if self.missing and not self.aws:
+        if self.suspended is not None and self.suspended != 0 and self.suspended != 1:
             return False
 
-        if self.echo and self.indent is not None:
+        if self.find and bool(self.email) and bool(self.org_label):
             return False
 
-        if self.is_update() and not self.shared_secret and not self.topic:
+        if (self.retrieve or self.create or self.update or self.delete) and \
+                (self.email is None or self.org_label is None):
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def is_import(self):
-        return self.__opts.import_peers
-
-
-    def is_create(self):
-        return self.__opts.create is not None
-
-
-    def is_update(self):
-        return self.__opts.update is not None
-
-
-    def is_remove(self):
-        return self.__opts.remove is not None
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    @property
-    def list(self):
-        return self.__opts.list
-
-
     @property
-    def missing(self):
-        return self.__opts.missing
+    def credentials_name(self):
+        return self.__opts.credentials_name
 
 
     @property
-    def create_hostname(self):
-        return None if self.__opts.create is None else self.__opts.create[0]
+    def find(self):
+        return self.__opts.find
 
 
     @property
-    def create_tag(self):
-        return None if self.__opts.create is None else self.__opts.create[1]
+    def retrieve(self):
+        return self.__opts.retrieve
 
 
     @property
-    def create_shared_secret(self):
-        return None if self.__opts.create is None else self.__opts.create[2]
+    def create(self):
+        return self.__opts.create
 
 
     @property
-    def create_topic(self):
-        return None if self.__opts.create is None else self.__opts.create[3]
-
-
-    @property
-    def update_hostname(self):
+    def update(self):
         return self.__opts.update
 
 
     @property
-    def remove_hostname(self):
-        return self.__opts.remove
+    def delete(self):
+        return self.__opts.delete
 
 
     @property
-    def hostname(self):
-        return self.__opts.hostname
+    def email(self):
+        return self.__opts.email
 
 
     @property
-    def shared_secret(self):
-        return self.__opts.shared_secret
+    def org_label(self):
+        return self.__opts.org_label
 
 
     @property
-    def topic(self):
-        return self.__opts.topic
+    def org_admin(self):
+        return self.__opts.org_admin
 
 
     @property
-    def aws(self):
-        return self.__opts.aws
+    def device_admin(self):
+        return self.__opts.device_admin
 
 
     @property
-    def echo(self):
-        return self.__opts.echo
+    def suspended(self):
+        return self.__opts.suspended
 
 
     @property
     def indent(self):
         return self.__opts.indent
 
 
@@ -207,14 +180,15 @@
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
+
     def __str__(self, *args, **kwargs):
-        return "CmdMQTTPeers:{import:%s, list:%s, missing:%s, create:%s, update:%s, " \
-               "remove:%s, hostname:%s, shared_secret:%s, topic:%s, aws:%s, echo:%s, indent:%s, " \
-               "verbose:%s}" %  \
-               (self.__opts.import_peers, self.list, self.missing, self.__opts.create, self.__opts.update,
-                self.__opts.remove, self.hostname, self.shared_secret, self.topic, self.aws, self.echo, self.indent,
-                self.verbose)
+        return "CmdOrganisationUsers:{credentials_name:%s, find:%s, create:%s, update:%s, delete:%s, " \
+               "email:%s, org_label:%s, org_admin:%s, device_admin:%s, suspended:%s, " \
+               "indent:%s, verbose:%s}" % \
+               (self.credentials_name, self.find, self.create, self.update, self.delete,
+                self.email, self.org_label, self.__opts.org_admin, self.__opts.device_admin, self.__opts.suspended,
+                self.indent, self.verbose)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_multi_chart.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_node.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_node.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisation_devices.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_organisations.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 """
-Created on 19 Jan 2022
+Created on 10 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdOrganisationDevices(object):
+class CmdOrganisations(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] { -F { -l ORG_LABEL | -t DEVICE_TAG } | "
-                                                    "-C -l ORG_LABEL -t DEVICE_TAG -p PATH_ROOT GROUP LOCATION"
-                                                    " -d DEPLOYMENT_LABEL | "
-                                                    "-D -t DEVICE_TAG } "
+        self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] { -F | "
+                                                    "-C -l LABEL -n LONG_NAME -u URL -o OWNER_EMAIL | "
+                                                    "-U LABEL [-l LABEL] [-n LONG_NAME] [-u URL] [-o OWNER_EMAIL] | "
+                                                    "-D LABEL } "
                                                     "[-i INDENT] [-v]", version="%prog 1.0")
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
         self.__parser.add_option("--Find", "-F", action="store_true", dest="find", default=False,
-                                 help="find devices for the given organisation or device tag")
+                                 help="find the organisations I belong to")
 
         self.__parser.add_option("--Create", "-C", action="store_true", dest="create", default=False,
-                                 help="create a device")
+                                 help="create an organisation")
 
-        self.__parser.add_option("--Delete", "-D", action="store_true", dest="delete", default=False,
-                                 help="delete the device")
+        self.__parser.add_option("--Update", "-U", type="string", action="store", dest="update",
+                                 help="update the organisation with the given LABEL")
+
+        self.__parser.add_option("--Delete", "-D", type="string", action="store", dest="delete",
+                                 help="delete the organisation")
 
         # fields...
-        self.__parser.add_option("--org-label", "-l", type="string", action="store", dest="org_label",
+        self.__parser.add_option("--label", "-l", type="string", action="store", dest="label",
                                  help="the organisation label")
 
-        self.__parser.add_option("--device-tag", "-t", type="string", action="store", dest="device_tag",
-                                 help="the device tag")
+        self.__parser.add_option("--long-name", "-n", type="string", action="store", dest="long_name",
+                                 help="the organisation long name")
 
-        self.__parser.add_option("--project", "-p", type="string", nargs=3, action="store", dest="project",
-                                 help="path root, group and location number")
+        self.__parser.add_option("--url", "-u", type="string", action="store", dest="url",
+                                 help="the organisation URL")
 
-        self.__parser.add_option("--deployment-label", "-d", type="string", action="store", dest="deployment_label",
-                                 help="the device's deployment label")
+        self.__parser.add_option("--owner", "-o", type="string", action="store", dest="owner",
+                                 help="the organisation owner email")
 
         # output...
         self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
@@ -66,30 +69,24 @@
 
         if self.find:
             count += 1
 
         if self.create:
             count += 1
 
-        if self.delete:
+        if self.update is not None:
             count += 1
 
-        if count != 1:
-            return False
-
-        if self.find and self.org_label is None and self.device_tag is None:
-            return False
-
-        if (self.create or self.delete) and (self.org_label is None or self.device_tag is None):
-            return False
+        if self.delete is not None:
+            count += 1
 
-        if self.delete and (self.__opts.project is None):
+        if count != 1:
             return False
 
-        if self.create and (self.__opts.project is None or self.deployment_label is None):
+        if self.create and (self.label is None or self.long_name is None or self.url is None or self.owner is None):
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
@@ -105,46 +102,41 @@
 
     @property
     def create(self):
         return self.__opts.create
 
 
     @property
-    def delete(self):
-        return self.__opts.delete
-
-
-    @property
-    def org_label(self):
-        return self.__opts.org_label
+    def update(self):
+        return self.__opts.update
 
 
     @property
-    def device_tag(self):
-        return self.__opts.device_tag
+    def delete(self):
+        return self.__opts.delete
 
 
     @property
-    def project_organisation(self):
-        return None if self.__opts.project is None else self.__opts.project[0]
+    def label(self):
+        return self.__opts.label
 
 
     @property
-    def project_group(self):
-        return None if self.__opts.project is None else self.__opts.project[1]
+    def long_name(self):
+        return self.__opts.long_name
 
 
     @property
-    def project_location(self):
-        return None if self.__opts.project is None else self.__opts.project[2]
+    def url(self):
+        return self.__opts.url
 
 
     @property
-    def deployment_label(self):
-        return self.__opts.deployment_label
+    def owner(self):
+        return self.__opts.owner
 
 
     @property
     def indent(self):
         return self.__opts.indent
 
 
@@ -156,11 +148,11 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdOrganisationDevices:{credentials_name:%s, find:%s, create:%s, delete:%s, " \
-               "org_label:%s, device_tag:%s, project:%s, deployment_label:%s, indent:%s, verbose:%s}" % \
-               (self.credentials_name, self.find, self.create, self.delete,
-                self.org_label, self.device_tag, self.__opts.project, self.deployment_label, self.indent, self.verbose)
+        return "CmdOrganisations:{credentials_name:%s, find:%s, create:%s, update:%s, delete:%s, " \
+               "label:%s, long_name:%s, url:%s, owner:%s, indent:%s, verbose:%s}" % \
+               (self.credentials_name, self.find, self.create, self.update, self.delete,
+                self.label, self.long_name, self.url, self.owner, self.indent, self.verbose)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisation_path_roots.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_organisation_path_roots.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisation_user_paths.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_organisation_user_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisation_users.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_alert_status.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,177 +1,142 @@
 """
-Created on 18 Jan 2022
+Created on 29 Jun 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_core.aws.manager.alert_status_manager import AlertStatusFindRequest
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdOrganisationUsers(object):
+class CmdAlertStatus(object):
     """unix command line handler"""
 
+    __CAUSES = {'L': '<L', 'U': '>U', 'N': 'NV', 'OK': 'OK'}
+
+    # --------------------------------------------------------------------------------------------------------------------
+
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] { -F [{ -e EMAIL | -l ORG_LABEL }] | "
-                                                    "-R -e EMAIL -l ORG_LABEL | "
-                                                    "-C -e EMAIL -l ORG_LABEL -o { 1 | 0 } -d { 1 | 0 } | "
-                                                    "-U -e EMAIL -l ORG_LABEL [-o { 1 | 0 }] [-d { 1 | 0 }] "
-                                                    "[-s { 1 | 0 }] | "
-                                                    "-D -e EMAIL -l ORG_LABEL } "
-                                                    "[-i INDENT] [-v]", version="%prog 1.0")
+        causes = ' | '.join(self.__CAUSES)
+
+        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] { -F { -l | -d [-a CAUSE] } | -D } "
+                                                    "[-i INDENT] [-v] ID",
+                                              version="%prog 1.0")
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
         # operations...
-        self.__parser.add_option("--Find", "-F", action="store_true", dest="find", default=False,
-                                 help="find users for the given username or organisation")
-
-        self.__parser.add_option("--Retrieve", "-R", action="store_true", dest="retrieve", default=False,
-                                 help="retrieve the user for the given username and organisation")
-
-        self.__parser.add_option("--Create", "-C", action="store_true", dest="create", default=False,
-                                 help="create a user")
-
-        self.__parser.add_option("--Update", "-U", action="store_true", dest="update", default=False,
-                                 help="Update the user")
-
-        self.__parser.add_option("--Delete", "-D", action="store_true", dest="delete", default=False,
-                                 help="delete the user for the given username and organisation")
-
-        # fields...
-        self.__parser.add_option("--email", "-e", type="string", action="store", dest="email",
-                                 help="the user's email address (exact match)")
+        self.__parser.add_option("--find", "-F", action="store_true", dest="find", default=False,
+                                 help="find alert status reports")
 
-        self.__parser.add_option("--org-label", "-l", type="string", action="store", dest="org_label",
-                                 help="the organisation label")
+        self.__parser.add_option("--delete", "-D", action="store_true", dest="delete", default=False,
+                                 help="delete the alert status history")
 
-        self.__parser.add_option("--org-admin", "-o", type="int", action="store", dest="org_admin",
-                                 help="the organisation administrator status")
+        # filters...
+        self.__parser.add_option("--latest", "-l", action="store_true", dest="latest", default=False,
+                                 help="find latest status report only")
 
-        self.__parser.add_option("--device-admin", "-d", type="int", action="store", dest="device_admin",
-                                 help="the device administrator status")
+        self.__parser.add_option("--history", "-d", action="store_true", dest="history", default=False,
+                                 help="find history of status reports")
 
-        self.__parser.add_option("--suspended", "-s", type="int", action="store", dest="suspended",
-                                 help="the suspended status")
+        self.__parser.add_option("--cause", "-a", type="string", action="store", dest="cause",
+                                 help="filter history by cause { %s }" % causes)
 
         # output...
         self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
                                  help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        count = 0
-
-        if self.find:
-            count += 1
-
-        if self.retrieve:
-            count += 1
-
-        if self.create:
-            count += 1
-
-        if self.update:
-            count += 1
-
-        if self.delete:
-            count += 1
-
-        if count != 1:
+        if self.id is None:
             return False
 
-        if self.org_admin is not None and self.org_admin != 0 and self.org_admin != 1:
+        if self.find == self.delete:
             return False
 
-        if self.device_admin is not None and self.device_admin != 0 and self.device_admin != 1:
+        if self.find and self.latest == self.history:
             return False
 
-        if self.suspended is not None and self.suspended != 0 and self.suspended != 1:
+        if not self.find and (self.latest or self.history):
             return False
 
-        if self.find and bool(self.email) and bool(self.org_label):
+        if self.latest and self.__opts.cause is not None:
             return False
 
-        if (self.retrieve or self.create or self.update or self.delete) and \
-                (self.email is None or self.org_label is None):
+        if self.__opts.cause is not None and self.__opts.cause not in self.__CAUSES:
             return False
 
         return True
 
 
+    def response_mode(self):
+        return AlertStatusFindRequest.Mode.LATEST if self.latest else AlertStatusFindRequest.Mode.HISTORY
+
+
     # ----------------------------------------------------------------------------------------------------------------
+    # properties: identity...
 
     @property
     def credentials_name(self):
         return self.__opts.credentials_name
 
 
     @property
-    def find(self):
-        return self.__opts.find
-
-
-    @property
-    def retrieve(self):
-        return self.__opts.retrieve
-
+    def id(self):
+        return self.__args[0] if self.__args else None
 
-    @property
-    def create(self):
-        return self.__opts.create
 
+    # ----------------------------------------------------------------------------------------------------------------
+    # properties: operations...
 
     @property
-    def update(self):
-        return self.__opts.update
+    def find(self):
+        return self.__opts.find
 
 
     @property
     def delete(self):
         return self.__opts.delete
 
 
-    @property
-    def email(self):
-        return self.__opts.email
-
+    # ----------------------------------------------------------------------------------------------------------------
+    # properties: filters...
 
     @property
-    def org_label(self):
-        return self.__opts.org_label
+    def latest(self):
+        return self.__opts.latest
 
 
     @property
-    def org_admin(self):
-        return self.__opts.org_admin
+    def history(self):
+        return self.__opts.history
 
 
     @property
-    def device_admin(self):
-        return self.__opts.device_admin
-
+    def cause(self):
+        return None if self.__opts.cause is None else self.__CAUSES[self.__opts.cause]
 
-    @property
-    def suspended(self):
-        return self.__opts.suspended
 
+    # ----------------------------------------------------------------------------------------------------------------
+    # properties: output...
 
     @property
     def indent(self):
         return self.__opts.indent
 
 
     @property
@@ -182,13 +147,11 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdOrganisationUsers:{credentials_name:%s, find:%s, create:%s, update:%s, delete:%s, " \
-               "email:%s, org_label:%s, org_admin:%s, device_admin:%s, suspended:%s, " \
+        return "CmdAlertStatus:{credentials_name:%s, id:%s, find:%s, delete:%s, latest:%s, history:%s, cause:%s, " \
                "indent:%s, verbose:%s}" % \
-               (self.credentials_name, self.find, self.create, self.update, self.delete,
-                self.email, self.org_label, self.__opts.org_admin, self.__opts.device_admin, self.__opts.suspended,
+               (self.credentials_name, self.id, self.find, self.delete, self.latest, self.history, self.__opts.cause,
                 self.indent, self.verbose)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_organisations.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_configuration_csv.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,158 +1,173 @@
 """
-Created on 10 Jan 2022
+Created on 7 Jul 2021
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 """
 
 import optparse
 
+from scs_core.aws.manager.configuration_finder import ConfigurationRequest
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdOrganisations(object):
+class CmdConfigurationCSV(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog  [-c CREDENTIALS] { -F | "
-                                                    "-C -l LABEL -n LONG_NAME -u URL -o OWNER_EMAIL | "
-                                                    "-U LABEL [-l LABEL] [-n LONG_NAME] [-u URL] [-o OWNER_EMAIL] | "
-                                                    "-D LABEL } "
-                                                    "[-i INDENT] [-v]", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] { -n | -s | -l OUTPUT_CSV | "
+                                                    "{ -d | -f } [-o OUTPUT_CSV_DIR] } [-t DEVICE_TAG [-e]] "
+                                                    "[-v] [NODE_1..NODE_N]", version="%prog 1.0")
 
         # identity...
         self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
                                  help="the stored credentials to be presented")
 
-        # operations...
-        self.__parser.add_option("--Find", "-F", action="store_true", dest="find", default=False,
-                                 help="find the organisations I belong to")
-
-        self.__parser.add_option("--Create", "-C", action="store_true", dest="create", default=False,
-                                 help="create an organisation")
+        # help...
+        self.__parser.add_option("--node-names", "-n", action="store_true", dest="node_names", default=False,
+                                 help="list the available nodes")
 
-        self.__parser.add_option("--Update", "-U", type="string", action="store", dest="update",
-                                 help="update the organisation with the given LABEL")
+        # mode...
+        self.__parser.add_option("--separate", "-s", action="store_true", dest="separate", default=False,
+                                 help="retrieve latest configurations to separate CSVs (ignores NODEs)")
 
-        self.__parser.add_option("--Delete", "-D", type="string", action="store", dest="delete",
-                                 help="delete the organisation")
+        self.__parser.add_option("--latest", "-l", type="string", action="store", dest="latest",
+                                 help="retrieve latest configurations to single CSV")
 
-        # fields...
-        self.__parser.add_option("--label", "-l", type="string", action="store", dest="label",
-                                 help="the organisation label")
+        self.__parser.add_option("--diff-histories", "-d", action="store_true", dest="diff_histories", default=False,
+                                 help="retrieve configuration history differences")
 
-        self.__parser.add_option("--long-name", "-n", type="string", action="store", dest="long_name",
-                                 help="the organisation long name")
+        self.__parser.add_option("--full-histories", "-f", action="store_true", dest="full_histories", default=False,
+                                 help="retrieve full configuration histories")
 
-        self.__parser.add_option("--url", "-u", type="string", action="store", dest="url",
-                                 help="the organisation URL")
+        # filter...
+        self.__parser.add_option("--device-tag", "-t", type="string", action="store", dest="device_tag",
+                                 help="the device for the history report")
 
-        self.__parser.add_option("--owner", "-o", type="string", action="store", dest="owner",
-                                 help="the organisation owner email")
+        self.__parser.add_option("--exactly", "-e", action="store_true", dest="exact_match", default=False,
+                                 help="exact match for tag")
 
         # output...
-        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
-                                 help="pretty-print the output with INDENT")
+        self.__parser.add_option("--output-csv-dir", "-o", type="string", action="store", dest="output_csv_dir",
+                                 help="the directory in which to write histories")
 
+        # narrative...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
         count = 0
 
-        if self.find:
+        if self.node_names:
+            count += 1
+
+        if self.separate:
             count += 1
 
-        if self.create:
+        if self.latest:
             count += 1
 
-        if self.update is not None:
+        if self.diff_histories:
             count += 1
 
-        if self.delete is not None:
+        if self.full_histories:
             count += 1
 
         if count != 1:
             return False
 
-        if self.create and (self.label is None or self.long_name is None or self.url is None or self.owner is None):
+        if self.device_tag is None and self.exact_match:
             return False
 
         return True
 
 
+    def request_mode(self):
+        if self.separate or self.latest:
+            return ConfigurationRequest.Mode.LATEST
+
+        if self.diff_histories:
+            return ConfigurationRequest.Mode.DIFF
+
+        if self.full_histories:
+            return ConfigurationRequest.Mode.HISTORY
+
+        return None
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
     def credentials_name(self):
         return self.__opts.credentials_name
 
 
     @property
-    def find(self):
-        return self.__opts.find
+    def node_names(self):
+        return self.__opts.node_names
 
 
     @property
-    def create(self):
-        return self.__opts.create
+    def separate(self):
+        return self.__opts.separate
 
 
     @property
-    def update(self):
-        return self.__opts.update
+    def latest(self):
+        return self.__opts.latest
 
 
     @property
-    def delete(self):
-        return self.__opts.delete
+    def diff_histories(self):
+        return self.__opts.diff_histories
 
 
     @property
-    def label(self):
-        return self.__opts.label
+    def full_histories(self):
+        return self.__opts.full_histories
 
 
     @property
-    def long_name(self):
-        return self.__opts.long_name
+    def device_tag(self):
+        return self.__opts.device_tag
 
 
     @property
-    def url(self):
-        return self.__opts.url
+    def exact_match(self):
+        return self.__opts.exact_match
 
 
     @property
-    def owner(self):
-        return self.__opts.owner
+    def output_csv_dir(self):
+        return self.__opts.output_csv_dir
 
 
     @property
-    def indent(self):
-        return self.__opts.indent
+    def verbose(self):
+        return self.__opts.verbose
 
 
     @property
-    def verbose(self):
-        return self.__opts.verbose
+    def nodes(self):
+        return self.__args
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdOrganisations:{credentials_name:%s, find:%s, create:%s, update:%s, delete:%s, " \
-               "label:%s, long_name:%s, url:%s, owner:%s, indent:%s, verbose:%s}" % \
-               (self.credentials_name, self.find, self.create, self.update, self.delete,
-                self.label, self.long_name, self.url, self.owner, self.indent, self.verbose)
+        return "CmdConfigurationCSV:{credentials_name:%s, node_names:%s, separate:%s, latest:%s, diff_histories:%s, " \
+               "full_histories:%s, device_tag:%s, exact_match:%s, output_csv_dir:%s, verbose:%s, nodes:%s}" %  \
+               (self.credentials_name, self.node_names, self.separate, self.latest, self.diff_histories,
+                self.full_histories, self.device_tag, self.exact_match, self.output_csv_dir, self.verbose, self.nodes)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_osio_api_auth.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_socket_receiver.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,48 @@
 """
-Created on 18 Feb 2017
+Created on 13 Jul 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
-
-example document:
-{"org-id": "south-coast-science-test-user", "api-key": "9fdfb841-3433-45b8-b223-3f5a283ceb8e"}
 """
 
 import optparse
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdOSIOAPIAuth(object):
+class CmdSocketReceiver(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-s ORG_ID API_KEY] [-v]", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [-p PORT] [-v]", version="%prog 1.0")
 
         # optional...
-        self.__parser.add_option("--set", "-s", type="string", nargs=2, action="store", dest="org_key",
-                                 help="set org ID and API key")
+        self.__parser.add_option("--port", "-p", type="int", nargs=1, action="store", default=2000, dest="port",
+                                 help="socket port (default 2000)")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def set(self):
-        return self.__opts.org_key is not None
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    @property
-    def org_id(self):
-        return None if self.__opts.org_key is None else self.__opts.org_key[0]
-
-
     @property
-    def api_key(self):
-        return None if self.__opts.org_key is None else self.__opts.org_key[1]
+    def port(self):
+        return self.__opts.port
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def __str__(self, *args, **kwargs):
-        return "CmdOSIOAPIAuth:{org_id:%s, api_key:%s, verbose:%s}" % (self.org_id, self.api_key, self.verbose)
+        return "CmdSocketReceiver:{port:%d, verbose:%s}" % (self.port, self.verbose)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_osio_client_auth.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_interval.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,79 +1,59 @@
 """
-Created on 19 Feb 2017
+Created on 16 Mar 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdOSIOClientAuth(object):
+class CmdSampleInterval(object):
     """
     unix command line handler
     """
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-u USER_ID] [-d DESCRIPTION] [-v]", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [-p PRECISION] [-v] [PATH]", version="%prog 1.0")
 
         # optional...
-        self.__parser.add_option("--user", "-u", type="string", nargs=1, action="store", dest="user_id",
-                                 help="set user-id (only if device has not yet been registered)")
-
-        self.__parser.add_option("--desc", "-d", type="string", nargs=1, action="store", dest="description",
-                                 help="set optional device description")
+        self.__parser.add_option("--prec", "-p", type="int", nargs=1, action="store", default=3, dest="precision",
+                                 help="precision (default 3 decimal places)")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def is_complete(self):
-        if self.user_id is None:
-            return False
-
-        return True
-
-
-    def set(self):
-        if self.__opts.user_id is None and self.__opts.description is None:
-            return False
-
-        return True
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
     @property
-    def user_id(self):
-        return self.__opts.user_id
+    def precision(self):
+        return self.__opts.precision
 
 
     @property
-    def description(self):
-        return self.__opts.description
+    def verbose(self):
+        return self.__opts.verbose
 
 
     @property
-    def verbose(self):
-        return self.__opts.verbose
+    def path(self):
+        return self.__args[0] if len(self.__args) > 0 else None
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdOSIOClientAuth:{user_id:%s, description:%s, verbose:%s}" % \
-               (self.user_id, self.description, self.verbose)
+        return "CmdSampleInterval:{precision:%s, verbose:%s, path:%s}" % (self.precision, self.verbose, self.path)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_osio_topic.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_uds.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
-Created on 17 Nov 2016
+Created on 25 Apr 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdOSIOTopic(object):
+class CmdUDS(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-v] PATH", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [-v] UDS_SUB", version="%prog 1.0")
 
         # optional...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
@@ -35,24 +35,24 @@
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def verbose(self):
-        return self.__opts.verbose
+    def path(self):
+        return self.__args[0] if len(self.__args) > 0 else None
 
 
     @property
-    def path(self):
-        return self.__args[0] if len(self.__args) > 0 else None
+    def verbose(self):
+        return self.__opts.verbose
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdOSIOTopic:{verbose:%s, path:%s}" % (self.verbose, self.path)
+        return "CmdUDS:{verbose:%s}" % self.verbose
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_osio_topic_publisher.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_sort.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,58 @@
 """
-Created on 19 Nov 2016
+Created on 19 Sep 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
-
-https://opensensorsio.helpscoutdocs.com/article/84-overriding-timestamp-information-in-message-payload
 """
 
 import optparse
 
-from scs_core.osio.config.project import Project
-
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdOSIOTopicPublisher(object):
+class CmdSampleSort(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog { -t TOPIC | -c { C | G | P | S | X } } [-o] [-v]",
-                                              version="%prog 1.0")
-
-        # compulsory...
-        self.__parser.add_option("--topic", "-t", type="string", nargs=1, action="store", dest="topic",
-                                 help="topic path")
-
-        self.__parser.add_option("--channel", "-c", type="string", nargs=1, action="store", dest="channel",
-                                 help="publication channel")
-
-        # optional...
-        self.__parser.add_option("--override", "-o", action="store_true", dest="override", default=False,
-                                 help="override OSIO reception datetime")
+        self.__parser = optparse.OptionParser(usage="%prog [-v] SORT_PATH_1 .. SORT_PATH_N", version="%prog 1.0")
 
+        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if bool(self.topic) == bool(self.channel):
-            return False
-
-        if self.channel and not Project.is_valid_channel(self.channel):
+        if len(self.__args) < 1:
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def topic(self):
-        return self.__opts.topic
-
-
-    @property
-    def channel(self):
-        return self.__opts.channel
-
-
-    @property
-    def override(self):
-        return self.__opts.override
+    def verbose(self):
+        return self.__opts.verbose
 
 
     @property
-    def verbose(self):
-        return self.__opts.verbose
+    def sort_paths(self):
+        return self.__args
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdOSIOTopicPublisher:{topic:%s, channel:%s, override:%s, verbose:%s}" % \
-                    (self.topic, self.channel, self.override, self.verbose)
+        return "CmdSampleSort:{verbose:%s, sort_paths:%s}" % (self.verbose, self.sort_paths)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_aggregate.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_aggregate.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_collator.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_concentration.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_concentration.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_distance.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_nullify.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,91 @@
 """
-Created on 11 Jul 2016
+Created on 4 Sep 2019
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSampleDistance(object):
+class CmdSampleNullify(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog -p LAT LNG [-i ISO] [-q QUALITY] [-v] GPS_PATH",
-                                              version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog -t TARGET_PATH -s SOURCE_PATH [-l LOWER] [-u UPPER]"
+                                                    " [-v]", version="%prog 1.0")
 
         # compulsory...
-        self.__parser.add_option("--position", "-p", type="float", nargs=2, action="store", dest="position",
-                                 help="position (in degrees)")
+        self.__parser.add_option("--target", "-t", type="string", nargs=1, action="store", dest="target",
+                                 help="field to be nullified")
+
+        self.__parser.add_option("--source", "-s", type="string", nargs=1, action="store", dest="source",
+                                 help="field providing the test value")
 
         # optional...
-        self.__parser.add_option("--iso-path", "-i", type="string", nargs=1, action="store", default="rec", dest="iso",
-                                 help="path for ISO 8601 datetime output (default 'rec')")
+        self.__parser.add_option("--lower", "-l", type="float", nargs=1, action="store", dest="lower",
+                                 help="lower bound")
 
-        self.__parser.add_option("--quality", "-q", type="int", nargs=1, action="store", dest="quality",
-                                 help="minimum acceptable GPS quality")
+        self.__parser.add_option("--upper", "-u", type="float", nargs=1, action="store", dest="upper",
+                                 help="upper bound")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.position is None or self.path is None:
+        if self.target is None or self.source is None:
+            return False
+
+        if self.lower is not None and self.upper is not None and self.upper <= self.lower:
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def position(self):
-        return self.__opts.position
+    def target(self):
+        return self.__opts.target
 
 
     @property
-    def lat(self):
-        return None if self.__opts.position is None else self.__opts.position[0]
+    def source(self):
+        return self.__opts.source
 
 
     @property
-    def lng(self):
-        return None if self.__opts.position is None else self.__opts.position[1]
+    def lower(self):
+        return self.__opts.lower
 
 
     @property
-    def iso(self):
-        return self.__opts.iso
-
-
-    @property
-    def quality(self):
-        return self.__opts.quality
+    def upper(self):
+        return self.__opts.upper
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
-    @property
-    def path(self):
-        return self.__args[0] if len(self.__args) > 0 else None
-
-
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdSampleDistance:{position:%s, iso:%s, quality:%s, verbose:%s, path:%s}" % \
-               (self.position, self.iso, self.quality, self.verbose, self.path)
+        return "CmdSampleNullify:{target:%s, source:%s, lower:%s, upper:%s, verbose:%s}" % \
+               (self.target, self.source, self.lower, self.upper, self.verbose)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_duplicates.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_duplicates.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_error.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_error.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_filter.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_filter.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_interval.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_record.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 """
-Created on 16 Mar 2017
+Created on 11 Jul 2016
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSampleInterval(object):
-    """
-    unix command line handler
-    """
+class CmdSampleRecord(object):
+    """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-p PRECISION] [-v] [PATH]", version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog [-v] [PATH]", version="%prog 1.0")
 
         # optional...
-        self.__parser.add_option("--prec", "-p", type="int", nargs=1, action="store", default=3, dest="precision",
-                                 help="precision (default 3 decimal places)")
-
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    @property
-    def precision(self):
-        return self.__opts.precision
+    def is_valid(self):
+        if self.path is None:
+            return False
+
+        return True
 
 
+    # ----------------------------------------------------------------------------------------------------------------
+
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
     @property
     def path(self):
@@ -52,8 +51,8 @@
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdSampleInterval:{precision:%s, verbose:%s, path:%s}" % (self.precision, self.verbose, self.path)
+        return "CmdSampleRecord:{verbose:%s, path:%s}" % (self.verbose, self.path)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_iso_8601.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_iso_8601.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_low_pass.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_low_pass.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_median.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_median.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_nullify.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_tally.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,91 +1,75 @@
 """
-Created on 4 Sep 2019
+Created on 22 Aug 2017
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSampleNullify(object):
+class CmdSampleTally(object):
     """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog -t TARGET_PATH -s SOURCE_PATH [-l LOWER] [-u UPPER]"
-                                                    " [-v]", version="%prog 1.0")
-
-        # compulsory...
-        self.__parser.add_option("--target", "-t", type="string", nargs=1, action="store", dest="target",
-                                 help="field to be nullified")
-
-        self.__parser.add_option("--source", "-s", type="string", nargs=1, action="store", dest="source",
-                                 help="field providing the test value")
+        self.__parser = optparse.OptionParser(usage="%prog [-t TALLY] [-p PRECISION] [-v] [PATH]", version="%prog 1.0")
 
         # optional...
-        self.__parser.add_option("--lower", "-l", type="float", nargs=1, action="store", dest="lower",
-                                 help="lower bound")
+        self.__parser.add_option("--tally", "-t", type="int", nargs=1, action="store", dest="tally",
+                                 help="generate a rolling aggregate for TALLY number of data points (default all)")
 
-        self.__parser.add_option("--upper", "-u", type="float", nargs=1, action="store", dest="upper",
-                                 help="upper bound")
+        self.__parser.add_option("--prec", "-p", type="int", nargs=1, action="store", default=None, dest="precision",
+                                 help="precision (default 0 decimal places)")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.target is None or self.source is None:
-            return False
-
-        if self.lower is not None and self.upper is not None and self.upper <= self.lower:
+        if self.tally is not None and self.tally < 1:
             return False
 
         return True
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def target(self):
-        return self.__opts.target
+    def tally(self):
+        return self.__opts.tally
 
 
     @property
-    def source(self):
-        return self.__opts.source
+    def precision(self):
+        return self.__opts.precision
 
 
     @property
-    def lower(self):
-        return self.__opts.lower
-
-
-    @property
-    def upper(self):
-        return self.__opts.upper
+    def verbose(self):
+        return self.__opts.verbose
 
 
     @property
-    def verbose(self):
-        return self.__opts.verbose
+    def path(self):
+        return self.__args[0] if len(self.__args) > 0 else None
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdSampleNullify:{target:%s, source:%s, lower:%s, upper:%s, verbose:%s}" % \
-               (self.target, self.source, self.lower, self.upper, self.verbose)
+        return "CmdSampleTally:{tally:%s, precision:%s, verbose:%s, path:%s}" % \
+                    (self.tally, self.precision, self.verbose, self.path)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_paths.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_record.py` & `scs-analysis-2.7.2/src/scs_analysis/handler/mqtt_reporter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,45 @@
 """
-Created on 11 Jul 2016
+Created on 6 Jul 2018
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
-import optparse
+import sys
+
+from scs_core.data.datetime import LocalizedDatetime
 
 
 # --------------------------------------------------------------------------------------------------------------------
+# reporter...
+
+class MQTTReporter(object):
+    """
+    classdocs
+    """
 
-class CmdSampleRecord(object):
-    """unix command line handler"""
+    # ----------------------------------------------------------------------------------------------------------------
 
-    def __init__(self):
+    def __init__(self, verbose):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-v] [PATH]", version="%prog 1.0")
-
-        # optional...
-        self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
-                                 help="report narrative to stderr")
-
-        self.__opts, self.__args = self.__parser.parse_args()
-
-
-    # ----------------------------------------------------------------------------------------------------------------
-
-    def is_valid(self):
-        if self.path is None:
-            return False
-
-        return True
+        self.__verbose = verbose
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    @property
-    def verbose(self):
-        return self.__opts.verbose
-
-
-    @property
-    def path(self):
-        return self.__args[0] if len(self.__args) > 0 else None
+    def print(self, status):
+        if not self.__verbose:
+            return
+
+        now = LocalizedDatetime.now().utc()
+        print("%s:         mqtt: %s" % (now.as_time(), status), file=sys.stderr)
+        sys.stderr.flush()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def print_help(self, file):
-        self.__parser.print_help(file)
-
-
     def __str__(self, *args, **kwargs):
-        return "CmdSampleRecord:{verbose:%s, path:%s}" % (self.verbose, self.path)
+        return "MQTTReporter:{verbose:%s}" % self.__verbose
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_slope.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_device_controller.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,126 +1,115 @@
 """
-Created on 23 Oct 2020
+Created on 17 Apr 2023
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
-from scs_core.data.timedelta import Timedelta
-
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSampleSlope(object):
-    """unix command line handler"""
+class CmdDeviceController(object):
+    """unix message line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog -n NAME [-i ISO] [-t TALLY] [-m [DD-]HH:MM[:SS]] [-x] "
-                                                    "[-p PRECISION] [-v] PATH", version="%prog 1.0")
-
-        # compulsory...
-        self.__parser.add_option("--name", "-n", type="string", nargs=1, action="store", dest="name",
-                                 help="slope field name (i.e. '1min')")
-
-        # optional...
-        self.__parser.add_option("--iso-path", "-i", type="string", nargs=1, action="store", default="rec", dest="iso",
-                                 help="path for ISO 8601 datetime field (default 'rec')")
+        self.__parser = optparse.OptionParser(usage="%prog [-c CREDENTIALS] -t DEVICE_TAG "
+                                                    "[-m CMD_TOKENS [{ [-w] [-i INDENT] | -s }]] [-v]",
+                                              version="%prog 1.0")
+
+        # identity...
+        self.__parser.add_option("--credentials", "-c", type="string", action="store", dest="credentials_name",
+                                 help="the stored credentials to be presented")
+
+        # target...
+        self.__parser.add_option("--device-tag", "-t", type="string", action="store", dest="device_tag",
+                                 help="the device tag")
+
+        # mode...
+        self.__parser.add_option("--message", "-m", type="string", nargs=1, action="store", dest="message",
+                                 help="send the given command line string")
+
+        # output...
+        self.__parser.add_option("--wrapper", "-w", action="store_true", dest="wrapper", default=False,
+                                 help="report message wrapper")
 
-        self.__parser.add_option("--tally", "-t", type="int", nargs=1, action="store", default=2, dest="tally",
-                                 help="compute for rolling TALLY number of data points (default 2)")
+        self.__parser.add_option("--std", "-s", action="store_true", dest="std", default=False,
+                                 help="write to stderr and stdout")
 
-        self.__parser.add_option("--max-interval", "-m", type="string", nargs=1, action="store", dest="max_interval",
-                                 help="restart regression on long intervals")
-
-        self.__parser.add_option("--exclude-incomplete", "-x", action="store_true", dest="exclude_incomplete",
-                                 default=False, help="exclude incomplete tallies")
-
-        self.__parser.add_option("--prec", "-p", type="int", nargs=1, action="store", default=6, dest="precision",
-                                 help="precision (default 6 decimal places)")
+        self.__parser.add_option("--indent", "-i", type="int", nargs=1, action="store", dest="indent",
+                                 help="pretty-print the output with INDENT")
 
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.name is None:
+        if self.message is not None and len(self.message) < 1:
             return False
 
-        if self.tally < 1:
+        if self.std and (self.indent is not None or self.wrapper):
             return False
 
-        if self.path is None:
+        if (self.wrapper or self.indent or self.std) and not self.message:
             return False
 
         return True
 
 
-    def is_valid_interval(self):
-        if self.__opts.max_interval is None:
-            return True
-
-        return self.max_interval is not None
-
-
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def name(self):
-        return self.__opts.name
+    def credentials_name(self):
+        return self.__opts.credentials_name
 
 
     @property
-    def iso(self):
-        return self.__opts.iso
+    def device_tag(self):
+        return self.__opts.device_tag
 
 
     @property
-    def tally(self):
-        return self.__opts.tally
+    def message(self):
+        return self.__opts.message
 
 
     @property
-    def max_interval(self):
-        return Timedelta.construct_from_flag(self.__opts.max_interval)
+    def wrapper(self):
+        return self.__opts.wrapper
 
 
     @property
-    def exclude_incomplete(self):
-        return self.__opts.exclude_incomplete
+    def std(self):
+        return self.__opts.std
 
 
     @property
-    def precision(self):
-        return self.__opts.precision
+    def indent(self):
+        return self.__opts.indent
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
-    @property
-    def path(self):
-        return self.__args[0] if len(self.__args) > 0 else None
-
-
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdSampleSlope:{name:%s, iso:%s, tally:%s, exclude_incomplete:%s, precision:%s, verbose:%s, " \
-               "path:%s}" % \
-               (self.name, self.iso, self.tally, self.exclude_incomplete, self.precision, self.verbose,
-                self.path)
+        return "CmdDeviceController:{credentials_name:%s, device_tag:%s, message:%s, wrapper:%s, std:%s, " \
+               "indent:%s, verbose:%s}" % \
+               (self.credentials_name, self.device_tag, self.message, self.wrapper, self.std,
+                self.indent, self.verbose)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_stats.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_stats.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_subset.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_subset.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_tally.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_time_shift.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,75 +1,91 @@
 """
-Created on 22 Aug 2017
+Created on 3 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
+from scs_core.data.timedelta import Timedelta
+
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSampleTally(object):
-    """unix command line handler"""
+class CmdSampleTimeShift(object):
+    """
+    unix command line handler
+    """
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog [-t TALLY] [-p PRECISION] [-v] [PATH]", version="%prog 1.0")
-
-        # optional...
-        self.__parser.add_option("--tally", "-t", type="int", nargs=1, action="store", dest="tally",
-                                 help="generate a rolling aggregate for TALLY number of data points (default all)")
+        self.__parser = optparse.OptionParser(usage="%prog -t { + | - } [[DD-]HH:]MM[:SS] [-v] [PATH]",
+                                              version="%prog 1.0")
 
-        self.__parser.add_option("--prec", "-p", type="int", nargs=1, action="store", default=None, dest="precision",
-                                 help="precision (default 0 decimal places)")
+        # functions...
+        self.__parser.add_option("--timedelta", "-t", type="string", nargs=2, action="store", dest="timedelta",
+                                 help="sign and offset in days / hours / minutes / seconds")
 
+        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.tally is not None and self.tally < 1:
+        if self.__opts.timedelta is None:
+            return False
+
+        if self.__opts.timedelta[0] != '+' and self.__opts.timedelta[0] != '-':
+            return False
+
+        if self.timedelta is None:
             return False
 
         return True
 
 
+    def is_valid_timedelta(self):
+        if self.__opts.timedelta is None:
+            return True
+
+        return self.timedelta is not None
+
+
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def tally(self):
-        return self.__opts.tally
+    def positive(self):
+        return None if self.__opts.timedelta is None else self.__opts.timedelta[0] == '+'
 
 
     @property
-    def precision(self):
-        return self.__opts.precision
+    def timedelta(self):
+        return Timedelta.construct_from_flag(self.__opts.timedelta[1])
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
     @property
     def path(self):
-        return self.__args[0] if len(self.__args) > 0 else None
+        return self.__args[0] if len(self.__args) > 0 else 'rec'
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdSampleTally:{tally:%s, precision:%s, verbose:%s, path:%s}" % \
-                    (self.tally, self.precision, self.verbose, self.path)
+        return "CmdSampleTimeShift:{timedelta:%s, verbose:%s, path:%s}" % \
+               (self.__opts.timedelta, self.verbose, self.path)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_time_shift.py` & `scs-analysis-2.7.2/src/scs_analysis/cmd/cmd_sample_timezone.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,91 +1,78 @@
 """
-Created on 3 Jan 2022
+Created on 19 Nov 2018
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
 import optparse
 
-from scs_core.data.timedelta import Timedelta
-
 
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSampleTimeShift(object):
-    """
-    unix command line handler
-    """
+class CmdSampleTimezone(object):
+    """unix command line handler"""
 
     def __init__(self):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog -t { + | - } [[DD-]HH:]MM[:SS] [-v] [PATH]",
-                                              version="%prog 1.0")
+        self.__parser = optparse.OptionParser(usage="%prog { -z | [-i ISO_PATH] TIMEZONE_NAME }", version="%prog 1.0")
+
+        # optional...
+        self.__parser.add_option("--zones", "-z", action="store_true", dest="zones", default=False,
+                                 help="list the available timezone names to stderr")
 
-        # functions...
-        self.__parser.add_option("--timedelta", "-t", type="string", nargs=2, action="store", dest="timedelta",
-                                 help="sign and offset in days / hours / minutes / seconds")
+        self.__parser.add_option("--iso-path", "-i", type="string", nargs=1, action="store", default="rec", dest="iso",
+                                 help="path for ISO 8601 datetime output (default 'rec')")
 
-        # output...
         self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
                                  help="report narrative to stderr")
 
         self.__opts, self.__args = self.__parser.parse_args()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def is_valid(self):
-        if self.__opts.timedelta is None:
-            return False
-
-        if self.__opts.timedelta[0] != '+' and self.__opts.timedelta[0] != '-':
+        if bool(self.timezone) == bool(self.__opts.zones):
             return False
 
-        if self.timedelta is None:
+        if self.iso is not None and self.timezone is None:
             return False
 
         return True
 
 
-    def is_valid_timedelta(self):
-        if self.__opts.timedelta is None:
-            return True
-
-        return self.timedelta is not None
-
-
     # ----------------------------------------------------------------------------------------------------------------
 
     @property
-    def positive(self):
-        return None if self.__opts.timedelta is None else self.__opts.timedelta[0] == '+'
+    def zones(self):
+        return self.__opts.zones
 
 
     @property
-    def timedelta(self):
-        return Timedelta.construct_from_flag(self.__opts.timedelta[1])
+    def iso(self):
+        return self.__opts.iso
 
 
     @property
     def verbose(self):
         return self.__opts.verbose
 
 
     @property
-    def path(self):
-        return self.__args[0] if len(self.__args) > 0 else 'rec'
+    def timezone(self):
+        return self.__args[0] if len(self.__args) > 0 else None
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
     def print_help(self, file):
         self.__parser.print_help(file)
 
 
     def __str__(self, *args, **kwargs):
-        return "CmdSampleTimeShift:{timedelta:%s, verbose:%s, path:%s}" % \
-               (self.__opts.timedelta, self.verbose, self.path)
+        return "CmdSampleTimezone:{zones:%s, iso:%s, verbose:%s, timezone:%s}" % \
+               (self.zones, self.iso, self.verbose, self.timezone)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cmd/cmd_sample_timezone.py` & `scs-analysis-2.7.2/src/scs_analysis/handler/sample_regression.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,78 +1,74 @@
 """
-Created on 19 Nov 2018
+Created on 16 Mar 2020
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 """
 
-import optparse
+from scs_core.data.datetime import LocalizedDatetime
+from scs_core.data.linear_regression import LinearRegression
+from scs_core.data.path_dict import PathDict
 
 
+# TODO: use named input_path and response_pth
 # --------------------------------------------------------------------------------------------------------------------
 
-class CmdSampleTimezone(object):
-    """unix command line handler"""
+class SampleRegression(object):
+    """
+    classdocs
+    """
 
-    def __init__(self):
+    # ----------------------------------------------------------------------------------------------------------------
+
+    def __init__(self, path, tally, precision):
         """
         Constructor
         """
-        self.__parser = optparse.OptionParser(usage="%prog { -z | [-i ISO_PATH] TIMEZONE_NAME }", version="%prog 1.0")
-
-        # optional...
-        self.__parser.add_option("--zones", "-z", action="store_true", dest="zones", default=False,
-                                 help="list the available timezone names to stderr")
-
-        self.__parser.add_option("--iso-path", "-i", type="string", nargs=1, action="store", default="rec", dest="iso",
-                                 help="path for ISO 8601 datetime output (default 'rec')")
-
-        self.__parser.add_option("--verbose", "-v", action="store_true", dest="verbose", default=False,
-                                 help="report narrative to stderr")
+        self.__path = path
+        self.__precision = precision
 
-        self.__opts, self.__args = self.__parser.parse_args()
+        self.__func = LinearRegression(tally=tally)
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def is_valid(self):
-        if bool(self.timezone) == bool(self.__opts.zones):
-            return False
+    def datum(self, sample):
+        if not sample.has_path(self.__path):
+            return None
 
-        if self.iso is not None and self.timezone is None:
-            return False
+        try:
+            rec_node = sample.node('rec')
+        except KeyError:
+            return None
 
-        return True
+        rec = LocalizedDatetime.construct_from_jdict(rec_node)
+        value = sample.node(self.__path)
 
+        self.__func.append(rec, value)
 
-    # ----------------------------------------------------------------------------------------------------------------
-
-    @property
-    def zones(self):
-        return self.__opts.zones
-
+        if not self.__func.has_regression():
+            return None
 
-    @property
-    def iso(self):
-        return self.__opts.iso
+        slope, intercept = self.__func.line()
 
+        if slope is None:
+            return None
 
-    @property
-    def verbose(self):
-        return self.__opts.verbose
+        target = PathDict()
 
+        for path in sample.paths():
+            if path == self.__path:
+                target.append(self.__path + '.src', value)
+                target.append(self.__path + '.slope', round(slope, self.__precision))
+                target.append(self.__path + '.intercept', round(intercept, self.__precision))
+            else:
+                target.copy(sample, path)
 
-    @property
-    def timezone(self):
-        return self.__args[0] if len(self.__args) > 0 else None
+        return target.node()
 
 
     # ----------------------------------------------------------------------------------------------------------------
 
-    def print_help(self, file):
-        self.__parser.print_help(file)
-
-
     def __str__(self, *args, **kwargs):
-        return "CmdSampleTimezone:{zones:%s, iso:%s, verbose:%s, timezone:%s}" % \
-               (self.zones, self.iso, self.verbose, self.timezone)
+        return "SampleRegression:{path:%s, func:%s}" % (self.__path, self.__func)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cognito_devices.py` & `scs-analysis-2.7.2/src/scs_analysis/cognito_devices.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 Created on 24 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The cognito_users utility is used to create, update and retrieve AWS Cognito identities. This utility can only be used
+The cognito_devices utility is used to create, update and retrieve AWS Cognito identities. This utility can only be used
 by organisation administrators and superusers.
 
 If the --Create function is used, an email is sent to the new user. The verification link in the email must be
 excercised in order for the account to gain a CONFIRMED status.
 
 SYNOPSIS
 cognito_devices.py  [-c CREDENTIALS] { -F [-t TAG] [-m] | -C TAG SHARED_SECRET | -U TAG SHARED_SECRET | -D TAG } \
 [-i INDENT] [-v]
 
 EXAMPLES
 cognito_devices.py -vi4 -c super -F -m
 
 DOCUMENT EXAMPLE
-{"username": "scs-ph1-28", "created": "2023-04-04T09:08:55Z", "last-updated": "2023-04-04T09:08:56Z"}
+{"username": "scs-bgx-401", "invoice": "INV-000123",
+"created": "2023-06-23T10:32:52+01:00", "last-updated": "2023-06-23T10:32:52+01:00"}
 
 SEE ALSO
 scs_analysis/cognito_credentials
 scs_analysis/cognito_users
 scs_analysis/organisation_devices
 
 RESOURCES
@@ -41,32 +42,31 @@
 
 from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_device import CognitoDeviceIdentity
 from scs_core.aws.security.cognito_device_finder import CognitoDeviceFinder
 from scs_core.aws.security.cognito_device_manager import CognitoDeviceManager
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
 from scs_core.aws.security.cognito_membership import CognitoMembership
-
 from scs_core.aws.security.organisation_manager import OrganisationManager
 
+from scs_core.client.http_exception import HTTPException, HTTPConflictException
+
 from scs_core.data.json import JSONify
 
-from scs_core.sys.http_exception import HTTPConflictException
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     logger = None
     credentials = None
-    auth = None
     finder = None
     report = None
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # cmd...
 
@@ -79,90 +79,66 @@
         Logging.config('cognito_devices', verbose=cmd.verbose)
         logger = Logging.getLogger()
 
         logger.info(cmd)
 
 
         # ------------------------------------------------------------------------------------------------------------
-        # auth...
+        # authentication...
 
-        gatekeeper = CognitoLoginManager(requests)
+        credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
 
-        # CognitoUserCredentials...
-        if not CognitoClientCredentials.exists(Host, name=cmd.credentials_name):
-            logger.error("Cognito credentials not available.")
-            exit(1)
-
-        try:
-            password = CognitoClientCredentials.password_from_user()
-            credentials = CognitoClientCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
-        except (KeyError, ValueError):
-            logger.error("incorrect password.")
+        if not credentials:
             exit(1)
 
+        gatekeeper = CognitoLoginManager(requests)
         auth = gatekeeper.user_login(credentials)
 
         if not auth.is_ok():
             logger.error("login: %s" % auth.authentication_status.description)
             exit(1)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # resources...
 
-        device_manager = CognitoDeviceManager(requests, auth.id_token)
+        device_manager = CognitoDeviceManager(requests)
         org_manager = OrganisationManager(requests)
 
         finder = CognitoDeviceFinder(requests)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
         if cmd.find:
             if cmd.tag is not None:
-                report = sorted(finder.find_by_tag(auth.id_token, cmd.tag))
+                report = sorted(finder.find_by_tag(auth.id_token, cmd.tag))   # TODO: Internal Server Error on null tag
 
             else:
                 report = sorted(finder.find_all(auth.id_token))
 
             if cmd.memberships:
                 org_devices = org_manager.find_devices(auth.id_token)
                 report = CognitoMembership.merge(report, org_devices)
 
-        if cmd.create:
-            if not CognitoDeviceIdentity.is_valid_password(cmd.create[1]):
-                logger.error("password must be at least 16 characters.")
-                exit(2)
-
-            # create...
-            identity = CognitoDeviceIdentity(cmd.create[0], cmd.create[1], None, None)
-
-            report = device_manager.create(identity)
-
         if cmd.update:
-            if not CognitoDeviceIdentity.is_valid_password(cmd.update[1]):
-                logger.error("password must be at least 16 characters.")
-                exit(2)
-
             # find...
-            device = finder.get_by_tag(auth.id_token, cmd.update[0])
+            device = finder.get_by_tag(auth.id_token, cmd.update_tag)
 
             if device is None:
                 logger.error("no device found for tag: '%s'." % cmd.update)
                 exit(1)
 
             # update...
-            report = CognitoDeviceIdentity(cmd.update[0], cmd.update[1], None, None)
-
-            auth = gatekeeper.user_login(credentials)                          # renew credentials
-            device_manager.update(report)
+            updated = CognitoDeviceIdentity(cmd.update_tag, None, cmd.update_invoice, None, None)
+            report = device_manager.update(auth.id_token, updated)
 
         if cmd.delete:
-            device_manager.delete(cmd.delete)
+            device_manager.delete(auth.id_token, cmd.delete)
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # end...
 
         if report is not None:
             print(JSONify.dumps(report, indent=cmd.indent))
@@ -172,7 +148,11 @@
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
     except HTTPConflictException as ex:
         logger.error("the tag '%s' is already in use." % report.tag)
         exit(1)
+
+    except HTTPException as ex:
+        logger.error(ex.error_report)
+        exit(1)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cognito_password.py` & `scs-analysis-2.7.2/src/scs_analysis/cognito_password.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,18 +36,19 @@
 from scs_analysis.cmd.cmd_cognito_password import CmdCognitoPassword
 
 from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager, AuthenticationStatus
 from scs_core.aws.security.cognito_password_manager import CognitoPasswordManager
 from scs_core.aws.security.cognito_user import CognitoUserIdentity
 
+from scs_core.client.http_exception import HTTPException, HTTPBadRequestException, HTTPUnauthorizedException, \
+    HTTPNotFoundException, HTTPNotAllowedException
+
 from scs_core.data.datum import Datum
 
-from scs_core.sys.http_exception import HTTPException, HTTPBadRequestException, HTTPUnauthorizedException, \
-    HTTPNotFoundException, HTTPNotAllowedException
 
 from scs_core.sys.logging import Logging
 
 from scs_host.comms.stdio import StdIO
 
 
 # --------------------------------------------------------------------------------------------------------------------
@@ -171,9 +172,9 @@
     # ----------------------------------------------------------------------------------------------------------------
     # end...
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
     except HTTPException as ex:
-        logger.error(repr(ex))
+        logger.error(ex.error_report)
         exit(1)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cognito_user_credentials.py` & `scs-analysis-2.7.2/src/scs_analysis/cognito_user_credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,18 +42,19 @@
 
 from scs_analysis.cmd.cmd_cognito_user_credentials import CmdCognitoUserCredentials
 
 from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
 from scs_core.aws.security.cognito_user import CognitoUserIdentity
 
+from scs_core.client.http_exception import HTTPException
+
 from scs_core.data.datum import Datum
 from scs_core.data.json import JSONify
 
-from scs_core.sys.http_exception import HTTPException
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
@@ -90,32 +91,32 @@
         logger.info(cmd)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
         if cmd.list:
-            for conf_name in CognitoClientCredentials.list(Host):
+            for conf_name in sorted(CognitoClientCredentials.list(Host)):
                 print(conf_name, file=sys.stderr)
             exit(0)
 
-        if cmd.set:
+        elif cmd.set:
             credentials = CognitoClientCredentials.from_user(cmd.credentials_name)
 
             if not Datum.is_email_address(credentials.email):
                 logger.error("The email address is not valid.")
                 exit(1)
 
             if not CognitoUserIdentity.is_valid_password(credentials.password):
                 logger.error("The password must include lower and upper case, numeric and punctuation characters.")
                 exit(1)
 
             credentials.save(Host, encryption_key=credentials.retrieval_password)
 
-        if cmd.update_password:
+        elif cmd.update_password:
             credentials = load_credentials(cmd.credentials_name)
 
             if credentials is None:
                 logger.error("credentials not found.")
                 exit(1)
 
             credentials = CognitoClientCredentials.from_user(cmd.credentials_name, existing_email=credentials.email)
@@ -159,9 +160,9 @@
         if credentials:
             print(JSONify.dumps(credentials, indent=cmd.is_valid()))
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
     except HTTPException as ex:
-        logger.error(ex.data)
+        logger.error(ex.error_report)
         exit(1)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cognito_user_identity.py` & `scs-analysis-2.7.2/src/scs_analysis/cognito_user_identity.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,19 @@
 
 from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
 from scs_core.aws.security.cognito_user import CognitoUserIdentity
 from scs_core.aws.security.cognito_user_finder import CognitoUserFinder
 from scs_core.aws.security.cognito_user_manager import CognitoUserCreator, CognitoUserEditor
 
+from scs_core.client.http_exception import HTTPException, HTTPConflictException
+
 from scs_core.data.datum import Datum
 from scs_core.data.json import JSONify
 
-from scs_core.sys.http_exception import HTTPConflictException
 from scs_core.sys.logging import Logging
 
 from scs_host.comms.stdio import StdIO
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
@@ -76,37 +77,30 @@
         Logging.config('cognito_user_identity', verbose=cmd.verbose)
         logger = Logging.getLogger()
 
         logger.info(cmd)
 
 
         # ------------------------------------------------------------------------------------------------------------
-        # auth...
+        # authentication...
 
         if not cmd.create:
-            gatekeeper = CognitoLoginManager(requests)
-
-            # CognitoUserCredentials...
-            if not CognitoClientCredentials.exists(Host, name=cmd.credentials_name):
-                logger.error("Cognito credentials not available.")
-                exit(1)
+            credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
 
-            try:
-                password = CognitoClientCredentials.password_from_user()
-                credentials = CognitoClientCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
-            except (KeyError, ValueError):
-                logger.error("incorrect password.")
+            if not credentials:
                 exit(1)
 
+            gatekeeper = CognitoLoginManager(requests)
             auth = gatekeeper.user_login(credentials)
 
             if not auth.is_ok():
                 logger.error("login: %s" % auth.authentication_status.description)
                 exit(1)
 
+
         # ------------------------------------------------------------------------------------------------------------
         # resources...
 
         if not cmd.create:
             finder = CognitoUserFinder(requests)
 
 
@@ -211,7 +205,11 @@
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
     except HTTPConflictException as ex:
         logger.error("the email address '%s' is already in use." % report.email)
         exit(1)
+
+    except HTTPException as ex:
+        logger.error(ex.error_report)
+        exit(1)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/cognito_users.py` & `scs-analysis-2.7.2/src/scs_analysis/organisation_users.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,221 +1,179 @@
 #!/usr/bin/env python3
 
 """
-Created on 24 Jan 2022
+Created on 18 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The cognito_users utility is used to create, update and retrieve AWS Cognito identities. This utility can only be used
-by organisation administrators and superusers.
-
-If the --Create function is used, an email is sent to the new user. The verification link in the email must be
-excercised in order for the account to gain a CONFIRMED status.
+The organisation_users utility is used to
 
 SYNOPSIS
-cognito_users.py  [-c CREDENTIALS] { -F [{ -e EMAIL_ADDR | -l ORG_LABEL | -c CONFIRMATION | -s { 1 | 0 } } }] | \
--C | -U -e EMAIL_ADDR | -D -e EMAIL_ADDR } [-i INDENT] [-v]
+organisation_users.py  [-c CREDENTIALS] { -F { -e EMAIL | -l ORG_LABEL } | \
+-R -e EMAIL -l ORG_LABEL | \
+-C -e EMAIL -l ORG_LABEL -o { 1 | 0 } -d { 1 | 0 } | \
+-U -e EMAIL -l ORG_LABEL [-o { 1 | 0 }] [-d { 1 | 0 }] [-s { 1 | 0 }] | \
+-D -e EMAIL -l ORG_LABEL } \
+[-i INDENT] [-v]
 
 EXAMPLES
-cognito_users.py -Fe bruno.beloff@southcoastscience.com
+organisation_users.py -F -l NARA
 
 DOCUMENT EXAMPLE
-{"username": "8", "creation-date": "2021-11-24T12:51:12Z", "confirmation-status": "CONFIRMED", "enabled": true,
-"email": "bruno.beloff@southcoastscience.com", "given-name": "Bruno", "family-name": "Beloff", "is-super": true}
+{"Username": 111, "OrgID": 1, "IsOrgAdmin": true, "IsDeviceAdmin": true, "IsSuspended": false}
 
 SEE ALSO
 scs_analysis/cognito_credentials
-scs_analysis/cognito_devices
-scs_analysis/organisation_users
-
-RESOURCES
-https://docs.aws.amazon.com/cognito/latest/developerguide/signing-up-users-in-your-app.html
-https://docs.aws.amazon.com/cognito/latest/developerguide/user-pool-settings-policies.html
+scs_analysis/cognito_users
 """
 
 import requests
 import sys
 
-from scs_analysis.cmd.cmd_cognito_users import CmdCognitoUsers
+from scs_analysis.cmd.cmd_organisation_users import CmdOrganisationUsers
 
 from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
-from scs_core.aws.security.cognito_membership import CognitoMembership
-from scs_core.aws.security.cognito_user import CognitoUserIdentity
 from scs_core.aws.security.cognito_user_finder import CognitoUserFinder
-from scs_core.aws.security.cognito_user_manager import CognitoUserCreator, CognitoUserEditor, CognitoUserDeleter
 
+from scs_core.aws.security.organisation import OrganisationUser
 from scs_core.aws.security.organisation_manager import OrganisationManager
 
+from scs_core.client.http_exception import HTTPException
+
 from scs_core.data.datum import Datum
 from scs_core.data.json import JSONify
 
-from scs_core.sys.http_exception import HTTPException, HTTPConflictException
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
-    cmd = None
     logger = None
-    gatekeeper = None
-    credentials = None
-    auth = None
-    finder = None
-    manager = None
+    cognito = None
     org = None
-    report = None
+    report = []
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # cmd...
 
-        cmd = CmdCognitoUsers()
+        cmd = CmdOrganisationUsers()
 
         if not cmd.is_valid():
             cmd.print_help(sys.stderr)
             exit(2)
 
-        Logging.config('cognito_users', verbose=cmd.verbose)
+        Logging.config('organisation_users', verbose=cmd.verbose)
         logger = Logging.getLogger()
 
         logger.info(cmd)
 
+        if cmd.email is not None and not Datum.is_email_address(cmd.email):
+            logger.error("email address '%s' is not valid." % cmd.email)
+            exit(2)
+
 
         # ------------------------------------------------------------------------------------------------------------
-        # auth...
+        # authentication...
 
-        if not cmd.create:
-            gatekeeper = CognitoLoginManager(requests)
+        credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
 
-            # CognitoUserCredentials...
-            if not CognitoClientCredentials.exists(Host, name=cmd.credentials_name):
-                logger.error("Cognito credentials not available.")
-                exit(1)
+        if not credentials:
+            exit(1)
 
-            try:
-                password = CognitoClientCredentials.password_from_user()
-                credentials = CognitoClientCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
-            except (KeyError, ValueError):
-                logger.error("incorrect password.")
-                exit(1)
+        gatekeeper = CognitoLoginManager(requests)
+        auth = gatekeeper.user_login(credentials)
 
-            auth = gatekeeper.user_login(credentials)
+        if not auth.is_ok():
+            logger.error("login: %s" % auth.authentication_status.description)
+            exit(1)
 
-            if not auth.is_ok():
-                logger.error("login: %s" % auth.authentication_status.description)
-                exit(1)
 
         # ------------------------------------------------------------------------------------------------------------
         # resources...
 
-        if not cmd.create:
-            finder = CognitoUserFinder(requests)
-
+        finder = CognitoUserFinder(requests)
         manager = OrganisationManager(requests)
 
+
+        # ------------------------------------------------------------------------------------------------------------
+        # validate...
+
+        if cmd.email:
+            cognito = finder.get_by_email(auth.id_token, cmd.email)
+
+            if cognito is None:
+                logger.error("no Cognito user found for email: '%s'." % cmd.email)
+                exit(1)
+
         if cmd.org_label:
             org = manager.get_organisation_by_label(auth.id_token, cmd.org_label)
 
             if org is None:
                 logger.error("no organisation found for label: '%s'." % cmd.org_label)
                 exit(1)
 
-
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
         if cmd.find:
-            if cmd.email is not None:
-                report = sorted(finder.find_by_email(auth.id_token, cmd.email))
-
-            elif cmd.org_label is not None:
-                org_users = manager.find_users_by_organisation(auth.id_token, org.org_id)
-                usernames = [org_user.username for org_user in org_users]
+            if cmd.email:
+                report = manager.find_users_by_username(auth.id_token, cognito.username)
 
-                report = sorted(finder.find_by_usernames(auth.id_token, usernames))
-
-            elif cmd.confirmation_status is not None:
-                report = sorted(finder.find_by_status(auth.id_token,
-                                                      CognitoUserIdentity.status(cmd.confirmation_status)))
-
-            elif cmd.enabled is not None:
-                report = sorted(finder.find_by_enabled(auth.id_token, cmd.enabled))
+            elif cmd.org_label:
+                report = manager.find_users_by_organisation(auth.id_token, org.org_id)
 
             else:
-                report = sorted(finder.find_all(auth.id_token))
+                report = manager.find_users(auth.id_token)
 
-            if cmd.memberships:
-                org_users = manager.find_users(auth.id_token)
-                report = CognitoMembership.merge(report, org_users)
+        if cmd.retrieve:
+            report = manager.get_user(auth.id_token, cognito.username, org.org_id)
 
         if cmd.create:
-            # create...
-            if not Datum.is_email_address(cmd.email):
-                logger.error("The email address '%s' is not valid." % cmd.email)
-                exit(1)
+            is_org_admin = cmd.org_admin == 1
+            is_device_admin = cmd.device_admin == 1
+            is_suspended = False
 
-            identity = CognitoUserIdentity(None, None, None, True,
-                                           False, cmd.email, cmd.given_name, cmd.family_name, None,
-                                           False, False, None)
-
-            manager = CognitoUserCreator(requests)
-            report = manager.create(identity)
+            report = OrganisationUser(cognito.username, org.org_id, is_org_admin, is_device_admin, is_suspended)
+            manager.assert_user(auth.id_token, report)
 
         if cmd.update:
-            # find...
-            identity = finder.get_by_email(auth.id_token, cmd.update)
+            user = manager.get_user(auth.id_token, cognito.username, org.org_id)
 
-            if identity is None:
-                logger.error("no identity found for email: '%s'." % cmd.update)
+            if user is None:
+                logger.error("no organisation user found for email: '%s' and label '%s'." % (cmd.email, cmd.org_label))
                 exit(1)
 
-            # update...
-            enabled = identity.enabled if cmd.enabled is None else cmd.enabled
-            email = identity.email if cmd.email is None else cmd.email
-            given_name = identity.given_name if cmd.given_name is None else cmd.given_name
-            family_name = identity.family_name if cmd.family_name is None else cmd.family_name
-
-            if not Datum.is_email_address(email):
-                logger.error("The email address '%s' is not valid." % email)
-                exit(1)
+            is_org_admin = user.is_org_admin if cmd.org_admin is None else bool(cmd.org_admin)
+            is_device_admin = user.is_device_admin if cmd.device_admin is None else bool(cmd.device_admin)
+            is_suspended = user.is_suspended if cmd.suspended is None else bool(cmd.suspended)
 
-            new_identity = CognitoUserIdentity(identity.username, None, None, enabled,
-                                               identity.email_verified, email, given_name, family_name, None,
-                                               identity.is_super, identity.is_tester, None)
-
-            auth = gatekeeper.user_login(credentials)                          # renew credentials
-            manager = CognitoUserEditor(requests, auth.id_token)
-            report = manager.update(new_identity)
+            report = OrganisationUser(cognito.username, org.org_id, is_org_admin, is_device_admin, is_suspended)
+            manager.assert_user(auth.id_token, report)
 
         if cmd.delete:
-            # TODO: delete user from organisations?
-            manager = CognitoUserDeleter(requests, auth.id_token)
-            manager.delete(cmd.delete)
+            manager.delete_user(auth.id_token, cognito.username, org.org_id)
 
 
-        # ------------------------------------------------------------------------------------------------------------
-        # end...
+    # ----------------------------------------------------------------------------------------------------------------
+    # end...
 
         if report is not None:
             print(JSONify.dumps(report, indent=cmd.indent))
 
         if cmd.find:
             logger.info("found: %s" % len(report))
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
-    except HTTPConflictException as ex:
-        logger.error("the email address '%s' is already in use." % cmd.email)
-        exit(1)
-
     except HTTPException as ex:
-        logger.error(ex.data)
+        logger.error(ex.error_report)
         exit(1)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/configuration_csv.py` & `scs-analysis-2.7.2/src/scs_analysis/configuration_csv.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,40 +58,39 @@
 import requests
 import sys
 
 from scs_analysis.cmd.cmd_configuration_csv import CmdConfigurationCSV
 from scs_analysis.handler.batch_download_reporter import BatchDownloadReporter
 from scs_analysis.handler.configuration_csv_generator import ConfigurationCSVGenerator
 
-from scs_core.aws.client.monitor_auth import MonitorAuth
 from scs_core.aws.manager.configuration_check_finder import ConfigurationCheckFinder, ConfigurationCheckRequest
 from scs_core.aws.manager.configuration_finder import ConfigurationFinder, ConfigurationRequest
+from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
+from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
 
-from scs_core.data.datetime import LocalizedDatetime
+from scs_core.client.http_exception import HTTPException
 
 from scs_core.estate.configuration import Configuration
 
 from scs_core.sample.configuration_sample import ConfigurationReport
 
 from scs_core.sys.filesystem import Filesystem
-from scs_core.sys.http_exception import HTTPException
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     configuration = Configuration.construct_from_jdict(None, skeleton=True)
     node_names = sorted(list(configuration.as_json().keys()))
 
     logger = None
-    auth = None
     configs = []
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # cmd...
 
         cmd = CmdConfigurationCSV()
@@ -108,53 +107,57 @@
                 logger.error('nodes must be in: %s' % str(node_names))
                 exit(2)
 
         logger.info(cmd)
 
 
         # ------------------------------------------------------------------------------------------------------------
+        # authentication...
+
+        credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
+
+        if not credentials:
+            exit(1)
+
+        gatekeeper = CognitoLoginManager(requests)
+        auth = gatekeeper.user_login(credentials)
+
+        if not auth.is_ok():
+            logger.error("login: %s" % auth.authentication_status.description)
+            exit(1)
+
+        # ------------------------------------------------------------------------------------------------------------
         # resources...
 
         # nodes...
         if cmd.node_names:
             print(node_names, file=sys.stderr)
             exit(0)
 
-        # MonitorAuth...
-        if not MonitorAuth.exists(Host):
-            logger.error('MonitorAuth not available.')
-            exit(1)
-
-        try:
-            auth = MonitorAuth.load(Host, encryption_key=MonitorAuth.password_from_user())
-        except (KeyError, ValueError):
-            logger.error('incorrect password.')
-            exit(1)
-
         # reporter...
         reporter = BatchDownloadReporter()
 
         # ConfigurationFinder...
-        configuration_finder = ConfigurationFinder(requests, auth, reporter=reporter)
-        check_finder = ConfigurationCheckFinder(requests, auth)
+        configuration_finder = ConfigurationFinder(requests, reporter=reporter)
+        check_finder = ConfigurationCheckFinder(requests)
 
         # ConfigurationCSVGenerator...
         csv_generator = ConfigurationCSVGenerator(cmd.verbose)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
         logger.info("retrieving check reports...")
-        checks = check_finder.find(None, None, None, ConfigurationCheckRequest.Mode.FULL)
+        checks = check_finder.find(auth.id_token, None, None, ConfigurationCheckRequest.Mode.FULL)
         check_reports = {check.tag: check.rec for check in checks.items}
 
         if cmd.separate or cmd.latest:
             logger.info("retrieving configurations...")
-            response = configuration_finder.find(cmd.device_tag, cmd.exact_match, cmd.request_mode())
+            response = configuration_finder.find(auth.id_token, cmd.device_tag, cmd.exact_match, cmd.request_mode())
             configs = [ConfigurationReport.construct(item, check_reports[item.tag]) for item in sorted(response)]
 
         if cmd.separate:
             for node in node_names:
                 path = node + '.csv'
                 logger.info("-")
                 logger.info(path)
@@ -166,33 +169,32 @@
             csv_generator.generate(configs, cmd.nodes, cmd.latest)
 
         if cmd.diff_histories or cmd.full_histories:
             if cmd.output_csv_dir is not None:
                 Filesystem.mkdir(cmd.output_csv_dir)
 
             logger.info("retrieving device tags...")
-            tag_response = configuration_finder.find(cmd.device_tag, cmd.exact_match,
+            tag_response = configuration_finder.find(auth.id_token, cmd.device_tag, cmd.exact_match,
                                                      ConfigurationRequest.Mode.TAGS_ONLY)
 
             for tag in sorted(tag_response):
                 filename = tag + '-configs.csv'
                 path = filename if cmd.output_csv_dir is None else os.path.join(cmd.output_csv_dir, filename)
 
                 logger.info("-")
                 logger.info(path)
 
-                response = configuration_finder.find(tag, True, cmd.request_mode())
+                response = configuration_finder.find(auth.id_token, tag, True, cmd.request_mode())
                 configs = sorted(response)
 
                 csv_generator.generate(configs, cmd.nodes, path)
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # end...
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
     except HTTPException as ex:
-        now = LocalizedDatetime.now().utc().as_iso8601()
-        logger.error("%s: HTTP response: %s (%s) %s" % (now, ex.status, ex.reason, ex.data))
+        logger.error(ex.error_report)
         exit(1)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/configuration_monitor.py` & `scs-analysis-2.7.2/src/scs_analysis/configuration_monitor.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,32 +27,32 @@
 
 import requests
 import sys
 
 from scs_analysis.cmd.cmd_configuration_monitor import CmdConfigurationMonitor
 from scs_analysis.handler.batch_download_reporter import BatchDownloadReporter
 
-from scs_core.aws.client.monitor_auth import MonitorAuth
 from scs_core.aws.manager.configuration_finder import ConfigurationFinder
+from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
+from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
+
+from scs_core.client.http_exception import HTTPException
 
-from scs_core.data.datetime import LocalizedDatetime
 from scs_core.data.json import JSONify
 
-from scs_core.sys.http_exception import HTTPException
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     logger = None
-    auth = None
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # cmd...
 
         cmd = CmdConfigurationMonitor()
 
@@ -63,46 +63,51 @@
         Logging.config('configuration_monitor', verbose=cmd.verbose)
         logger = Logging.getLogger()
 
         logger.info(cmd)
 
 
         # ------------------------------------------------------------------------------------------------------------
-        # resources...
+        # authentication...
 
-        if not MonitorAuth.exists(Host):
-            logger.error('MonitorAuth not available.')
+        credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
+
+        if not credentials:
             exit(1)
 
-        try:
-            auth = MonitorAuth.load(Host, encryption_key=MonitorAuth.password_from_user())
-        except (KeyError, ValueError):
-            logger.error('incorrect password.')
+        gatekeeper = CognitoLoginManager(requests)
+        auth = gatekeeper.user_login(credentials)
+
+        if not auth.is_ok():
+            logger.error("login: %s" % auth.authentication_status.description)
             exit(1)
 
+
+        # ------------------------------------------------------------------------------------------------------------
+        # resources...
+
         # reporter...
         reporter = BatchDownloadReporter()
 
         # ConfigurationFinder...
-        finder = ConfigurationFinder(requests, auth, reporter=reporter)
+        finder = ConfigurationFinder(requests, reporter=reporter)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
-        response = finder.find(cmd.tag_filter, cmd.exact_match, cmd.response_mode())
+        response = finder.find(auth.id_token, cmd.tag_filter, cmd.exact_match, cmd.response_mode())
         items = list(response)
 
         print(JSONify.dumps(sorted(items), indent=cmd.indent))
         logger.info('retrieved: %s' % len(items))
 
 
         # ------------------------------------------------------------------------------------------------------------
         # end...
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
     except HTTPException as ex:
-        now = LocalizedDatetime.now().utc().as_iso8601()
-        logger.error("%s: HTTP response: %s (%s) %s" % (now, ex.status, ex.reason, ex.data))
+        logger.error(ex.error_report)
         exit(1)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/configuration_monitor_check.py` & `scs-analysis-2.7.2/src/scs_analysis/configuration_monitor_check.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,40 +32,44 @@
 
 SEE ALSO
 scs_analysis/configuration_csv
 scs_analysis/configuration_monitor
 scs_analysis/monitor_auth
 
 scs_mfr/configuration
+
+BUGS
+Result code not currently in use.
 """
 
 import requests
 import sys
 
 from scs_analysis.cmd.cmd_configuration_monitor_check import CmdConfigurationMonitorCheck
 
-from scs_core.aws.client.monitor_auth import MonitorAuth
 from scs_core.aws.manager.configuration_check_finder import ConfigurationCheckFinder
 from scs_core.aws.manager.configuration_check_requester import ConfigurationCheckRequester
 
+from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
+from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
+
+from scs_core.client.http_exception import HTTPException
+
 from scs_core.data.json import JSONify
-from scs_core.data.datetime import LocalizedDatetime
 
-from scs_core.sys.http_exception import HTTPException
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     logger = None
-    auth = None
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # cmd...
 
         cmd = CmdConfigurationMonitorCheck()
 
@@ -76,46 +80,51 @@
         Logging.config('configuration_monitor_check', verbose=cmd.verbose)
         logger = Logging.getLogger()
 
         logger.info(cmd)
 
 
         # ------------------------------------------------------------------------------------------------------------
-        # resources...
+        # authentication...
+
+        credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
 
-        if not MonitorAuth.exists(Host):
-            logger.error('MonitorAuth not available.')
+        if not credentials:
             exit(1)
 
-        try:
-            auth = MonitorAuth.load(Host, encryption_key=MonitorAuth.password_from_user())
-        except (KeyError, ValueError):
-            logger.error('incorrect password.')
+        gatekeeper = CognitoLoginManager(requests)
+        auth = gatekeeper.user_login(credentials)
+
+        if not auth.is_ok():
+            logger.error("login: %s" % auth.authentication_status.description)
             exit(1)
 
-        finder = ConfigurationCheckFinder(requests, auth)
-        requester = ConfigurationCheckRequester(requests, auth)
+
+        # ------------------------------------------------------------------------------------------------------------
+        # resources...
+
+        finder = ConfigurationCheckFinder(requests)
+        requester = ConfigurationCheckRequester(requests)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # run...
 
-        if cmd.check_tag:
-            response = requester.request(cmd.check_tag)
+        if cmd.force:
+            response = requester.request(auth.id_token, cmd.force)
             print(response.result, file=sys.stderr)
             exit(0 if response.result == 'OK' else 1)
 
-        response = finder.find(cmd.tag_filter, cmd.exact_match, cmd.result_code, cmd.response_mode())
+        response = finder.find(auth.id_token, cmd.tag_filter, cmd.exact_match, cmd.response_mode())
         print(JSONify.dumps(sorted(response.items), indent=cmd.indent))
         logger.info('retrieved: %s' % len(response.items))
 
 
         # ------------------------------------------------------------------------------------------------------------
         # end...
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
     except HTTPException as ex:
-        now = LocalizedDatetime.now().utc().as_iso8601()
-        logger.error("%s: HTTP response: %s (%s) %s" % (now, ex.status, ex.reason, ex.data))
+        logger.error(ex.error_report)
         exit(1)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/csv_collation_summary.py` & `scs-analysis-2.7.2/src/scs_analysis/csv_collation_summary.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/csv_collator.py` & `scs-analysis-2.7.2/src/scs_analysis/csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/csv_join.py` & `scs-analysis-2.7.2/src/scs_analysis/csv_join.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/csv_reader.py` & `scs-analysis-2.7.2/src/scs_analysis/csv_reader.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/csv_segmentor.py` & `scs-analysis-2.7.2/src/scs_analysis/csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/csv_writer.py` & `scs-analysis-2.7.2/src/scs_analysis/csv_writer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/handler/aws_mqtt_publisher.py` & `scs-analysis-2.7.2/src/scs_analysis/handler/aws_mqtt_publisher.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/handler/aws_mqtt_subscription_handler.py` & `scs-analysis-2.7.2/src/scs_analysis/handler/aws_mqtt_subscription_handler.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/handler/batch_download_reporter.py` & `scs-analysis-2.7.2/src/scs_analysis/handler/batch_download_reporter.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/handler/configuration_csv_generator.py` & `scs-analysis-2.7.2/src/scs_analysis/handler/configuration_csv_generator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/handler/csv_collator.py` & `scs-analysis-2.7.2/src/scs_analysis/handler/csv_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/handler/csv_segmentor.py` & `scs-analysis-2.7.2/src/scs_analysis/handler/csv_segmentor.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/handler/sample_midpoint.py` & `scs-analysis-2.7.2/src/scs_analysis/handler/sample_midpoint.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/histo_chart.py` & `scs-analysis-2.7.2/src/scs_analysis/histo_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/localised_datetime.py` & `scs-analysis-2.7.2/src/scs_analysis/localised_datetime.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/monitor_auth.py` & `scs-analysis-2.7.2/src/scs_analysis/monitor_auth.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/multi_chart.py` & `scs-analysis-2.7.2/src/scs_analysis/multi_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/node.py` & `scs-analysis-2.7.2/src/scs_analysis/node.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/organisation_devices.py` & `scs-analysis-2.7.2/src/scs_analysis/organisation_devices.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,19 +40,20 @@
 
 from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
 
 from scs_core.aws.security.organisation import Organisation, OrganisationPathRoot, OrganisationDevice
 from scs_core.aws.security.organisation_manager import OrganisationManager
 
+from scs_core.client.http_exception import HTTPException
+
 from scs_core.data.datetime import LocalizedDatetime
 from scs_core.data.datum import Datum
 from scs_core.data.json import JSONify
 
-from scs_core.sys.http_exception import HTTPException
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
@@ -96,31 +97,22 @@
 
         if cmd.deployment_label is not None and not OrganisationDevice.is_valid_deployment_label(cmd.deployment_label):
             logger.error("the deployment label '%s' is not valid." % cmd.deployment_label)
             exit(2)
 
 
         # ------------------------------------------------------------------------------------------------------------
-        # auth...
-
-        gatekeeper = CognitoLoginManager(requests)
+        # authentication...
 
-        # CognitoUserCredentials...
-        if not CognitoClientCredentials.exists(Host, name=cmd.credentials_name):
-            logger.error("Cognito credentials not available.")
-            exit(1)
+        credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
 
-        try:
-            password = CognitoClientCredentials.password_from_user()
-            credentials = CognitoClientCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
-        except (KeyError, ValueError):
-            logger.error("incorrect password.")
+        if not credentials:
             exit(1)
 
-
+        gatekeeper = CognitoLoginManager(requests)
         auth = gatekeeper.user_login(credentials)
 
         if not auth.is_ok():
             logger.error("login: %s" % auth.authentication_status.description)
             exit(1)
 
 
@@ -175,9 +167,9 @@
         if cmd.find:
             logger.info("found: %s" % len(report))
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
     except HTTPException as ex:
-        logger.error(ex.data)
+        logger.error(ex.error_report)
         exit(1)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/organisation_path_roots.py` & `scs-analysis-2.7.2/src/scs_analysis/organisation_path_roots.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,17 +32,18 @@
 from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
 
 from scs_core.aws.security.organisation import Organisation, OrganisationPathRoot
 from scs_core.aws.security.organisation_manager import OrganisationManager
 from scs_core.aws.security.opr_membership import OPRMembership
 
+from scs_core.client.http_exception import HTTPException
+
 from scs_core.data.json import JSONify
 
-from scs_core.sys.http_exception import HTTPException
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
@@ -73,30 +74,22 @@
 
         if cmd.path_root is not None and not OrganisationPathRoot.is_valid_path_root(cmd.path_root):
             logger.error("the path root '%s' is not valid." % cmd.path_root)
             exit(2)
 
 
         # ------------------------------------------------------------------------------------------------------------
-        # auth...
+        # authentication...
 
-        gatekeeper = CognitoLoginManager(requests)
+        credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
 
-        # CognitoUserCredentials...
-        if not CognitoClientCredentials.exists(Host, name=cmd.credentials_name):
-            logger.error("Cognito credentials not available.")
-            exit(1)
-
-        try:
-            password = CognitoClientCredentials.password_from_user()
-            credentials = CognitoClientCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
-        except (KeyError, ValueError):
-            logger.error("incorrect password.")
+        if not credentials:
             exit(1)
 
+        gatekeeper = CognitoLoginManager(requests)
         auth = gatekeeper.user_login(credentials)
 
         if not auth.is_ok():
             logger.error("login: %s" % auth.authentication_status.description)
             exit(1)
 
 
@@ -156,9 +149,9 @@
         if cmd.find:
             logger.info("found: %s" % len(report))
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
     except HTTPException as ex:
-        logger.error(ex.data)
+        logger.error(ex.error_report)
         exit(1)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/organisation_user_paths.py` & `scs-analysis-2.7.2/src/scs_analysis/organisation_user_paths.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,19 +34,19 @@
 from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
 
 from scs_core.aws.security.organisation import OrganisationPathRoot, OrganisationUserPath
 from scs_core.aws.security.organisation_manager import OrganisationManager
 from scs_core.aws.security.cognito_user_finder import CognitoUserFinder
 
-
 from scs_core.data.datum import Datum
 from scs_core.data.json import JSONify
 
-from scs_core.sys.http_exception import HTTPException
+from scs_core.client.http_exception import HTTPException
+
 from scs_core.sys.logging import Logging
 
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
@@ -80,30 +80,22 @@
 
         if cmd.path_extension is not None and not OrganisationUserPath.is_valid_path_extension(cmd.path_extension):
             logger.error("path extension '%s' is not valid." % cmd.path_extension)
             exit(2)
 
 
         # ------------------------------------------------------------------------------------------------------------
-        # auth...
-
-        gatekeeper = CognitoLoginManager(requests)
+        # authentication...
 
-        # CognitoUserCredentials...
-        if not CognitoClientCredentials.exists(Host, name=cmd.credentials_name):
-            logger.error("Cognito credentials not available.")
-            exit(1)
+        credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
 
-        try:
-            password = CognitoClientCredentials.password_from_user()
-            credentials = CognitoClientCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
-        except (KeyError, ValueError):
-            logger.error("incorrect password.")
+        if not credentials:
             exit(1)
 
+        gatekeeper = CognitoLoginManager(requests)
         auth = gatekeeper.user_login(credentials)
 
         if not auth.is_ok():
             logger.error("login: %s" % auth.authentication_status.description)
             exit(1)
 
 
@@ -160,9 +152,9 @@
         if cmd.find:
             logger.info("found: %s" % len(report))
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
     except HTTPException as ex:
-        logger.error(ex.data)
+        logger.error(ex.error_report)
         exit(1)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/organisation_users.py` & `scs-analysis-2.7.2/src/scs_analysis/organisations.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,177 +1,158 @@
 #!/usr/bin/env python3
 
 """
-Created on 18 Jan 2022
+Created on 10 Jan 2022
 
 @author: Bruno Beloff (bruno.beloff@southcoastscience.com)
 
 source repo: scs_analysis
 
 DESCRIPTION
-The organisation_users utility is used to
+The organisations utility is used to
 
 SYNOPSIS
-organisation_users.py  [-c CREDENTIALS] { -F { -e EMAIL | -l ORG_LABEL } | \
--R -e EMAIL -l ORG_LABEL | \
--C -e EMAIL -l ORG_LABEL -o { 1 | 0 } -d { 1 | 0 } | \
--U -e EMAIL -l ORG_LABEL [-o { 1 | 0 }] [-d { 1 | 0 }] [-s { 1 | 0 }] | \
--D -e EMAIL -l ORG_LABEL } \
-[-i INDENT] [-v]
+organisations.py  { -F | -C -l LABEL -n LONG_NAME -u URL -o OWNER_EMAIL | \
+-U LABEL [-l LABEL] [-n LONG_NAME] [-u URL] [-o OWNER_EMAIL] | -D LABEL } [-i INDENT] [-v]
 
 EXAMPLES
-organisation_users.py -F -l NARA
+organisations.py -F
 
 DOCUMENT EXAMPLE
-{"Username": 111, "OrgID": 1, "IsOrgAdmin": true, "IsDeviceAdmin": true, "IsSuspended": false}
+{"OrgID": 1, "Label": "SCS", "LongName": "South Coast Science", "URL": "https://www.southcoastscience.com",
+"Owner": "bruno.beloff@southcoastscience.com"}
 
 SEE ALSO
 scs_analysis/cognito_credentials
-scs_analysis/cognito_users
 """
 
 import requests
 import sys
 
-from scs_analysis.cmd.cmd_organisation_users import CmdOrganisationUsers
+from scs_analysis.cmd.cmd_organisations import CmdOrganisations
 
 from scs_core.aws.security.cognito_client_credentials import CognitoClientCredentials
 from scs_core.aws.security.cognito_login_manager import CognitoLoginManager
-from scs_core.aws.security.cognito_user_finder import CognitoUserFinder
 
-from scs_core.aws.security.organisation import OrganisationUser
+from scs_core.aws.security.organisation import Organisation
 from scs_core.aws.security.organisation_manager import OrganisationManager
 
+from scs_core.client.http_exception import HTTPException
 
-from scs_core.data.datum import Datum
 from scs_core.data.json import JSONify
 
-from scs_core.sys.http_exception import HTTPException
 from scs_core.sys.logging import Logging
 
+from scs_host.comms.stdio import StdIO
 from scs_host.sys.host import Host
 
 
 # --------------------------------------------------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     logger = None
-    cognito = None
-    org = None
-    report = []
+    report = None
 
     try:
         # ------------------------------------------------------------------------------------------------------------
         # cmd...
 
-        cmd = CmdOrganisationUsers()
+        cmd = CmdOrganisations()
 
         if not cmd.is_valid():
             cmd.print_help(sys.stderr)
             exit(2)
 
-        Logging.config('organisation_users', verbose=cmd.verbose)
+        Logging.config('organisations', verbose=cmd.verbose)       # level=logging.DEBUG
         logger = Logging.getLogger()
 
         logger.info(cmd)
 
-        if cmd.email is not None and not Datum.is_email_address(cmd.email):
-            logger.error("email address '%s' is not valid." % cmd.email)
+        if cmd.label is not None and not Organisation.is_valid_label(cmd.label):
+            logger.error("the label '%s' is not valid." % cmd.label)
             exit(2)
 
+        if cmd.long_name is not None and not Organisation.is_valid_long_name(cmd.long_name):
+            logger.error("the long name '%s' is not valid." % cmd.long_name)
+            exit(2)
 
-        # ------------------------------------------------------------------------------------------------------------
-        # auth...
+        if cmd.url is not None and not Organisation.is_valid_url(cmd.url):
+            logger.error("the URL '%s' is not valid." % cmd.url)
+            exit(2)
 
-        gatekeeper = CognitoLoginManager(requests)
+        if cmd.owner is not None and not Organisation.is_valid_owner(cmd.owner):
+            logger.error("the owner email address '%s' is not valid." % cmd.owner)
+            exit(2)
 
-        # CognitoUserCredentials...
-        if not CognitoClientCredentials.exists(Host, name=cmd.credentials_name):
-            logger.error("Cognito credentials not available.")
-            exit(1)
 
-        try:
-            password = CognitoClientCredentials.password_from_user()
-            credentials = CognitoClientCredentials.load(Host, name=cmd.credentials_name, encryption_key=password)
-        except (KeyError, ValueError):
-            logger.error("incorrect password.")
+        # ------------------------------------------------------------------------------------------------------------
+        # authentication...
+
+        credentials = CognitoClientCredentials.load_for_user(Host, name=cmd.credentials_name)
+
+        if not credentials:
             exit(1)
 
+        gatekeeper = CognitoLoginManager(requests)
         auth = gatekeeper.user_login(credentials)
 
         if not auth.is_ok():
             logger.error("login: %s" % auth.authentication_status.description)
             exit(1)
 
 
         # ------------------------------------------------------------------------------------------------------------
         # resources...
 
-        finder = CognitoUserFinder(requests)
         manager = OrganisationManager(requests)
 
 
         # ------------------------------------------------------------------------------------------------------------
-        # validate...
-
-        if cmd.email:
-            cognito = finder.get_by_email(auth.id_token, cmd.email)
-
-            if cognito is None:
-                logger.error("no Cognito user found for email: '%s'." % cmd.email)
-                exit(1)
-
-        if cmd.org_label:
-            org = manager.get_organisation_by_label(auth.id_token, cmd.org_label)
-
-            if org is None:
-                logger.error("no organisation found for label: '%s'." % cmd.org_label)
-                exit(1)
-
-        # ------------------------------------------------------------------------------------------------------------
         # run...
 
         if cmd.find:
-            if cmd.email:
-                report = manager.find_users_by_username(auth.id_token, cognito.username)
-
-            elif cmd.org_label:
-                report = manager.find_users_by_organisation(auth.id_token, org.org_id)
-
-            else:
-                report = manager.find_users(auth.id_token)
-
-        if cmd.retrieve:
-            report = manager.get_user(auth.id_token, cognito.username, org.org_id)
+            report = sorted(manager.find_organisations(auth.id_token))
 
         if cmd.create:
-            is_org_admin = cmd.org_admin == 1
-            is_device_admin = cmd.device_admin == 1
-            is_suspended = False
-
-            report = OrganisationUser(cognito.username, org.org_id, is_org_admin, is_device_admin, is_suspended)
-            manager.assert_user(auth.id_token, report)
+            org = Organisation(0, cmd.label, cmd.long_name, cmd.url, cmd.owner)
+            report = manager.insert_organisation(auth.id_token, org)
 
         if cmd.update:
-            user = manager.get_user(auth.id_token, cognito.username, org.org_id)
+            # find...
+            org = manager.get_organisation_by_label(auth.id_token, cmd.update)
 
-            if user is None:
-                logger.error("no organisation user found for email: '%s' and label '%s'." % (cmd.email, cmd.org_label))
+            if org is None:
+                logger.error("no organisation found for label: '%s'." % cmd.update)
                 exit(1)
 
-            is_org_admin = user.is_org_admin if cmd.org_admin is None else bool(cmd.org_admin)
-            is_device_admin = user.is_device_admin if cmd.device_admin is None else bool(cmd.device_admin)
-            is_suspended = user.is_suspended if cmd.suspended is None else bool(cmd.suspended)
+            # update...
+            label = org.label if cmd.label is None else cmd.label
+            long_name = org.long_name if cmd.long_name is None else cmd.long_name
+            url = org.url if cmd.url is None else cmd.url
+            owner = org.owner if cmd.owner is None else cmd.owner
 
-            report = OrganisationUser(cognito.username, org.org_id, is_org_admin, is_device_admin, is_suspended)
-            manager.assert_user(auth.id_token, report)
+            report = Organisation(org.org_id, label, long_name, url, owner)
+            manager.update_organisation(auth.id_token, report)
 
         if cmd.delete:
-            manager.delete_user(auth.id_token, cognito.username, org.org_id)
+            # find...
+            org = manager.get_organisation_by_label(auth.id_token, cmd.delete)
+
+            if org is None:
+                logger.error("no organisation found for label: '%s'" % cmd.delete)
+                exit(1)
+
+            # check...
+            response = StdIO.prompt('Are you sure? (Y/n)')
+            if response != 'Y':
+                exit(0)
+
+            # delete...
+            manager.delete_organisation(auth.id_token, org.org_id)
 
 
     # ----------------------------------------------------------------------------------------------------------------
     # end...
 
         if report is not None:
             print(JSONify.dumps(report, indent=cmd.indent))
@@ -179,9 +160,9 @@
         if cmd.find:
             logger.info("found: %s" % len(report))
 
     except KeyboardInterrupt:
         print(file=sys.stderr)
 
     except HTTPException as ex:
-        logger.error(ex.data)
+        logger.error(ex.error_report)
         exit(1)
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_aggregate.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_aggregate.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_average.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_average.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 the document that is to be averaged. The node is typically a leaf node integer or float. The output of the
 sample_average utility includes the source value, and the average value.
 
 SYNOPSIS
 sample_average.py [-t TALLY] [-p PRECISION] [-v] [PATH]
 
 EXAMPLES
-osio_topic_history.py -m1 /orgs/south-coast-science-demo/brighton/loc/1/gases | sample_average.py -t3 -p1 val.CO.cnc
+aws_topic_history.py -m1 /orgs/south-coast-science-demo/brighton/loc/1/gases | sample_average.py -t3 -p1 val.CO.cnc
 
 DOCUMENT EXAMPLE - INPUT
 {"tag": "scs-bgx-401", "rec": "2018-03-27T09:54:41.042+00:00", "val": {
 "NO2": {"weV": 0.29563, "aeV": 0.280879, "weC": 0.009569, "cnc": 61.0},
 "Ox": {"weV": 0.406819, "aeV": 0.387443, "weC": -0.010706, "cnc": 34.7},
 "NO": {"weV": 0.319692, "aeV": 0.292129, "weC": 0.028952, "cnc": 165.5},
 "CO": {"weV": 0.395819, "aeV": 0.289317, "weC": 0.113108, "cnc": 311.3},
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_collator.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_collator.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_concentration.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_concentration.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_distance.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_distance.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_duplicates.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_duplicates.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_error.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_error.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_interval.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 the sample_interval utility includes the date / time value, and the time difference from the preceding value
 in seconds.
 
 SYNOPSIS
 sample_interval.py [-p PRECISION] [-v] [PATH]
 
 EXAMPLES
-osio_topic_history.py -m1 /orgs/south-coast-science-demo/brighton/loc/1/gases | sample_interval.py -p3 rec
+aws_topic_history.py -m1 /orgs/south-coast-science-demo/brighton/loc/1/gases | sample_interval.py -p3 rec
 
 DOCUMENT EXAMPLE - INPUT
 {"tag": "scs-bgx-401", "rec": "2018-03-27T09:54:41.042+00:00", "val": {
 "NO2": {"weV": 0.29563, "aeV": 0.280879, "weC": 0.009569, "cnc": 61.0},
 "Ox": {"weV": 0.406819, "aeV": 0.387443, "weC": -0.010706, "cnc": 34.7},
 "NO": {"weV": 0.319692, "aeV": 0.292129, "weC": 0.028952, "cnc": 165.5},
 "CO": {"weV": 0.395819, "aeV": 0.289317, "weC": 0.113108, "cnc": 311.3},
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_iso_8601.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_iso_8601.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_low_pass.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_low_pass.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 the document that is to be filtered. The node is typically a leaf node integer or float. The output of the
 sample_low_pass utility includes the source value, and the smoothed value.
 
 SYNOPSIS
 sample_low_pass.py -d DELTA_T -c CUT_OFF [-p PRECISION] [-v] [PATH]
 
 EXAMPLES
-osio_topic_history.py -m60 /orgs/south-coast-science-demo/brighton/loc/1/gases | \
+aws_topic_history.py -m60 /orgs/south-coast-science-demo/brighton/loc/1/gases | \
 sample_low_pass.py -d 10.0 -c 0.02 -p 1 val.CO.cnc
 
 DOCUMENT EXAMPLE - INPUT
 {"tag": "scs-bgx-401", "rec": "2018-03-27T09:54:41.042+00:00", "val": {
 "NO2": {"weV": 0.29563, "aeV": 0.280879, "weC": 0.009569, "cnc": 61.0},
 "Ox": {"weV": 0.406819, "aeV": 0.387443, "weC": -0.010706, "cnc": 34.7},
 "NO": {"weV": 0.319692, "aeV": 0.292129, "weC": 0.028952, "cnc": 165.5},
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_max.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_max.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 If there are multiple input documents with the same maximum value, the first document only is written to stdout.
 
 SYNOPSIS
 sample_max.py [-v] [PATH]
 
 EXAMPLES
-osio_topic_history.py -m60 /orgs/south-coast-science-demo/brighton/loc/1/gases | sample_max.py val.CO.cnc
+aws_topic_history.py -m60 /orgs/south-coast-science-demo/brighton/loc/1/gases | sample_max.py val.CO.cnc
 
 DOCUMENT EXAMPLE - INPUT
 {"tag": "scs-bgx-401", "rec": "2018-03-27T09:54:41.042+00:00", "val": {
 "NO2": {"weV": 0.29563, "aeV": 0.280879, "weC": 0.009569, "cnc": 61.0},
 "Ox": {"weV": 0.406819, "aeV": 0.387443, "weC": -0.010706, "cnc": 34.7},
 "NO": {"weV": 0.319692, "aeV": 0.292129, "weC": 0.028952, "cnc": 165.5},
 "CO": {"weV": 0.395819, "aeV": 0.289317, "weC": 0.113108, "cnc": 311.3},
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_median.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_median.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 the document that is to be filtered. The node is typically a leaf node integer or float. The output of the
 sample_median utility includes the source value, and the smoothed value.
 
 SYNOPSIS
 sample_median.py [-w SIZE] [-p PRECISION] [-v] [PATH]
 
 EXAMPLES
-osio_topic_history.py -m60 /orgs/south-coast-science-demo/brighton/loc/1/gases | \
+aws_topic_history.py -m60 /orgs/south-coast-science-demo/brighton/loc/1/gases | \
 sample_median.py -w 3 -p 1 val.CO.cnc
 
 DOCUMENT EXAMPLE - INPUT
 {"tag": "scs-bgx-401", "rec": "2018-03-27T09:54:41.042+00:00", "val": {
 "NO2": {"weV": 0.29563, "aeV": 0.280879, "weC": 0.009569, "cnc": 61.0},
 "Ox": {"weV": 0.406819, "aeV": 0.387443, "weC": -0.010706, "cnc": 34.7},
 "NO": {"weV": 0.319692, "aeV": 0.292129, "weC": 0.028952, "cnc": 165.5},
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_midpoint.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_midpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 the document that is to be averaged. The node is typically a leaf node integer or float. The output of the
 sample_midpoint utility includes the source value, and the midpoint value.
 
 SYNOPSIS
 sample_midpoint.py [-t TALLY] [-p PRECISION] [-v] [PATH]
 
 EXAMPLES
-osio_topic_history.py -m60 /orgs/south-coast-science-demo/brighton/loc/1/gases | \
+aws_topic_history.py -m60 /orgs/south-coast-science-demo/brighton/loc/1/gases | \
 sample_midpoint.py -t360 -p1 val.CO.cnc
 
 DOCUMENT EXAMPLE - INPUT
 {"tag": "scs-bgx-401", "rec": "2018-03-27T09:54:41.042+00:00", "val": {
 "NO2": {"weV": 0.29563, "aeV": 0.280879, "weC": 0.009569, "cnc": 61.0},
 "Ox": {"weV": 0.406819, "aeV": 0.387443, "weC": -0.010706, "cnc": 34.7},
 "NO": {"weV": 0.319692, "aeV": 0.292129, "weC": 0.028952, "cnc": 165.5},
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_min.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_min.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 If there are multiple input documents with the same maximum value, the first document only is written to stdout.
 
 SYNOPSIS
 sample_min.py [-v] [PATH]
 
 EXAMPLES
-osio_topic_history.py -m60 /orgs/south-coast-science-demo/brighton/loc/1/gases | sample_min.py val.CO.cnc
+aws_topic_history.py -m60 /orgs/south-coast-science-demo/brighton/loc/1/gases | sample_min.py val.CO.cnc
 
 DOCUMENT EXAMPLE - INPUT
 {"tag": "scs-bgx-401", "rec": "2018-03-27T09:54:41.042+00:00", "val": {
 "NO2": {"weV": 0.29563, "aeV": 0.280879, "weC": 0.009569, "cnc": 61.0},
 "Ox": {"weV": 0.406819, "aeV": 0.387443, "weC": -0.010706, "cnc": 34.7},
 "NO": {"weV": 0.319692, "aeV": 0.292129, "weC": 0.028952, "cnc": 165.5},
 "CO": {"weV": 0.395819, "aeV": 0.289317, "weC": 0.113108, "cnc": 311.3},
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_noise.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_noise.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_nullify.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_nullify.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_paths.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_paths.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_regression.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 the document that is to be averaged. The node is typically a leaf node integer or float. The output of the
 sample_regression utility includes the last source value, slope and intercept.
 
 SYNOPSIS
 sample_regression.py [-t TALLY] [-p PRECISION] [-v] [PATH]
 
 EXAMPLES
-osio_topic_history.py -m60 /orgs/south-coast-science-demo/brighton/loc/1/gases | \
+aws_topic_history.py -m60 /orgs/south-coast-science-demo/brighton/loc/1/gases | \
 sample_regression.py -t360 -p3 val.CO.cnc
 
 DOCUMENT EXAMPLE - INPUT
 {"tag": "scs-bgx-401", "rec": "2018-03-27T09:54:41.042+00:00", "val": {
 "NO2": {"weV": 0.29563, "aeV": 0.280879, "weC": 0.009569, "cnc": 61.0},
 "Ox": {"weV": 0.406819, "aeV": 0.387443, "weC": -0.010706, "cnc": 34.7},
 "NO": {"weV": 0.319692, "aeV": 0.292129, "weC": 0.028952, "cnc": 165.5},
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_slope.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_slope.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_sort.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_sort.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_stats.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_stats.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_subset.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_subset.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_time_shift.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_time_shift.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/sample_timezone.py` & `scs-analysis-2.7.2/src/scs_analysis/sample_timezone.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/single_chart.py` & `scs-analysis-2.7.2/src/scs_analysis/single_chart.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/socket_receiver.py` & `scs-analysis-2.7.2/src/scs_analysis/socket_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/timer.py` & `scs-analysis-2.7.2/src/scs_analysis/timer.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis/uds_receiver.py` & `scs-analysis-2.7.2/src/scs_analysis/uds_receiver.py`

 * *Files identical despite different names*

### Comparing `scs-analysis-2.0.0/src/scs_analysis.egg-info/PKG-INFO` & `scs-analysis-2.7.2/src/scs_analysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-analysis
-Version: 2.0.0
+Version: 2.7.2
 Summary: Information management and analysis utilities for South Coast Science data consumers
 Home-page: https://github.com/south-coast-science/scs_analysis
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `scs-analysis-2.0.0/src/scs_analysis.egg-info/SOURCES.txt` & `scs-analysis-2.7.2/src/scs_analysis.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 src/scs_analysis/access_key.py
 src/scs_analysis/alert.py
 src/scs_analysis/alert_status.py
 src/scs_analysis/aws_api_auth.py
 src/scs_analysis/aws_byline.py
 src/scs_analysis/aws_client_auth.py
 src/scs_analysis/aws_mqtt_client.py
-src/scs_analysis/aws_mqtt_control.py
 src/scs_analysis/aws_topic_history.py
 src/scs_analysis/aws_topic_publisher.py
 src/scs_analysis/aws_upload_interval.py
 src/scs_analysis/baseline.py
 src/scs_analysis/baseline_conf.py
 src/scs_analysis/cognito_devices.py
 src/scs_analysis/cognito_password.py
@@ -28,31 +27,25 @@
 src/scs_analysis/configuration_monitor_check.py
 src/scs_analysis/csv_collation_summary.py
 src/scs_analysis/csv_collator.py
 src/scs_analysis/csv_join.py
 src/scs_analysis/csv_reader.py
 src/scs_analysis/csv_segmentor.py
 src/scs_analysis/csv_writer.py
+src/scs_analysis/device_controller.py
 src/scs_analysis/histo_chart.py
 src/scs_analysis/localised_datetime.py
 src/scs_analysis/monitor_auth.py
-src/scs_analysis/mqtt_peers.py
 src/scs_analysis/multi_chart.py
 src/scs_analysis/node.py
 src/scs_analysis/organisation_devices.py
 src/scs_analysis/organisation_path_roots.py
 src/scs_analysis/organisation_user_paths.py
 src/scs_analysis/organisation_users.py
 src/scs_analysis/organisations.py
-src/scs_analysis/osio_api_auth.py
-src/scs_analysis/osio_client_auth.py
-src/scs_analysis/osio_mqtt_client.py
-src/scs_analysis/osio_mqtt_control.py
-src/scs_analysis/osio_topic_history.py
-src/scs_analysis/osio_topic_publisher.py
 src/scs_analysis/sample_aggregate.py
 src/scs_analysis/sample_average.py
 src/scs_analysis/sample_collator.py
 src/scs_analysis/sample_concentration.py
 src/scs_analysis/sample_distance.py
 src/scs_analysis/sample_duplicates.py
 src/scs_analysis/sample_error.py
@@ -108,32 +101,26 @@
 src/scs_analysis/cmd/cmd_configuration_monitor_check.py
 src/scs_analysis/cmd/cmd_csv_collation_summary.py
 src/scs_analysis/cmd/cmd_csv_collator.py
 src/scs_analysis/cmd/cmd_csv_join.py
 src/scs_analysis/cmd/cmd_csv_reader.py
 src/scs_analysis/cmd/cmd_csv_segmentor.py
 src/scs_analysis/cmd/cmd_csv_writer.py
+src/scs_analysis/cmd/cmd_device_controller.py
 src/scs_analysis/cmd/cmd_histo_chart.py
 src/scs_analysis/cmd/cmd_localised_datetime.py
 src/scs_analysis/cmd/cmd_monitor_auth.py
 src/scs_analysis/cmd/cmd_mqtt_client.py
-src/scs_analysis/cmd/cmd_mqtt_control.py
-src/scs_analysis/cmd/cmd_mqtt_peers.py
 src/scs_analysis/cmd/cmd_multi_chart.py
 src/scs_analysis/cmd/cmd_node.py
 src/scs_analysis/cmd/cmd_organisation_devices.py
 src/scs_analysis/cmd/cmd_organisation_path_roots.py
 src/scs_analysis/cmd/cmd_organisation_user_paths.py
 src/scs_analysis/cmd/cmd_organisation_users.py
 src/scs_analysis/cmd/cmd_organisations.py
-src/scs_analysis/cmd/cmd_osio_api_auth.py
-src/scs_analysis/cmd/cmd_osio_client_auth.py
-src/scs_analysis/cmd/cmd_osio_topic.py
-src/scs_analysis/cmd/cmd_osio_topic_history.py
-src/scs_analysis/cmd/cmd_osio_topic_publisher.py
 src/scs_analysis/cmd/cmd_sample_aggregate.py
 src/scs_analysis/cmd/cmd_sample_collator.py
 src/scs_analysis/cmd/cmd_sample_concentration.py
 src/scs_analysis/cmd/cmd_sample_distance.py
 src/scs_analysis/cmd/cmd_sample_duplicates.py
 src/scs_analysis/cmd/cmd_sample_error.py
 src/scs_analysis/cmd/cmd_sample_filter.py
@@ -158,11 +145,9 @@
 src/scs_analysis/handler/aws_mqtt_publisher.py
 src/scs_analysis/handler/aws_mqtt_subscription_handler.py
 src/scs_analysis/handler/batch_download_reporter.py
 src/scs_analysis/handler/configuration_csv_generator.py
 src/scs_analysis/handler/csv_collator.py
 src/scs_analysis/handler/csv_segmentor.py
 src/scs_analysis/handler/mqtt_reporter.py
-src/scs_analysis/handler/osio_mqtt_client_handler.py
-src/scs_analysis/handler/osio_mqtt_control_handler.py
 src/scs_analysis/handler/sample_midpoint.py
 src/scs_analysis/handler/sample_regression.py
```

