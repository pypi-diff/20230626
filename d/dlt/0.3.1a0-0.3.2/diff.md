# Comparing `tmp/dlt-0.3.1a0.tar.gz` & `tmp/dlt-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.3.1a0.tar", max compression
+gzip compressed data, was "dlt-0.3.2.tar", max compression
```

## Comparing `dlt-0.3.1a0.tar` & `dlt-0.3.2.tar`

### file list

```diff
@@ -1,214 +1,219 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.3.1a0/LICENSE.txt
--rw-r--r--   0        0        0     4131 2023-06-07 10:42:04.941010 dlt-0.3.1a0/README.md
--rw-r--r--   0        0        0     1711 2023-04-30 21:17:44.388805 dlt-0.3.1a0/dlt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 21:17:44.388805 dlt-0.3.1a0/dlt/cli/__init__.py
--rw-r--r--   0        0        0    16723 2023-06-07 10:42:04.941010 dlt-0.3.1a0/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     3886 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    14636 2023-05-29 18:11:09.008705 dlt-0.3.1a0/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0    14722 2023-05-29 18:11:09.008705 dlt-0.3.1a0/dlt/cli/deploy_command_helpers.py
--rw-r--r--   0        0        0     1853 2023-04-30 21:17:44.388805 dlt-0.3.1a0/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-06-07 10:42:04.941010 dlt-0.3.1a0/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    18756 2023-06-07 10:42:04.941010 dlt-0.3.1a0/dlt/cli/init_command.py
--rw-r--r--   0        0        0    10503 2023-05-28 13:56:42.331452 dlt-0.3.1a0/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0     9588 2023-06-07 10:42:04.941010 dlt-0.3.1a0/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     4505 2023-05-24 16:38:22.528779 dlt-0.3.1a0/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1899 2023-05-23 16:25:33.987923 dlt-0.3.1a0/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0     3753 2023-05-29 18:11:09.008705 dlt-0.3.1a0/dlt/cli/utils.py
--rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/__init__.py
--rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.3.1a0/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      442 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     5078 2023-05-24 16:38:22.528779 dlt-0.3.1a0/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     3469 2023-06-03 16:59:51.259756 dlt-0.3.1a0/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     6741 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0     7912 2023-04-22 20:26:30.632198 dlt-0.3.1a0/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1791 2023-05-14 20:33:31.539348 dlt-0.3.1a0/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      306 2023-05-07 23:03:04.659469 dlt-0.3.1a0/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0      664 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/providers/airflow.py
--rw-r--r--   0        0        0     1116 2023-05-07 23:03:04.659469 dlt-0.3.1a0/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1335 2023-05-07 23:03:04.659469 dlt-0.3.1a0/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     1981 2023-05-07 23:03:04.659469 dlt-0.3.1a0/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0     3662 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/providers/google_secrets.py
--rw-r--r--   0        0        0     1306 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0    12390 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    18788 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0      971 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     1817 2023-05-07 23:03:04.659469 dlt-0.3.1a0/dlt/common/configuration/specs/api_credentials.py
--rw-r--r--   0        0        0     2109 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/specs/aws_credentials.py
--rw-r--r--   0        0        0    14214 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     5483 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     3387 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     1818 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/configuration/specs/connection_string_credentials.py
--rw-r--r--   0        0        0     2125 2023-04-24 18:26:21.111453 dlt-0.3.1a0/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0    12725 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/common/configuration/specs/gcp_credentials.py
--rw-r--r--   0        0        0      725 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0     2455 2023-04-30 21:17:44.388805 dlt-0.3.1a0/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0     6036 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.3.1a0/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     5893 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     2400 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0     5159 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0      189 2023-05-29 18:11:09.008705 dlt-0.3.1a0/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     2228 2023-06-13 23:16:30.618251 dlt-0.3.1a0/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0    11099 2023-05-29 18:11:09.008705 dlt-0.3.1a0/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     6465 2023-06-08 07:50:27.863474 dlt-0.3.1a0/dlt/common/exceptions.py
--rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/git.py
--rw-r--r--   0        0        0     5253 2023-05-14 20:33:31.539348 dlt-0.3.1a0/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.3.1a0/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.3.1a0/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0     1536 2023-04-29 12:58:55.943219 dlt-0.3.1a0/dlt/common/jsonpath.py
--rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1197 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.3.1a0/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    13382 2023-05-14 20:33:31.539348 dlt-0.3.1a0/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.3.1a0/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.3.1a0/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/pendulum.py
--rw-r--r--   0        0        0    18949 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.3.1a0/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.3.1a0/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5069 2023-04-24 18:26:21.111453 dlt-0.3.1a0/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      174 2023-04-30 21:17:44.388805 dlt-0.3.1a0/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      705 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0     2635 2023-05-14 11:08:47.420838 dlt-0.3.1a0/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      105 2023-04-30 21:17:44.388805 dlt-0.3.1a0/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5590 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/common/runners/venv.py
--rw-r--r--   0        0        0       36 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0    13923 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/runtime/collector.py
--rw-r--r--   0        0        0     4501 2023-05-14 20:33:31.539348 dlt-0.3.1a0/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0      647 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/init.py
--rw-r--r--   0        0        0     4002 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/logger.py
--rw-r--r--   0        0        0     2052 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     7170 2023-05-14 20:33:31.539348 dlt-0.3.1a0/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2493 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     2027 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.3.1a0/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0      720 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.3.1a0/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0    25164 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.3.1a0/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    23080 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/schema/utils.py
--rw-r--r--   0        0        0     1467 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/source.py
--rw-r--r--   0        0        0      554 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     1649 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/storages/configuration.py
--rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     3107 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0    10891 2023-05-14 20:33:31.539348 dlt-0.3.1a0/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0     2690 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    21812 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     2409 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     8600 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     9486 2023-06-08 07:50:27.863474 dlt-0.3.1a0/dlt/common/storages/transactional_file.py
--rw-r--r--   0        0        0     2525 2023-04-24 18:26:21.111453 dlt-0.3.1a0/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     2634 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/common/time.py
--rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.3.1a0/dlt/common/typing.py
--rw-r--r--   0        0        0    14285 2023-06-13 23:16:30.618251 dlt-0.3.1a0/dlt/common/utils.py
--rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/validation.py
--rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/common/wei.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/bigquery/README.md
--rw-r--r--   0        0        0     1813 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/destinations/bigquery/__init__.py
--rw-r--r--   0        0        0    12370 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/bigquery/bigquery.py
--rw-r--r--   0        0        0      386 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/destinations/bigquery/configuration.py
--rw-r--r--   0        0        0    10342 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/destinations/bigquery/sql_client.py
--rw-r--r--   0        0        0     1935 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/destinations/duckdb/__init__.py
--rw-r--r--   0        0        0     7207 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/duckdb/configuration.py
--rw-r--r--   0        0        0     2754 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/duckdb/duck.py
--rw-r--r--   0        0        0     6936 2023-04-21 22:25:54.789942 dlt-0.3.1a0/dlt/destinations/duckdb/sql_client.py
--rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/dummy/__init__.py
--rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.3.1a0/dlt/destinations/dummy/configuration.py
--rw-r--r--   0        0        0     4989 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/dummy/dummy.py
--rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0     1270 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/destinations/filesystem/__init__.py
--rw-r--r--   0        0        0     2253 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/filesystem/configuration.py
--rw-r--r--   0        0        0     4935 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/filesystem/filesystem.py
--rw-r--r--   0        0        0     1419 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/filesystem/filesystem_client.py
--rw-r--r--   0        0        0     5005 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    15639 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/postgres/README.md
--rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/destinations/postgres/__init__.py
--rw-r--r--   0        0        0     1316 2023-05-29 18:11:09.008705 dlt-0.3.1a0/dlt/destinations/postgres/configuration.py
--rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/postgres/postgres.py
--rw-r--r--   0        0        0     6074 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/destinations/postgres/sql_client.py
--rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.3.1a0/dlt/destinations/redshift/README.md
--rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/destinations/redshift/__init__.py
--rw-r--r--   0        0        0      570 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/destinations/redshift/configuration.py
--rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/destinations/redshift/redshift.py
--rw-r--r--   0        0        0     7117 2023-05-28 13:56:42.341452 dlt-0.3.1a0/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    10090 2023-05-28 13:56:42.341452 dlt-0.3.1a0/dlt/destinations/sql_merge_job.py
--rw-r--r--   0        0        0     1931 2023-04-24 18:26:21.111453 dlt-0.3.1a0/dlt/destinations/typing.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.1a0/dlt/extract/__init__.py
--rw-r--r--   0        0        0    26516 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/extract/decorators.py
--rw-r--r--   0        0        0    12995 2023-06-07 08:32:53.261010 dlt-0.3.1a0/dlt/extract/exceptions.py
--rw-r--r--   0        0        0     8312 2023-06-13 20:43:40.978251 dlt-0.3.1a0/dlt/extract/extract.py
--rw-r--r--   0        0        0    14954 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/extract/incremental.py
--rw-r--r--   0        0        0    32327 2023-06-13 20:43:40.978251 dlt-0.3.1a0/dlt/extract/pipe.py
--rw-r--r--   0        0        0     9683 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/extract/schema.py
--rw-r--r--   0        0        0    38391 2023-06-13 20:43:40.978251 dlt-0.3.1a0/dlt/extract/source.py
--rw-r--r--   0        0        0     4308 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/extract/typing.py
--rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.3.1a0/dlt/extract/utils.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.3.1a0/dlt/helpers/__init__.py
--rw-r--r--   0        0        0    13783 2023-05-28 13:56:42.341452 dlt-0.3.1a0/dlt/helpers/airflow_helper.py
--rw-r--r--   0        0        0     2907 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     3583 2023-03-23 14:48:32.561618 dlt-0.3.1a0/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    13032 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     2490 2023-05-29 14:13:02.438979 dlt-0.3.1a0/dlt/helpers/pandas_helper.py
--rw-r--r--   0        0        0     1035 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/helpers/parquet.py
--rw-r--r--   0        0        0    13378 2023-05-29 14:13:02.438979 dlt-0.3.1a0/dlt/helpers/streamlit_helper.py
--rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/load/__init__.py
--rw-r--r--   0        0        0     1005 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/load/configuration.py
--rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.3.1a0/dlt/load/exceptions.py
--rw-r--r--   0        0        0    19925 2023-06-08 14:19:13.923473 dlt-0.3.1a0/dlt/load/load.py
--rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1101 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/normalize/configuration.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.1a0/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    16538 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/normalize/normalize.py
--rw-r--r--   0        0        0    13081 2023-05-28 13:56:42.341452 dlt-0.3.1a0/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     1858 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      379 2023-05-24 16:38:22.538779 dlt-0.3.1a0/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     3100 2023-05-28 13:56:42.341452 dlt-0.3.1a0/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     8733 2023-06-07 08:32:53.271010 dlt-0.3.1a0/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.3.1a0/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    59020 2023-06-07 08:32:53.271010 dlt-0.3.1a0/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0      985 2023-04-30 21:17:44.398805 dlt-0.3.1a0/dlt/pipeline/progress.py
--rw-r--r--   0        0        0     4186 2023-06-07 08:32:53.271010 dlt-0.3.1a0/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0     7990 2023-04-03 18:50:36.903525 dlt-0.3.1a0/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     4625 2023-05-29 18:11:09.018705 dlt-0.3.1a0/dlt/pipeline/track.py
--rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/pipeline/typing.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.3.1a0/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/reflection/names.py
--rw-r--r--   0        0        0     5617 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      124 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/sources/__init__.py
--rw-r--r--   0        0        0      320 2023-05-07 23:03:04.669469 dlt-0.3.1a0/dlt/sources/credentials.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.3.1a0/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0     9243 2023-05-29 14:13:02.418979 dlt-0.3.1a0/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.3.1a0/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.3.1a0/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.3.1a0/dlt/version.py
--rw-r--r--   0        0        0     4278 2023-06-13 23:16:43.718251 dlt-0.3.1a0/pyproject.toml
--rw-r--r--   0        0        0     7548 1970-01-01 00:00:00.000000 dlt-0.3.1a0/setup.py
--rw-r--r--   0        0        0     7546 1970-01-01 00:00:00.000000 dlt-0.3.1a0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.3.2/LICENSE.txt
+-rw-r--r--   0        0        0     4144 2023-06-21 13:07:51.602230 dlt-0.3.2/README.md
+-rw-r--r--   0        0        0     1708 2023-06-21 13:07:51.602230 dlt-0.3.2/dlt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 21:17:44.388805 dlt-0.3.2/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    17127 2023-06-25 21:57:41.225402 dlt-0.3.2/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     3974 2023-06-23 11:37:08.764341 dlt-0.3.2/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    15046 2023-06-21 13:07:51.602230 dlt-0.3.2/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0    14849 2023-06-22 15:45:03.707967 dlt-0.3.2/dlt/cli/deploy_command_helpers.py
+-rw-r--r--   0        0        0     1853 2023-04-30 21:17:44.388805 dlt-0.3.2/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-06-07 10:42:04.941010 dlt-0.3.2/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    18756 2023-06-07 10:42:04.941010 dlt-0.3.2/dlt/cli/init_command.py
+-rw-r--r--   0        0        0    10508 2023-06-22 15:45:03.707967 dlt-0.3.2/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0     9588 2023-06-21 13:07:51.602230 dlt-0.3.2/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     4505 2023-05-24 16:38:22.528779 dlt-0.3.2/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1899 2023-05-23 16:25:33.987923 dlt-0.3.2/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0     3753 2023-05-29 18:11:09.008705 dlt-0.3.2/dlt/cli/utils.py
+-rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.3.2/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.3.2/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      442 2023-05-29 14:13:02.418979 dlt-0.3.2/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     5078 2023-05-24 16:38:22.528779 dlt-0.3.2/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     3469 2023-06-03 16:59:51.259756 dlt-0.3.2/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     6741 2023-05-29 14:13:02.418979 dlt-0.3.2/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0     7912 2023-06-20 19:08:58.883105 dlt-0.3.2/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1791 2023-05-14 20:33:31.539348 dlt-0.3.2/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      344 2023-06-21 13:07:51.602230 dlt-0.3.2/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0      664 2023-05-29 14:13:02.418979 dlt-0.3.2/dlt/common/configuration/providers/airflow.py
+-rw-r--r--   0        0        0     1116 2023-05-07 23:03:04.659469 dlt-0.3.2/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1335 2023-05-07 23:03:04.659469 dlt-0.3.2/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     1981 2023-05-07 23:03:04.659469 dlt-0.3.2/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0     3662 2023-05-29 14:13:02.418979 dlt-0.3.2/dlt/common/configuration/providers/google_secrets.py
+-rw-r--r--   0        0        0     1306 2023-05-24 16:38:22.538779 dlt-0.3.2/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0    12880 2023-06-21 13:07:51.602230 dlt-0.3.2/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    18788 2023-06-20 20:37:15.263105 dlt-0.3.2/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0      971 2023-05-29 14:13:02.418979 dlt-0.3.2/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     1817 2023-05-07 23:03:04.659469 dlt-0.3.2/dlt/common/configuration/specs/api_credentials.py
+-rw-r--r--   0        0        0     2109 2023-05-29 14:13:02.418979 dlt-0.3.2/dlt/common/configuration/specs/aws_credentials.py
+-rw-r--r--   0        0        0    14214 2023-05-29 14:13:02.418979 dlt-0.3.2/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     5483 2023-05-29 14:13:02.418979 dlt-0.3.2/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     3387 2023-06-07 08:32:53.261010 dlt-0.3.2/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     1818 2023-05-24 16:38:22.538779 dlt-0.3.2/dlt/common/configuration/specs/connection_string_credentials.py
+-rw-r--r--   0        0        0     2125 2023-04-24 18:26:21.111453 dlt-0.3.2/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0    12725 2023-05-07 23:03:04.669469 dlt-0.3.2/dlt/common/configuration/specs/gcp_credentials.py
+-rw-r--r--   0        0        0      725 2023-05-07 23:03:04.669469 dlt-0.3.2/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0     2455 2023-04-30 21:17:44.388805 dlt-0.3.2/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0     6036 2023-05-29 14:13:02.418979 dlt-0.3.2/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.3.2/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.3.2/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.3.2/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.3.2/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0     6203 2023-06-22 15:45:03.707967 dlt-0.3.2/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     2727 2023-06-22 15:45:03.707967 dlt-0.3.2/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.3.2/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0     8556 2023-06-22 15:45:03.707967 dlt-0.3.2/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0      189 2023-05-29 18:11:09.008705 dlt-0.3.2/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     2250 2023-06-22 15:45:03.707967 dlt-0.3.2/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0    11099 2023-05-29 18:11:09.008705 dlt-0.3.2/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     6465 2023-06-08 07:50:27.863474 dlt-0.3.2/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.3.2/dlt/common/git.py
+-rw-r--r--   0        0        0     5253 2023-05-14 20:33:31.539348 dlt-0.3.2/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.3.2/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.3.2/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0     1536 2023-04-29 12:58:55.943219 dlt-0.3.2/dlt/common/jsonpath.py
+-rw-r--r--   0        0        0        0 2023-06-22 15:45:03.707967 dlt-0.3.2/dlt/common/libs/__init__.py
+-rw-r--r--   0        0        0     1041 2023-06-22 15:45:03.707967 dlt-0.3.2/dlt/common/libs/pyarrow.py
+-rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.3.2/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1197 2023-05-07 23:03:04.669469 dlt-0.3.2/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.3.2/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.3.2/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    13382 2023-05-14 20:33:31.539348 dlt-0.3.2/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.3.2/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.3.2/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.3.2/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.3.2/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.3.2/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.3.2/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.3.2/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.3.2/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.3.2/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    19069 2023-06-22 15:45:03.707967 dlt-0.3.2/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.3.2/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.3.2/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.3.2/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5069 2023-04-24 18:26:21.111453 dlt-0.3.2/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      174 2023-04-30 21:17:44.388805 dlt-0.3.2/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0      705 2023-05-24 16:38:22.538779 dlt-0.3.2/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0     2635 2023-05-14 11:08:47.420838 dlt-0.3.2/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.3.2/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.3.2/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.3.2/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      105 2023-04-30 21:17:44.388805 dlt-0.3.2/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5590 2023-05-07 23:03:04.669469 dlt-0.3.2/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0       36 2023-04-30 21:17:44.398805 dlt-0.3.2/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0    13923 2023-06-07 08:32:53.261010 dlt-0.3.2/dlt/common/runtime/collector.py
+-rw-r--r--   0        0        0     4501 2023-05-14 20:33:31.539348 dlt-0.3.2/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0      647 2023-04-30 21:17:44.398805 dlt-0.3.2/dlt/common/runtime/init.py
+-rw-r--r--   0        0        0     4002 2023-04-30 21:17:44.398805 dlt-0.3.2/dlt/common/runtime/logger.py
+-rw-r--r--   0        0        0     2052 2023-04-30 21:17:44.398805 dlt-0.3.2/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     7170 2023-05-14 20:33:31.539348 dlt-0.3.2/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2493 2023-04-30 21:17:44.398805 dlt-0.3.2/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     2027 2023-04-30 21:17:44.398805 dlt-0.3.2/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.3.2/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0      720 2023-04-30 21:17:44.398805 dlt-0.3.2/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.3.2/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.3.2/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.3.2/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0    25164 2023-05-29 14:13:02.418979 dlt-0.3.2/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.3.2/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    23080 2023-06-07 08:32:53.261010 dlt-0.3.2/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0     1467 2023-05-24 16:38:22.538779 dlt-0.3.2/dlt/common/source.py
+-rw-r--r--   0        0        0      554 2023-05-24 16:38:22.538779 dlt-0.3.2/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     1649 2023-05-24 16:38:22.538779 dlt-0.3.2/dlt/common/storages/configuration.py
+-rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.3.2/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     3107 2023-06-07 08:32:53.261010 dlt-0.3.2/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0    11872 2023-06-21 13:07:51.612230 dlt-0.3.2/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0     2690 2023-05-24 16:38:22.538779 dlt-0.3.2/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    21812 2023-05-24 16:38:22.538779 dlt-0.3.2/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     2409 2023-05-24 16:38:22.538779 dlt-0.3.2/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     8600 2023-06-07 08:32:53.261010 dlt-0.3.2/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     9506 2023-06-25 19:18:14.825402 dlt-0.3.2/dlt/common/storages/transactional_file.py
+-rw-r--r--   0        0        0     2525 2023-04-24 18:26:21.111453 dlt-0.3.2/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     2634 2023-05-07 23:03:04.669469 dlt-0.3.2/dlt/common/time.py
+-rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.3.2/dlt/common/typing.py
+-rw-r--r--   0        0        0    14285 2023-06-21 13:07:51.612230 dlt-0.3.2/dlt/common/utils.py
+-rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.3.2/dlt/common/validation.py
+-rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.3.2/dlt/common/wei.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.3.2/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.3.2/dlt/destinations/bigquery/README.md
+-rw-r--r--   0        0        0     1824 2023-06-22 15:45:03.707967 dlt-0.3.2/dlt/destinations/bigquery/__init__.py
+-rw-r--r--   0        0        0    12559 2023-06-22 15:45:03.707967 dlt-0.3.2/dlt/destinations/bigquery/bigquery.py
+-rw-r--r--   0        0        0      386 2023-05-07 23:03:04.669469 dlt-0.3.2/dlt/destinations/bigquery/configuration.py
+-rw-r--r--   0        0        0    10342 2023-06-25 21:49:43.075402 dlt-0.3.2/dlt/destinations/bigquery/sql_client.py
+-rw-r--r--   0        0        0     1946 2023-06-25 20:39:31.755402 dlt-0.3.2/dlt/destinations/duckdb/__init__.py
+-rw-r--r--   0        0        0     7211 2023-06-25 21:57:41.225402 dlt-0.3.2/dlt/destinations/duckdb/configuration.py
+-rw-r--r--   0        0        0     4114 2023-06-23 11:37:08.764341 dlt-0.3.2/dlt/destinations/duckdb/duck.py
+-rw-r--r--   0        0        0     6936 2023-06-25 21:49:43.085402 dlt-0.3.2/dlt/destinations/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.3.2/dlt/destinations/dummy/__init__.py
+-rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.3.2/dlt/destinations/dummy/configuration.py
+-rw-r--r--   0        0        0     4989 2023-05-29 14:13:02.418979 dlt-0.3.2/dlt/destinations/dummy/dummy.py
+-rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.3.2/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0     1270 2023-06-25 11:33:44.534161 dlt-0.3.2/dlt/destinations/filesystem/__init__.py
+-rw-r--r--   0        0        0     2253 2023-05-29 14:13:02.418979 dlt-0.3.2/dlt/destinations/filesystem/configuration.py
+-rw-r--r--   0        0        0     5111 2023-06-25 19:18:14.825402 dlt-0.3.2/dlt/destinations/filesystem/filesystem.py
+-rw-r--r--   0        0        0     1419 2023-05-29 14:13:02.418979 dlt-0.3.2/dlt/destinations/filesystem/filesystem_client.py
+-rw-r--r--   0        0        0     5028 2023-06-21 13:07:51.612230 dlt-0.3.2/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    16206 2023-06-25 21:49:43.085402 dlt-0.3.2/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.3.2/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.3.2/dlt/destinations/postgres/README.md
+-rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.3.2/dlt/destinations/postgres/__init__.py
+-rw-r--r--   0        0        0     1377 2023-06-22 15:45:03.707967 dlt-0.3.2/dlt/destinations/postgres/configuration.py
+-rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.3.2/dlt/destinations/postgres/postgres.py
+-rw-r--r--   0        0        0     6074 2023-06-25 21:49:43.085402 dlt-0.3.2/dlt/destinations/postgres/sql_client.py
+-rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.3.2/dlt/destinations/redshift/README.md
+-rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.3.2/dlt/destinations/redshift/__init__.py
+-rw-r--r--   0        0        0      570 2023-05-07 23:03:04.669469 dlt-0.3.2/dlt/destinations/redshift/configuration.py
+-rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.3.2/dlt/destinations/redshift/redshift.py
+-rw-r--r--   0        0        0     1916 2023-06-23 11:37:08.764341 dlt-0.3.2/dlt/destinations/snowflake/__init__.py
+-rw-r--r--   0        0        0     4076 2023-06-25 11:33:44.534161 dlt-0.3.2/dlt/destinations/snowflake/configuration.py
+-rw-r--r--   0        0        0     7479 2023-06-23 11:37:08.764341 dlt-0.3.2/dlt/destinations/snowflake/snowflake.py
+-rw-r--r--   0        0        0     7113 2023-06-25 21:49:43.085402 dlt-0.3.2/dlt/destinations/snowflake/sql_client.py
+-rw-r--r--   0        0        0     7389 2023-06-25 21:49:43.085402 dlt-0.3.2/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    10338 2023-06-22 15:45:03.707967 dlt-0.3.2/dlt/destinations/sql_merge_job.py
+-rw-r--r--   0        0        0     1931 2023-04-24 18:26:21.111453 dlt-0.3.2/dlt/destinations/typing.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.2/dlt/extract/__init__.py
+-rw-r--r--   0        0        0    26516 2023-06-07 08:32:53.261010 dlt-0.3.2/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    12995 2023-06-07 08:32:53.261010 dlt-0.3.2/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0     8312 2023-06-21 13:07:51.612230 dlt-0.3.2/dlt/extract/extract.py
+-rw-r--r--   0        0        0    14954 2023-05-24 16:38:22.538779 dlt-0.3.2/dlt/extract/incremental.py
+-rw-r--r--   0        0        0    35424 2023-06-25 11:33:44.534161 dlt-0.3.2/dlt/extract/pipe.py
+-rw-r--r--   0        0        0     9683 2023-05-24 16:38:22.538779 dlt-0.3.2/dlt/extract/schema.py
+-rw-r--r--   0        0        0    38391 2023-06-21 13:07:51.612230 dlt-0.3.2/dlt/extract/source.py
+-rw-r--r--   0        0        0     4308 2023-05-24 16:38:22.538779 dlt-0.3.2/dlt/extract/typing.py
+-rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.3.2/dlt/extract/utils.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.3.2/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0    13783 2023-05-28 13:56:42.341452 dlt-0.3.2/dlt/helpers/airflow_helper.py
+-rw-r--r--   0        0        0     3110 2023-06-23 11:37:08.764341 dlt-0.3.2/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.3.2/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.3.2/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.3.2/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     4827 2023-06-23 11:37:08.764341 dlt-0.3.2/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    13032 2023-04-30 21:17:44.398805 dlt-0.3.2/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     2490 2023-05-29 14:13:02.438979 dlt-0.3.2/dlt/helpers/pandas_helper.py
+-rw-r--r--   0        0        0    13378 2023-05-29 14:13:02.438979 dlt-0.3.2/dlt/helpers/streamlit_helper.py
+-rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.3.2/dlt/load/__init__.py
+-rw-r--r--   0        0        0     1005 2023-05-24 16:38:22.538779 dlt-0.3.2/dlt/load/configuration.py
+-rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.3.2/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    19925 2023-06-08 14:19:13.923473 dlt-0.3.2/dlt/load/load.py
+-rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.3.2/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1101 2023-05-24 16:38:22.538779 dlt-0.3.2/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.3.2/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    16488 2023-06-22 15:45:03.707967 dlt-0.3.2/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0    13137 2023-06-22 15:45:03.707967 dlt-0.3.2/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     1971 2023-06-22 15:45:03.707967 dlt-0.3.2/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      379 2023-05-24 16:38:22.538779 dlt-0.3.2/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.3.2/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     3100 2023-05-28 13:56:42.341452 dlt-0.3.2/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     8733 2023-06-07 08:32:53.271010 dlt-0.3.2/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.3.2/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    59746 2023-06-22 15:45:03.707967 dlt-0.3.2/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0      985 2023-04-30 21:17:44.398805 dlt-0.3.2/dlt/pipeline/progress.py
+-rw-r--r--   0        0        0     4186 2023-06-07 08:32:53.271010 dlt-0.3.2/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0     7990 2023-06-21 13:07:51.612230 dlt-0.3.2/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     4625 2023-05-29 18:11:09.018705 dlt-0.3.2/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.3.2/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.3.2/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.3.2/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.3.2/dlt/reflection/names.py
+-rw-r--r--   0        0        0     5617 2023-05-07 23:03:04.669469 dlt-0.3.2/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.3.2/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      124 2023-05-07 23:03:04.669469 dlt-0.3.2/dlt/sources/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-07 23:03:04.669469 dlt-0.3.2/dlt/sources/credentials.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.3.2/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.3.2/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0     9243 2023-05-29 14:13:02.418979 dlt-0.3.2/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.3.2/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.3.2/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.3.2/dlt/version.py
+-rw-r--r--   0        0        0     4460 2023-06-25 21:57:41.225402 dlt-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     7704 1970-01-01 00:00:00.000000 dlt-0.3.2/setup.py
+-rw-r--r--   0        0        0     7706 1970-01-01 00:00:00.000000 dlt-0.3.2/PKG-INFO
```

### Comparing `dlt-0.3.1a0/LICENSE.txt` & `dlt-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/README.md` & `dlt-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 - **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.
 - **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.
 - **Incremental Loading:** Load only new or changed data and avoid loading old records again.
 - **Open Source:** Free and Apache 2.0 Licensed.
 
 ## Ready to use Sources and Destinations
 
