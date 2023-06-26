# Comparing `tmp/galaxy-config-23.0.2.tar.gz` & `tmp/galaxy-config-23.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/config/dist/.tmp-2s26mh3a/galaxy-config-23.0.2.tar", last modified: Tue Jun 13 17:05:49 2023, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/config/dist/.tmp-5l0mdfwj/galaxy-config-23.0.3.tar", last modified: Mon Jun 26 09:49:51 2023, max compression
```

## Comparing `galaxy-config-23.0.2.tar` & `galaxy-config-23.0.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:49.000000 galaxy-config-23.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-13 17:04:36.000000 galaxy-config-23.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-13 17:05:49.000000 galaxy-config-23.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:49.000000 galaxy-config-23.0.2/galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:49.000000 galaxy-config-23.0.2/galaxy/config/
--rw-r--r--   0 runner    (1001) docker     (123)    62353 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20123 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/config_manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:49.000000 galaxy-config-23.0.2/galaxy/config/sample/
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/auth_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/build_sites.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/container_resolvers_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/data_manager_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)   113255 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/datatypes_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/disposable_email_blocklist.conf.sample
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/environment_modules_mapping.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/error_report.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/file_sources_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)   124190 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/galaxy.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)    53359 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/job_conf.sample.yml
--rw-r--r--   0 runner    (1001) docker     (123)    79082 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/job_conf.xml.sample_advanced
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/job_conf.xml.sample_basic
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/job_metrics_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/job_resource_params_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/lmod_modules_mapping.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/local_conda_mapping.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/object_store_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/oidc_backends_config.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/oidc_config.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/reports.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/themes_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/tool_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/tool_data_table_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/tool_destinations.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/tool_recommendations_overwrite.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)    14874 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/tool_shed.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/tool_sheds_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/trs_servers_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/user_preferences_extra_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/workflow_resource_mapper_conf.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/workflow_resource_params_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/sample/workflow_schedulers_conf.xml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:49.000000 galaxy-config-23.0.2/galaxy/config/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)   146525 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/schemas/config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/schemas/job_config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/schemas/reports_config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)    21370 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/schemas/tool_shed_config_schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/config/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:05:49.000000 galaxy-config-23.0.2/galaxy_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-13 17:05:49.000000 galaxy-config-23.0.2/galaxy_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-13 17:05:49.000000 galaxy-config-23.0.2/galaxy_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:05:49.000000 galaxy-config-23.0.2/galaxy_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-13 17:05:49.000000 galaxy-config-23.0.2/galaxy_config.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-13 17:05:49.000000 galaxy-config-23.0.2/galaxy_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:05:49.000000 galaxy-config-23.0.2/galaxy_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-13 17:05:49.000000 galaxy-config-23.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-13 17:04:37.000000 galaxy-config-23.0.2/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:49:51.000000 galaxy-config-23.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-26 09:48:32.000000 galaxy-config-23.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-26 09:49:51.000000 galaxy-config-23.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:49:51.000000 galaxy-config-23.0.3/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:49:51.000000 galaxy-config-23.0.3/galaxy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    62353 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20123 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/config_manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:49:51.000000 galaxy-config-23.0.3/galaxy/config/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/auth_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/build_sites.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/container_resolvers_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/data_manager_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)   113255 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/datatypes_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/disposable_email_blocklist.conf.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/environment_modules_mapping.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/error_report.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/file_sources_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)   124190 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/galaxy.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)    53359 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/job_conf.sample.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    79082 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/job_conf.xml.sample_advanced
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/job_conf.xml.sample_basic
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/job_metrics_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/job_resource_params_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/lmod_modules_mapping.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/local_conda_mapping.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/object_store_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/oidc_backends_config.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/oidc_config.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/reports.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/themes_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/tool_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/tool_data_table_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/tool_destinations.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/tool_recommendations_overwrite.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)    14874 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/tool_shed.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/tool_sheds_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/trs_servers_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/user_preferences_extra_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/workflow_resource_mapper_conf.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/workflow_resource_params_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/sample/workflow_schedulers_conf.xml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:49:51.000000 galaxy-config-23.0.3/galaxy/config/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)   146525 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/schemas/config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/schemas/job_config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/schemas/reports_config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    21370 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/schemas/tool_shed_config_schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/config/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:49:51.000000 galaxy-config-23.0.3/galaxy_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-26 09:49:51.000000 galaxy-config-23.0.3/galaxy_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-26 09:49:51.000000 galaxy-config-23.0.3/galaxy_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:49:51.000000 galaxy-config-23.0.3/galaxy_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 09:49:51.000000 galaxy-config-23.0.3/galaxy_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 09:49:51.000000 galaxy-config-23.0.3/galaxy_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 09:49:51.000000 galaxy-config-23.0.3/galaxy_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-26 09:49:51.000000 galaxy-config-23.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 09:48:33.000000 galaxy-config-23.0.3/test-requirements.txt
```

### Comparing `galaxy-config-23.0.2/LICENSE` & `galaxy-config-23.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/PKG-INFO` & `galaxy-config-23.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-config
-Version: 23.0.2
+Version: 23.0.3
 Summary: Galaxy configuration
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.3 (2023-06-26)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.2 (2023-06-13)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.1 (2023-06-08)
```

### Comparing `galaxy-config-23.0.2/galaxy/config/__init__.py` & `galaxy-config-23.0.3/galaxy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/config_manage.py` & `galaxy-config-23.0.3/galaxy/config/config_manage.py`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/auth_conf.xml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/auth_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/build_sites.yml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/build_sites.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/container_resolvers_conf.xml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/container_resolvers_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/datatypes_conf.xml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/datatypes_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/environment_modules_mapping.yml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/environment_modules_mapping.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/error_report.yml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/error_report.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/file_sources_conf.yml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/file_sources_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/galaxy.yml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/galaxy.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/job_conf.sample.yml` & `galaxy-config-23.0.3/galaxy/config/sample/job_conf.sample.yml`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/job_conf.xml.sample_advanced` & `galaxy-config-23.0.3/galaxy/config/sample/job_conf.xml.sample_advanced`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/job_metrics_conf.xml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/job_metrics_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/job_resource_params_conf.xml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/job_resource_params_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/lmod_modules_mapping.yml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/lmod_modules_mapping.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/object_store_conf.xml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/object_store_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/oidc_backends_config.xml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/oidc_backends_config.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/oidc_config.xml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/oidc_config.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/reports.yml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/reports.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/themes_conf.yml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/themes_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/tool_conf.xml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/tool_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/tool_data_table_conf.xml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/tool_data_table_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/tool_destinations.yml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/tool_destinations.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/tool_recommendations_overwrite.yml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/tool_recommendations_overwrite.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/tool_shed.yml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/tool_shed.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/trs_servers_conf.yml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/trs_servers_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/user_preferences_extra_conf.yml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/user_preferences_extra_conf.yml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/workflow_resource_params_conf.xml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/workflow_resource_params_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/sample/workflow_schedulers_conf.xml.sample` & `galaxy-config-23.0.3/galaxy/config/sample/workflow_schedulers_conf.xml.sample`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/schema.py` & `galaxy-config-23.0.3/galaxy/config/schema.py`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/schemas/config_schema.yml` & `galaxy-config-23.0.3/galaxy/config/schemas/config_schema.yml`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/schemas/job_config_schema.yml` & `galaxy-config-23.0.3/galaxy/config/schemas/job_config_schema.yml`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/schemas/reports_config_schema.yml` & `galaxy-config-23.0.3/galaxy/config/schemas/reports_config_schema.yml`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/schemas/tool_shed_config_schema.yml` & `galaxy-config-23.0.3/galaxy/config/schemas/tool_shed_config_schema.yml`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/script.py` & `galaxy-config-23.0.3/galaxy/config/script.py`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy/config/templates.py` & `galaxy-config-23.0.3/galaxy/config/templates.py`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/galaxy_config.egg-info/PKG-INFO` & `galaxy-config-23.0.3/galaxy_config.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-config
-Version: 23.0.2
+Version: 23.0.3
 Summary: Galaxy configuration
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,20 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+23.0.3 (2023-06-26)
+-------------------
+
+No recorded changes since last release
+
+-------------------
 23.0.2 (2023-06-13)
 -------------------
 
 No recorded changes since last release
 
 -------------------
 23.0.1 (2023-06-08)
```

### Comparing `galaxy-config-23.0.2/galaxy_config.egg-info/SOURCES.txt` & `galaxy-config-23.0.3/galaxy_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-config-23.0.2/setup.cfg` & `galaxy-config-23.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-config
 url = https://github.com/galaxyproject/galaxy
-version = 23.0.2
+version = 23.0.3
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util
 	boltons
 	jinja2
```

