# Comparing `tmp/vdk-core-0.3.902182978.tar.gz` & `tmp/vdk-core-0.3.911694257.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdk-core-0.3.902182978.tar", last modified: Fri Jun 16 09:16:05 2023, max compression
+gzip compressed data, was "dist/vdk-core-0.3.911694257.tar", last modified: Mon Jun 26 09:57:55 2023, max compression
```

## Comparing `vdk-core-0.3.902182978.tar` & `vdk-core-0.3.911694257.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2460 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1542 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1483 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      440 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/api/
--rw-rw-rw-   0 root         (0) root         (0)     2561 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/api/data_job.py
--rw-rw-rw-   0 root         (0) root         (0)    18539 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/api/job_input.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/api/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     6715 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/api/plugin/connection_hook_spec.py
--rw-rw-rw-   0 root         (0) root         (0)     7784 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/api/plugin/core_hook_spec.py
--rw-rw-rw-   0 root         (0) root         (0)     2586 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/api/plugin/hook_markers.py
--rw-rw-rw-   0 root         (0) root         (0)    25728 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/api/plugin/plugin_input.py
--rw-rw-rw-   0 root         (0) root         (0)     4057 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/api/plugin/plugin_registry.py
--rw-rw-rw-   0 root         (0) root         (0)     3961 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/api/plugin/plugin_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/internal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/
--rw-rw-rw-   0 root         (0) root         (0)     5894 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/builtin_hook_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/config/
--rw-rw-rw-   0 root         (0) root         (0)     5112 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/config/config_help.py
--rw-rw-rw-   0 root         (0) root         (0)     9440 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/config/job_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11179 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/config/log_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11191 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/config/vdk_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/
--rw-rw-rw-   0 root         (0) root         (0)     3123 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/connection_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1425 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/connection_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4661 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py
--rw-rw-rw-   0 root         (0) root         (0)     2316 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/execution_cursor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/impl/
--rw-rw-rw-   0 root         (0) root         (0)     6464 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/impl/router.py
--rw-rw-rw-   0 root         (0) root         (0)     1672 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py
--rw-rw-rw-   0 root         (0) root         (0)    10056 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py
--rw-rw-rw-   0 root         (0) root         (0)    10048 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/managed_cursor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/pep249/
--rw-rw-rw-   0 root         (0) root         (0)     2958 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2274 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py
--rw-rw-rw-   0 root         (0) root         (0)     3980 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/debug/
--rw-rw-rw-   0 root         (0) root         (0)     5746 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/debug/debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/ingestion/
--rw-rw-rw-   0 root         (0) root         (0)    29371 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py
--rw-rw-rw-   0 root         (0) root         (0)     5646 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     4069 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)    13247 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py
--rw-rw-rw-   0 root         (0) root         (0)     4631 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1849 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/internal_hookspecs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/job_properties/
--rw-rw-rw-   0 root         (0) root         (0)      897 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     1242 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py
--rw-rw-rw-   0 root         (0) root         (0)     3700 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2362 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/job_properties/properties_config.py
--rw-rw-rw-   0 root         (0) root         (0)     8208 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/job_properties/properties_router.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/notification/
--rw-rw-rw-   0 root         (0) root         (0)     4654 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/notification/notification.py
--rw-rw-rw-   0 root         (0) root         (0)    10656 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/notification/notification_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7985 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/notification/notification_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/
--rw-rw-rw-   0 root         (0) root         (0)     9148 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/cli_run.py
--rw-rw-rw-   0 root         (0) root         (0)    13573 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1752 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/execution_environment.py
--rw-rw-rw-   0 root         (0) root         (0)     5515 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/execution_results.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/execution_state.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/execution_tracking.py
--rw-rw-rw-   0 root         (0) root         (0)     7130 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/file_based_step.py
--rw-rw-rw-   0 root         (0) root         (0)     3911 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/job_context.py
--rw-rw-rw-   0 root         (0) root         (0)     7082 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/job_input.py
--rw-rw-rw-   0 root         (0) root         (0)     4856 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/run_status.py
--rw-rw-rw-   0 root         (0) root         (0)     1366 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py
--rw-rw-rw-   0 root         (0) root         (0)     7959 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/standalone_data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/step.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/templates/
--rw-rw-rw-   0 root         (0) root         (0)     3806 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/templates/template_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/termination_message/
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/termination_message/file_util.py
--rw-rw-rw-   0 root         (0) root         (0)     3119 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/termination_message/writer.py
--rw-rw-rw-   0 root         (0) root         (0)     1161 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/version/
--rw-rw-rw-   0 root         (0) root         (0)     2657 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/version/new_version_check.py
--rw-rw-rw-   0 root         (0) root         (0)     4973 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2764 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/version/version.py
--rw-rw-rw-   0 root         (0) root         (0)     6471 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/cli_entry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/internal/core/
--rw-rw-rw-   0 root         (0) root         (0)     9586 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2355 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/core/context.py
--rw-rw-rw-   0 root         (0) root         (0)    21237 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/core/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     5683 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/core/statestore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/internal/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     5200 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/plugin/plugin.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/plugin/plugin_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk/internal/util/
--rw-rw-rw-   0 root         (0) root         (0)     1234 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/util/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     2598 2023-06-16 09:15:42.000000 vdk-core-0.3.902182978/src/vdk/internal/util/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-06-16 09:16:03.000000 vdk-core-0.3.902182978/src/vdk/internal/vdk_build_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2460 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4333 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk_core.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk_core.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-16 09:16:05.000000 vdk-core-0.3.902182978/src/vdk_core.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-16 09:16:03.000000 vdk-core-0.3.902182978/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1542 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      440 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/api/
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/api/data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)    18539 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/api/job_input.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/api/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     6715 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/api/plugin/connection_hook_spec.py
+-rw-rw-rw-   0 root         (0) root         (0)     7784 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/api/plugin/core_hook_spec.py
+-rw-rw-rw-   0 root         (0) root         (0)     2586 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/api/plugin/hook_markers.py
+-rw-rw-rw-   0 root         (0) root         (0)    25728 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/api/plugin/plugin_input.py
+-rw-rw-rw-   0 root         (0) root         (0)     4057 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/api/plugin/plugin_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3961 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/api/plugin/plugin_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/internal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)     5894 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/builtin_hook_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/config/
+-rw-rw-rw-   0 root         (0) root         (0)     5112 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/config/config_help.py
+-rw-rw-rw-   0 root         (0) root         (0)     9440 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/config/job_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11179 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/config/log_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11191 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/config/vdk_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/
+-rw-rw-rw-   0 root         (0) root         (0)     3123 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/connection_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1425 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/connection_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4661 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2316 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/execution_cursor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/impl/
+-rw-rw-rw-   0 root         (0) root         (0)     6464 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/impl/router.py
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    10056 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10048 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/managed_cursor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/pep249/
+-rw-rw-rw-   0 root         (0) root         (0)     2958 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2274 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3980 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/debug/
+-rw-rw-rw-   0 root         (0) root         (0)     6082 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/debug/debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/ingestion/
+-rw-rw-rw-   0 root         (0) root         (0)    29371 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4069 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)    13247 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py
+-rw-rw-rw-   0 root         (0) root         (0)     4631 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/internal_hookspecs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/job_properties/
+-rw-rw-rw-   0 root         (0) root         (0)      897 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     3700 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2362 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/job_properties/properties_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     8208 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/job_properties/properties_router.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/notification/
+-rw-rw-rw-   0 root         (0) root         (0)     4654 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/notification/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)    10656 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/notification/notification_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7985 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/notification/notification_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/
+-rw-rw-rw-   0 root         (0) root         (0)     9148 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/cli_run.py
+-rw-rw-rw-   0 root         (0) root         (0)    13573 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/execution_environment.py
+-rw-rw-rw-   0 root         (0) root         (0)     5515 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/execution_results.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/execution_state.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/execution_tracking.py
+-rw-rw-rw-   0 root         (0) root         (0)     7130 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/file_based_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     3911 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/job_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     7082 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/job_input.py
+-rw-rw-rw-   0 root         (0) root         (0)     4856 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/run_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7959 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/standalone_data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/step.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3806 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/templates/template_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/termination_message/
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/termination_message/file_util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3119 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/termination_message/writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/version/
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/version/new_version_check.py
+-rw-rw-rw-   0 root         (0) root         (0)     4973 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2764 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/version/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     6471 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/cli_entry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/internal/core/
+-rw-rw-rw-   0 root         (0) root         (0)     9586 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/core/context.py
+-rw-rw-rw-   0 root         (0) root         (0)    21237 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/core/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5683 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/core/statestore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/internal/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     5200 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/plugin/plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/plugin/plugin_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk/internal/util/
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/util/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2598 2023-06-26 09:57:33.000000 vdk-core-0.3.911694257/src/vdk/internal/util/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-06-26 09:57:53.000000 vdk-core-0.3.911694257/src/vdk/internal/vdk_build_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk_core.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk_core.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-26 09:57:55.000000 vdk-core-0.3.911694257/src/vdk_core.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-26 09:57:53.000000 vdk-core-0.3.911694257/version.txt
```

### Comparing `vdk-core-0.3.902182978/PKG-INFO` & `vdk-core-0.3.911694257/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-core
-Version: 0.3.902182978
+Version: 0.3.911694257
 Summary: Versatile Data Kit SDK Core
 Home-page: https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Author: VMware Inc.
 Author-email: taurus@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/projects/vdk-core/README.md
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Platform: any
```

### Comparing `vdk-core-0.3.902182978/README.md` & `vdk-core-0.3.911694257/README.md`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/setup.cfg` & `vdk-core-0.3.911694257/setup.cfg`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/api/data_job.py` & `vdk-core-0.3.911694257/src/vdk/api/data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/api/job_input.py` & `vdk-core-0.3.911694257/src/vdk/api/job_input.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/api/plugin/connection_hook_spec.py` & `vdk-core-0.3.911694257/src/vdk/api/plugin/connection_hook_spec.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/api/plugin/core_hook_spec.py` & `vdk-core-0.3.911694257/src/vdk/api/plugin/core_hook_spec.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/api/plugin/hook_markers.py` & `vdk-core-0.3.911694257/src/vdk/api/plugin/hook_markers.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/api/plugin/plugin_input.py` & `vdk-core-0.3.911694257/src/vdk/api/plugin/plugin_input.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/api/plugin/plugin_registry.py` & `vdk-core-0.3.911694257/src/vdk/api/plugin/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/api/plugin/plugin_utils.py` & `vdk-core-0.3.911694257/src/vdk/api/plugin/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/builtin_hook_impl.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/builtin_hook_impl.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/config/config_help.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/config/config_help.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/config/job_config.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/config/job_config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/config/log_config.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/config/log_config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/config/vdk_config.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/config/vdk_config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/connection_hooks.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/connection_hooks.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/connection_plugin.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/connection_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/execution_cursor.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/execution_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/impl/router.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/impl/router.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/managed_cursor.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/managed_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/debug/debug.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/debug/debug.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,14 +35,28 @@
         :return: The hook call invocation as string
         """
         d = self.__dict__.copy()
         del d["_name"]
         return f"<ParsedCall {self._name!r}(**{d!r})>"
 
 
+def pluggy_result_to_string(outcome: Any) -> str:
+    try:
+        result = outcome.get_result()
+    except BaseException as e:
+        outcome.force_exception(e)
+        return ""
+
+    result_string = ""
+    for item in result:
+        result_string = f"\nJSON config override is {item}"
+
+    return result_string
+
+
 class HookRecorder:
     """Record all hooks invocations.
 
     This wraps all the hook calls/invocations, recording each call
     before propagating the normal calls.
     """
 
@@ -62,15 +76,15 @@
 
         def after(outcome: Any, hook_name: str, hook_impls: Any, kwargs: Any) -> None:
             print(
                 f"<<------ Finished call hook {hook_name}\n"
                 f"         with args:\n"
                 f"         {kwargs}.\n"
                 f"         Hook Impl: {hook_impls}\n",
-                f"         Outcome: {vars(outcome)}",
+                f"         Outcome: {pluggy_result_to_string(outcome)}",
                 file=sys.stderr,
             )
 
         self._undo_wrapping = (
             self._plugin_registry.plugin_manager().add_hookcall_monitoring(
                 before, after
             )
```

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/internal_hookspecs.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/internal_hookspecs.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/job_properties/properties_config.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/job_properties/properties_config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/job_properties/properties_router.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/job_properties/properties_router.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/notification/notification.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/notification/notification.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/notification/notification_base.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/notification/notification_base.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/notification/notification_configuration.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/notification/notification_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/cli_run.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/cli_run.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/data_job.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/execution_environment.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/execution_environment.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/execution_results.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/execution_results.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/execution_state.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/execution_state.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/execution_tracking.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/execution_tracking.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/file_based_step.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/file_based_step.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/job_context.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/job_context.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/job_input.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/job_input.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/standalone_data_job.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/standalone_data_job.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/run/step.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/run/step.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/templates/template_impl.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/templates/template_impl.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/termination_message/file_util.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/termination_message/file_util.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/termination_message/writer.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/termination_message/writer.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/version/new_version_check.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/version/new_version_check.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/builtin_plugins/version/version.py` & `vdk-core-0.3.911694257/src/vdk/internal/builtin_plugins/version/version.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/cli_entry.py` & `vdk-core-0.3.911694257/src/vdk/internal/cli_entry.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/core/config.py` & `vdk-core-0.3.911694257/src/vdk/internal/core/config.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/core/context.py` & `vdk-core-0.3.911694257/src/vdk/internal/core/context.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/core/errors.py` & `vdk-core-0.3.911694257/src/vdk/internal/core/errors.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/core/statestore.py` & `vdk-core-0.3.911694257/src/vdk/internal/core/statestore.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/plugin/plugin.py` & `vdk-core-0.3.911694257/src/vdk/internal/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/util/decorators.py` & `vdk-core-0.3.911694257/src/vdk/internal/util/decorators.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk/internal/util/utils.py` & `vdk-core-0.3.911694257/src/vdk/internal/util/utils.py`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.902182978/src/vdk_core.egg-info/PKG-INFO` & `vdk-core-0.3.911694257/src/vdk_core.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-core
-Version: 0.3.902182978
+Version: 0.3.911694257
 Summary: Versatile Data Kit SDK Core
 Home-page: https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Author: VMware Inc.
 Author-email: taurus@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/projects/vdk-core/README.md
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Platform: any
```

### Comparing `vdk-core-0.3.902182978/src/vdk_core.egg-info/SOURCES.txt` & `vdk-core-0.3.911694257/src/vdk_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