-Explore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/verified-sources/chess) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/destinations/bigquery).
+Explore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/dlt-ecosystem/verified-sources) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/dlt-ecosystem/destinations).
 
 ## Documentation
 
 For detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).
 
 ## Examples
```

### Comparing `dlt-0.3.1a0/dlt/__init__.py` & `dlt-0.3.2/dlt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     $ dlt pipeline dlt_magnus_games show
 
 
 Or start with our pipeline template with sample chess.com data loaded to bigquery
 
     $ dlt init chess duckdb
 
-For more detailed info, see https://dlthub.com/docs/getting-started
+For more detailed info, see https://dlthub.com/docs/walkthroughs
 """
 
 from dlt.version import __version__
 from dlt.common.configuration.accessors import config, secrets
 from dlt.common.typing import TSecretValue as _TSecretValue
 from dlt.common.configuration.specs import CredentialsConfiguration as _CredentialsConfiguration
 from dlt.common.pipeline import source_state as state
```

### Comparing `dlt-0.3.1a0/dlt/cli/_dlt.py` & `dlt-0.3.2/dlt/cli/_dlt.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 from dlt.common.schema import Schema
 from dlt.common.typing import DictStrAny
 from dlt.common.runners import Venv
 
 import dlt.cli.echo as fmt
 from dlt.cli import utils
 from dlt.cli.init_command import init_command, list_verified_sources_command, DLT_INIT_DOCS_URL, DEFAULT_VERIFIED_SOURCES_REPO
-from dlt.cli.deploy_command import PipelineWasNotRun, deploy_command, DLT_DEPLOY_DOCS_URL, DeploymentMethods, COMMAND_DEPLOY_REPO_LOCATION
+from dlt.cli.deploy_command import PipelineWasNotRun, deploy_command, DLT_DEPLOY_DOCS_URL, DeploymentMethods, COMMAND_DEPLOY_REPO_LOCATION, SecretFormats
 from dlt.cli.pipeline_command import pipeline_command, DLT_PIPELINE_COMMAND_DOCS_URL
 from dlt.cli.telemetry_command import DLT_TELEMETRY_DOCS_URL, change_telemetry_status_command, telemetry_status_command
 from dlt.pipeline.exceptions import CannotRestorePipelineException
 
 
 @utils.track_command("init", False, "source_name", "destination_name")
 def init_command_wrapper(source_name: str, destination_name: str, use_generic_template: bool, repo_location: str, branch: str) -> int:
     try:
         init_command(source_name, destination_name, use_generic_template, repo_location, branch)
     except Exception as ex:
         click.secho(str(ex), err=True, fg="red")
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_INIT_DOCS_URL))
-        raise
+        return -1
     return 0
 
 
 @utils.track_command("list_sources", False)
 def list_verified_sources_command_wrapper(repo_location: str, branch: str) -> int:
     try:
         list_verified_sources_command(repo_location, branch)
@@ -38,58 +38,52 @@
         click.secho(str(ex), err=True, fg="red")
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_INIT_DOCS_URL))
         return -1
     return 0
 
 
 @utils.track_command("deploy", False, "deployment_method")
-def deploy_command_wrapper(
-    pipeline_script_path: str,
-    deployment_method: str,
-    schedule: Optional[str],
-    run_on_push: bool,
-    run_on_dispatch: bool,
-    repo_location: str,
-    branch: Optional[str]) -> int:
+def deploy_command_wrapper(pipeline_script_path: str, deployment_method: str, repo_location: str, branch: Optional[str] = None, **kwargs: Any
+) -> int:
     try:
         utils.ensure_git_command("deploy")
     except Exception as ex:
         click.secho(str(ex), err=True, fg="red")
         return -1
 
     from git import InvalidGitRepositoryError, NoSuchPathError
     try:
-        deploy_command(pipeline_script_path, deployment_method, schedule, run_on_push, run_on_dispatch, repo_location, branch)
+        deploy_command(pipeline_script_path=pipeline_script_path, deployment_method=deployment_method, repo_location=repo_location, branch=branch, **kwargs)
     except (CannotRestorePipelineException, PipelineWasNotRun) as ex:
         click.secho(str(ex), err=True, fg="red")
         fmt.note("You must run the pipeline locally successfully at least once in order to deploy it.")
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_DEPLOY_DOCS_URL))
-        return -1
+        return -2
     except InvalidGitRepositoryError:
         click.secho(
             "No git repository found for pipeline script %s." % fmt.bold(pipeline_script_path),
             err=True,
             fg="red"
         )
         fmt.note("If you do not have a repository yet, you can do either of:")
         fmt.note("- Run the following command to initialize new repository: %s" % fmt.bold("git init"))
         fmt.note("- Add your local code to Github as described here: %s" % fmt.bold("https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/adding-locally-hosted-code-to-github"))
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_DEPLOY_DOCS_URL))
-        return -1
+        return -3
     except NoSuchPathError as path_ex:
         click.secho(
             "The pipeline script does not exist\n%s" % str(path_ex),
             err=True,
             fg="red"
         )
-        return -1
+        return -4
     except Exception as ex:
         click.secho(str(ex), err=True, fg="red")
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_DEPLOY_DOCS_URL))
-        return -1
+        return -5
         # TODO: display stack trace if with debug flag
     return 0
 
 
 @utils.track_command("pipeline", True, "operation")
 def pipeline_command_wrapper(
         operation: str, pipeline_name: str, pipelines_dir: str, verbosity: int, **command_kwargs: Any
@@ -104,15 +98,15 @@
     except Exception as ex:
         click.secho(str(ex), err=True, fg="red")
         return 1
 
 
 @utils.track_command("schema", False, "operation")
 def schema_command_wrapper(file_path: str, format_: str, remove_defaults: bool) -> int:
-    with open(file_path, "br") as f:
+    with open(file_path, "rb") as f:
         if os.path.splitext(file_path)[1][1:] == "json":
             schema_dict: DictStrAny = json.load(f)
         else:
             schema_dict = yaml.safe_load(f)
     s = Schema.from_dict(schema_dict)
     if format_ == "json":
         schema_str = json.dumps(s.to_dict(remove_defaults=remove_defaults), pretty=True)
@@ -192,27 +186,30 @@
     init_cmd.add_argument("--list-verified-sources", "-l",  default=False, action="store_true", help="List available verified sources")
     init_cmd.add_argument("source", nargs='?', help="Name of data source for which to create a pipeline. Adds existing verified source or creates a new pipeline template if verified source for your data source is not yet implemented.")
     init_cmd.add_argument("destination", nargs='?', help="Name of a destination ie. bigquery or redshift")
     init_cmd.add_argument("--location", default=DEFAULT_VERIFIED_SOURCES_REPO, help="Advanced. Uses a specific url or local path to verified sources repository.")
     init_cmd.add_argument("--branch", default=None, help="Advanced. Uses specific branch of the init repository to fetch the template.")
     init_cmd.add_argument("--generic", default=False, action="store_true", help="When present uses a generic template with all the dlt loading code present will be used. Otherwise a debug template is used that can be immediately run to get familiar with the dlt sources.")
 
+    # deploy
     deploy_cmd = subparsers.add_parser("deploy", help="Creates a deployment package for a selected pipeline script")
     deploy_cmd.add_argument("pipeline_script_path", metavar="pipeline-script-path", help="Path to a pipeline script")
-    deploy_cmd.add_argument(
-        "deployment_method",
-        metavar="deployment-method",
-        choices=list(map(lambda value: value.value, DeploymentMethods.__members__.values())),
-        default=DeploymentMethods.github_actions.value,
-        help="Deployment method: %s" % ", ".join(map(lambda value: value.value, DeploymentMethods.__members__.values())))
     deploy_cmd.add_argument("--schedule", required=False, help="A schedule with which to run the pipeline, in cron format. Example: '*/30 * * * *' will run the pipeline every 30 minutes.")
-    deploy_cmd.add_argument("--run-manually", default=True, action="store_true", help="Allows the pipeline to be run manually form Github Actions UI.")
-    deploy_cmd.add_argument("--run-on-push", default=False, action="store_true", help="Runs the pipeline with every push to the repository.")
     deploy_cmd.add_argument("--location", default=COMMAND_DEPLOY_REPO_LOCATION, help="Advanced. Uses a specific url or local path to pipelines repository.")
     deploy_cmd.add_argument("--branch", default=None, help="Advanced. Uses specific branch of the deploy repository to fetch the template.")
+    deploy_sub_parsers = deploy_cmd.add_subparsers(dest="deployment_method")
+
+    # deploy github actions
+    deploy_github_cmd = deploy_sub_parsers.add_parser(DeploymentMethods.github_actions.value, help="Deploys the pipeline to Github Actions")
+    deploy_github_cmd.add_argument("--run-manually", default=True, action="store_true", help="Allows the pipeline to be run manually form Github Actions UI.")
+    deploy_github_cmd.add_argument("--run-on-push", default=False, action="store_true", help="Runs the pipeline with every push to the repository.")
+
+    # deploy airflow composer
+    deploy_airflow_cmd = deploy_sub_parsers.add_parser(DeploymentMethods.airflow_composer.value, help="Deploys the pipeline to Airflow")
+    deploy_airflow_cmd.add_argument("--secrets-format", default=SecretFormats.env, choices=[v.value for v in SecretFormats], required=False, help="Format of the secrets")
 
     schema = subparsers.add_parser("schema", help="Shows, converts and upgrades schemas")
     schema.add_argument("file", help="Schema file name, in yaml or json format, will autodetect based on extension")
     schema.add_argument("--format", choices=["json", "yaml"], default="yaml", help="Display schema in this format")
     schema.add_argument("--remove-defaults", action="store_true", help="Does not show default hint values")
 
     pipe_cmd = subparsers.add_parser("pipeline", help="Operations on pipelines that were ran locally")
@@ -281,15 +278,22 @@
         else:
             if not args.source or not args.destination:
                 init_cmd.print_usage()
                 return -1
             else:
                 return init_command_wrapper(args.source, args.destination, args.generic, args.location, args.branch)
     elif args.command == "deploy":
-        return deploy_command_wrapper(args.pipeline_script_path, args.deployment_method, args.schedule, args.run_on_push, args.run_manually, args.location, args.branch)
+        deploy_args = vars(args)
+        return deploy_command_wrapper(
+            pipeline_script_path=deploy_args.pop("pipeline_script_path"),
+            deployment_method=deploy_args.pop("deployment_method"),
+            repo_location=deploy_args.pop("location"),
+            branch=deploy_args.pop("branch"),
+            **deploy_args
+        )
     elif args.command == "telemetry":
         return telemetry_status_command_wrapper()
     else:
         print_help(parser)
         return -1
```

### Comparing `dlt-0.3.1a0/dlt/cli/config_toml_writer.py` & `dlt-0.3.2/dlt/cli/config_toml_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,16 @@
     overwrite_existing: bool,
     default_value: Any = None,
     is_default_of_interest: bool = False
 ) -> None:
     # skip if table contains the name already
     if name in toml_table and not overwrite_existing:
         return
-    # do not dump final fields
-    if is_final_type(hint) or is_optional_type(hint):
+    # do not dump final and optional fields if they are not of special interest
+    if (is_final_type(hint) or is_optional_type(hint) or default_value is not None) and not is_default_of_interest:
         return
     # get the inner hint to generate cool examples
     hint = extract_inner_hint(hint)
     if is_base_configuration_inner_hint(hint):
         inner_table = tomlkit.table(is_super_table=True)
         write_spec(inner_table, hint(), overwrite_existing)
         if len(inner_table) > 0:
@@ -71,15 +71,15 @@
     else:
         if default_value is None:
             example_value = generate_typed_example(name, hint)
             toml_table[name] = example_value
             # tomlkit not supporting comments on boolean
             if not isinstance(example_value, bool):
                 toml_table[name].comment("please set me up!")
-        elif is_default_of_interest:
+        else:
             toml_table[name] = default_value
 
 
 def write_spec(toml_table: TOMLTable, config: BaseConfiguration, overwrite_existing: bool) -> None:
     for name, hint in config.get_resolvable_fields().items():
         default_value = getattr(config, name, None)
         # check if field is of particular interest and should be included if it has default
```

### Comparing `dlt-0.3.1a0/dlt/cli/deploy_command.py` & `dlt-0.3.2/dlt/cli/deploy_command.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,75 +1,60 @@
 import os
-from typing import Optional, Any
+from typing import Optional, Any, Type
 import yaml
 from enum import Enum
 from importlib.metadata import version as pkg_version
 
-from dlt.common.configuration.providers import SECRETS_TOML
+from dlt.common.configuration.providers import SECRETS_TOML, SECRETS_TOML_KEY, StringTomlProvider
 from dlt.common.configuration.paths import make_dlt_settings_path
 from dlt.common.configuration.utils import serialize_value
 from dlt.common.git import is_dirty
 
 from dlt.cli import utils
 from dlt.cli import echo as fmt
-from dlt.cli.deploy_command_helpers import (BaseDeployment, ask_files_overwrite, generate_pip_freeze, github_origin_to_url, serialize_templated_yaml,
-                                            wrap_template_str, PipelineWasNotRun)
+from dlt.cli.deploy_command_helpers import (PipelineWasNotRun, BaseDeployment, ask_files_overwrite, generate_pip_freeze, github_origin_to_url, serialize_templated_yaml,
+                                            wrap_template_str)
 
 from dlt.version import DLT_PKG_NAME
 
 from dlt.common.destination.reference import DestinationReference
 
 REQUIREMENTS_GITHUB_ACTION = "requirements_github_action.txt"
 DLT_DEPLOY_DOCS_URL = "https://dlthub.com/docs/walkthroughs/deploy-a-pipeline"
-DLT_AIRFLOW_GCP_DOCS_URL = "https://dlthub.com/docs/running-in-production/orchestrators/airflow-gcp-cloud-composer"
+DLT_AIRFLOW_GCP_DOCS_URL = "https://dlthub.com/docs/walkthroughs/deploy-a-pipeline/deploy-with-airflow-composer"
 AIRFLOW_GETTING_STARTED = "https://airflow.apache.org/docs/apache-airflow/stable/start.html"
 AIRFLOW_DAG_TEMPLATE_SCRIPT = "dag_template.py"
 AIRFLOW_CLOUDBUILD_YAML = "cloudbuild.yaml"
 COMMAND_REPO_LOCATION = "https://github.com/dlt-hub/dlt-%s-template.git"
 COMMAND_DEPLOY_REPO_LOCATION = COMMAND_REPO_LOCATION % "deploy"
 
 
 class DeploymentMethods(Enum):
     github_actions = "github-action"
     airflow_composer = "airflow-composer"
 
 
-def deploy_command(
-    pipeline_script_path: str,
-    deployment_method: str,
-    schedule: Optional[str],
-    run_on_push: bool,
-    run_on_dispatch: bool,
-    repo_location: str,
-    branch: Optional[str] = None,
+class SecretFormats(Enum):
+    env = "env"
+    toml = "toml"
+
+
+def deploy_command(pipeline_script_path: str, deployment_method: str, repo_location: str, branch: Optional[str] = None, **kwargs: Any
 ) -> None:
+
     # get current repo local folder
-    deployment_obj: BaseDeployment = None
+    deployment_class: Type[BaseDeployment] = None
     if deployment_method == DeploymentMethods.github_actions.value:
-        deployment_obj = GithubActionDeployment(
-            pipeline_script_path=pipeline_script_path,
-            schedule=schedule,
-            run_on_push=run_on_push,
-            run_on_dispatch=run_on_dispatch,
-            repo_location=repo_location,
-            branch=branch
-        )
+        deployment_class = GithubActionDeployment
     elif deployment_method == DeploymentMethods.airflow_composer.value:
-        deployment_obj = AirflowDeployment(
-            pipeline_script_path=pipeline_script_path,
-            schedule=schedule,
-            run_on_push=run_on_push,
-            run_on_dispatch=run_on_dispatch,
-            repo_location=repo_location,
-            branch=branch
-        )
+        deployment_class = AirflowDeployment
     else:
         raise ValueError(f"Deployment method '{deployment_method}' is not supported. Only {', '.join([m.value for m in DeploymentMethods])} are available.'")
 
-    deployment_obj.run_deployment()
+    deployment_class(pipeline_script_path=pipeline_script_path, location=repo_location, branch=branch, **kwargs).run_deployment()
 
 
 class GithubActionDeployment(BaseDeployment):
     def _generate_workflow(self, *args: Optional[Any]) -> None:
         self.deployment_method = DeploymentMethods.github_actions.value
         if self.schedule_description is None:
             raise ValueError(
@@ -244,23 +229,36 @@
         ))
         fmt.echo("2. Set _BUCKET_NAME up in %s/%s file. " % (
             fmt.bold(utils.AIRFLOW_BUILD_FOLDER), fmt.bold(AIRFLOW_CLOUDBUILD_YAML),
         ))
         if len(self.secret_envs) == 0 and len(self.envs) == 0:
             fmt.echo("3. Your pipeline does not seem to need any secrets.")
         else:
-            fmt.echo("3. Add the following secret values (typically stored in %s): \n%s\n%s\nin ENVIRONMENT VARIABLES using Google Composer UI" % (
-                fmt.bold(make_dlt_settings_path(SECRETS_TOML)),
-                fmt.bold("\n".join(self.env_prov.get_key_name(s_v.key, *s_v.sections) for s_v in self.secret_envs)),
-                fmt.bold("\n".join(self.env_prov.get_key_name(v.key, *v.sections) for v in self.envs)),
-            ))
-            fmt.echo()
-            # if fmt.confirm("Do you want to list the environment variables in the format suitable for Airflow?", default=True):
-            self._echo_secrets()
-            self._echo_envs()
+            if self.secrets_format == SecretFormats.env.value:
+                fmt.echo("3. Add the following secret values (typically stored in %s): \n%s\n%s\nin ENVIRONMENT VARIABLES using Google Composer UI" % (
+                    fmt.bold(make_dlt_settings_path(SECRETS_TOML)),
+                    fmt.bold("\n".join(self.env_prov.get_key_name(s_v.key, *s_v.sections) for s_v in self.secret_envs)),
+                    fmt.bold("\n".join(self.env_prov.get_key_name(v.key, *v.sections) for v in self.envs)),
+                ))
+                fmt.echo()
+                # if fmt.confirm("Do you want to list the environment variables in the format suitable for Airflow?", default=True):
+                self._echo_secrets()
+                self._echo_envs()
+            elif self.secrets_format == SecretFormats.toml.value:
+                # build toml
+                fmt.echo(f"3. Add the following toml-string in the Google Composer UI as the {SECRETS_TOML_KEY} variable.")
+                fmt.echo()
+                toml_provider = StringTomlProvider("")
+                for s_v in self.secret_envs:
+                    toml_provider.set_value(s_v.key, s_v.value, None, *s_v.sections)
+                for s_v in self.envs:
+                    toml_provider.set_value(s_v.key, s_v.value, None, *s_v.sections)
+                fmt.echo(toml_provider.dumps())
+            else:
+                raise ValueError(self.secrets_format)
 
         fmt.echo("4. Add dlt package below using Google Composer UI.")
         fmt.echo(fmt.bold(self.artifacts["requirements_txt"]))
         fmt.note("You may need to add more packages ie. when your source requires additional dependencies")
         fmt.echo("5. Commit and push the pipeline files to github:")
         fmt.echo("a. Add stage deployment files to commit. Use your Git UI or the following command")
```

### Comparing `dlt-0.3.1a0/dlt/cli/deploy_command_helpers.py` & `dlt-0.3.2/dlt/cli/deploy_command_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,26 +33,29 @@
 GITHUB_URL = "https://github.com/"
 
 
 class BaseDeployment(abc.ABC):
     def __init__(
         self,
         pipeline_script_path: str,
+        location: str,
         schedule: Optional[str],
-        run_on_push: bool,
-        run_on_dispatch: bool,
-        repo_location: str,
-        branch: Optional[str] = None
+        run_on_push: bool = False,
+        run_on_dispatch: bool = False,
+        branch: Optional[str] = None,
+        secrets_format: Optional[str] = None,
+        **_kwargs: Any
     ):
         self.pipeline_script_path = pipeline_script_path
         self.schedule = schedule
         self.run_on_push = run_on_push
         self.run_on_dispatch = run_on_dispatch
-        self.repo_location = repo_location
+        self.repo_location = location
         self.branch = branch
+        self.secrets_format = secrets_format
 
         self.pipelines_dir: Optional[str] = None
         self.pipeline_name: Optional[str] = None
 
         self.deployment_method: str
         self.repo: Repo
         self.repo_storage: FileStorage
@@ -269,15 +272,15 @@
 
     # compute excludes to compute includes as set difference
     excludes = set(req.strip() for req in requirements_blacklist if not req.strip().startswith("#"))
     includes = [node.project_name for node in nodes if node.project_name not in excludes]
 
     # prepare new filtered DAG
     tree = tree.sort()
-    tree = tree.filter(includes, None)
+    tree = tree.filter_nodes(includes, None)
     nodes = tree.keys()
     branch_keys = {r.key for r in chain.from_iterable(tree.values())}
     nodes = [p for p in nodes if p.key not in branch_keys]
 
     # detect and warn on conflict
     conflicts = pipdeptree.conflicting_deps(tree)
     cycles = pipdeptree.cyclic_deps(tree)
```

### Comparing `dlt-0.3.1a0/dlt/cli/echo.py` & `dlt-0.3.2/dlt/cli/echo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/cli/init_command.py` & `dlt-0.3.2/dlt/cli/init_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/cli/pipeline_command.py` & `dlt-0.3.2/dlt/cli/pipeline_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         for k, v in state["_local"].items():
             if not isinstance(v, dict):
                 fmt.echo("%s: %s" % (fmt.style(k, fg="green"), v))
         fmt.echo()
         if p.default_schema_name is None:
             fmt.warning("This pipeline does not have a default schema")
         else:
-            is_single_schema = len(p.schema_names)
+            is_single_schema = len(p.schema_names) == 1
             for schema_name in  p.schema_names:
                 fmt.echo("Resources in schema: %s" % fmt.bold(schema_name))
                 schema = p.schemas[schema_name]
                 data_tables = {t["name"]: t for t in schema.data_tables()}
                 for resource_name, tables in group_tables_by_resource(data_tables).items():
                     res_state_slots = 0
                     if sources_state:
```

### Comparing `dlt-0.3.1a0/dlt/cli/pipeline_files.py` & `dlt-0.3.2/dlt/cli/pipeline_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             posix_file = posixpath.join(*Path(posix_file).parts)
             try:
                 blob_sha3 = tree.join(posix_file).hexsha
             except KeyError:
                 # if directory is dirty and we do not have git sha
                 blob_sha3 = None
 
-            with open(os.path.join(repo_path, file), "br") as f:
+            with open(os.path.join(repo_path, file), "rb") as f:
                 file_blob = f.read()
             files_sha[file] = {
                 "commit_sha": commit_sha,
                 "git_sha": blob_sha3,
                 "sha3_256":  hashlib.sha3_256(file_blob).hexdigest()
             }
 
@@ -221,15 +221,15 @@
     dest_storage: FileStorage
 ) -> Tuple[List[str], List[str]]:
     """Use files index from .sources to identify modified files via sha3 content hash"""
 
     conflict_modified: List[str] = []
 
     def is_file_modified(file: str, entry: TVerifiedSourceFileEntry) -> bool:
-        with dest_storage.open_file(file, "br") as f:
+        with dest_storage.open_file(file, "rb") as f:
             file_blob = f.read()
         # file exists but was not changed
         return hashlib.sha3_256(file_blob).hexdigest() != entry["sha3_256"]
 
     for file, entry in remote_new.items():
         if dest_storage.has_file(file):
             # if incoming file is different from local
```

### Comparing `dlt-0.3.1a0/dlt/cli/source_detection.py` & `dlt-0.3.2/dlt/cli/source_detection.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/cli/telemetry_command.py` & `dlt-0.3.2/dlt/cli/telemetry_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/cli/utils.py` & `dlt-0.3.2/dlt/cli/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/arithmetics.py` & `dlt-0.3.2/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/accessors.py` & `dlt-0.3.2/dlt/common/configuration/accessors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/container.py` & `dlt-0.3.2/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/exceptions.py` & `dlt-0.3.2/dlt/common/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/inject.py` & `dlt-0.3.2/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/paths.py` & `dlt-0.3.2/dlt/common/configuration/paths.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/providers/airflow.py` & `dlt-0.3.2/dlt/common/configuration/providers/airflow.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/providers/context.py` & `dlt-0.3.2/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/providers/dictionary.py` & `dlt-0.3.2/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/providers/environ.py` & `dlt-0.3.2/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/providers/google_secrets.py` & `dlt-0.3.2/dlt/common/configuration/providers/google_secrets.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/providers/provider.py` & `dlt-0.3.2/dlt/common/configuration/providers/provider.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/providers/toml.py` & `dlt-0.3.2/dlt/common/configuration/providers/toml.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,35 @@
         return True
 
     @property
     def is_empty(self) -> bool:
         return len(self._toml.body) == 0
 
 
+class StringTomlProvider(BaseTomlProvider):
+
+    def __init__(self, toml_string: str) -> None:
+        super().__init__(StringTomlProvider.loads(toml_string))
+
+    def dumps(self) -> str:
+        return tomlkit.dumps(self._toml)
+
+    @staticmethod
+    def loads(toml_string: str) -> tomlkit.TOMLDocument:
+        return tomlkit.parse(toml_string)
+
+    @property
+    def supports_secrets(self) -> bool:
+        return True
+
+    @property
+    def name(self) -> str:
+        return "memory"
+
+
 class VaultTomlProvider(BaseTomlProvider):
     """A toml-backed Vault abstract config provider.
 
     This provider allows implementation of providers that store secrets in external vaults: like Hashicorp, Google Secrets or Airflow Metadata.
     The basic working principle is obtain config and secrets values from Vault keys and reconstitute a `secrets.toml` like document that is then used
     as a cache.
```

### Comparing `dlt-0.3.1a0/dlt/common/configuration/resolve.py` & `dlt-0.3.2/dlt/common/configuration/resolve.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/specs/__init__.py` & `dlt-0.3.2/dlt/common/configuration/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/specs/api_credentials.py` & `dlt-0.3.2/dlt/common/configuration/specs/api_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/specs/aws_credentials.py` & `dlt-0.3.2/dlt/common/configuration/specs/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.3.2/dlt/common/configuration/specs/base_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/specs/config_providers_context.py` & `dlt-0.3.2/dlt/common/configuration/specs/config_providers_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.3.2/dlt/common/configuration/specs/config_section_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/specs/connection_string_credentials.py` & `dlt-0.3.2/dlt/common/configuration/specs/connection_string_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/specs/exceptions.py` & `dlt-0.3.2/dlt/common/configuration/specs/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/specs/gcp_credentials.py` & `dlt-0.3.2/dlt/common/configuration/specs/gcp_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/specs/known_sections.py` & `dlt-0.3.2/dlt/common/configuration/specs/known_sections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.3.2/dlt/common/configuration/specs/run_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/configuration/utils.py` & `dlt-0.3.2/dlt/common/configuration/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/data_types/type_helpers.py` & `dlt-0.3.2/dlt/common/data_types/type_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/data_writers/buffered.py` & `dlt-0.3.2/dlt/common/data_writers/buffered.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import gzip
 from typing import List, IO, Any, Optional, Type
 
 from dlt.common.utils import uniq_id
 from dlt.common.typing import TDataItem, TDataItems
 from dlt.common.data_writers import TLoaderFileFormat
 from dlt.common.data_writers.exceptions import BufferedDataWriterClosed, DestinationCapabilitiesRequired, InvalidFileNameTemplateException
 from dlt.common.data_writers.writers import DataWriter
@@ -14,42 +15,46 @@
 class BufferedDataWriter:
 
     @configspec
     class BufferedDataWriterConfiguration(BaseConfiguration):
         buffer_max_items: int = 5000
         file_max_items: Optional[int] = None
         file_max_bytes: Optional[int] = None
+        disable_compression: bool = False
         _caps: Optional[DestinationCapabilitiesContext] = None
 
         __section__ = known_sections.DATA_WRITER
 
 
     @with_config(spec=BufferedDataWriterConfiguration)
     def __init__(
         self,
         file_format: TLoaderFileFormat,
         file_name_template: str,
         *,
         buffer_max_items: int = 5000,
         file_max_items: int = None,
         file_max_bytes: int = None,
+        disable_compression: bool = False,
         _caps: DestinationCapabilitiesContext = None
     ):
         self.file_format = file_format
         self._file_format_spec = DataWriter.data_format_from_file_format(self.file_format)
         if self._file_format_spec.requires_destination_capabilities and not _caps:
             raise DestinationCapabilitiesRequired(file_format)
         self._caps = _caps
         # validate if template has correct placeholders
         self.file_name_template = file_name_template
         self.closed_files: List[str] = []  # all fully processed files
         # buffered items must be less than max items in file
         self.buffer_max_items = min(buffer_max_items, file_max_items or buffer_max_items)
         self.file_max_bytes = file_max_bytes
         self.file_max_items = file_max_items
+        # the open function is either gzip.open or open
+        self.open = gzip.open if self._file_format_spec.supports_compression and not disable_compression else open
 
         self._current_columns: TTableSchemaColumns = None
         self._file_name: str = None
         self._buffered_items: List[TDataItem] = []
         self._writer: DataWriter = None
         self._file: IO[Any] = None
         self._closed = False
@@ -78,15 +83,15 @@
             self._flush_items()
         # rotate the file if max_bytes exceeded
         if self._file:
             # rotate on max file size
             if self.file_max_bytes and self._file.tell() >= self.file_max_bytes:
                 self._rotate_file()
             # rotate on max items
-            if self.file_max_items and self._writer.items_count >= self.file_max_items:
+            elif self.file_max_items and self._writer.items_count >= self.file_max_items:
                 self._rotate_file()
 
     def close(self) -> None:
         self._ensure_open()
         self._flush_and_close_file()
         self._closed = True
 
@@ -106,17 +111,17 @@
 
     def _flush_items(self) -> None:
         if len(self._buffered_items) > 0:
             # we only open a writer when there are any items in the buffer and first flush is requested
             if not self._writer:
                 # create new writer and write header
                 if self._file_format_spec.is_binary_format:
-                    self._file = open(self._file_name, "wb")
+                    self._file = self.open(self._file_name, "wb") # type: ignore
                 else:
-                    self._file = open(self._file_name, "wt", encoding="utf-8")
+                    self._file = self.open(self._file_name, "wt", encoding="utf-8") # type: ignore
                 self._writer = DataWriter.from_file_format(self.file_format, self._file, caps=self._caps)
                 self._writer.write_header(self._current_columns)
             # write buffer
             self._writer.write_data(self._buffered_items)
             self._buffered_items.clear()
 
     def _flush_and_close_file(self) -> None:
```

### Comparing `dlt-0.3.1a0/dlt/common/data_writers/escape.py` & `dlt-0.3.2/dlt/common/data_writers/escape.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,7 +64,13 @@
 
 escape_postgres_identifier = escape_redshift_identifier
 
 
 def escape_bigquery_identifier(v: str) -> str:
     # https://cloud.google.com/bigquery/docs/reference/standard-sql/lexical
     return "`" + v.replace("\\", "\\\\").replace("`","\\`") + "`"
+
+
+def escape_snowflake_identifier(v: str) -> str:
+    # Snowcase uppercase all identifiers unless quoted. Match this here so queries on information schema work without issue
+    # See also https://docs.snowflake.com/en/sql-reference/identifiers-syntax#double-quoted-identifiers
+    return escape_postgres_identifier(v.upper())
```

### Comparing `dlt-0.3.1a0/dlt/common/data_writers/exceptions.py` & `dlt-0.3.2/dlt/common/data_writers/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/data_writers/writers.py` & `dlt-0.3.2/dlt/common/data_writers/writers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import abc
+
 # import jsonlines
 from dataclasses import dataclass
-from typing import Any, Dict, Sequence, IO, Type
+from typing import Any, Dict, Sequence, IO, Type, Optional, List, cast
 
 from dlt.common import json
 from dlt.common.typing import StrAny
 from dlt.common.schema.typing import TTableSchemaColumns
 from dlt.common.destination import TLoaderFileFormat, DestinationCapabilitiesContext
-
+from dlt.common.configuration import with_config, known_sections, configspec
+from dlt.common.configuration.specs import BaseConfiguration
 
 @dataclass
 class TFileFormatSpec:
     file_format: TLoaderFileFormat
     file_extension: str
     is_binary_format: bool
     supports_schema_changes: bool
     requires_destination_capabilities: bool = False
+    supports_compression: bool = False
 
 
 class DataWriter(abc.ABC):
     def __init__(self, f: IO[Any], caps: DestinationCapabilitiesContext = None) -> None:
         self._f = f
         self._caps = caps
         self.items_count = 0
@@ -62,14 +65,16 @@
     def class_factory(file_format: TLoaderFileFormat) -> Type["DataWriter"]:
         if file_format == "jsonl":
             return JsonlWriter
         elif file_format == "puae-jsonl":
             return JsonlListPUAEncodeWriter
         elif file_format == "insert_values":
             return InsertValuesWriter
+        elif file_format == "parquet":
+            return ParquetDataWriter  # type: ignore
         else:
             raise ValueError(file_format)
 
 
 class JsonlWriter(DataWriter):
 
     def write_header(self, columns_schema: TTableSchemaColumns) -> None:
@@ -82,30 +87,42 @@
             self._f.write(b"\n")
 
     def write_footer(self) -> None:
         pass
 
     @classmethod
     def data_format(cls) -> TFileFormatSpec:
-        return TFileFormatSpec("jsonl", "jsonl", True, True)
+        return TFileFormatSpec(
+            "jsonl",
+            file_extension="jsonl",
+            is_binary_format=True,
+            supports_schema_changes=True,
+            supports_compression=True,
+        )
 
 
 class JsonlListPUAEncodeWriter(JsonlWriter):
 
     def write_data(self, rows: Sequence[Any]) -> None:
         # skip JsonlWriter when calling super
         super(JsonlWriter, self).write_data(rows)
         # write all rows as one list which will require to write just one line
         # encode types with PUA characters
         json.typed_dump(rows, self._f)
         self._f.write(b"\n")
 
     @classmethod
     def data_format(cls) -> TFileFormatSpec:
-        return TFileFormatSpec("puae-jsonl", "jsonl", True, True)
+        return TFileFormatSpec(
+            "puae-jsonl",
+            file_extension="jsonl",
+            is_binary_format=True,
+            supports_schema_changes=True,
+            supports_compression=True,
+        )
 
 
 class InsertValuesWriter(DataWriter):
 
     def __init__(self, f: IO[Any], caps: DestinationCapabilitiesContext = None) -> None:
         super().__init__(f, caps)
         self._chunks_written = 0
@@ -148,8 +165,79 @@
 
     def write_footer(self) -> None:
         assert self._chunks_written > 0
         self._f.write(";")
 
     @classmethod
     def data_format(cls) -> TFileFormatSpec:
+        return TFileFormatSpec(
+            "insert_values",
+            file_extension="insert_values",
+            is_binary_format=False,
+            supports_schema_changes=False,
+            supports_compression=True,
+            requires_destination_capabilities=True,
+        )
         return TFileFormatSpec("insert_values", "insert_values", False, False, requires_destination_capabilities=True)
+
+
+@configspec
+class ParquetDataWriterConfiguration(BaseConfiguration):
+    flavor: str = "spark"
+    version: str = "2.4"
+    data_page_size: int = 1024 * 1024
+
+    __section__: str = known_sections.DATA_WRITER
+
+class ParquetDataWriter(DataWriter):
+
+    @with_config(spec=ParquetDataWriterConfiguration)
+    def __init__(self,
+                 f: IO[Any],
+                 caps: DestinationCapabilitiesContext = None,
+                 *,
+                 flavor: str = "spark",
+                 version: str = "2.4",
+                 data_page_size: int = 1024 * 1024
+                 ) -> None:
+        super().__init__(f, caps)
+        from dlt.common.libs.pyarrow import pyarrow
+
+        self.writer: Optional[pyarrow.parquet.ParquetWriter] = None
+        self.schema: Optional[pyarrow.Schema] = None
+        self.complex_indices: List[str] = None
+        self.parquet_flavor = flavor
+        self.parquet_version = version
+        self.parquet_data_page_size = data_page_size
+
+    def write_header(self, columns_schema: TTableSchemaColumns) -> None:
+        from dlt.common.libs.pyarrow import pyarrow, get_py_arrow_datatype
+
+        # build schema
+        self.schema = pyarrow.schema([pyarrow.field(name, get_py_arrow_datatype(schema_item["data_type"]), nullable=schema_item["nullable"]) for name, schema_item in columns_schema.items()])
+        # find row items that are of the complex type (could be abstracted out for use in other writers?)
+        self.complex_indices = [i for i, field in columns_schema.items() if field["data_type"] == "complex"]
+        self.writer = pyarrow.parquet.ParquetWriter(self._f, self.schema, flavor=self.parquet_flavor, version=self.parquet_version, data_page_size=self.parquet_data_page_size)
+
+
+    def write_data(self, rows: Sequence[Any]) -> None:
+        super().write_data(rows)
+        from dlt.common.libs.pyarrow import pyarrow
+
+        # replace complex types with json
+        for key in self.complex_indices:
+            for row in rows:
+                if key in row:
+                    row[key] = json.dumps(row[key]) if row[key] else row[key]
+
+        table = pyarrow.Table.from_pylist(rows, schema=self.schema)
+        # Write
+        self.writer.write_table(table)
+
+    def write_footer(self) -> None:
+        self.writer.close()
+        self.writer = None
+
+
+    @classmethod
+    def data_format(cls) -> TFileFormatSpec:
+        return TFileFormatSpec("parquet", "parquet", True, False, requires_destination_capabilities=True, supports_compression=False)
```

### Comparing `dlt-0.3.1a0/dlt/common/destination/capabilities.py` & `dlt-0.3.2/dlt/common/destination/capabilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 # known loader file formats
 # jsonl - new line separated json documents
 # puae-jsonl - internal extract -> normalize format bases on jsonl
 # insert_values - insert SQL statements
 # sql - any sql statement
-TLoaderFileFormat = Literal["jsonl", "puae-jsonl", "insert_values", "sql"]
+TLoaderFileFormat = Literal["jsonl", "puae-jsonl", "insert_values", "sql", "parquet"]
 
 
 @configspec(init=True)
 class DestinationCapabilitiesContext(ContainerInjectableContext):
     """Injectable destination capabilities required for many Pipeline stages ie. normalize"""
     preferred_loader_file_format: TLoaderFileFormat
     supported_loader_file_formats: List[TLoaderFileFormat]
@@ -34,15 +34,15 @@
     # do not allow to create default value, destination caps must be always explicitly inserted into container
     can_create_default: ClassVar[bool] = False
 
     @staticmethod
     def generic_capabilities(preferred_loader_file_format: TLoaderFileFormat = None) -> "DestinationCapabilitiesContext":
         caps = DestinationCapabilitiesContext()
         caps.preferred_loader_file_format = preferred_loader_file_format
-        caps.supported_loader_file_formats = ["jsonl", "insert_values"]
+        caps.supported_loader_file_formats = ["jsonl", "insert_values", "parquet"]
         caps.escape_identifier = identity
         caps.escape_literal = serialize_value
         caps.max_identifier_length = 65536
         caps.max_column_identifier_length = 65536
         caps.max_query_length = 32 * 1024 * 1024
         caps.is_max_query_length_in_bytes = True
         caps.max_text_data_type_length = 1024 * 1024 * 1024
```

### Comparing `dlt-0.3.1a0/dlt/common/destination/reference.py` & `dlt-0.3.2/dlt/common/destination/reference.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/exceptions.py` & `dlt-0.3.2/dlt/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/git.py` & `dlt-0.3.2/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/json/__init__.py` & `dlt-0.3.2/dlt/common/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/json/_orjson.py` & `dlt-0.3.2/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/json/_simplejson.py` & `dlt-0.3.2/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/jsonpath.py` & `dlt-0.3.2/dlt/common/jsonpath.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/normalizers/configuration.py` & `dlt-0.3.2/dlt/common/normalizers/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/normalizers/json/__init__.py` & `dlt-0.3.2/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/normalizers/json/relational.py` & `dlt-0.3.2/dlt/common/normalizers/json/relational.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/normalizers/naming/direct.py` & `dlt-0.3.2/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.3.2/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.3.2/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/normalizers/naming/naming.py` & `dlt-0.3.2/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.3.2/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/normalizers/utils.py` & `dlt-0.3.2/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/pipeline.py` & `dlt-0.3.2/dlt/common/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from dlt.common.exceptions import DestinationHasFailedJobs, PipelineStateNotAvailable, ResourceNameNotAvailable, SourceSectionNotAvailable
 from dlt.common.schema import Schema
 from dlt.common.schema.typing import TColumnKey, TColumnSchema, TWriteDisposition
 from dlt.common.source import get_current_pipe_name
 from dlt.common.storages.load_storage import LoadPackageInfo
 from dlt.common.typing import DictStrAny, REPattern
 from dlt.common.jsonpath import delete_matches, TAnyJsonPath
+from dlt.common.data_writers.writers import TLoaderFileFormat
 
 
 class ExtractInfo(NamedTuple):
     """A tuple holding information on extracted data items. Returned by pipeline `extract` method."""
     def asdict(self) -> DictStrAny:
         return {}
 
@@ -175,16 +176,17 @@
         destination: TDestinationReferenceArg = None,
         dataset_name: str = None,
         credentials: Any = None,
         table_name: str = None,
         write_disposition: TWriteDisposition = None,
         columns: Sequence[TColumnSchema] = None,
         primary_key: TColumnKey = None,
-        schema: Schema = None
-    ) -> LoadInfo:
+        schema: Schema = None,
+        loader_file_format: TLoaderFileFormat = None
+        ) -> LoadInfo:
         ...
 
     def _set_context(self, is_active: bool) -> None:
         """Called when pipeline context activated or deactivate"""
 
     def _make_schema_with_default_name(self) -> Schema:
         """Make a schema from the pipeline name using the name normalizer. "_pipeline" suffix is removed if present"""
```

### Comparing `dlt-0.3.1a0/dlt/common/reflection/spec.py` & `dlt-0.3.2/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/reflection/utils.py` & `dlt-0.3.2/dlt/common/reflection/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/runners/configuration.py` & `dlt-0.3.2/dlt/common/runners/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/runners/pool_runner.py` & `dlt-0.3.2/dlt/common/runners/pool_runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/runners/runnable.py` & `dlt-0.3.2/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/runners/stdout.py` & `dlt-0.3.2/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/runners/synth_pickle.py` & `dlt-0.3.2/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/runners/venv.py` & `dlt-0.3.2/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/runtime/collector.py` & `dlt-0.3.2/dlt/common/runtime/collector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/runtime/exec_info.py` & `dlt-0.3.2/dlt/common/runtime/exec_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/runtime/init.py` & `dlt-0.3.2/dlt/common/runtime/init.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/runtime/logger.py` & `dlt-0.3.2/dlt/common/runtime/logger.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/runtime/prometheus.py` & `dlt-0.3.2/dlt/common/runtime/prometheus.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/runtime/segment.py` & `dlt-0.3.2/dlt/common/runtime/segment.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/runtime/sentry.py` & `dlt-0.3.2/dlt/common/runtime/sentry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/runtime/signals.py` & `dlt-0.3.2/dlt/common/runtime/signals.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/runtime/slack.py` & `dlt-0.3.2/dlt/common/runtime/slack.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/runtime/telemetry.py` & `dlt-0.3.2/dlt/common/runtime/telemetry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/schema/detections.py` & `dlt-0.3.2/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/schema/exceptions.py` & `dlt-0.3.2/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/schema/schema.py` & `dlt-0.3.2/dlt/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/schema/typing.py` & `dlt-0.3.2/dlt/common/schema/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/schema/utils.py` & `dlt-0.3.2/dlt/common/schema/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/source.py` & `dlt-0.3.2/dlt/common/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/storages/__init__.py` & `dlt-0.3.2/dlt/common/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/storages/configuration.py` & `dlt-0.3.2/dlt/common/storages/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/storages/data_item_storage.py` & `dlt-0.3.2/dlt/common/storages/data_item_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/storages/exceptions.py` & `dlt-0.3.2/dlt/common/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/storages/file_storage.py` & `dlt-0.3.2/dlt/common/storages/file_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import gzip
 import os
 import re
 import stat
 import errno
 import tempfile
 import shutil
 import pathvalidate
-from typing import IO, Any, List
+from typing import IO, Any, Optional, List, cast
 from dlt.common.typing import AnyFun
 
 from dlt.common.utils import encoding_for_mode, uniq_id
 
 
 FILE_COMPONENT_INVALID_CHARACTERS = re.compile(r"[.%{}]")
 
@@ -87,14 +88,16 @@
                 os.rmdir(folder_path)
         else:
             raise NotADirectoryError(folder_path)
 
     def open_file(self, relative_path: str, mode: str = "r") -> IO[Any]:
         if "b" not in mode and "t" not in mode:
             mode = mode + self.file_type
+        if "r" in mode:
+            return FileStorage.open_zipsafe_ro(self.make_full_path(relative_path), mode)
         return open(self.make_full_path(relative_path), mode, encoding=encoding_for_mode(mode))
 
     def open_temp(self, delete: bool = False, mode: str = "w", file_type: str = None) -> IO[Any]:
         mode = mode + file_type or self.file_type
         return tempfile.NamedTemporaryFile(dir=self.storage_path, mode=mode, delete=delete, encoding=encoding_for_mode(mode))
 
     def has_file(self, relative_path: str) -> bool:
@@ -247,7 +250,23 @@
     def rmtree_del_ro(action: AnyFun, name: str, exc: Any) -> Any:
         if action is os.unlink or action is os.remove or action is os.rmdir:
             os.chmod(name, stat.S_IWRITE)
             if os.path.isdir(name):
                 os.rmdir(name)
             else:
                 os.remove(name)
+
+    @staticmethod
+    def open_zipsafe_ro(path: str, mode: str = "r", **kwargs: Any) -> IO[Any]:
+        """Opens a file using gzip.open if it is a gzip file, otherwise uses open."""
+        assert "r" in mode, "FileStorage.open_zipsafe_ro only supports read modes"
+        encoding = kwargs.pop("encoding", encoding_for_mode(mode))
+        origmode = str(mode)
+        try:
+            if encoding is not None and mode == "r":
+                mode += "t"  # gzip requires text mode explicitly to use encoding
+            f = gzip.open(path, mode, encoding=encoding, **kwargs)
+            # Force gzip to read the first few bytes and check the magic number
+            f.read(2), f.seek(0)
+            return cast(IO[Any], f)
+        except (gzip.BadGzipFile, OSError):
+            return open(path, origmode, encoding=encoding, **kwargs)
```

### Comparing `dlt-0.3.1a0/dlt/common/storages/live_schema_storage.py` & `dlt-0.3.2/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/storages/load_storage.py` & `dlt-0.3.2/dlt/common/storages/load_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/storages/normalize_storage.py` & `dlt-0.3.2/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/storages/schema_storage.py` & `dlt-0.3.2/dlt/common/storages/schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/storages/transactional_file.py` & `dlt-0.3.2/dlt/common/storages/transactional_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
             name = lock["name"]
             if not name.startswith(self.lock_prefix):
                 continue
             # Purge stale locks
             mtime = self.extract_mtime(lock)
             if now - mtime > timedelta(seconds=TransactionalFile.LOCK_TTL_SECONDS):
                 try: # Janitors can race, so we ignore errors
-                    self._fs.rm(name)
+                    self._fs.rm_file(name)
                 except OSError:
                     pass
                 continue
             # The name is timestamp + random suffix and is time sortable
             output.append(name)
         if not output:
             raise RuntimeError(f"When syncing locks for path {self.path} and lock {self.lock_path} no lock file was found")
@@ -142,15 +142,15 @@
     def rollback(self) -> None:
         """Rolls back the transaction."""
         if not self._is_locked:
             raise RuntimeError("Cannot rollback without a lock.")
         if self._original_contents is not None:
             self.write(self._original_contents)
         elif self._fs.isfile(self.path):
-            self._fs.rm(self.path)
+            self._fs.rm_file(self.path)
 
     def acquire_lock(self, blocking: bool = True, timeout: float = -1, jitter_mean: float = 0) -> bool:
         """Acquires a lock on a path. Mimics the stdlib's `threading.Lock` interface.
 
         Acquire a lock, blocking or non-blocking.
 
         When invoked with the blocking argument set to True (the default), block until
@@ -181,15 +181,15 @@
         self._fs.touch(self.lock_path)
         locks = self._sync_locks()
         active_lock = min(locks)
         start = time.time()
 
         while active_lock != self.lock_path:
             if not blocking or (timeout > 0 and time.time() - start > timeout):
-                self._fs.rm(self.lock_path)
+                self._fs.rm_file(self.lock_path)
                 return False
 
             time.sleep(random.random() + TransactionalFile.POLLING_INTERVAL)
             locks = self._sync_locks()
             if self.lock_path not in locks:
                 self._fs.touch(self.lock_path)
                 locks = self._sync_locks()
@@ -204,15 +204,15 @@
     def release_lock(self) -> None:
         """Releases a lock on a key.
 
         This is idempotent and safe to call multiple times.
         """
         if self._is_locked:
             self._stop_heartbeat()
-            self._fs.rm(self.lock_path)
+            self._fs.rm_file(self.lock_path)
             self._is_locked = False
             self._original_contents = None
 
     @contextmanager
     def lock(self, timeout: t.Optional[float] = None) -> t.Iterator[None]:
         """A context manager that acquires and releases a lock on a path.
```

### Comparing `dlt-0.3.1a0/dlt/common/storages/versioned_storage.py` & `dlt-0.3.2/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/time.py` & `dlt-0.3.2/dlt/common/time.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/typing.py` & `dlt-0.3.2/dlt/common/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/utils.py` & `dlt-0.3.2/dlt/common/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/validation.py` & `dlt-0.3.2/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/common/wei.py` & `dlt-0.3.2/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/destinations/bigquery/__init__.py` & `dlt-0.3.2/dlt/destinations/bigquery/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def _configure(config: BigQueryClientConfiguration = config.value) -> BigQueryClientConfiguration:
     return config
 
 
 def capabilities() -> DestinationCapabilitiesContext:
     caps = DestinationCapabilitiesContext()
     caps.preferred_loader_file_format = "jsonl"
-    caps.supported_loader_file_formats = ["jsonl", "sql"]
+    caps.supported_loader_file_formats = ["jsonl", "sql", "parquet"]
     caps.escape_identifier = escape_bigquery_identifier
     caps.escape_literal = None
     caps.max_identifier_length = 1024
     caps.max_column_identifier_length = 300
     caps.max_query_length = 1024 * 1024
     caps.is_max_query_length_in_bytes = False
     caps.max_text_data_type_length = 10 * 1024 * 1024
```

### Comparing `dlt-0.3.1a0/dlt/destinations/bigquery/bigquery.py` & `dlt-0.3.2/dlt/destinations/bigquery/bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,29 +173,29 @@
                 elif reason in BQ_TERMINAL_REASONS:
                     # google.api_core.exceptions.BadRequest - will not be processed ie bad job name
                     raise LoadJobTerminalException(file_path)
                 else:
                     raise DestinationTransientException(gace)
         return job
 
-    def _get_table_update_sql(self, table_name: str, new_columns: Sequence[TColumnSchema], generate_alter: bool, separate_alters: bool = False) -> str:
+    def _get_table_update_sql(self, table_name: str, new_columns: Sequence[TColumnSchema], generate_alter: bool, separate_alters: bool = False) -> List[str]:
         sql = super()._get_table_update_sql(table_name, new_columns, generate_alter)
         canonical_name = self.sql_client.make_qualified_table_name(table_name)
 
-        cluster_list = [self.capabilities.escape_identifier(c["name"]) for c in new_columns if c.get("cluster", False)]
-        partition_list = [self.capabilities.escape_identifier(c["name"]) for c in new_columns if c.get("partition", False)]
+        cluster_list = [self.capabilities.escape_identifier(c["name"]) for c in new_columns if c.get("cluster")]
+        partition_list = [self.capabilities.escape_identifier(c["name"]) for c in new_columns if c.get("partition")]
 
         # partition by must be added first
         if len(partition_list) > 0:
             if len(partition_list) > 1:
                 raise DestinationSchemaWillNotUpdate(canonical_name, partition_list, "Partition requested for more than one column")
             else:
-                sql += f"\nPARTITION BY DATE({partition_list[0]})"
+                sql[0] = sql[0] + f"\nPARTITION BY DATE({partition_list[0]})"
         if len(cluster_list) > 0:
-                sql += "\nCLUSTER BY " + ",".join(cluster_list)
+            sql[0] = sql[0] + "\nCLUSTER BY " + ",".join(cluster_list)
 
         return sql
 
     def _get_column_def_sql(self, c: TColumnSchema) -> str:
         name = self.capabilities.escape_identifier(c["name"])
         return f"{name} {self._to_db_type(c['data_type'])} {self._gen_not_null(c['nullable'])}"
 
@@ -224,22 +224,28 @@
             return True, schema_table
         except gcp_exceptions.NotFound:
             return False, schema_table
 
     def _create_load_job(self, table_name: str, write_disposition: TWriteDisposition, file_path: str) -> bigquery.LoadJob:
         # append to table for merge loads (append to stage) and regular appends
         bq_wd = bigquery.WriteDisposition.WRITE_TRUNCATE if write_disposition == "replace" else bigquery.WriteDisposition.WRITE_APPEND
+
+        # choose correct source format
+        source_format = bigquery.SourceFormat.NEWLINE_DELIMITED_JSON
+        if file_path.endswith("parquet"):
+            source_format = bigquery.SourceFormat.PARQUET
+
         # if merge then load to staging
         with self.sql_client.with_staging_dataset(write_disposition == "merge"):
             job_id = BigQueryLoadJob.get_job_id_from_file_path(file_path)
             job_config = bigquery.LoadJobConfig(
                 autodetect=False,
                 write_disposition=bq_wd,
                 create_disposition=bigquery.CreateDisposition.CREATE_NEVER,
-                source_format=bigquery.SourceFormat.NEWLINE_DELIMITED_JSON,
+                source_format=source_format,
                 ignore_unknown_values=False,
                 max_bad_records=0)
             with open(file_path, "rb") as f:
                 return self.sql_client.native_connection.load_table_from_file(
                         f,
                         self.sql_client.make_qualified_table_name(table_name, escape=False),
                         job_id=job_id,
```

### Comparing `dlt-0.3.1a0/dlt/destinations/bigquery/sql_client.py` & `dlt-0.3.2/dlt/destinations/bigquery/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/destinations/duckdb/__init__.py` & `dlt-0.3.2/dlt/destinations/duckdb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def _configure(config: DuckDbClientConfiguration = config.value) -> DuckDbClientConfiguration:
     return config
 
 
 def capabilities() -> DestinationCapabilitiesContext:
     caps = DestinationCapabilitiesContext()
     caps.preferred_loader_file_format = "insert_values"
-    caps.supported_loader_file_formats = ["insert_values", "sql"]
+    caps.supported_loader_file_formats = ["insert_values", "parquet", "sql"]
     caps.escape_identifier = escape_postgres_identifier
     caps.escape_literal = escape_duckdb_literal
     caps.max_identifier_length = 65536
     caps.max_column_identifier_length = 65536
     caps.naming_convention = "duck_case"
     caps.max_query_length = 32 * 1024 * 1024
     caps.is_max_query_length_in_bytes = True
```

### Comparing `dlt-0.3.1a0/dlt/destinations/duckdb/configuration.py` & `dlt-0.3.2/dlt/destinations/duckdb/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import threading
 from pathvalidate import is_valid_filepath
-from typing import Any, Final, Optional, Tuple
+from typing import Any, ClassVar, Final, List, Optional, Tuple
 
 from dlt.common import logger
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import ConnectionStringCredentials
 from dlt.common.configuration.specs.exceptions import InvalidConnectionString
 from dlt.common.destination.reference import DestinationClientDwhConfiguration
 from dlt.common.typing import TSecretValue
@@ -22,15 +22,15 @@
     username: Optional[str] = None
     host: Optional[str] = None
     port: Optional[int] = None
     database: Optional[str] = None
 
     read_only: bool = False  # open database read/write
 
-    # __config_gen_annotations__: ClassVar[List[str]] = ["database"]
+    __config_gen_annotations__: ClassVar[List[str]] = []
 
     def borrow_conn(self, read_only: bool) -> Any:
         import duckdb
 
         if not hasattr(self, "_conn_lock"):
             self._conn_lock = threading.Lock()
```

### Comparing `dlt-0.3.1a0/dlt/destinations/duckdb/duck.py` & `dlt-0.3.2/dlt/destinations/postgres/postgres.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,84 @@
+import platform
+
+from dlt.common.wei import EVM_DECIMAL_PRECISION
+if platform.python_implementation() == "PyPy":
+    import psycopg2cffi as psycopg2
+    from psycopg2cffi.sql import SQL, Composed
+else:
+    import psycopg2
+    from psycopg2.sql import SQL, Composed
+
+
 from typing import ClassVar, Dict, Optional
 
 from dlt.common.arithmetics import DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.data_types import TDataType
 from dlt.common.schema import TColumnSchema, TColumnHint, Schema
 
 from dlt.destinations.insert_job_client import InsertValuesJobClient
 
-from dlt.destinations.duckdb import capabilities
-from dlt.destinations.duckdb.sql_client import DuckDbSqlClient
-from dlt.destinations.duckdb.configuration import DuckDbClientConfiguration
+from dlt.destinations.postgres import capabilities
+from dlt.destinations.postgres.sql_client import Psycopg2SqlClient
+from dlt.destinations.postgres.configuration import PostgresClientConfiguration
 
 
 SCT_TO_PGT: Dict[TDataType, str] = {
-    "complex": "JSON",
-    "text": "VARCHAR",
-    "double": "DOUBLE",
-    "bool": "BOOLEAN",
-    "date": "DATE",
-    "timestamp": "TIMESTAMP WITH TIME ZONE",
-    "bigint": "BIGINT",
-    "binary": "BLOB",
-    "decimal": f"DECIMAL({DEFAULT_NUMERIC_PRECISION},{DEFAULT_NUMERIC_SCALE})"
+    "complex": "jsonb",
+    "text": "varchar",
+    "double": "double precision",
+    "bool": "boolean",
+    "timestamp": "timestamp with time zone",
+    "date": "date",
+    "bigint": "bigint",
+    "binary": "bytea",
+    "decimal": f"numeric({DEFAULT_NUMERIC_PRECISION},{DEFAULT_NUMERIC_SCALE})"
 }
 
 PGT_TO_SCT: Dict[str, TDataType] = {
-    "VARCHAR": "text",
-    "JSON": "complex",
-    "DOUBLE": "double",
-    "BOOLEAN": "bool",
-    "DATE": "date",
-    "TIMESTAMP WITH TIME ZONE": "timestamp",
-    "BIGINT": "bigint",
-    "BLOB": "binary",
-    "DECIMAL": "decimal"
+    "varchar": "text",
+    "jsonb": "complex",
+    "double precision": "double",
+    "boolean": "bool",
+    "timestamp with time zone": "timestamp",
+    "date": "date",
+    "bigint": "bigint",
+    "bytea": "binary",
+    "numeric": "decimal"
 }
 
 HINT_TO_POSTGRES_ATTR: Dict[TColumnHint, str] = {
     "unique": "UNIQUE"
 }
 
-
-class DuckDbClient(InsertValuesJobClient):
+class PostgresClient(InsertValuesJobClient):
 
     capabilities: ClassVar[DestinationCapabilitiesContext] = capabilities()
 
-    def __init__(self, schema: Schema, config: DuckDbClientConfiguration) -> None:
-        sql_client = DuckDbSqlClient(
+    def __init__(self, schema: Schema, config: PostgresClientConfiguration) -> None:
+        sql_client = Psycopg2SqlClient(
             self.make_dataset_name(schema, config.dataset_name, config.default_schema_name),
             config.credentials
         )
         super().__init__(schema, config, sql_client)
-        self.config: DuckDbClientConfiguration = config
-        self.sql_client: DuckDbSqlClient = sql_client  # type: ignore
+        self.config: PostgresClientConfiguration = config
+        self.sql_client = sql_client
         self.active_hints = HINT_TO_POSTGRES_ATTR if self.config.create_indexes else {}
 
     def _get_column_def_sql(self, c: TColumnSchema) -> str:
         hints_str = " ".join(self.active_hints.get(h, "") for h in self.active_hints.keys() if c.get(h, False) is True)
         column_name = self.capabilities.escape_identifier(c["name"])
         return f"{column_name} {self._to_db_type(c['data_type'])} {hints_str} {self._gen_not_null(c['nullable'])}"
 
     @staticmethod
     def _to_db_type(sc_t: TDataType) -> str:
         if sc_t == "wei":
-            return "DECIMAL(38,0)"
+            return f"numeric({2*EVM_DECIMAL_PRECISION},{EVM_DECIMAL_PRECISION})"
         return SCT_TO_PGT[sc_t]
 
     @staticmethod
     def _from_db_type(pq_t: str, precision: Optional[int], scale: Optional[int]) -> TDataType:
-        # duckdb provides the types with scale and precision
-        pq_t = pq_t.split("(")[0].upper()
-        if pq_t == "DECIMAL":
-            if precision == 38 and scale == 0:
+        if pq_t == "numeric":
+            if precision == 2*EVM_DECIMAL_PRECISION and scale == EVM_DECIMAL_PRECISION:
                 return "wei"
-        return PGT_TO_SCT[pq_t]
+        return PGT_TO_SCT.get(pq_t, "text")
```

### Comparing `dlt-0.3.1a0/dlt/destinations/duckdb/sql_client.py` & `dlt-0.3.2/dlt/destinations/duckdb/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/destinations/dummy/__init__.py` & `dlt-0.3.2/dlt/destinations/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/destinations/dummy/configuration.py` & `dlt-0.3.2/dlt/destinations/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/destinations/dummy/dummy.py` & `dlt-0.3.2/dlt/destinations/dummy/dummy.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/destinations/exceptions.py` & `dlt-0.3.2/dlt/destinations/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/destinations/filesystem/__init__.py` & `dlt-0.3.2/dlt/destinations/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/destinations/filesystem/configuration.py` & `dlt-0.3.2/dlt/destinations/filesystem/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/destinations/filesystem/filesystem.py` & `dlt-0.3.2/dlt/destinations/filesystem/filesystem.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from dlt.common.destination.reference import NewLoadJob, TLoadJobState, LoadJob, JobClientBase
 from dlt.destinations.job_impl import EmptyLoadJob
 from dlt.destinations.filesystem import capabilities
 from dlt.destinations.filesystem.configuration import FilesystemClientConfiguration
 from dlt.destinations.filesystem.filesystem_client import client_from_config
 from dlt.common.storages import LoadStorage
 
-lock = threading.Lock()
 
 class LoadFilesystemJob(LoadJob):
     def __init__(
             self,
             local_path: str,
             dataset_path: str,
             *,
@@ -40,16 +39,19 @@
         # replace existing files. also check if dir exists for bucket storages that cannot create dirs
         if write_disposition == 'replace' and fs_client.isdir(dataset_path):
             job_info = LoadStorage.parse_job_file_name(file_name)
             search_prefix = posixpath.join(dataset_path, f"{schema_name}.{job_info.table_name}.")
             # NOTE: glob implementation in fsspec does not look thread safe, way better is to use ls and then filter
             all_files: List[str] = fs_client.ls(dataset_path, detail=False, refresh=True)
             items = [item for item in all_files if item.startswith(search_prefix)]
-            if items:
-                fs_client.rm(items)
+            # NOTE: deleting in chunks on s3 does not raise on access denied, file non existing and probably other errors
+            # if items:
+            #     fs_client.rm(items[0])
+            for item in items:
+                fs_client.rm_file(item)
 
         destination_file_name = LoadFilesystemJob.make_destination_filename(file_name, schema_name, load_id)
         fs_client.put_file(local_path, posixpath.join(dataset_path, destination_file_name))
 
     @staticmethod
     def make_destination_filename(file_name: str, schema_name: str, load_id: str) -> str:
         job_info = LoadStorage.parse_job_file_name(file_name)
```

### Comparing `dlt-0.3.1a0/dlt/destinations/filesystem/filesystem_client.py` & `dlt-0.3.2/dlt/destinations/filesystem/filesystem_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/destinations/insert_job_client.py` & `dlt-0.3.2/dlt/destinations/insert_job_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     def exception(self) -> str:
         # this part of code should be never reached
         raise NotImplementedError()
 
     def _insert(self, qualified_table_name: str, write_disposition: TWriteDisposition, file_path: str) -> Iterator[List[str]]:
         # WARNING: maximum redshift statement is 16MB https://docs.aws.amazon.com/redshift/latest/dg/c_redshift-sql.html
         # the procedure below will split the inserts into max_query_length // 2 packs
-        with open(file_path, "r", encoding="utf-8") as f:
+        with FileStorage.open_zipsafe_ro(file_path, "r", encoding="utf-8") as f:
             header = f.readline()
             values_mark = f.readline()
             # properly formatted file has a values marker at the beginning
             assert values_mark == "VALUES\n"
 
             insert_sql = []
             if write_disposition == "replace":
```

### Comparing `dlt-0.3.1a0/dlt/destinations/job_client_impl.py` & `dlt-0.3.2/dlt/destinations/job_client_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 class SqlLoadJob(LoadJob):
     """A job executing sql statement, without followup trait"""
 
     def __init__(self, file_path: str, sql_client: SqlClientBase[Any]) -> None:
         super().__init__(FileStorage.get_file_name_from_file_path(file_path))
         # execute immediately if client present
-        with open(file_path, "r", encoding="utf-8") as f:
+        with FileStorage.open_zipsafe_ro(file_path, "r", encoding="utf-8") as f:
             sql = f.read()
         with sql_client.begin_transaction():
             sql_client.execute_sql(sql)
 
     def state(self) -> TLoadJobState:
         # this job is always done
         return "completed"
@@ -227,50 +227,59 @@
         sql_updates = []
         schema_update: TSchemaTables = {}
         for table_name in only_tables or self.schema.tables:
             exists, storage_table = self.get_storage_table(table_name)
             new_columns = self._create_table_update(table_name, storage_table)
             if len(new_columns) > 0:
                 # build and add sql to execute
-                sql = self._get_table_update_sql(table_name, new_columns, exists)
-                if not sql.endswith(";"):
-                    sql += ";"
-                sql_updates.append(sql)
+                sql_statements = self._get_table_update_sql(table_name, new_columns, exists)
+                for sql in sql_statements:
+                    if not sql.endswith(";"):
+                        sql += ";"
+                    sql_updates.append(sql)
                 # create a schema update for particular table
                 partial_table = copy(self.schema.get_table(table_name))
                 # keep only new columns
                 partial_table["columns"] = {c["name"]: c for c in new_columns}
                 schema_update[table_name] = partial_table
 
         return sql_updates, schema_update
 
-    def _get_table_update_sql(self, table_name: str, new_columns: Sequence[TColumnSchema], generate_alter: bool) -> str:
+    def _make_add_column_sql(self, new_columns: Sequence[TColumnSchema]) -> List[str]:
+        """Make one or more  ADD COLUMN sql clauses to be joined in ALTER TABLE statement(s)"""
+        return [f"ADD COLUMN {self._get_column_def_sql(c)}" for c in new_columns]
+
+    def _get_table_update_sql(self, table_name: str, new_columns: Sequence[TColumnSchema], generate_alter: bool) -> List[str]:
         # build sql
         canonical_name = self.sql_client.make_qualified_table_name(table_name)
+        sql_result: List[str] = []
         if not generate_alter:
             # build CREATE
             sql = f"CREATE TABLE {canonical_name} (\n"
             sql += ",\n".join([self._get_column_def_sql(c) for c in new_columns])
             sql += ")"
+            sql_result.append(sql)
         else:
-            sql = f"ALTER TABLE {canonical_name}\n"
+            sql_base = f"ALTER TABLE {canonical_name}\n"
+            add_column_statements = self._make_add_column_sql(new_columns)
             if self.capabilities.alter_add_multi_column:
                 column_sql = ",\n"
+                sql_result.append(sql_base + column_sql.join(add_column_statements))
             else:
                 # build ALTER as separate statement for each column (redshift limitation)
-                column_sql = ";" + sql
-            sql += column_sql.join([f"ADD COLUMN {self._get_column_def_sql(c)}" for c in new_columns])
+                sql_result.extend([sql_base + col_statement for col_statement in add_column_statements])
+
         # scan columns to get hints
         if generate_alter:
             # no hints may be specified on added columns
             for hint in COLUMN_HINTS:
                 if any(c.get(hint, False) is True for c in new_columns):
                     hint_columns = [self.capabilities.escape_identifier(c["name"]) for c in new_columns if c.get(hint, False)]
                     raise DestinationSchemaWillNotUpdate(canonical_name, hint_columns, f"{hint} requested after table was created")
-        return sql
+        return sql_result
 
     @abstractmethod
     def _get_column_def_sql(self, c: TColumnSchema) -> str:
         pass
 
     @staticmethod
     def _gen_not_null(v: bool) -> str:
```

### Comparing `dlt-0.3.1a0/dlt/destinations/job_impl.py` & `dlt-0.3.2/dlt/destinations/job_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/destinations/postgres/__init__.py` & `dlt-0.3.2/dlt/destinations/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/destinations/postgres/configuration.py` & `dlt-0.3.2/dlt/destinations/postgres/configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     connect_timeout: int = 15
 
     __config_gen_annotations__: ClassVar[List[str]] = ["port", "connect_timeout"]
 
     def parse_native_representation(self, native_value: Any) -> None:
         super().parse_native_representation(native_value)
         self.connect_timeout = int(self.query.get("connect_timeout", self.connect_timeout))
+        if not self.is_partial():
+            self.resolve()
 
     def on_resolved(self) -> None:
         self.database = self.database.lower()
 
     def to_url(self) -> URL:
         url = super().to_url()
         url.update_query_pairs([("connect_timeout", str(self.connect_timeout))])
```

### Comparing `dlt-0.3.1a0/dlt/destinations/postgres/postgres.py` & `dlt-0.3.2/dlt/destinations/redshift/redshift.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,84 +1,103 @@
 import platform
 
-from dlt.common.wei import EVM_DECIMAL_PRECISION
+from dlt.destinations.postgres.sql_client import Psycopg2SqlClient
 if platform.python_implementation() == "PyPy":
     import psycopg2cffi as psycopg2
-    from psycopg2cffi.sql import SQL, Composed
+    # from psycopg2cffi.sql import SQL, Composed
 else:
     import psycopg2
-    from psycopg2.sql import SQL, Composed
-
+    # from psycopg2.sql import SQL, Composed
 
-from typing import ClassVar, Dict, Optional
+from typing import ClassVar, Dict, Optional, Sequence
 
 from dlt.common.arithmetics import DEFAULT_NUMERIC_PRECISION, DEFAULT_NUMERIC_SCALE
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.data_types import TDataType
 from dlt.common.schema import TColumnSchema, TColumnHint, Schema
 
 from dlt.destinations.insert_job_client import InsertValuesJobClient
+from dlt.destinations.exceptions import DatabaseTerminalException
+
+from dlt.destinations.redshift import capabilities
+from dlt.destinations.redshift.configuration import RedshiftClientConfiguration
 
-from dlt.destinations.postgres import capabilities
-from dlt.destinations.postgres.sql_client import Psycopg2SqlClient
-from dlt.destinations.postgres.configuration import PostgresClientConfiguration
 
 
 SCT_TO_PGT: Dict[TDataType, str] = {
-    "complex": "jsonb",
-    "text": "varchar",
+    "complex": "super",
+    "text": "varchar(max)",
     "double": "double precision",
     "bool": "boolean",
-    "timestamp": "timestamp with time zone",
     "date": "date",
+    "timestamp": "timestamp with time zone",
     "bigint": "bigint",
-    "binary": "bytea",
+    "binary": "varbinary",
     "decimal": f"numeric({DEFAULT_NUMERIC_PRECISION},{DEFAULT_NUMERIC_SCALE})"
 }
 
 PGT_TO_SCT: Dict[str, TDataType] = {
-    "varchar": "text",
-    "jsonb": "complex",
+    "super": "complex",
+    "varchar(max)": "text",
     "double precision": "double",
     "boolean": "bool",
-    "timestamp with time zone": "timestamp",
     "date": "date",
+    "timestamp with time zone": "timestamp",
     "bigint": "bigint",
-    "bytea": "binary",
+    "binary varying": "binary",
     "numeric": "decimal"
 }
 
-HINT_TO_POSTGRES_ATTR: Dict[TColumnHint, str] = {
-    "unique": "UNIQUE"
+HINT_TO_REDSHIFT_ATTR: Dict[TColumnHint, str] = {
+    "cluster": "DISTKEY",
+    # it is better to not enforce constraints in redshift
+    # "primary_key": "PRIMARY KEY",
+    "sort": "SORTKEY"
 }
 
-class PostgresClient(InsertValuesJobClient):
+
+class RedshiftSqlClient(Psycopg2SqlClient):
+
+    capabilities: ClassVar[DestinationCapabilitiesContext] = capabilities()
+
+    @staticmethod
+    def _maybe_make_terminal_exception_from_data_error(pg_ex: psycopg2.DataError) -> Optional[Exception]:
+        if "Cannot insert a NULL value into column" in pg_ex.pgerror:
+            # NULL violations is internal error, probably a redshift thing
+            return DatabaseTerminalException(pg_ex)
+        if "Numeric data overflow" in pg_ex.pgerror:
+            return DatabaseTerminalException(pg_ex)
+        if "Precision exceeds maximum" in pg_ex.pgerror:
+            return DatabaseTerminalException(pg_ex)
+        return None
+
+
+class RedshiftClient(InsertValuesJobClient):
 
     capabilities: ClassVar[DestinationCapabilitiesContext] = capabilities()
 
-    def __init__(self, schema: Schema, config: PostgresClientConfiguration) -> None:
-        sql_client = Psycopg2SqlClient(
+    def __init__(self, schema: Schema, config: RedshiftClientConfiguration) -> None:
+        sql_client = RedshiftSqlClient (
             self.make_dataset_name(schema, config.dataset_name, config.default_schema_name),
             config.credentials
         )
         super().__init__(schema, config, sql_client)
-        self.config: PostgresClientConfiguration = config
         self.sql_client = sql_client
-        self.active_hints = HINT_TO_POSTGRES_ATTR if self.config.create_indexes else {}
+        self.config: RedshiftClientConfiguration = config
 
     def _get_column_def_sql(self, c: TColumnSchema) -> str:
-        hints_str = " ".join(self.active_hints.get(h, "") for h in self.active_hints.keys() if c.get(h, False) is True)
+        hints_str = " ".join(HINT_TO_REDSHIFT_ATTR.get(h, "") for h in HINT_TO_REDSHIFT_ATTR.keys() if c.get(h, False) is True)
         column_name = self.capabilities.escape_identifier(c["name"])
         return f"{column_name} {self._to_db_type(c['data_type'])} {hints_str} {self._gen_not_null(c['nullable'])}"
 
     @staticmethod
     def _to_db_type(sc_t: TDataType) -> str:
         if sc_t == "wei":
-            return f"numeric({2*EVM_DECIMAL_PRECISION},{EVM_DECIMAL_PRECISION})"
+            return f"numeric({DEFAULT_NUMERIC_PRECISION},0)"
         return SCT_TO_PGT[sc_t]
 
     @staticmethod
     def _from_db_type(pq_t: str, precision: Optional[int], scale: Optional[int]) -> TDataType:
         if pq_t == "numeric":
-            if precision == 2*EVM_DECIMAL_PRECISION and scale == EVM_DECIMAL_PRECISION:
+            if precision == DEFAULT_NUMERIC_PRECISION and scale == 0:
                 return "wei"
         return PGT_TO_SCT.get(pq_t, "text")
```

### Comparing `dlt-0.3.1a0/dlt/destinations/postgres/sql_client.py` & `dlt-0.3.2/dlt/destinations/postgres/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/destinations/redshift/README.md` & `dlt-0.3.2/dlt/destinations/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/destinations/redshift/__init__.py` & `dlt-0.3.2/dlt/destinations/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/destinations/redshift/configuration.py` & `dlt-0.3.2/dlt/destinations/redshift/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/destinations/sql_client.py` & `dlt-0.3.2/dlt/destinations/sql_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from functools import wraps
 import inspect
 from types import TracebackType
-from typing import Any, ClassVar, ContextManager, Generic, Iterator, Optional, Sequence, Tuple, Type, AnyStr
+from typing import Any, ClassVar, ContextManager, Generic, Iterator, Optional, Sequence, Tuple, Type, AnyStr, List
 
 from dlt.common.typing import TFun
 from dlt.common.destination import DestinationCapabilitiesContext
 
 from dlt.destinations.exceptions import DestinationConnectionError, LoadClientNotConnected
 from dlt.destinations.typing import DBApi, TNativeConn, DBApiCursor, DataFrame, DBTransaction
 
@@ -61,23 +61,22 @@
         pass
 
     @abstractmethod
     def drop_dataset(self) -> None:
         pass
 
     def truncate_tables(self, *tables: str) -> None:
-        sql = ";\n".join(f"TRUNCATE TABLE {self.make_qualified_table_name(t)}" for t in tables)
-        self.execute_sql(sql)
+        statements = [f"TRUNCATE TABLE {self.make_qualified_table_name(t)};" for t in tables]
+        self.execute_fragments(statements)
 
     def drop_tables(self, *tables: str) -> None:
         if not tables:
             return
-        clauses = (f"DROP TABLE IF EXISTS {self.make_qualified_table_name(table)}" for table in tables)
-        sql = ";\n".join(clauses)
-        self.execute_sql(sql)
+        statements = [f"DROP TABLE IF EXISTS {self.make_qualified_table_name(table)};" for table in tables]
+        self.execute_fragments(statements)
 
     @abstractmethod
     def execute_sql(self, sql: AnyStr, *args: Any, **kwargs: Any) -> Optional[Sequence[Sequence[Any]]]:
         pass
 
     @abstractmethod
     def execute_query(self, query: AnyStr, *args: Any, **kwargs: Any) -> ContextManager[DBApiCursor]:
@@ -93,14 +92,19 @@
         pass
 
     def make_qualified_table_name(self, table_name: str, escape: bool = True) -> str:
         if escape:
             table_name = self.capabilities.escape_identifier(table_name)
         return f"{self.fully_qualified_dataset_name(escape=escape)}.{table_name}"
 
+    def escape_column_name(self, column_name: str, escape: bool = True) -> str:
+        if escape:
+            return self.capabilities.escape_identifier(column_name)
+        return column_name
+
     @contextmanager
     def with_alternative_dataset_name(self, dataset_name: str) -> Iterator["SqlClientBase[TNativeConn]"]:
         """Sets the `dataset_name` as the default dataset during the lifetime of the context. Does not modify any search paths in the existing connection."""
         current_dataset_name = self.dataset_name
         try:
             self.dataset_name = dataset_name
             yield self
@@ -145,18 +149,21 @@
         self.fetchall = curr.fetchall  # type: ignore
         self.fetchmany = curr.fetchmany  # type: ignore
         self.fetchone = curr.fetchone  # type: ignore
 
     def __getattr__(self, name: str) -> Any:
         return getattr(self.native_cursor, name)
 
+    def _get_columns(self) -> List[str]:
+        return [c[0] for c in self.native_cursor.description]
+
     def df(self, chunk_size: int = None, **kwargs: Any) -> Optional[DataFrame]:
         from dlt.helpers.pandas_helper import _wrap_result
 
-        columns = [c[0] for c in self.native_cursor.description]
+        columns = self._get_columns()
         if chunk_size is None:
             return _wrap_result(self.native_cursor.fetchall(), columns, **kwargs)
         else:
             df = _wrap_result(self.native_cursor.fetchmany(chunk_size), columns, **kwargs)
             # if no rows return None
             if df.shape[0] == 0:
                 return None
```

### Comparing `dlt-0.3.1a0/dlt/destinations/sql_merge_job.py` & `dlt-0.3.2/dlt/destinations/sql_merge_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 
         First we store the root_keys of root table elements to be deleted in the temp table. Then we use the temp table to delete records from root and all child tables in the destination dataset.
         At the end we copy the data from the staging dataset into destination dataset.
         """
         top_table = table_chain[0]
         file_info = ParsedLoadJobFileName(top_table["name"], uniq_id()[:10], 0, "sql")
         try:
-            sql = cls.gen_merge_sql(table_chain, sql_client)
+            # Remove line breaks from multiline statements and write one SQL statement per line in output file
+            # to support clients that need to execute one statement at a time (i.e. snowflake)
+            sql = [' '.join(stmt.splitlines()) for stmt in cls.gen_merge_sql(table_chain, sql_client)]
             job = cls(file_info.job_id(), "running")
             job._save_text_file("\n".join(sql))
         except Exception:
             # return failed job
             failed_text = "Tried to generate a merge sql job for the following tables:"
             tables_str = yaml.dump(table_chain, allow_unicode=True, default_flow_style=False, sort_keys=False)
             job = cls(file_info.job_id(), "failed", pretty_format_exception())
```

### Comparing `dlt-0.3.1a0/dlt/destinations/typing.py` & `dlt-0.3.2/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/extract/decorators.py` & `dlt-0.3.2/dlt/extract/decorators.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/extract/exceptions.py` & `dlt-0.3.2/dlt/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/extract/extract.py` & `dlt-0.3.2/dlt/extract/extract.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/extract/incremental.py` & `dlt-0.3.2/dlt/extract/incremental.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/extract/pipe.py` & `dlt-0.3.2/dlt/extract/pipe.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import types
 import asyncio
 import makefun
 from asyncio import Future
 from concurrent.futures import ThreadPoolExecutor
 from copy import copy
 from threading import Thread
-from typing import Any, ContextManager, Optional, Sequence, Union, Callable, Iterable, Iterator, List, NamedTuple, Awaitable, Tuple, Type, TYPE_CHECKING
+from typing import Any, ContextManager, Optional, Sequence, Union, Callable, Iterable, Iterator, List, NamedTuple, Awaitable, Tuple, Type, TYPE_CHECKING, Literal
 
 from dlt.common import sleep
 from dlt.common.configuration import configspec
 from dlt.common.configuration.inject import with_config
 from dlt.common.configuration.specs import BaseConfiguration, ContainerInjectableContext
 from dlt.common.configuration.container import Container
 from dlt.common.exceptions import PipelineException
@@ -61,14 +61,16 @@
     Iterable[TPipedDataItems],
     Iterator[TPipedDataItems],
     Callable[[TDataItems, Optional[Any]], TPipedDataItems],
     Callable[[TDataItems, Optional[Any]], Iterator[TPipedDataItems]],
     Callable[[TDataItems, Optional[Any]], Iterator[ResolvablePipeItem]]
 ]
 
+TPipeNextItemMode = Union[Literal["fifo"], Literal["round_robin"]]
+
 
 class ForkPipe:
     def __init__(self, pipe: "Pipe", step: int = -1, copy_on_fork: bool = False) -> None:
         """A transformer that forks the `pipe` and sends the data items to forks added via `add_pipe` method."""
         self._pipes: List[Tuple["Pipe", int]] = []
         self.copy_on_fork = copy_on_fork
         """If true, the data items going to a forked pipe will be copied"""
@@ -420,62 +422,70 @@
 
     @configspec
     class PipeIteratorConfiguration(BaseConfiguration):
         max_parallel_items: int = 20
         workers: int = 5
         futures_poll_interval: float = 0.01
         copy_on_fork: bool = False
+        next_item_mode: str = "fifo"
 
         __section__ = "extract"
 
-    def __init__(self, max_parallel_items: int, workers: int, futures_poll_interval: float) -> None:
+    def __init__(self, max_parallel_items: int, workers: int, futures_poll_interval: float, next_item_mode: TPipeNextItemMode) -> None:
         self.max_parallel_items = max_parallel_items
         self.workers = workers
         self.futures_poll_interval = futures_poll_interval
 
+        self._round_robin_index: int = -1
+        self._initial_sources_count: int = 0
         self._async_pool: asyncio.AbstractEventLoop = None
         self._async_pool_thread: Thread = None
         self._thread_pool: ThreadPoolExecutor = None
         self._sources: List[SourcePipeItem] = []
         self._futures: List[FuturePipeItem] = []
+        self._next_item_mode = next_item_mode
 
     @classmethod
     @with_config(spec=PipeIteratorConfiguration)
-    def from_pipe(cls, pipe: Pipe, *, max_parallel_items: int = 20, workers: int = 5, futures_poll_interval: float = 0.01) -> "PipeIterator":
+    def from_pipe(cls, pipe: Pipe, *, max_parallel_items: int = 20, workers: int = 5, futures_poll_interval: float = 0.01, next_item_mode: TPipeNextItemMode = "fifo") -> "PipeIterator":
         # join all dependent pipes
         if pipe.parent:
             pipe = pipe.full_pipe()
         # clone pipe to allow multiple iterations on pipe based on iterables/callables
         pipe = pipe._clone()
         # head must be iterator
         pipe.evaluate_gen()
         assert isinstance(pipe.gen, Iterator)
         # create extractor
-        extract = cls(max_parallel_items, workers, futures_poll_interval)
+        extract = cls(max_parallel_items, workers, futures_poll_interval, next_item_mode)
         # add as first source
         extract._sources.append(SourcePipeItem(pipe.gen, 0, pipe, None))
+        cls._initial_sources_count = 1
         return extract
 
     @classmethod
     @with_config(spec=PipeIteratorConfiguration)
     def from_pipes(
         cls,
         pipes: Sequence[Pipe],
         yield_parents: bool = True,
         *,
         max_parallel_items: int = 20,
         workers: int = 5,
         futures_poll_interval: float = 0.01,
-        copy_on_fork: bool = False
+        copy_on_fork: bool = False,
+        next_item_mode: TPipeNextItemMode = "fifo"
     ) -> "PipeIterator":
+
         # print(f"max_parallel_items: {max_parallel_items} workers: {workers}")
-        extract = cls(max_parallel_items, workers, futures_poll_interval)
+        extract = cls(max_parallel_items, workers, futures_poll_interval, next_item_mode)
         # clone all pipes before iterating (recursively) as we will fork them (this add steps) and evaluate gens
         pipes = PipeIterator.clone_pipes(pipes)
 
+
         def _fork_pipeline(pipe: Pipe) -> None:
             if pipe.parent:
                 # fork the parent pipe
                 pipe.evaluate_gen()
                 pipe.parent.fork(pipe, copy_on_fork=copy_on_fork)
                 # make the parent yield by sending a clone of item to itself with position at the end
                 if yield_parents and pipe.parent in pipes:
@@ -486,17 +496,22 @@
                 # head of independent pipe must be iterator
                 pipe.evaluate_gen()
                 assert isinstance(pipe.gen, Iterator)
                 # add every head as source only once
                 if not any(i.pipe == pipe for i in extract._sources):
                     extract._sources.append(SourcePipeItem(pipe.gen, 0, pipe, None))
 
-        for pipe in reversed(pipes):
+        # reverse pipes for current mode, as we start processing from the back
+        if next_item_mode == "fifo":
+            pipes.reverse()
+        for pipe in pipes:
             _fork_pipeline(pipe)
 
+        extract._initial_sources_count = len(extract._sources)
+
         return extract
 
     def __next__(self) -> PipeItem:
         pipe_item: Union[ResolvablePipeItem, SourcePipeItem] = None
         # __next__ should call itself to remove the `while` loop and continue clauses but that may lead to stack overflows: there's no tail recursion opt in python
         # https://stackoverflow.com/questions/13591970/does-python-optimize-tail-recursion (see Y combinator on how it could be emulated)
         while True:
@@ -663,25 +678,32 @@
         item = future.result()
         if isinstance(item, DataItemWithMeta):
             return ResolvablePipeItem(item.data, step, pipe, item.meta)
         else:
             return ResolvablePipeItem(item, step, pipe, meta)
 
     def _get_source_item(self) -> ResolvablePipeItem:
+        if self._next_item_mode == "fifo":
+            return self._get_source_item_current()
+        elif self._next_item_mode == "round_robin":
+            return self._get_source_item_round_robin()
+
+    def _get_source_item_current(self) -> ResolvablePipeItem:
         # no more sources to iterate
         if len(self._sources) == 0:
             return None
-
-        # get items from last added iterator, this makes the overall Pipe as close to FIFO as possible
-        gen, step, pipe, meta = self._sources[-1]
-        # print(f"got {pipe.name} {pipe._pipe_id}")
-        # register current pipe name during the execution of gen
-        set_current_pipe_name(pipe.name)
         try:
-            item = next(gen)
+            # get items from last added iterator, this makes the overall Pipe as close to FIFO as possible
+            gen, step, pipe, meta = self._sources[-1]
+            # print(f"got {pipe.name} {pipe._pipe_id}")
+            # register current pipe name during the execution of gen
+            set_current_pipe_name(pipe.name)
+            item = None
+            while item is None:
+                item = next(gen)
             # full pipe item may be returned, this is used by ForkPipe step
             # to redirect execution of an item to another pipe
             if isinstance(item, ResolvablePipeItem):
                 return item
             else:
                 # keep the item assigned step and pipe when creating resolvable item
                 if isinstance(item, DataItemWithMeta):
@@ -693,16 +715,56 @@
             self._sources.pop()
             return self._get_source_item()
         except (PipelineException, ExtractorException, DltSourceException, PipeException):
             raise
         except Exception as ex:
             raise ResourceExtractionError(pipe.name, gen, str(ex), "generator") from ex
 
+    def _get_source_item_round_robin(self) -> ResolvablePipeItem:
+        sources_count = len(self._sources)
+        # no more sources to iterate
+        if sources_count == 0:
+            return None
+        # if there are currently more sources than added initially, we need to process the new ones first
+        if sources_count > self._initial_sources_count:
+            return self._get_source_item_current()
+        try:
+            # print(f"got {pipe.name} {pipe._pipe_id}")
+            # register current pipe name during the execution of gen
+            item = None
+            while item is None:
+                self._round_robin_index = (self._round_robin_index + 1) % sources_count
+                gen, step, pipe, meta = self._sources[self._round_robin_index]
+                set_current_pipe_name(pipe.name)
+                item = next(gen)
+            # full pipe item may be returned, this is used by ForkPipe step
+            # to redirect execution of an item to another pipe
+            if isinstance(item, ResolvablePipeItem):
+                return item
+            else:
+                # keep the item assigned step and pipe when creating resolvable item
+                if isinstance(item, DataItemWithMeta):
+                    return ResolvablePipeItem(item.data, step, pipe, item.meta)
+                else:
+                    return ResolvablePipeItem(item, step, pipe, meta)
+        except StopIteration:
+            # remove empty iterator and try another source
+            self._sources.pop(self._round_robin_index)
+            # we need to decrease the index to keep the round robin order
+            self._round_robin_index -= 1
+            # since in this case we have popped an initial source, we need to decrease the initial sources count
+            self._initial_sources_count -= 1
+            return self._get_source_item_round_robin()
+        except (PipelineException, ExtractorException, DltSourceException, PipeException):
+            raise
+        except Exception as ex:
+            raise ResourceExtractionError(pipe.name, gen, str(ex), "generator") from ex
+
     @staticmethod
-    def clone_pipes(pipes: Sequence[Pipe]) -> Sequence[Pipe]:
+    def clone_pipes(pipes: Sequence[Pipe]) -> List[Pipe]:
         """This will clone pipes and fix the parent/dependent references"""
         cloned_pipes = [p._clone() for p in pipes]
         cloned_pairs = {id(p): c for p, c in zip(pipes, cloned_pipes)}
 
         for clone in cloned_pipes:
             while True:
                 if not clone.parent:
```

### Comparing `dlt-0.3.1a0/dlt/extract/schema.py` & `dlt-0.3.2/dlt/extract/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/extract/source.py` & `dlt-0.3.2/dlt/extract/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/extract/typing.py` & `dlt-0.3.2/dlt/extract/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/extract/utils.py` & `dlt-0.3.2/dlt/extract/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/helpers/airflow_helper.py` & `dlt-0.3.2/dlt/helpers/airflow_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/helpers/dbt/__init__.py` & `dlt-0.3.2/dlt/helpers/dbt/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 
 def _default_profile_name(credentials: DestinationClientDwhConfiguration) -> str:
     profile_name = credentials.destination_name
     # in case of credentials with default add default to the profile name
     if isinstance(credentials.credentials, CredentialsWithDefault):
         if credentials.credentials.has_default_credentials():
             profile_name += "_default"
+    elif profile_name == 'snowflake':
+        if getattr(credentials.credentials, 'private_key', None):
+            # snowflake with private key is a separate profile
+            profile_name += '_pkey'
     return profile_name
 
 
 def _create_dbt_deps(destination_names: List[str], dbt_version: str = DEFAULT_DBT_VERSION) -> List[str]:
     if dbt_version:
         # if parses as version use "==" operator
         with contextlib.suppress(ValueError):
```

### Comparing `dlt-0.3.1a0/dlt/helpers/dbt/configuration.py` & `dlt-0.3.2/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.3.2/dlt/helpers/dbt/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/helpers/dbt/exceptions.py` & `dlt-0.3.2/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/helpers/dbt/profiles.yml` & `dlt-0.3.2/dlt/helpers/dbt/profiles.yml`

 * *Files 12% similar despite different names*

```diff
@@ -80,7 +80,41 @@
       type: duckdb
       schema: "{{ var('destination_dataset_name', var('source_dataset_name')) }}"
       path: "{{ env_var('CREDENTIALS__DATABASE') }}"
       extensions:
         - httpfs
         - parquet
       # TODO: emit the config of duck db
+
+
+# snowflake with password auth
+snowflake:
+  target: analytics
+  outputs:
+    analytics:
+      type: snowflake
+      account: "{{ env_var('CREDENTIALS__HOST') }}"
+      user: "{{ env_var('CREDENTIALS__USERNAME') }}"
+      password: "{{ env_var('CREDENTIALS__PASSWORD') }}"
+      database: "{{ env_var('CREDENTIALS__DATABASE') }}"
+      role: "{{ env_var('CREDENTIALS__ROLE', '') }}"
+      schema: "{{ var('destination_dataset_name', var('source_dataset_name')) }}"
+      warehouse: "{{ env_var('CREDENTIALS__WAREHOUSE') }}"
+      threads: 4
+
+
+# snowflake with private key auth
+snowflake_pkey:
+  target: analytics
+  outputs:
+    analytics:
+      type: snowflake
+      account: "{{ env_var('CREDENTIALS__HOST') }}"
+      user: "{{ env_var('CREDENTIALS__USERNAME') }}"
+      database: "{{ env_var('CREDENTIALS__DATABASE') }}"
+      password: "{{ env_var('CREDENTIALS__PASSWORD') }}"
+      role: "{{ env_var('CREDENTIALS__ROLE', '') }}"
+      schema: "{{ var('destination_dataset_name', var('source_dataset_name')) }}"
+      warehouse: "{{ env_var('CREDENTIALS__WAREHOUSE') }}"
+      private_key: "{{ env_var('CREDENTIALS__PRIVATE_KEY') }}"
+      private_key_passphrase: "{{ env_var('CREDENTIALS__PRIVATE_KEY_PASSPHRASE', '') }}"
+      threads: 4
```

### Comparing `dlt-0.3.1a0/dlt/helpers/dbt/runner.py` & `dlt-0.3.2/dlt/helpers/dbt/runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/helpers/pandas_helper.py` & `dlt-0.3.2/dlt/helpers/pandas_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/helpers/streamlit_helper.py` & `dlt-0.3.2/dlt/helpers/streamlit_helper.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/load/configuration.py` & `dlt-0.3.2/dlt/load/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/load/exceptions.py` & `dlt-0.3.2/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/load/load.py` & `dlt-0.3.2/dlt/load/load.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/normalize/configuration.py` & `dlt-0.3.2/dlt/normalize/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/normalize/normalize.py` & `dlt-0.3.2/dlt/normalize/normalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,23 +38,23 @@
         self.collector = collector
         self.pool: ProcessPool = None
         self.normalize_storage: NormalizeStorage = None
         self.load_storage: LoadStorage = None
         self.schema_storage: SchemaStorage = None
 
         # setup storages
-        self.create_storages(config.destination_capabilities.preferred_loader_file_format)
+        self.create_storages()
         # create schema storage with give type
         self.schema_storage = schema_storage or SchemaStorage(self.config._schema_storage_config, makedirs=True)
 
-    def create_storages(self, loader_file_format: TLoaderFileFormat) -> None:
+    def create_storages(self) -> None:
         # pass initial normalize storage config embedded in normalize config
         self.normalize_storage = NormalizeStorage(True, config=self.config._normalize_storage_config)
         # normalize saves in preferred format but can read all supported formats
-        self.load_storage = LoadStorage(True, loader_file_format, LoadStorage.ALL_SUPPORTED_FILE_FORMATS, config=self.config._load_storage_config)
+        self.load_storage = LoadStorage(True, self.config.destination_capabilities.preferred_loader_file_format, LoadStorage.ALL_SUPPORTED_FILE_FORMATS, config=self.config._load_storage_config)
 
 
     @staticmethod
     def load_or_create_schema(schema_storage: SchemaStorage, schema_name: str) -> Schema:
         try:
             schema = schema_storage.load_schema(schema_name)
             logger.info(f"Loaded schema with name {schema_name} with version {schema.stored_version}")
@@ -66,15 +66,15 @@
     @staticmethod
     def w_normalize_files(
             normalize_storage_config: NormalizeStorageConfiguration,
             loader_storage_config: LoadStorageConfiguration,
             destination_caps: DestinationCapabilitiesContext,
             stored_schema: TStoredSchema,
             load_id: str,
-            extracted_items_files: Sequence[str]
+            extracted_items_files: Sequence[str],
         ) -> TWorkerRV:
 
         schema_updates: List[TSchemaUpdate] = []
         total_items = 0
         # process all files with data items and write to buffered item storage
         with Container().injectable_context(destination_caps):
             schema = Schema.from_stored_schema(stored_schema)
@@ -226,15 +226,15 @@
     def map_single(self, schema: Schema, load_id: str, files: Sequence[str]) -> TMapFuncRV:
         result = Normalize.w_normalize_files(
             self.normalize_storage.config,
             self.load_storage.config,
             self.config.destination_capabilities,
             schema.to_dict(),
             load_id,
-            files
+            files,
         )
         self.update_schema(schema, result[0])
         self.collector.update("Files", len(result[2]))
         self.collector.update("Items", result[1])
         return result[0]
 
     def spool_files(self, schema_name: str, load_id: str, map_f: TMapFuncType, files: Sequence[str]) -> None:
```

### Comparing `dlt-0.3.1a0/dlt/pipeline/__init__.py` & `dlt-0.3.2/dlt/pipeline/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from dlt.common.typing import TSecretValue, Any
 from dlt.common.configuration import with_config
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.inject import get_orig_args, last_config
 from dlt.common.destination.reference import DestinationReference, TDestinationReferenceArg
 from dlt.common.pipeline import LoadInfo, PipelineContext, get_dlt_pipelines_dir
+from dlt.common.data_writers import TLoaderFileFormat
 
 from dlt.pipeline.configuration import PipelineConfiguration, ensure_correct_pipeline_kwargs
 from dlt.pipeline.pipeline import Pipeline
 from dlt.pipeline.progress import _from_name as collector_from_name, TCollectorArg, _NULL_COLLECTOR
 
 
 @overload
@@ -32,16 +33,16 @@
 
     ### Summary
     The `pipeline` functions allows you to pass the destination name to which the data should be loaded, the name of the dataset and several other options that govern loading of the data.
     The created `Pipeline` object lets you load the data from any source with `run` method or to have more granular control over the loading process with `extract`, `normalize` and `load` methods.
 
     Please refer to the following doc pages
     - Write your first pipeline walkthrough: https://dlthub.com/docs/walkthroughs/create-a-pipeline
-    - Pipeline architecture and data loading steps: https://dlthub.com/docs/architecture
-    - List of supported destinations: https://dlthub.com/docs/destinations/bigquery
+    - Pipeline architecture and data loading steps: https://dlthub.com/docs/reference
+    - List of supported destinations: https://dlthub.com/docs/dlt-ecosystem/destinations
 
     ### Args:
         pipeline_name (str, optional): A name of the pipeline that will be used to identify it in monitoring events and to restore its state and data schemas on subsequent runs.
         Defaults to the file name of pipeline script with `dlt_` prefix added.
 
         pipelines_dir (str, optional): A working directory in which pipeline state and temporary files will be stored. Defaults to user home directory: `~/dlt/pipelines/`.
```

### Comparing `dlt-0.3.1a0/dlt/pipeline/configuration.py` & `dlt-0.3.2/dlt/pipeline/configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from typing import Any, Optional
 
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import RunConfiguration, BaseConfiguration
 from dlt.common.typing import AnyFun, TSecretValue
 from dlt.common.utils import digest256
+from dlt.common.data_writers import TLoaderFileFormat
 
 
 
 @configspec
 class PipelineConfiguration(BaseConfiguration):
     pipeline_name: Optional[str] = None
     pipelines_dir: Optional[str] = None
     destination_name: Optional[str] = None
+    loader_file_format: Optional[TLoaderFileFormat] = None
     dataset_name: Optional[str] = None
     pipeline_salt: Optional[TSecretValue] = None
     restore_from_destination: bool = True
     """Enables the `run` method of the `Pipeline` object to restore the pipeline state and schemas from the destination"""
     enable_runtime_trace: bool = True
     """Enables the tracing. Tracing saves the execution trace locally and is required by `dlt deploy`."""
     use_single_dataset: bool = True
```

### Comparing `dlt-0.3.1a0/dlt/pipeline/dbt.py` & `dlt-0.3.2/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/pipeline/exceptions.py` & `dlt-0.3.2/dlt/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/pipeline/helpers.py` & `dlt-0.3.2/dlt/pipeline/helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/pipeline/pipeline.py` & `dlt-0.3.2/dlt/pipeline/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from dlt.common.runners import pool_runner as runner
 from dlt.common.storages import LiveSchemaStorage, NormalizeStorage, LoadStorage, SchemaStorage, FileStorage, NormalizeStorageConfiguration, SchemaStorageConfiguration, LoadStorageConfiguration
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import DestinationReference, JobClientBase, DestinationClientConfiguration, DestinationClientDwhConfiguration, TDestinationReferenceArg
 from dlt.common.pipeline import ExtractInfo, LoadInfo, NormalizeInfo, PipelineContext, SupportsPipeline, TPipelineLocalState, TPipelineState, StateInjectableContext
 from dlt.common.schema import Schema
 from dlt.common.utils import is_interactive
+from dlt.common.data_writers import TLoaderFileFormat
 
 from dlt.destinations.exceptions import DatabaseUndefinedRelation
 
 from dlt.extract.exceptions import DataItemRequiredForDynamicTableHints, SourceExhausted
 from dlt.extract.extract import ExtractorStorage, extract_with_schema
 from dlt.extract.source import DltResource, DltSource
 from dlt.normalize import Normalize
@@ -279,15 +280,15 @@
         except Exception as exc:
             # TODO: provide metrics from extractor
             raise PipelineStepFailed(self, "extract", exc, ExtractInfo()) from exc
 
     @with_runtime_trace
     @with_schemas_sync
     @with_config_section((known_sections.NORMALIZE,))
-    def normalize(self, workers: int = 1) -> NormalizeInfo:
+    def normalize(self, workers: int = 1, loader_file_format: TLoaderFileFormat = None) -> NormalizeInfo:
         """Normalizes the data prepared with `extract` method, infers the schema and creates load packages for the `load` method. Requires `destination` to be known."""
         if is_interactive() and workers > 1:
             raise NotImplementedError("Do not use normalize workers in interactive mode ie. in notebook")
         # check if any schema is present, if not then no data was extracted
         if not self.default_schema_name:
             return None
 
@@ -298,15 +299,15 @@
             workers=workers,
             pool_type="none" if workers == 1 else "process",
             _schema_storage_config=self._schema_storage_config,
             _normalize_storage_config=self._normalize_storage_config,
             _load_storage_config=self._load_storage_config
         )
         # run with destination context
-        with self._maybe_destination_capabilities():
+        with self._maybe_destination_capabilities(loader_file_format=loader_file_format):
             # shares schema storage with the pipeline so we do not need to install
             normalize = Normalize(collector=self.collector, config=normalize_config, schema_storage=self._schema_storage)
             try:
                 with signals.delayed_signals():
                     runner.run_pool(normalize.config, normalize)
                 return NormalizeInfo()
             except Exception as n_ex:
@@ -363,15 +364,16 @@
         destination: TDestinationReferenceArg = None,
         dataset_name: str = None,
         credentials: Any = None,
         table_name: str = None,
         write_disposition: TWriteDisposition = None,
         columns: Sequence[TColumnSchema] = None,
         primary_key: TColumnKey = None,
-        schema: Schema = None
+        schema: Schema = None,
+        loader_file_format: TLoaderFileFormat = None
     ) -> LoadInfo:
         """Loads the data from `data` argument into the destination specified in `destination` and dataset specified in `dataset_name`.
 
         ### Summary
         This method will `extract` the data from the `data` argument, infer the schema, `normalize` the data into a load package (ie. jsonl or PARQUET files representing tables) and then `load` such packages into the `destination`.
 
         The data may be supplied in several forms:
@@ -411,14 +413,16 @@
 
             columns (Sequence[TColumnSchema], optional): A list of column schemas. Typed dictionary describing column names, data types, write disposition and performance hints that gives you full control over the created table schema.
 
             primary_key (str | Sequence[str]): A column name or a list of column names that comprise a private key. Typically used with "merge" write disposition to deduplicate loaded data.
 
             schema (Schema, optional): An explicit `Schema` object in which all table schemas will be grouped. By default `dlt` takes the schema from the source (if passed in `data` argument) or creates a default one itself.
 
+            loader_file_format (Literal["jsonl", "puae-jsonl", "insert_values", "sql", "parquet"], optional). The file format the loader will use to create the load package. Not all file_formats are compatible with all destinations. Defaults to the preferred file format of the selected destination.
+
         ### Raises:
             PipelineStepFailed when a problem happened during `extract`, `normalize` or `load` steps.
         ### Returns:
             LoadInfo: Information on loaded data including the list of package ids and failed job statuses. Please not that `dlt` will not raise if a single job terminally fails. Such information is provided via LoadInfo.
         """
         signals.raise_if_signalled()
         self._set_destination(destination)
@@ -428,25 +432,25 @@
         if self.config.restore_from_destination and not self.full_refresh and not self._state_restored and (self.destination or destination):
             self.sync_destination(destination, dataset_name)
             # sync only once
             self._state_restored = True
 
         # normalize and load pending data
         if self.list_extracted_resources():
-            self.normalize()
+            self.normalize(loader_file_format=loader_file_format)
         if self.list_normalized_load_packages():
             # if there were any pending loads, load them and **exit**
             if data is not None:
                 logger.warn("The pipeline `run` method will now load the pending load packages. The data you passed to the run function will not be loaded. In order to do that you must run the pipeline again")
             return self.load(destination, dataset_name, credentials=credentials)
 
         # extract from the source
         if data is not None:
             self.extract(data, table_name=table_name, write_disposition=write_disposition, columns=columns, primary_key=primary_key, schema=schema)
-            self.normalize()
+            self.normalize(loader_file_format=loader_file_format)
             return self.load(destination, dataset_name, credentials=credentials)
         else:
             return None
 
     @with_schemas_sync
     def sync_destination(self, destination: TDestinationReferenceArg = None, dataset_name: str = None) -> None:
         """Synchronizes pipeline state with the `destination`'s state kept in `dataset_name`
@@ -922,21 +926,23 @@
         destination_mod = DestinationReference.from_name(destination)
         self.destination = destination_mod or self.destination
         with self._maybe_destination_capabilities():
             # default normalizers must match the destination
             self._set_default_normalizers()
 
     @contextmanager
-    def _maybe_destination_capabilities(self) -> Iterator[DestinationCapabilitiesContext]:
+    def _maybe_destination_capabilities(self, loader_file_format: TLoaderFileFormat = None) -> Iterator[DestinationCapabilitiesContext]:
         try:
             caps: DestinationCapabilitiesContext = None
             injected_caps: ContextManager[DestinationCapabilitiesContext] = None
             if self.destination:
                 injected_caps = self._container.injectable_context(self._get_destination_capabilities())
                 caps = injected_caps.__enter__()
+                if loader_file_format:
+                    caps.preferred_loader_file_format = loader_file_format
             yield caps
         finally:
             if injected_caps:
                 injected_caps.__exit__(None, None, None)
 
     def _set_default_normalizers(self) -> None:
         self._default_naming, _ = import_normalizers(default_normalizers())
```

### Comparing `dlt-0.3.1a0/dlt/pipeline/progress.py` & `dlt-0.3.2/dlt/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/pipeline/state_sync.py` & `dlt-0.3.2/dlt/pipeline/state_sync.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/pipeline/trace.py` & `dlt-0.3.2/dlt/pipeline/trace.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,12 +203,12 @@
 def save_trace(trace_path: str, trace: PipelineTrace) -> None:
     with open(os.path.join(trace_path, TRACE_FILE_NAME), mode="bw") as f:
         f.write(pickle.dumps(trace))
 
 
 def load_trace(trace_path: str) -> PipelineTrace:
     try:
-        with open(os.path.join(trace_path, TRACE_FILE_NAME), mode="br") as f:
+        with open(os.path.join(trace_path, TRACE_FILE_NAME), mode="rb") as f:
             return pickle.load(f)  # type: ignore
     except (AttributeError, FileNotFoundError):
         # on incompatible pickling / file not found return no trace
         return None
```

### Comparing `dlt-0.3.1a0/dlt/pipeline/track.py` & `dlt-0.3.2/dlt/pipeline/track.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/reflection/names.py` & `dlt-0.3.2/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/reflection/script_inspector.py` & `dlt-0.3.2/dlt/reflection/script_inspector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/reflection/script_visitor.py` & `dlt-0.3.2/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/sources/helpers/requests/__init__.py` & `dlt-0.3.2/dlt/sources/helpers/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/sources/helpers/requests/retry.py` & `dlt-0.3.2/dlt/sources/helpers/requests/retry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/sources/helpers/requests/session.py` & `dlt-0.3.2/dlt/sources/helpers/requests/session.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/sources/helpers/transform.py` & `dlt-0.3.2/dlt/sources/helpers/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/dlt/version.py` & `dlt-0.3.2/dlt/version.py`

 * *Files identical despite different names*

### Comparing `dlt-0.3.1a0/pyproject.toml` & `dlt-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.3.1a0"
+version = "0.3.2"
 description = "DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
@@ -27,29 +27,27 @@
 pendulum = ">=2.1.2"
 simplejson = ">=3.17.5"
 PyYAML = ">=5.4.1"
 json-logging = "1.4.1rc0"
 semver = ">=2.13.0"
 sentry-sdk = ">=1.4.3"
 hexbytes = ">=0.2.2"
-cachetools = ">=5.2.0"
 tzdata = ">=2022.1"
 tomlkit = ">=0.11.3"
-asyncstdlib = ">=3.10.5"
 pathvalidate = ">=2.5.2"
 SQLAlchemy = ">=1.4.0"
 typing-extensions = ">=4.0.0"
 makefun = ">=1.15.0"
 click = ">=7.1"
 requirements-parser = ">=0.5.0"
 setuptools = ">=65.6.0"
 humanize = ">=4.4.0"
 astunparse = ">=1.6.3"
 cron-descriptor = ">=1.2.32"
-pipdeptree = ">=2.3.3"
+pipdeptree = ">=2.9.3"
 gitpython = ">=3.1.29"
 pytz = ">=2022.6"
 giturlparse = ">=0.10.0"
 orjson = {version = "^3.8.6", markers="platform_python_implementation != 'PyPy'"}
 tenacity = "^8.2.2"
 jsonpath-ng = "^1.5.3"
 deprecated = "^1.2.13"
@@ -65,18 +63,20 @@
 
 duckdb = {version = ">=0.6.1,<0.9.0", optional = true}
 
 dbt-core = {version = ">=1.3.0,<1.5.0", optional = true}
 dbt-redshift = {version = ">=1.3.0,<1.5.0", optional = true}
 dbt-bigquery = {version = ">=1.3.0,<1.5.0", optional = true}
 dbt-duckdb = {version = ">=1.3.0,<1.5.0", optional = true}
+dbt-snowflake = {version = ">=1.3.0,<1.5.0", optional = true}
 s3fs = {version = "^2023.5.0", optional = true}
 gcsfs = {version = "^2023.5.0", optional = true}
 boto3 = {version = ">=1.26", optional = true}
 fsspec = "^2023.5.0"
+snowflake-connector-python = {version = "^3.0.4", optional = true, extras = ["pandas"]}
 
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.4"
 mypy = "1.2.0"
 flake8 = "^5.0.0"
@@ -94,24 +94,26 @@
 types-python-dateutil = ">=2.8.15"
 flake8-tidy-imports = ">=4.8.0"
 flake8-encodings = "^0.5.0"
 flake8-builtins = "^1.5.3"
 types-SQLAlchemy = ">=1.4.53"
 
 [tool.poetry.extras]
-dbt = ["dbt-core", "dbt-redshift", "dbt-bigquery", "dbt-duckdb"]
+dbt = ["dbt-core", "dbt-redshift", "dbt-bigquery", "dbt-duckdb", "dbt-snowflake"]
 gcp = ["grpcio", "google-cloud-bigquery", "db-dtypes", "gcsfs"]
 # bigquery is alias on gcp extras
 bigquery = ["grpcio", "google-cloud-bigquery", "pyarrow", "db-dtypes", "gcsfs"]
 postgres = ["psycopg2-binary", "psycopg2cffi"]
 redshift = ["psycopg2-binary", "psycopg2cffi"]
+pyarrow = ["pyarrow"]
 duckdb = ["duckdb"]
 filesystem = ["s3fs", "boto3"]
 s3 = ["s3fs", "boto3"]
 gs = ["gcsfs"]
+snowflake = ["snowflake-connector-python"]
 
 [tool.poetry.scripts]
 dlt = "dlt.cli._dlt:_main"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.10.0"
 types-click = "^7.1.8"
```

### Comparing `dlt-0.3.1a0/setup.py` & `dlt-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
  'dlt.common.configuration',
  'dlt.common.configuration.providers',
  'dlt.common.configuration.specs',
  'dlt.common.data_types',
  'dlt.common.data_writers',
  'dlt.common.destination',
  'dlt.common.json',
+ 'dlt.common.libs',
  'dlt.common.normalizers',
  'dlt.common.normalizers.json',
  'dlt.common.normalizers.naming',
  'dlt.common.reflection',
  'dlt.common.runners',
  'dlt.common.runtime',
  'dlt.common.schema',
@@ -23,14 +24,15 @@
  'dlt.destinations',
  'dlt.destinations.bigquery',
  'dlt.destinations.duckdb',
  'dlt.destinations.dummy',
  'dlt.destinations.filesystem',
  'dlt.destinations.postgres',
  'dlt.destinations.redshift',
+ 'dlt.destinations.snowflake',
  'dlt.extract',
  'dlt.helpers',
  'dlt.helpers.dbt',
  'dlt.load',
  'dlt.normalize',
  'dlt.pipeline',
  'dlt.reflection',
@@ -41,30 +43,28 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=5.4.1',
  'SQLAlchemy>=1.4.0',
  'astunparse>=1.6.3',
- 'asyncstdlib>=3.10.5',
- 'cachetools>=5.2.0',
  'click>=7.1',
  'cron-descriptor>=1.2.32',
  'deprecated>=1.2.13,<2.0.0',
  'fsspec>=2023.5.0,<2024.0.0',
  'gitpython>=3.1.29',
  'giturlparse>=0.10.0',
  'hexbytes>=0.2.2',
  'humanize>=4.4.0',
  'json-logging==1.4.1rc0',
  'jsonpath-ng>=1.5.3,<2.0.0',
  'makefun>=1.15.0',
  'pathvalidate>=2.5.2',
  'pendulum>=2.1.2',
- 'pipdeptree>=2.3.3',
+ 'pipdeptree>=2.9.3',
  'pytz>=2022.6',
  'requests>=2.26.0',
  'requirements-parser>=0.5.0',
  'semver>=2.13.0',
  'sentry-sdk>=1.4.3',
  'setuptools>=65.6.0',
  'simplejson>=3.17.5',
@@ -78,35 +78,38 @@
  'bigquery': ['grpcio>=1.50.0',
               'google-cloud-bigquery>=2.26.0',
               'pyarrow>=8.0.0',
               'gcsfs>=2023.5.0,<2024.0.0'],
  'dbt': ['dbt-core>=1.3.0,<1.5.0',
          'dbt-redshift>=1.3.0,<1.5.0',
          'dbt-bigquery>=1.3.0,<1.5.0',
-         'dbt-duckdb>=1.3.0,<1.5.0'],
+         'dbt-duckdb>=1.3.0,<1.5.0',
+         'dbt-snowflake>=1.3.0,<1.5.0'],
  'duckdb': ['duckdb>=0.6.1,<0.9.0'],
  'filesystem': ['s3fs>=2023.5.0,<2024.0.0', 'boto3>=1.26'],
  'gcp': ['grpcio>=1.50.0',
          'google-cloud-bigquery>=2.26.0',
          'gcsfs>=2023.5.0,<2024.0.0'],
  'gs': ['gcsfs>=2023.5.0,<2024.0.0'],
  'postgres': ['psycopg2-binary>=2.9.1'],
  'postgres:platform_python_implementation == "PyPy"': ['psycopg2cffi>=2.9.0'],
+ 'pyarrow': ['pyarrow>=8.0.0'],
  'redshift': ['psycopg2-binary>=2.9.1'],
  'redshift:platform_python_implementation == "PyPy"': ['psycopg2cffi>=2.9.0'],
- 's3': ['s3fs>=2023.5.0,<2024.0.0', 'boto3>=1.26']}
+ 's3': ['s3fs>=2023.5.0,<2024.0.0', 'boto3>=1.26'],
+ 'snowflake': ['snowflake-connector-python[pandas]>=3.0.4,<4.0.0']}
 
 entry_points = \
 {'console_scripts': ['dlt = dlt.cli._dlt:_main']}
 
 setup_kwargs = {
     'name': 'dlt',
-    'version': '0.3.1a0',
+    'version': '0.3.2',
     'description': 'DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.',
-    'long_description': '<h1 align="center">\n    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>\n</h1>\n<p align="center">\nBe it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.\n</p>\n\n<div align="center">\n  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">\n    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n</div>\n\n## Installation\n\ndlt supports Python 3.8+.\n\n```bash\npip install dlt\n```\n\n## Quick Start\n\nLoad chess game data from chess.com API and save it in DuckDB:\n\n```python\nimport dlt\nfrom chess import chess # a utility function that grabs data from the chess.com API\n\n# create a dlt pipeline that will load chess game data to the DuckDB destination\npipeline = dlt.pipeline(\n    pipeline_name=\'chess_pipeline\',\n    destination=\'duckdb\',\n    dataset_name=\'games_data\'\n)\n\n# use chess.com API to grab data about a few players\ndata = chess([\'magnuscarlsen\', \'rpragchess\'], start_month=\'2022/11\', end_month=\'2022/12\')\n\n# extract, normalize, and load the data\npipeline.run(data)\n```\n\nTry it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**\n\n## Features\n\n- **Automatic Schema:** Data structure inspection and schema creation for the destination.\n- **Data Normalization:** Consistent and verified data before loading.\n- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.\n- **Scalable:** Adapts to growing data needs in production.\n- **Easy Maintenance:** Clear data pipeline structure for updates.\n- **Rapid Exploration:** Quickly explore and gain insights from new data sources.\n- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.\n- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.\n- **Incremental Loading:** Load only new or changed data and avoid loading old records again.\n- **Open Source:** Free and Apache 2.0 Licensed.\n\n## Ready to use Sources and Destinations\n\nExplore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/verified-sources/chess) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/destinations/bigquery).\n\n## Documentation\n\nFor detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).\n\n## Examples\n\nYou can find examples for various use cases in the [examples](docs/examples) folder.\n\n## Get Involved\n\nThe dlt project is quickly growing, and we\'re excited to have you join our community! Here\'s how you can get involved:\n\n- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)\n- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.\n- **Contribute Verified Sources**: Contribute your custom sources to the [dlt-hub/verified-sources](https://github.com/dlt-hub/verified-sources) to help other folks in handling their data tasks.\n- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.\n- **Improve documentation**: Help us enhance the dlt documentation.\n\n## License\n\nDLT is released under the [Apache 2.0 License](LICENSE.txt).\n',
+    'long_description': '<h1 align="center">\n    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>\n</h1>\n<p align="center">\nBe it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.\n</p>\n\n<div align="center">\n  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">\n    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n</div>\n\n## Installation\n\ndlt supports Python 3.8+.\n\n```bash\npip install dlt\n```\n\n## Quick Start\n\nLoad chess game data from chess.com API and save it in DuckDB:\n\n```python\nimport dlt\nfrom chess import chess # a utility function that grabs data from the chess.com API\n\n# create a dlt pipeline that will load chess game data to the DuckDB destination\npipeline = dlt.pipeline(\n    pipeline_name=\'chess_pipeline\',\n    destination=\'duckdb\',\n    dataset_name=\'games_data\'\n)\n\n# use chess.com API to grab data about a few players\ndata = chess([\'magnuscarlsen\', \'rpragchess\'], start_month=\'2022/11\', end_month=\'2022/12\')\n\n# extract, normalize, and load the data\npipeline.run(data)\n```\n\nTry it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**\n\n## Features\n\n- **Automatic Schema:** Data structure inspection and schema creation for the destination.\n- **Data Normalization:** Consistent and verified data before loading.\n- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.\n- **Scalable:** Adapts to growing data needs in production.\n- **Easy Maintenance:** Clear data pipeline structure for updates.\n- **Rapid Exploration:** Quickly explore and gain insights from new data sources.\n- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.\n- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.\n- **Incremental Loading:** Load only new or changed data and avoid loading old records again.\n- **Open Source:** Free and Apache 2.0 Licensed.\n\n## Ready to use Sources and Destinations\n\nExplore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/dlt-ecosystem/verified-sources) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/dlt-ecosystem/destinations).\n\n## Documentation\n\nFor detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).\n\n## Examples\n\nYou can find examples for various use cases in the [examples](docs/examples) folder.\n\n## Get Involved\n\nThe dlt project is quickly growing, and we\'re excited to have you join our community! Here\'s how you can get involved:\n\n- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)\n- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.\n- **Contribute Verified Sources**: Contribute your custom sources to the [dlt-hub/verified-sources](https://github.com/dlt-hub/verified-sources) to help other folks in handling their data tasks.\n- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.\n- **Improve documentation**: Help us enhance the dlt documentation.\n\n## License\n\nDLT is released under the [Apache 2.0 License](LICENSE.txt).\n',
     'author': 'dltHub Inc.',
     'author_email': 'services@dlthub.com',
     'maintainer': 'Marcin Rudolf',
     'maintainer_email': 'marcin@dlthub.com',
     'url': 'https://github.com/dlt-hub',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `dlt-0.3.1a0/PKG-INFO` & `dlt-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.3.1a0
+Version: 0.3.2
 Summary: DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
@@ -24,28 +24,29 @@
 Provides-Extra: bigquery
 Provides-Extra: dbt
 Provides-Extra: duckdb
 Provides-Extra: filesystem
 Provides-Extra: gcp
 Provides-Extra: gs
 Provides-Extra: postgres
+Provides-Extra: pyarrow
 Provides-Extra: redshift
 Provides-Extra: s3
+Provides-Extra: snowflake
 Requires-Dist: PyYAML (>=5.4.1)
 Requires-Dist: SQLAlchemy (>=1.4.0)
 Requires-Dist: astunparse (>=1.6.3)
-Requires-Dist: asyncstdlib (>=3.10.5)
 Requires-Dist: boto3 (>=1.26); extra == "filesystem" or extra == "s3"
-Requires-Dist: cachetools (>=5.2.0)
 Requires-Dist: click (>=7.1)
 Requires-Dist: cron-descriptor (>=1.2.32)
 Requires-Dist: dbt-bigquery (>=1.3.0,<1.5.0); extra == "dbt"
 Requires-Dist: dbt-core (>=1.3.0,<1.5.0); extra == "dbt"
 Requires-Dist: dbt-duckdb (>=1.3.0,<1.5.0); extra == "dbt"
 Requires-Dist: dbt-redshift (>=1.3.0,<1.5.0); extra == "dbt"
+Requires-Dist: dbt-snowflake (>=1.3.0,<1.5.0); extra == "dbt"
 Requires-Dist: deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: duckdb (>=0.6.1,<0.9.0); extra == "duckdb"
 Requires-Dist: fsspec (>=2023.5.0,<2024.0.0)
 Requires-Dist: gcsfs (>=2023.5.0,<2024.0.0); extra == "gcp" or extra == "bigquery" or extra == "gs"
 Requires-Dist: gitpython (>=3.1.29)
 Requires-Dist: giturlparse (>=0.10.0)
 Requires-Dist: google-cloud-bigquery (>=2.26.0); extra == "gcp" or extra == "bigquery"
@@ -54,26 +55,27 @@
 Requires-Dist: humanize (>=4.4.0)
 Requires-Dist: json-logging (==1.4.1rc0)
 Requires-Dist: jsonpath-ng (>=1.5.3,<2.0.0)
 Requires-Dist: makefun (>=1.15.0)
 Requires-Dist: orjson (>=3.8.6,<4.0.0); platform_python_implementation != "PyPy"
 Requires-Dist: pathvalidate (>=2.5.2)
 Requires-Dist: pendulum (>=2.1.2)
-Requires-Dist: pipdeptree (>=2.3.3)
+Requires-Dist: pipdeptree (>=2.9.3)
 Requires-Dist: psycopg2-binary (>=2.9.1); extra == "postgres" or extra == "redshift"
 Requires-Dist: psycopg2cffi (>=2.9.0); (platform_python_implementation == "PyPy") and (extra == "postgres" or extra == "redshift")
-Requires-Dist: pyarrow (>=8.0.0); extra == "bigquery"
+Requires-Dist: pyarrow (>=8.0.0); extra == "bigquery" or extra == "pyarrow"
 Requires-Dist: pytz (>=2022.6)
 Requires-Dist: requests (>=2.26.0)
 Requires-Dist: requirements-parser (>=0.5.0)
 Requires-Dist: s3fs (>=2023.5.0,<2024.0.0); extra == "filesystem" or extra == "s3"
 Requires-Dist: semver (>=2.13.0)
 Requires-Dist: sentry-sdk (>=1.4.3)
 Requires-Dist: setuptools (>=65.6.0)
 Requires-Dist: simplejson (>=3.17.5)
+Requires-Dist: snowflake-connector-python[pandas] (>=3.0.4,<4.0.0); extra == "snowflake"
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: tomlkit (>=0.11.3)
 Requires-Dist: typing-extensions (>=4.0.0)
 Requires-Dist: tzdata (>=2022.1)
 Project-URL: Repository, https://github.com/dlt-hub/dlt
 Description-Content-Type: text/markdown
 
@@ -139,15 +141,15 @@
 - **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.
 - **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.
 - **Incremental Loading:** Load only new or changed data and avoid loading old records again.
 - **Open Source:** Free and Apache 2.0 Licensed.
 
 ## Ready to use Sources and Destinations
 
-Explore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/verified-sources/chess) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/destinations/bigquery).
+Explore ready to use sources (e.g. Google Sheets) in the [Verified Sources docs](https://dlthub.com/docs/dlt-ecosystem/verified-sources) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/dlt-ecosystem/destinations).
 
 ## Documentation
 
 For detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).
 
 ## Examples
```

